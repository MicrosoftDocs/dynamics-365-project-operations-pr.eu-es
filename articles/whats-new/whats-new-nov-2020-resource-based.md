---
title: 2020ko azaroko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Artikulu honetan, Project Operations-en 2020ko azaroko bertsioan eskuragarri dauden kalitate-eguneratzeei buruzko informazioa ematen da, baliabideetan oinarritutako edo biltegiratu gabeko agertokietarako.
author: sigitac
ms.date: 10/30/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: b98c968a040c14f4d11c350885e2cbb984596c48
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923403"
---
# <a name="whats-new-november-2020---project-operations-for-resourcenon-stocked-based-scenarios"></a>2020ko azaroko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu hau honako hauei aplikatzen zaie Dynamics 365 Project Operations osagaiak eta bertsioak:

- Project Operations CDS ingurunearen 4.4.0.70 bertsioa
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance bertsioa 10.0.14 bertsioa

## <a name="updates-to-project-operations-for-resource-non-stocked-based-scenarios"></a>Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations-en eguneratzeak

### <a name="project-operations-on-cds"></a>Project Operations CDSn

| Ezaugarrien eremua                 | Erreferentzia-zenbakia | Kalitatearen eguneratzea                                                                                                                                                                    |
|------------------------------|------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   Abaguneen kudeaketa       | 2036993          | Aurrekontu lerroa eta baliabideak esleitzeko kontratu lerroak aurrekontu irabazleetan eguneratzen dira aurrekontu lerro mota dagoenean **Zeregin guztiak**.                                                 |
| Fakturazioa eta prezioak          | 2070392          | Fakturan proiektuen kontratu lerroak aldi bakoitzean handitzen dira **Freskatu fakturen eragiketak** hautatuta dago.                                                                         |
| Proiektuaren antolaketa             | 2043336          | Ezin da proiektuko taldeko kideen erregistroa ezabatu.                                                                                                                                  |
| Proiektuaren antolaketa             | 2046013          | Portaera inkoherentea Estimazioen etiketako zutabeetarako karga garaian vs. denbora-fase motaren aldaketan.                                                                                   |
| Proiektuaren antolaketa             | 2046647          | Hasierako eta amaierako orduak ordubete itxita daude proiektuaren taldeko kideek baliabide eskakizunak sortzen dituztenean.                                                                      |
| Proiektuaren antolaketa             | 2053879          | (Datozen CDS hedapenaren arabera) PublishUnassignedAssignments-ek zeregina gordetzeko saiakera hausten du errorea, "ConditionOperator.In-i emandako balioa hutsik dagoenean".                       |
| Proiektuaren antolaketa             | 2055501          | **Proiektuaren hasiera-data** hutsik utziz gero, huts egiten du ordutegian.                                                                                                      |
| Proiektuaren antolaketa             | 2066817          | Ezin da baliabide generiko bat sortu jendeko hautatzailea erabiliz **Zereginak** fitxa.                                                                                                   |
| Proiektuaren antolaketa             | 2067034          | **Ikusi xehetasunak** botoia ez dago erabilgarri **Atazaren xehetasunak** orrialdea.                                                                                                       |
| Baliabideen kudeaketa          | 2046667          | Taldekide generikoak ez dira ezabatzen baliabide guztiak bete ondoren ere.                                                                                                    |
| Denbora eta gastuen sarrera bizkorra | 2047499          | **Berria** Denbora sartzeko orrian botoiak irekitzen du **Posta elektronikoaren sinadura berria** orrialdea.                                                                                               |
| Denbora eta gastuen sarrera bizkorra | 2059859          | Gastu sarrera sortzerakoan ustekabeko leihoa irekitzen da.                                                                                                                         |
| Beste batzuk                        | 2044181          | (Erosketa agindua desinstalatzen) msdyn_ProjectServiceCore_Patch eta msdyn Project zerbitzuaren oinarrizko irtenbideak desinstalatzen saiatzean, "Grabaketa ez dago erabilgarri" errorea gertatzen da.  |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance-en

