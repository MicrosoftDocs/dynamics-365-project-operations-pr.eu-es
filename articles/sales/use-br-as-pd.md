---
title: Erabili baliabide erreserbagarriak prezio-dimentsio gisa
description: Artikulu honek erreserba daitezkeen baliabideak prezioen dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du.
author: Rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: c467c45885bbd8931eccc75862f537c0f46433ef
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914801"
---
# <a name="use-a-bookable-resource-as-a-pricing-dimension"></a>Erabili baliabide erreserbagarriak prezio-dimentsio gisa

 _**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_ 

Artikulu honek erreserba daitezkeen baliabideak prezioen dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du. Zure prezio estrategia erreserbatzeko baliabide bakoitzak prezio edo kostu tasa jakin bat izan dezan konfiguratuta badago, erabili erreserbagarri den baliabide bat prezioen dimentsio gisa.

## <a name="prerequisites"></a>Aurrebaldintzak
Artikulu honetako prozedurak osatu aurretik, prezioen dimentsioko irtenbide berri bat izan behar duzu zure erakundearentzat. Oraindik sortu ez baduzu, ikusi [Sortu eremu eta entitate pertsonalizatuak](../pricing-costing/create-custom-fields-entities-pricing-dimensions.md).

## <a name="add-the-bookable-resource-field-to-forms-and-views"></a>Gehitu Baliabide erreserbagarria eremua inprimakietan eta ikuspegietan
**Baliabide erreserbagarria** eremua prezioen dimentsioaren irtenbidean ikusgai egiteko, eremua entitate gisa forma eta ikuspegi guztietara gehitu behar duzu.

Hurrengo taulan kutxaz kanpoko forma eta ikuspegi guztiak zerrendatzen dira, entitatearen arabera. Eremu berria gehitu beharko duzu pertsonalizatutako entitateetako inprimaki edo ikuspegi osagarrietara.

|   Entity        | Inprimakiak   |Ikuspegiak        |
| ------------------------------|---------------------------------|----------------------------------|
|  Funtzioaren prezioa| Informazioa | - Baliabide-kategorien prezio aktiboak<br> - Baliabide-kategorien prezioekin erlazionatuta |
|  Funtzio-prezioaren gainprezioa| Informazioa| - Funtzio-prezioaren gainprezio aktiboa<br>- Funtzio-prezioaren gainprezioarekin erlazionatuta |
|  Eskaintzaren lerroaren xehetasunak| - Proiektuari buruzko informazioa<br>- Sorrera bizkorreko proiektua| - Eskaintzaren lerroaren xehetasun aktiboak<br>- Konbinatutako eskaintzaren lerroen xehetasunak<br>- Eskaintzaren lerroen xehetasunekin erlazionatuta |
|  Proiektu-kontratuaren lerroaren xehetasunak| - Proiektuari buruzko informazioa<br>- Sorrera bizkorreko proiektua| - Kontratuaren lerroaren xehetasun konbinatuak<br>- Kontratuaren lerroaren xehetasun aktiboak<br>- Kontratuaren lerroen xehetasunekin erlazionatuta |
|  Proiektuaren zeregina| - Informazioa<br>- Inprimaki berria| &nbsp; |
|  Proiektu-taldeko kidea| - Informazioa<br>- Inprimaki berria| - Proiektu-taldeko kide aktiboak<br>- Proiektuaren taldeko kideak<br>- Proiektu-taldeko kideekin erlazionatuta |
|  Denbora-sarrera| - Informazioa<br>- Sortu denbora-sarrera| - Nire denbora-sarrerak, dataren arabera<br>- Aste honetako nire denbora-sarrerak<br>- Onartu beharreko denbora-sarrerak|
|  Kutxako liburuaren lerroa| - Informazioa<br>- Sorrera bizkorra| - Kutxako liburuaren lerro aktiboak<br>- Kutxako liburuaren lerroekin erlazionatuta |
|  Fakturaren lerroaren xehetasunak| - Informazioa<br>- Sorrera bizkorra| - Fakturaren lerroen xehetasun aktiboak<br>- Kobra daitezkeen fakturen transakzioak<br>- Doako fakturen transakzioak<br>- Fakturaren lerroen xehetasunekin erlazionatuta <br>- Kobra ezin daitezkeen fakturaren transakzioak|
|  Unekoa"| - Informazioa<br>- Benetako datu aktiboak| Benetako datuekin erlazionatuta |

## <a name="set-up-a-bookable-resource-as-a-pricing-dimension"></a>Konfiguratu baliabide erreserbagarriak prezio-dimentsio gisa
Baliabide erreserbagarriak prezio-dimentsio gisa konfiguratzeko, jarraitu urrats hauek:

1. Joan **Ezarpenak** > **Parametroak** atalera. 
2. **Parametroa** orrialdean, **Zenbatekoan oinarritutako prezio-dimentsioak** fitxan, egiaztatu agertzen den saretak **Prezio-dimentsioak** entitateko erregistroak erakusten dituela. 
2. Gehitu **Baliabide erreserbagarriak** prezio-dimentsioen zerrenda honetara **msdyn_bookableresource** gisa. 
3. **Kostuan aplikagarria** eta **Salmentetan aplikagarria**, hautatu balio bat.
4. **Neurriaren mota** eremuan, hautatu **Zenbatekoan oinarrituta** aukera. 
5. Aukeratu baliabide erreserbagarriaren kostua eta salmenta lehentasuna. Normalean, erreserbatzeko baliabide batek du lehentasun handiena prezioen dimentsio gisa sartuta. Ezarri lehentasuna **1** (edo **0** lehentasuna zenbatzen duzunaren arabera) portaera hori ziurtatzeko.

## <a name="set-up-pricing-dimension-field-names"></a>Konfiguratu prezio-dimentsio aktiboen eremuak

Prezioen dimentsioaren eremuaren izena denean **Funtzioaren prezioa** taula bere eremuaren izenaren desberdina da prezioen lehenetsiak funtzionatu behar duen beste edozein entitateren kasuan, prezioen dimentsioaren erregistroa izen desberdinen berri izan behar da.  

Baliabide erresbagarri baterako, **Proiektuko taldekideak** entitateak beste izen bat du **Funtzioaren prezioa** entitatearekin konparatuta: 

 - **Proiektuko taldekideak** entitatea = **msdyn_bookableresourceid**
 - **Rolaren prezioa** entitatea = **msdyn_bookableresource**

Prezioen dimentsioaren erregistroa **msydn_bookableresource** aldea jakinarazi behar da.

1. Egin klik bikoitza errenkadan **Prezioen neurriak** saretan dimentsio orria irekitzeko **msdyn_bookableresource** baliabidekoa.
2. Dimentsioaren orrian, **Erlazionatutakoa** fitxan, hautatu **Prezioen dimentsioaren eremu-izenak** aukeran.

  ![Prezio-dimentsioaren eremu-izenak fitxa.](media/PD-fieldname.png)

3. Elkartzen den ikuspegian, hautatu **Gehitu prezioen dimentsioaren eremu berria** aukeran.

  ![Gehitu prezio-dimentsio eremu berriak.](media/Add-NewPD-fieldname.png)

  Honek irekitzen du **Prezioen dimentsioaren eremu berriaren izena** orrialdea **msdyn_bookableresource** baliabiderako. 

4. **Prezioen dimentsio eremuaren izen berria** orrialdean, gehitu **msdyn_projectteam** **Entitatearen izen lokalean**.
5. Gehitu **msdyn_bookableresourceid** **Eremuaren izenean**.

 ![Prezio-dimentsioaren eremu-izena.](media/PD-fieldname-Added.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]