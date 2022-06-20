---
title: Proiektuaren antolaketa APIaren errendimendua
description: Artikulu honek Proiektuaren egutegiko APIen errendimendu-erreferentziari buruzko informazioa eskaintzen du eta erabilera egokiena lortzeko praktika onenak identifikatzen ditu.
author: ruhercul
ms.date: 11/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 1ee1bd8e4412ee1d10f445628c5dc87cc9fa91d3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911167"
---
# <a name="project-schedule-api-performance"></a>Proiektuaren antolaketa APIaren errendimendua

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egin, webgunerako proiektua_

Artikulu honek Project schedule aplikazioen programazio-interfazeen (API) errendimendu-erreferentziari buruzko informazioa eskaintzen du eta erabilera optimizatzeko praktika onenak identifikatzen ditu.

## <a name="project-scheduling-service"></a>Proiektuen antolaketa-zerbitzua
Proiektuen antolaketa-zerbitzua Microsoft Azure-n exekutatzen den maizter anitzeko zerbitzua da. Interakzioa hobetzeko diseinatuta dago, erabiltzaileek proiektuetan lan egiten dutenean esperientzia azkarra eta arina eskainiz. Hobekuntza hori aldaketa-eskaerak onartuz, prozesatu eta gero emaitza berehala itzuliz lortzen da. Zerbitzuak modu asinkronoan jarraitzen du Dataverse-n eta ez die erabiltzaileei beste eragiketa batzuk egitea eragozten.

Proiektuaren egutegiko APIak Proiektuak Antolatzeko Zerbitzuan oinarritzen dira artikulu honen ondorengo ataletan xehetasun gehiagorekin deskribatzen diren eskaerak exekutatzeko.

Proiektuak antolatzeko APIak honako zereginen xehetasunen egituraren (WBS) entitate hauekin lan egiteko diseinatuta daude:

  - Project
  - Proiektuaren zeregina
  - Proiektuaren zereginen mendekotasuna
  - Proiektu-taldeko kidea
  - Baliabide-esleipena
  
Erabiltzek prest dauden eremuak eta eremu pertsonalizatuak onartzen dira. Besterik adierazi ezean, ohiko eragiketa guztiak onartzen dira, hala nola sortu, eguneratu eta ezabatu. Informazio gehiagorako, ikusi [Erabili Proiektuak antolatzeko APIak eragiketak eta programazio entitateak egiteko](schedule-api-preview.md).

Proiektuak antolatzeko APIen barruan, lan-unitate-eredu bat gehitu da. Eredu hau OperationSet gisa ezagutzen da, eta transakzio bakarrean hainbat eskaera prozesatu behar direnean erabil daiteke.

Ondorengo ilustrazioak bazkide batek eginbide hau erabiltzen denean biziko duen fluxua erakusten du.

![Dataverse eta proiektuen antolaketa-zerbitzuaren fluxua.](./media/dataverse-project-scheduling-service-flow.png)

**1. urratsa**: Bezero batek API dei bat egiten du Open Data Protocol (OData) amaierako puntu batera Dataverse-n OperationSet bat sortzeko.

**2. urratsa**: OperationSet berria sortu ondoren, **OperationSetId** balio bat itzultzen da.

**3. urratsa**: bezeroak **OperationSetId** balioa erabiltzen du Proiektuak antolatzeko API eskaera bat egiteko. Emaitza programazio-entitate batean sortu, eguneratu edo ezabatu eskaera bat da. Eskaera hau egiten denean, metadatuen baliozkotzea egiten da. Balioztatzeak huts egiten badu, eskaera amaitu egiten da eta errore bat itzultzen da.

**4a-4c urratsak**: Urrats hauek ONARTU fasea adierazten dute. Bezeroak deitzen du **ExecuteOperationSetV1** APIa, aldaketa guztiak proiektuak antolatzeko zerbitzura lote batean bidaltzen dituena. Proiektuak Planifikatzeko Zerbitzuak bere balioztatzeak egiten ditu lotean egindako eskaeren arabera. Balidazio hutsek lotea desegin eta salbuespen bat itzultzen diote deitzaileari. Proiektua Antolatzeko Zerbitzuak lotea ongi onartzen badu, OperationSet egoera eguneratzen da, OperationSet Proiektua Planifikatzeko Zerbitzuak prozesatzen ari dela islatzeko.

**5. urratsa**: Urrats honek IRAUNKETA fasea adierazten du. Project Scheduling Service-k era asinkronoan idazten du lotea Dataverse transakzio batean. Idazketa-eragiketa arrakastatsua bada, OperationSet gisa markatuko da **Osatua**. Edozein akatsek transakzioari eta lotzeari uko egiten diote, eta OperationSet gisa markatzen da **Huts egin du**.

