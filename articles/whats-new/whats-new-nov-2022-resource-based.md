---
title: Nobedadeak 2022ko azaroa - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak
description: Artikulu honek Microsoft Dynamics 365 Project Operations ren 2022ko azaroko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du baliabideetan edo hornituta ez dauden agertokietarako.
author: ryansandness
ms.date: 12/16/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ryansandness
ms.openlocfilehash: 509e303aeb0567627590fd89c6888b59a414c6f1
ms.sourcegitcommit: 952fcefe33de192ad48f4108c3adbe658fd7b94f
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/08/2022
ms.locfileid: "9831119"
---
# <a name="whats-new-november-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Nobedadeak 2022ko azaroa - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.58.0.119
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.30 bertsioan

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2781818 | Gakoa ez da aurkitu errorea materialaren erabileraren erregistroaren prezio lehenetsia ezartzean. |
| Fakturazioa eta prezioak | 2922373 | Ezin da lotu aurrekontu-lerroa aurrekontu galdu gisa itxi den proiektuarekin. |
| Fakturazioa eta prezioak | 2943206 | **Kontratu-lerroa** eremua Proiektuaren Entitatean Aukerakoa izan beharko litzateke. |
| Fakturazioa eta prezioak | 2953182 | Hobetu errore-mezua zuzenketa-fakturetarako.|
| Fakturazioa eta prezioak | 2959500 | Ezin da aurrekontu-lerroa lotu galdutako aurrekontu batekin dagoeneko lotuta dagoen proiektu-zeregin bati.|
| Fakturazioa eta prezioak | 2959560 | "Bezero hau proiektuaren kontratuan dago jada" mezua jaso da aurrekontua ixtean toki jakin batzuetan irabazi bezala. |
| Fakturazioa eta prezioak | 3031727 | Baliabideen esleipenek huts egin dute "msdyn_Company" derrigorrezko eremua errorearekin. |
| Fakturazioa eta prezioak | 3036905 | Enpresa jabea ez da inoiz hasieratzen ProjectTeamMember-en. |
| Abaguneen kudeaketa | 2763519 | Erreferentzia nuluaren errorea EnsureProjectContractAllowsUpdates-en. |
| Abaguneen kudeaketa | 2783798 | Proiektuaren estimazioak aurrekontu-lerroan inportatzean, zereginen deskribapenak falta dira gastuen eta materialen estimazioetarako.|
| Abaguneen kudeaketa | 2988635 | Hobetu errore-mezuaren deskribapena Bezeroa aurrekontuan ezabatzean. |
| Abaguneen kudeaketa | 3001191 | Ezin da aurrekontua sortu Opportunity-tik non fakturazio-metodoa nulu gisa zehaztuta dagoen. |
| Bertsio-berritu | 3012324 | Proiektuaren bihurketak huts egin du bere izenean Tab bezalako kontrol karaktereak dituen proiektu batean. || Proiektuaren antolaketa eta jarraipena | 2790384 | Pending OperationSet denbora-muga laburregia da. |
| Proiektuaren antolaketa eta jarraipena | 3044275 | Lokalizazioa falta da: missingProjectSchedulerErrorMessage. |
| Proiektuaren antolaketa eta jarraipena | 3044277 | Project Recon sareta ez da kargatzen programatzailea ezarri gabe dagoenean.|
| Baliabideen kudeaketa | 2943153 | Eguneratu Jarraipena fitxa Iraupenerako bi hamartar erakusteko.|
| Azpikontratazioa | 2932774 | Saltzaileen faktura-lerroa irakurtzeko soilik errorea gaizki botatzean. |
| Azpikontratazioa | 2939556 | Saltzaileen fakturaren goiburuaren egoera ez da ezarri behar Zirriborroa linean ezabatzea aktibo ez badago. |
| Denbora eta gastua | 2939998 | Hartu TESA bertsio berria ProjOps-en. |


### <a name="project-management-and-accounting-in-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Finantzan

Eguneratze honetan jasotako arazoen konponketen inguruko informazioa lortzeko, hasi saioa Microsoft Dynamics Lifecycle Services-en eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=745468).
