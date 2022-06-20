---
title: Proiektuetan oinarritutako kontratuaren lerroen ikuspegi orokorra
description: Artikulu honetan, proiektuetan oinarritutako kontratu-ildoekin nola lan egin ematen da.
author: rumant
ms.date: 10/28/2020
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: d32edac6537a4b0f51e9d2f72cb4a7342606d2c5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931407"
---
# <a name="project-based-contract-lines-overview"></a>Proiektuetan oinarritutako kontratuaren lerroen ikuspegi orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations proiektuan oinarritutako kontratu lerroak proiektu batean egindako lanen osagai zehatzen aurrekontua eta fakturazio akordioak atxikitzeko diseinatuta daude. Proiektuan oinarritutako kontratu lerroaren egitura proiektuaren kalkuluen eta fakturazio eszenatokietarako hedatzen da, honako kontzeptu hauekin:

- Fakturazio-metodoa
- Proiektuen eta zereginen esleipena
- Transakzio klaseak barne
- Ez gainditzeko muga
- Aplikagarritasun konfigurazioa
- Aurrekontuak kontratuaren lineako xehetasunak erabiliz
- Kontratuaren lerroaren bezeroa

Ondorengo taulan eremuko eremuak biltzen dira **Orokorra** proiektuan oinarritutako kontratu-lerroen fitxa, proiektuan oinarritutako lan zehatza eta finkatua finkatzeko eta fakturazio moldaketak egiteko oinarriak finkatzen laguntzen dutenak.