## <a name="performance-methodology"></a>Errendimenduaren metodologia
Exekuzio-denbora deialditik deialdira arteko denbora gisa definitzen da **ExecuteOperationSetV1** API Proiektuak Antolatzeko Zerbitzuak idazten amaitu arte Dataverse. Eragiketa guztiak 2.200 aldiz exekutatzen dira eta P99 exekuzio denboraren neurketak jakinarazi dira. Erregistro bakarreko eta bulk eragiketak neurtzen dira.

Erregistro bakarreko eragiketa baterako, OperationSet-ek eskaera bat dauka. Masakako eragiketetarako, 20, 50 edo 100 eskaera ditu. Solteen tamaina bakoitza bereizita ematen da.

Eragiketa hauek UR 15 Project Operations Lite inplementazio batean exekutatzen dira Ipar Amerikan.

## <a name="results"></a>Emaitzak
### <a name="create-operations"></a>Sortu eragiketak
#### <a name="single-record-create-operations"></a>Erregistro bakarreko sortzeko eragiketak
Hurrengo taulak erregistro bakarra sortzeko exekuzio-denborak erakusten ditu. Denborak segundotan adierazten dira.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">Erregistro&nbsp;&nbsp;&nbsp;mota</th>
    <th class="tg-0lax" colspan="2">Denbora</th>
  </tr>
  <tr>
    <th class="tg-0lax">Beharrezko eremuak</th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Project</td>
    <td class="tg-0lax">2.5</td>
    <td class="tg-0lax">3.78</td>
  </tr>
  <tr>
    <td class="tg-0lax">Ataza</td>
    <td class="tg-0lax">8.82</td>
    <td class="tg-0lax">9.34</td>
  </tr>
  <tr>
    <td class="tg-0lax">Esleipena</td>
    <td class="tg-0lax">9.19</td>
    <td class="tg-0lax">9.19</td>
  </tr>
  <tr>
    <td class="tg-0lax">Taldeko kidea</td>
    <td class="tg-0lax">0.84</td>
    <td class="tg-0lax">4.2</td>
  </tr>
  <tr>
    <td class="tg-0lax">Mendekotasuna</td>
    <td class="tg-0lax">8.84</td>
    <td class="tg-0lax">8.84</td>
  </tr>
</tbody>
</table>

#### <a name="bulk-create-operations"></a>Sortze masiboaren eragiketak
Hurrengo taulak erregistro ugari sortzeko exekuzio-denborak erakusten ditu. Zehazki, Microsoft-ek 20, 50 eta 100 erregistro sortzeko exekuzio-denborak neurtu zituen OperationSet bakarrean. Denborak segundotan adierazten dira.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="3">Erregistro&nbsp;&nbsp;&nbsp;mota</th>
    <th class="tg-0lax" colspan="6">Denbora</th>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2">20 erregistro</th>
    <th class="tg-0lax" colspan="2">50 erregistro</th>
    <th class="tg-0lax" colspan="2">100 erregistro</th>
  </tr>
  <tr>
    <th class="tg-0lax">Beharrezko eremuak</th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
    <th class="tg-0lax">Beharrezko eremuak</th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
    <th class="tg-0lax">Beharrezko eremuak</th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Ataza</td>
    <td class="tg-0lax">19.92</td>
    <td class="tg-0lax">38.35</td>
    <td class="tg-0lax">36.67</td>
    <td class="tg-0lax">99.13</td>
    <td class="tg-0lax">116.77</td>
    <td class="tg-0lax">174.06</td>
  </tr>
  <tr>
    <td class="tg-0lax">Esleipena</td>
    <td class="tg-0lax">13.94</td>
    <td class="tg-0lax">13.94</td>
    <td class="tg-0lax">43.95</td>
    <td class="tg-0lax">43.95</td>
    <td class="tg-0lax">69.38</td>
    <td class="tg-0lax">69.38</td>
  </tr>
  <tr>
    <td class="tg-0lax">Mendekotasuna</td>
    <td class="tg-0lax">30.04</td>
    <td class="tg-0lax">30.04</td>
    <td class="tg-0lax">77.82</td>
    <td class="tg-0lax">77.82</td>
    <td class="tg-0lax">176.89</td>
    <td class="tg-0lax">176.89</td>
  </tr>
</tbody>
</table>

> [!NOTE] 
> Sortze masiboko eragiketak **Proiektua** eta **Taldeko kidea** entitateak ez dira taula honetan sartzen, eragiketa horien exekuzio-denbora exekuzio-denboraren antza duelako erregistro bakarra sortzeko APIari hainbat aldiz deitzen zaionean. API hauek berehala exekutatzen dira Dataverse-n.

