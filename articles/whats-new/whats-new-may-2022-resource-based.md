---
title: Nobedadeak 2022ko maiatza - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak
description: Gai honek Microsoft-en 2022ko maiatzeko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du Dynamics 365 Project Operations baliabideetan/ez hornituta oinarritutako eszenatokietarako.
author: sigitac
ms.date: 05/02/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d3ac63f0d33d36cc5b6d4cea3ab8167e5974cfe6
ms.sourcegitcommit: 7e419a5f73f80fa887084e3b212c90586fc397dd
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/05/2022
ms.locfileid: "8710105"
---
# <a name="whats-new-may-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Nobedadeak 2022ko maiatza - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft-en osagai eta bertsio hauei dagokie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.42.0.70
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.26 bertsioan

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta Finantza irtenbidearen bertsioa. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa bat pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa bikoitzeko arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak
### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Baliabideen kudeaketa | 2634019 | Enpresen baliozkotzeetarako errore-mezuak hobetu dira taldekide generikoak baliabide gisa gehitzean. |
| Proiektuaren antolaketa eta jarraipena | 2648515 | Eguneratze mugatuak **jabea**, **·**, eta **egoera** programazio entitateetan. |
| Fakturazioa eta prezioak | 2653167 | The **Estimazioak** sareta hamartarren bereizleak formatu ezarpenak jarraitu behar ditu **Aukera pertsonalak**. |
| Fakturazioa eta prezioak| 2662251 | Baloreak **Unitatea zuzendua** eta **Unitate taldea** eremuak lehenetsitako materialaren estimazioetan erregistroak sortzean. |
| Fakturazioa eta prezioak| 2571408 | Fakturatu gabeko salmenten errealak faktura-zirriborro bat sortzerakoan fakturaren ID proforma batekin zigilatzen dira. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance-en

Eguneratze honetan sartzen diren akatsen konponketei buruzko informazioa lortzeko, hasi saioa hemen Microsoft Dynamics Lifecycle Services (LCS) eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864).
