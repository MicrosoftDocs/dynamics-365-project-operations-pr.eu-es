---
title: 2022ko ekaina berritasunak - Baliabideetan oinarritutako eszenatokietarako proiektu-eragiketak/biltegiratu gabeak
description: Artikulu honek Microsoften Dynamics 365 Project Operations 2022ko ekaineko bertsioan eskuragarri dauden kalitate-eguneratzeei buruzko informazioa ematen du, biltegiratutako baliabide/ez-biltegietan oinarritutako agertokietarako.
author: sigitac
ms.date: 06/03/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: fde1f0be42eecfc5ee809cb9b2191d3aeae57131
ms.sourcegitcommit: 51745acac29dfacba43a4003d86baff4d6ca2fb8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/14/2022
ms.locfileid: "8959596"
---
# <a name="whats-new-june-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>2022ko ekaina berritasunak - Baliabideetan oinarritutako eszenatokietarako proiektu-eragiketak/biltegiratu gabeak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu hau Microsoft-en osagai eta bertsio hauei aplikatzen zaie Dynamics 365 Project Operations:

- Proiektu-eragiketak ingurune 4.43.0.77 bertsio batean Dataverse
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.27 bertsioa

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo taulan, Project Operations-en 2022ko ekaineko bertsioan aldatu edo erantsi diren idazkera dualeko mapak erakusten dira.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| --- | --- | --- |
| Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices) | 1.0.0.1 | Heredatutako eremua erabilerarik gabe utzi zuen eta eremu berrira joan zen hornitzailearen fakturaren egoeraren jarraipena egiteko. |

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta Finantza irtenbidearen bertsioa. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa bat pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa bikoitzeko arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Azpikontratazioa | 2708885 | Erabiltzaile batek baliabide erreserbagarrien erreserba-erregistro bat sortzen duenean agertzen den errore-mezua zuzendu da, eta bertan ez da baliabide erreserbagarririk betetzen. |
| Proiektuaren antolaketa eta jarraipena | 2629441 | Lan-fluxua aktibatzeko logika zuzendu da, proiektuaren lanak eguneratzen direnean bukle amaigabea saihesten laguntzeko. |
| Denbora eta gastua | 2641209 | Esleipen/erreserben denbora-sarreraren inportazioek baliabide erreserbagarrien erreferentzia bat gorde behar dute. |
| Proiektuaren antolaketa eta jarraipena | 2651148 | Proiektuaren buruak babestuta egon behar du.|
| Proiektuaren antolaketa eta jarraipena | 2653145 | Balidazioak gehitu ziren, bere izenean baliozkoak ez diren karaktereak izango dituen proiektu-erregistrorik sortu ezin dela bermatzeko. |
| Denbora eta gastua | 2654710 | **Orria entzun Orria entzun Aprobazioak**. |
| Fakturazioa eta prezioak | 2667805 | Balidazioak gehitu ziren fakturatutako salmenten benetako datuak sortzen ez laguntzeko, fakturatu gabeko salmenten benetako daturik ez badago. |
| Fakturazioa eta prezioak | 2668378 | Balidazioak gehitu ziren, prezio pertsonalizatuen dimentsio bat ez osatzeko, izen logiko bat eta landa-izen bat osatzen ez bada. |
| Azpikontratazioa | 2677485 | Hornitzailearen faktura-lineen eskritura dualaren maparen xede-bertsioa eguneratu da. |
| Denbora eta gastua | 2700428 | Onarpenen logika hobetu da, proiekturako beste onarpen-multzo batzuk prozesatu ahal izango direla bermatzeko, baita onarpen-multzoetako bat sistemaren lanetan trabatuta badago ere. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuen kudeaketa eta kontabilitatea Finantzetan

Eguneratze honetan sartzen diren akatsen zuzenketei buruzko informazioa lortzeko, hasi Lifecycle Services (LCS) saioa Microsoft Dynamics eta kontsulta ezazu [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=673271).