Ondorengo ilustrazioak exekuzio-denboren grafiko bat erakusten du **Zeregina**, **Esleipena** eta **Mendekotasuna** entitateak 20, 50 eta 100 erregistro sortzen direnean eta onartzen diren eremu guztiak erabiltzen direnean.

![Sortu erregistroaren exekuzio denbora grafikoa.](./media/create-record-execution-time.png)

### <a name="update-operations"></a>Eguneratu eragiketak
#### <a name="single-record-update-operations"></a>Erregistro bakarreko eguneratzeko eragiketak
Hurrengo taulak erregistro bakarra eguneratzeko exekuzio-denborak erakusten ditu. Denborak segundotan adierazten dira.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">Erregistro&nbsp;&nbsp;&nbsp;mota</th>
    <th class="tg-0lax" colspan="2">Denbora</th>
  </tr>
  <tr>
    <th class="tg-0lax">Beharrezko eremuak </th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Project</td>
    <td class="tg-0lax">9.53</td>
    <td class="tg-0lax">13.91</td>
  </tr>
  <tr>
    <td class="tg-0lax">Ataza</td>
    <td class="tg-0lax">8.82</td>
    <td class="tg-0lax">9.91</td>
  </tr>
  <tr>
    <td class="tg-0lax">Taldeko kidea</td>
    <td class="tg-0lax">9</td>
    <td class="tg-0lax">8.96</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> Eguneratu eragiketak **Baliabide-esleipenak** eta **Proiektuaren ataza menpekotasuna** entitateak ez dira onartzen.

#### <a name="bulk-update-operations"></a>Eguneratze masiboaren eragiketak
Hurrengo taulak erregistro ugari eguneratzeko exekuzio-denborak erakusten ditu. Zehazki, Microsoft-ek 20, 50 eta 100 erregistro eguneratzeko exekuzio-denborak neurtu zituen OperationSet bakarrean. Denborak segundotan adierazten dira.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="3">Erregistro&nbsp;&nbsp;&nbsp;mota</th>
    <th class="tg-0lax" colspan="6">Denbora</th>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2">20 erregistro</th>
    <th class="tg-0lax" colspan="2">50 erregistro</th>
    <th class="tg-0lax" colspan="2">100 erregistro</th>
  </tr>
  <tr>
    <th class="tg-0lax">Beharrezko eremuak</th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
    <th class="tg-0lax">Beharrezko eremuak</th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
    <th class="tg-0lax">Beharrezko eremuak</th>
    <th class="tg-0lax">Onartutako eremu guztiak</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Ataza</td>
    <td class="tg-0lax">8.91</td>
    <td class="tg-0lax">38.71</td>
    <td class="tg-0lax">20.92</td>
    <td class="tg-0lax">87.13</td>
    <td class="tg-0lax">36.68</td>
    <td class="tg-0lax">190.34</td>
  </tr>
  <tr>
    <td class="tg-0lax">Taldeko kidea</td>
    <td class="tg-0lax">20.52</td>
    <td class="tg-0lax">26.06</td>
    <td class="tg-0lax">41.93</td>
    <td class="tg-0lax">44.51</td>
    <td class="tg-0lax">38.63</td>
    <td class="tg-0lax">66.53</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> Eguneratu eragiketak **Baliabide-esleipenak** eta **Proiektuaren ataza menpekotasuna** entitateak ez dira onartzen.

Ondorengo ilustrazioak exekuzio-denboren grafiko bat erakusten du Zeregina eta Taldeko kidea entitateak 20, 50 eta 100 erregistro eguneratzen direnean eta onartzen diren eremu guztiak erabiltzen direnean.

![Eguneratu erregistroaren exekuzio denbora grafikoa.](./media/update-record-execution-time.png)

### <a name="delete-operations"></a>Ezabatu eragiketak
#### <a name="single-record-delete-operations"></a>Erregistro bakarreko ezabatzeko eragiketak
Hurrengo taulak erregistro bakarra ezabatzeko exekuzio-denborak erakusten ditu. Denborak segundotan adierazten dira.

| Erregistro mota | Denbora  |
|-------------|-------|
| Ataza        | 20.12 |
| Esleipena  | 10.86 |
| Taldeko kidea | 12.52 |
| Mendekotasuna  | 20.89 |

> [!NOTE]
> Ezabatu eragiketak **Proiektua** entitateak ez dira onartzen.