| Ezaugarrien eremua        | Erreferentzia-zenbakia | Kalitatearen eguneratzea                                                                                                                                                            |
|---------------------|------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Diru-sarreren aitorpena | [451662](https://fix.lcs.dynamics.com/Issue/Details/?bugId=451662)           | Proiektuaren kalkuluen ehuneko osoa okerra da kontratuak atzerriko moneta erabiltzen duenean eta lanaren aurrerapenaren ehunekoa metodo osorako.                     |
| Diru-sarreren aitorpena | [469894](https://fix.lcs.dynamics.com/Issue/Details/?bugId=469894)           | Ezin dira aurrekontuak argitaratu **Benetako kostua** osatze metodoa.                                                                                                    |
| Diru-sarreren aitorpena | [485439](https://fix.lcs.dynamics.com/Issue/Details/?bugId=485439)           | Ezabatzeak huts egiten du bonuaren desoreka akats baten ondorioz, konpainiaren moneta eta transakzioaren moneta desberdinak direnean.                                              |
| Gastuen kudeaketa  | [456882](https://fix.lcs.dynamics.com/Issue/Details/?bugId=456822)           | Administratzaile ez diren erabiltzaileentzat, adibidez, gastu lerro zutabeen bilaketa balioak **Proiektuaren IDa** eta **Gastuen kategoria** ez dira datuen konektorearen markoan behar bezala erakusten. |
| Gastuen kudeaketa  | [469300](https://fix.lcs.dynamics.com/Issue/Details/?bugId=469300)           | Linearen propietate lehenetsia ez da Gastu kategorietan agertzen.                                                                                                         |
| Gastuen kudeaketa  | [469302](https://fix.lcs.dynamics.com/Issue/Details/?bugId=469302)           | Gastuen integrazioak gastuaren txosteneko lineako ondasuna sartu behar du.                                                                                             |
| Fakturazioa           | [462499](https://fix.lcs.dynamics.com/Issue/Details/?bugId=462499)           | Ezin dira proiektuaren faktura proposamenak bidali, FD konbinazioa balioztatu ez dela dioen errore mezu bat delako.                                                    |
| Fakturazioa           | [470614](https://fix.lcs.dynamics.com/Issue/Details/?bugId=470614)           | Ezin dira ikusi transakzioak **faktura** xehetasunen orria.                                                                                                              |
| Fakturazioa           | [480070](https://fix.lcs.dynamics.com/Issue/Details/?bugId=480070)           | Faktura proposamenen lerroak ezabatu daitezke.                                                                                                                                  |
| Proiektuaren kontabilitatea  | [470293](https://fix.lcs.dynamics.com/Issue/Details/?bugId=470293)           | **Iragarpena** menuko elementuak ez dira ikusgai **Proiektuak** zerrenda orria.                                                                                                   |
| Proiektuaren kontabilitatea  | [475873](https://fix.lcs.dynamics.com/Issue/Details/?bugId=475873)           | Ezin da ireki **Proiektuaren adierazpena**   > **Transakzioak eta aurreikuspenak**.                                                                                                       |
| Proiektuaren kontabilitatea  | [475879](https://fix.lcs.dynamics.com/Issue/Details/?bugId=475879)           | **Doitu kontabilitatea** ez dago gaituta fakturatutako proiektuen transakzioetarako.                                                                                                  |
| Proiektuaren kontabilitatea  | [480962](https://fix.lcs.dynamics.com/Issue/Details/?bugId=480962)           | Kontabilitate xehetasunak ez daude **ProjCDSActualsImport** mahaia **Integrazioa** aldizkaria argitaratzen da.                                                  |
| Proiektuaren kontabilitatea  | [482558](https://fix.lcs.dynamics.com/Issue/Details/?bugId=482558)           | Proiektuaren iragarpen sarrera bikoiztu egiten da baliabideen esleipena kendu eta gero irakurtzean.                                                                            |
| Proiektuaren kontabilitatea  | [502019](https://fix.lcs.dynamics.com/Issue/Details/?bugId=502019)           | Project ID esteka hautatzeak ez du CDS esteka sakonaren URLa irekitzen.                                                                                                         |
| Proiektuaren kontabilitatea  | [505458](https://fix.lcs.dynamics.com/Issue/Details/?bugId=505458)           | Ezin da eguneko hasiera data eguneratu CDS zerbitzuan.                                                                                                                           |
| Proiektuaren kontabilitatea  | [510041](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510041)           | Funtzioa gaituta, kontratu lerro anitz ez dira posible CDS integraziorik gabe.                                                                                   |

### <a name="regulatory-updates"></a>Araudiaren eguneratzeak
Finantza eta Operazio aplikazioen arauzko eguneratzeei buruzko informazio gehiago lortzeko, ikus [Araudiaren eguneraketak](/dynamics365/finance/localizations/regulatory-updates). LCS-en saioa hasi eta aurreikusitako arauzko eguneratzeak ikus ditzakezu Arazoak bilatzeko tresna erabiliz. Arazoen bilaketak herrialdearen, eginbide motaren eta askapenaren arabera bilatzeko aukera ematen du.


[!INCLUDE[footer-include](../includes/footer-banner.md)]