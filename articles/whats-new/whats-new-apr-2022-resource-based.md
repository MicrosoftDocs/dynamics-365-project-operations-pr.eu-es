---
title: Nobedadeak 2022ko apirila - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak
description: Gai honek Microsoft-en 2022ko apirileko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du Dynamics 365 Project Operations baliabideetan/ez hornituta oinarritutako eszenatokietarako.
author: sigitac
ms.date: 04/08/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: dc713e7a0dd6993e38ce3e3b2ba19f796a6f4773
ms.sourcegitcommit: 9916f536a71b6a0078297402564ac79308ec6890
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/18/2022
ms.locfileid: "8613310"
---
# <a name="whats-new-april-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Nobedadeak 2022ko apirila - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft-en osagai eta bertsio hauei dagokie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.41.0.45
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.26 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Kontratazio-kategoriak proiektuko erosketa-aginduetan eta saltzaileen zain dauden fakturetan erabil daitezke. Informazio gehiagorako, ikus [Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin](configure-procurement-categories.md).

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ondorengo taulak Project Operations-en 2022ko martxoko bertsioan aldatu edo gehitu diren idazketa bikoitzeko mapak erakusten ditu.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| -------------- | ------------------- | ------------|
| Project Operations integrazio proiektua hornitzaile faktura lerro esportatzeko entitatea msdyn\_ proiektuenhornitzailefakturalerroak | 1.0.0.4 | Mapa honek erosketa-eskaerekin eta saltzaileen zain dauden fakturekin erosketa-kategoriak erabiltzea onartzen du. |

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta Finantza irtenbidearen bertsioa. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa bat pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa bikoitzeko arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| ------------ | ---------------- | -------------- |
| Denbora eta gastua | 2573900 | The **Onarpen Modernoa** funtzioak lehenespenez gaituta egon behar du. |
| Fakturazioa eta prezioak | 2603313 | Produktu bat duten aurrekontu- eta kontratu-lerroak gehitzea eragozten zuen bikoiztutako erregistro-errore bat konpondu da. |
| Inplementazioa eta konfigurazioa | 2611368 | Bezeroek soluzioari bost entitate pertsonalizatu gehitzeko gai izan behar dute aplikazioen diseinatzaile modernoa erabiliz. |
| Denbora eta gastua | 2628285 | Denbora-sarrera inportatzean baliabide-kategoria egokia ezartzeko gaitasunari eragiten zion arazo bat konpondu da. |
|   Abaguneen kudeaketa| 2628815 | Eguneratu aipu-lerroaren xehetasunen deskribapenaren karaktere-muga ataza-gaiaren karaktere-mugarekin bat etor dadin, gaiak 100 karaktere baino luzeagoak diren zereginetarako inportazioak arrakasta izan dezan. |
| Denbora eta gastua| 2629547 | The **Nork bidalia** proiektuaren onespenen eremuak erregistroa aurkeztu duen erabiltzailea adierazi behar du. |
| Denbora eta gastua| 2629865 | The **Kopiatu kategoria** proiektuak kopiatzen direnean zereginei buruzko eremua. |
| Denbora eta gastua| 2636463 | Onarpenen iragazkiak onarpen-inprimaki modernoetan konpondu dira. |
| Proiektuaren antolaketa eta jarraipena | 2648300 | Proiektuaren jabea aldatzea eragozten duen arazo bat konpondu da. |
| Fakturazioa eta prezioak | 2563000 | Ez dira onartu behar fakturatu gabeko salmenta baterako egunkari-lerroak, moneta kontratuaren moneta desberdina den. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance-en

Eguneratze honetan sartzen diren akatsen konponketei buruzko informazioa lortzeko, hasi saioa hemen Microsoft Dynamics Lifecycle Services (LCS) eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864).