#### <a name="bulk-delete-operations"></a>Ezabatze masiboaren eragiketak
Hurrengo taulak erregistro ugari ezabatzeko exekuzio-denborak erakusten ditu. Zehazki, Microsoft-ek 20, 50 eta 100 erregistro ezabatzeko exekuzio-denborak neurtu zituen OperationSet bakarrean. Denborak segundotan adierazten dira.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">Erregistro&nbsp;&nbsp;&nbsp;mota</th>
    <th class="tg-0lax" colspan="3">Denbora</th>
  </tr>
  <tr>
    <th class="tg-0lax">20 erregistro</th>
    <th class="tg-0lax">50 erregistro</th>
    <th class="tg-0lax">100 erregistro</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">Ataza</td>
    <td class="tg-0lax">20.91</td>
    <td class="tg-0lax">67.43</td>
    <td class="tg-0lax">71.96</td>
  </tr>
  <tr>
    <td class="tg-0lax">Esleipena</td>
    <td class="tg-0lax">11.75</td>
    <td class="tg-0lax">25.79</td>
    <td class="tg-0lax">47.66</td>
  </tr>
  <tr>
    <td class="tg-0lax">Taldeko kidea</td>
    <td class="tg-0lax">9.78</td>
    <td class="tg-0lax">39.73</td>
    <td class="tg-0lax">24.33</td>
  </tr>
  <tr>
    <td class="tg-0lax">Mendekotasuna</td>
    <td class="tg-0lax">24.61</td>
    <td class="tg-0lax">54.9</td>
    <td class="tg-0lax">109.16</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> Ezabatu eragiketak **Proiektua** entitateak ez dira onartzen.

Ondorengo ilustrazioak exekuzio-denboren grafiko bat erakusten du **Zeregina**, **Esleipena**, **Taldeko kidea** eta **Mendekotasuna** entitateak 20, 50 eta 100 erregistro ezabatzen direnean.

![Ezabatu erregistroaren exekuzio denbora grafikoa.](./media/delete-record-execution-time.png)

## <a name="observations"></a>Behaketak
Erregistro-eragiketa bakoitzeko, **ExecuteOperationSet** APIak 800 milisegundo inguru behar ditu eskaera bat Proiektuen Planifikazio Zerbitzura bidaltzeko. Proiektuak Antolatzeko Zerbitzuak bost segundo inguru behar ditu karga eta deia prozesatzeko Dataverse. Gainerako exekuzio-denbora negozio-logika exekutatzen eta datu-basean datuak idazten igarotzen da Dataverse-n.

100 erregistro sortzen, eguneratzen edo ezabatzen direnean, **ExecuteOperationSet** APIak hiru segundo inguru behar ditu eskaera Proiektuak Antolatzeko Zerbitzura bidaltzeko. Proiektuak Antolatzeko Zerbitzuak bost segundo inguru behar ditu eskaerak eta deia prozesatzeko Dataverse. Masakako eragiketek a ordaindu behar dute **Proiektuak Antolatzeko Zerbitzuaren zerga** behin, OperationSet-eko erregistro guztietarako. Hori dela eta, eragiketa masiboek erregistro bakarreko eragiketek baino batez besteko exekuzio denbora nabarmen txikiagoa dute.

## <a name="scenarios"></a>Inguruneak
Ondorengo taulak proiektuaren egutegiko APIak agertoki zehatzak betetzeko erabiltzen diren exekuzio-denborak erakusten ditu. Denborak segundotan adierazten dira.

| Egoera                                                                   | Denbora  |
|----------------------------------------------------------------------------|-------|
| Sortu 40 zeregin dituen proiektu bat.                                      | 36.01 |
| Sortu 40 zeregin eta 20 mendekotasun dituen proiektu bat.                  | 38.11 |
| Sortu 40 zeregin eta 30 esleipen dituen proiektu bat.                   | 60.17 |
| Sortu 40 zeregin, 20 mendekotasun eta 30 esleipen dituen proiektu bat. | 60.27 |

## <a name="best-practices"></a>Jardunbide egokiak
Aurreko egoeraren emaitzetan oinarrituta, APIek hobeto funtzionatzen dute baldintza hauetan:

  - Talde ahalik eta eragiketa gehien. Eragiketa masiboen batez besteko exekuzio-denbora hobea da erregistro bakarreko eragiketen batez besteko exekuzio-denbora baino. Erabiltzen diren OperationSets zenbat eta txikiagoa izan, orduan eta azkarragoa izango da batez besteko exekuzio-denbora.
  - Ezarri zure eszenatokia betetzeko behar diren gutxieneko atributuak soilik. Izan hautatzailea OperationSet eskaera batean derrigorrezkoak ez diren eremu motei buruz. Atzerriko gakoak edo bilketa-eremuak dituzten eremuek errendimenduari eragin negatiboa izango diote.
