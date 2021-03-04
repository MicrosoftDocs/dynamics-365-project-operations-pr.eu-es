---
title: 2020ko azaroko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Gai honek informazioa eskaintzen du 2020ko azaroan Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruz, baliabideetan / stockean oinarritutako egoeretarako.
author: sigitac
manager: Annbe
ms.date: 10/30/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c7ec9360401bf214ae867769b0e48e545a6bad48
ms.sourcegitcommit: 64d0de964a9b66c015ffcf1db62cbb6216cb3187
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/03/2020
ms.locfileid: "4367250"
---
# <a name="whats-new-november-2020---project-operations-for-resourcenon-stocked-based-scenarios"></a>2020ko azaroko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations CDS ingurunearen 4.4.0.70 bertsioa
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.14 bertsioa

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

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Dynamics 365 Finance-n

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
Eguneratze arautzaileei buruzko informazioa lortzeko Finance and Operations aplikazioak, ikusi [Araudiaren eguneratzeak](https://docs.microsoft.com/dynamics365/finance/localizations/regulatory-updates). LCS-en saioa hasi eta aurreikusitako arauzko eguneratzeak ikus ditzakezu Arazoak bilatzeko tresna erabiliz. Arazoen bilaketak herrialdearen, eginbide motaren eta askapenaren arabera bilatzeko aukera ematen du.


[!INCLUDE[footer-include](../includes/footer-banner.md)]