| Eremua | Deskribapena | Downstream eragina |
| --- | --- | --- |
| **Izena** | Kontratuaren lerroaren izena. Honek kalkulatzen ari den kontratuaren osagai diskretua identifikatzen du. Aurrekontu batetik sortutako proiektu kontratu baterako, balio hori proiektuan oinarritutako aurrekontu lerroaren dagokion balio batetik kopiatzen da. | Faktura sortzen denean kontratu lerro honetatik sortzen den proiektuaren faktura lerroan kopiatutako izena. |
| **Fakturazio-metodoa** | Aurrekontu batetik sortutako proiektu kontratu baterako, aurrekontuaren lerroaren dagokion balio batetik kopiatzen da. Hau da aukera multzo, Project Operations-ek onartzen dituzten bi kontratazio eredu nagusiak adierazten dituena:</br>- **Prezio finkoa**</br>- **Denbora eta materiala** | Aipatutako kontratu lerroaren fakturazio metodoan oinarrituta, benetako transakzioa prozesatuko da. Benetakoak aipatzen duen kontratu lerroak denbora eta materiala fakturatzeko metodoa badu, kostuen eta fakturatu gabeko salmenten benetako erregistroak sortzen dira. Benetakoak aipatzen duen kontratu-lerroak prezio finkoko fakturazio-metodoa badu, benetako kostua soilik sortzen da. |
| **Project** | Erabili eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko. | Balio hau honekin batera erabiliko da **Zereginak barne** eta **Barne transakzio klaseak** kontratu-lerroaren erreferentzia benetako edo kalkulatutako linea-erregistro batean ebazteko. |
| **Gehitutako zereginak** | Kontratu lerro honek hautatutako proiektuaren proiektuko zeregin guztiak edo zereginen azpimultzo bat bakarrik biltzen dituen adierazten du. Aukera multzo bat da, balore hauek ditu:</br>- **Proiektuen zeregin guztiak**</br>- - **Hautatutako proiektu-zereginak soilik**. Eremu honetako balio huts bat hautatzearen berdina da **Proiektuaren zeregin guztiak**. | **Aukeratutako zereginak soilik** hautatuta dago, zeregin zehatzak hautatu eta kontratu lerro honekin lotu ditzakezu **Zereginen fakturazio konfigurazioa** fitxan **Proiektua** orrialdea. Balio hau honekin batera erabiliko da **Proiektua** eta **Barne transakzio klaseak** kontratu-lerroaren erreferentzia benetako edo aurrekontuko lerro erregistro batean ebazteko. |
| **Idatzi denbora** | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak kontratuaren lerro honetan sartuko diren. **Ez** balioak kontratuaren lerroan sartzen ez diren transakzioak edo denbora-transakzioak adierazten du. **Bai** balioak egingo dutela adierazten du. | Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko. |
| **Idatzi gastua** | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren gastuen kostuak kontratuaren lerro honetan sartuko diren. **Ez** balioak kontratuaren lerroan sartzen ez diren gastuen kostuak adierazten du. **Bai** balioak egingo dutela adierazten du. | Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko. |
| **Sartu materialak** | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren materialaren kostuak kontratuaren lerro honetan sartuko diren. **Ez** balioa adierazten du materialaren kostuak kontratuaren lerro honetan ez diren sartuko. **Bai** balioak egingo dutela adierazten du. | Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko. |
| **Idatzi prezioa** | **Bai**/**Ez** balioa adierazten du hautatutako proiektuaren komisioak kontratuaren lerro honetan sartuko diren. **Ez** balioak kontratuaren lerroan sartzen ez diren zergak adierazten du. **Bai** balioak egingo dutela adierazten du. | Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko. |
| **Kontratatutako zenbatekoa** | Prezio finkoko kontratu lerroan, zenbateko hori bezeroari fakturatuko zaion hitzarmenaren balioa da, kontratu lerro honi lotutako lan osagai guztiengatik. Denboraren eta materialaren kontratuaren lerroan, zenbateko hori bezeroari fakturatuko zaion aurreikusitako balioa da, kontratu lerro honi lotutako lan osagai guztiengatik. Aurrekontu batetik sortutako proiektu kontratu baterako, aurrekontuaren lerroaren dagokion balio batetik kopiatzen da. Proiektuan oinarritutako kontratu lerro batek lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta kontratuaren lerroaren xehetasunen zenbatekoaren arabera laburbiltzen da. | Kontratu-lerroak lerroaren xehetasunak dituenean, balio hori alda daiteke lerroaren xehetasunen zenbatekoak aldatuta. Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarrien gaineko zerga aurretik zenbatekoa sortzeko erabiltzen da. |
| **Aurreikusitako zerga** | Erabiltzaileak eremu hau alda dezake, aurreikusitako zergaren zenbatekoa kontratu lerroan sartzeko. Proiektuan oinarritutako kontratu lerro batek lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta kontratuaren lerroaren xehetasunen zerga-zenbatekoaren arabera laburbiltzen da. | Kontratu-lerroak lerroaren xehetasunak dituenean, balio hori alda daiteke lerroaren xehetasunen zerga-zenbatekoak aldatuta. Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarrien gaineko zerga sortzeko erabiltzen da. |
| **Kontratatutako zenbatekoa, zergaren ondoren** | Kontratatuaren lerroaren zenbatekoa zergaren ondoren. Eremu hau irakurtzeko soilik da eta honela kalkulatzen da **Kontratatutako zenbatekoa + Zerga**. | Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarriak sortzeko erabiltzen da. |
| **Ez gainditzeko muga** | Erabiltzaileak eremu hau edita dezake eta fakturazio metodoa denbora eta material gisa ezarrita duten proiektuetan oinarritutako kontratu lerroetan bakarrik dago erabilgarri. | Erabiltzaileak eremu hau edita dezake. Denboraz eta materialaz egindako benetako batek kontratu-lerro hau denboraz eta materialez aipatzen duenean, benetako zenbatekoa kontratu-lerroan gainditu ezin den mugaren arabera ebaluatzen da. Ebaluazio hori dagoeneko gastatutako eta konprometitutako zenbatekoak kontabilizatu ondoren amaitzen da. |
| **Bezeroaren aurrekontua** | Eremu hau editagarria da eta aurrekontuaren lerroaren dagokion balio batetik kopiatzen da kontratua eskaintza batetik sortu bada. | Eremu hau informaziorako bakarrik erabiltzen da eta ez du beheranzko esangurarik. |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a>Proiektuetan oinarritutako kontratu lerroen Orokorreko fitxako aukeren baliozkotze arauak

1. araua: **Zereginak barne** eremua hutsik dago edo ezarrita dago **Proiektuaren zeregin guztiak**, proiektuaren zeregin guztiak kontratu lerroan sartzen dira.

2. araua: **Zereginak barne** eremua hutsik dago edo esplizituki ezarrita dago **Proiektuaren zeregin guztiak**, proiektu bat eta transakzio klase jakin bat proiektuan oinarritutako kontratu lerro batean bakarrik sar daitezke.

3. araua: **Zereginak barne** eremua ezarrita dago **Hautatutako proiektuak soilik**, proiektu bat eta transakzio klase jakin bat kontratuaren proiektuan oinarritutako kontratuaren hainbat lerrotan sar daitezke.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p>
                    <strong>Kontratua</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>Kontratuaren lerroa</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="67" valign="top">
                <p>
                    <strong>Gehitutako zereginak</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Idatzi denbora</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>Idatzi gastua</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Materialak barne</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Gehitu</strong>
                </p>
                <p>
                    <strong>Tasa</strong>
                </p>
            </td>
            <td width="53" valign="top">
                <p>
                    <strong>Baliozkoa/Baliogabea da</strong>
                </p>
            </td>
            <td width="250" valign="top">
                <p>
                    <strong>Arrazoia</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
2. araua haustea. P1 proiektuaren denbora, gastuak, materialak eta tasak Kontratuaren lerroetan, CL1 eta CL2 barne daude.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
2. araua haustea. P1 proiektuaren denbora, materialak eta tasak Kontratuaren lerroetan, CL1 eta CL2 barne daude.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
P1 proiektuaren denbora, materialak eta tasak CL1 barne daude.
                </p>
                <ul>
                    <li>
P1 proiektuaren gastuak QL2n sartzen dira.
                    </li>
                </ul>
                <p>
Kontratuaren lerro bakoitzean sartzen denaren gainetik ez dago gainjartzerik eta, beraz, baliozkoa da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
No </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Baliogabea da </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
2. araua haustea </p>
                <p>
P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materialak, gastuak eta tasak sartzen dira.
                </p>
                <p>
CL2-k P1 proiektu osorako denbora, materialak, gastuak eta tasak biltzen ditu eta, beraz, C1-en sartutakoarekin gainjartzen da.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hutsik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
Baliozkoa </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
3. arauaren arabera </p>
                <p>
P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak, materialak eta tasak sartzen dira.
                </p>
                <p>
CL2k barne ditu P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira.
                </p>
                <p>
Balidazio osagarri bakarra CL1-eko zereginen azpimultzoaren inguruan kokatzen da, CL2-ren zereginen azpimultzoaren desberdina dela gainjartzerik ez dagoela ziurtatzeko. Sistemak zereginak lotzen dituenean egiten du.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
A1 </p>
            </td>
            <td width="67" valign="top">
                <p>
Hautatutako zereginak soilik </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
