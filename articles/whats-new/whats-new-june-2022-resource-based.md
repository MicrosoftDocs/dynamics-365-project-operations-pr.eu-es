---
title: Nobedadeak 2022ko ekainean - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak
description: Artikulu honek Microsoft-en 2022ko ekaineko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du Dynamics 365 Project Operations baliabideetan/ez hornituta oinarritutako eszenatokietarako.
author: sigitac
ms.date: 06/03/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 32bc7793c5a0ee8c04272d3ffcbd290b39fce4cc
ms.sourcegitcommit: 7772d72a7c96a44ffb23369f8ffb436813449239
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/20/2022
ms.locfileid: "9031316"
---
# <a name="whats-new-june-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Nobedadeak 2022ko ekainean - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu hau Microsoft-en osagai eta bertsio hauei aplikatzen zaie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.43.0.77 edo 4.43.0.119
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.27 bertsioan

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo taulak Project Operations 2022ko ekaineko bertsioan aldatu edo gehitu diren idazketa bikoitzeko mapak erakusten ditu.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| --- | --- | --- |
| Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices) | 1.0.0.1 | Eremu zaharra zaharkituta eta eremu berriarekin mapatu da hornitzaileen fakturen egoeraren jarraipena egiteko. |

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta Finantza irtenbidearen bertsioa. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa bikoitzeko arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Azpikontratazioa | 2708885 | Erabiltzaileak erreserba daitezkeen baliabideen erreserbaren goiburuko erregistroa sortzen denean agertzen den errore-mezua konpondu da, non erreserba daitekeen baliabiderik betetzen ez den. |
| Proiektuaren antolaketa eta jarraipena | 2629441 | Lan-fluxua abiarazteko logika zuzendu da proiektuko zereginak eguneratzen direnean begizta infinitua saihesteko. |
| Denbora eta gastua | 2641209 | Esleipenetatik/erreserbatik denbora-sarrera inportatzeak erreserba daitezkeen baliabideen erreferentzia gorde behar du. |
| Proiektuaren antolaketa eta jarraipena | 2651148 | Proiektuaren dokumentuaren goiburua zaindu behar da.|
| Proiektuaren antolaketa eta jarraipena | 2653145 | Balidazioak gehitu dira bere izenan balio ez duten karaktereak dituen proiektu-erregistro bat sortu ezin dela ziurtatzeko. |
| Denbora eta gastua | 2654710 | Iragazkia zuzendu du **Onarpenak** orrialdea. |
| Fakturazioa eta prezioak | 2667805 | Balidazioak gehitu dira fakturatutako salmenta errealak sortzea saihesteko, fakturatu gabeko salmenten benetako babesa existitzen ez bada. |
| Fakturazioa eta prezioak | 2668378 | Balidazioak gehitu dira prezio pertsonalizatuen dimentsio bat gehitzea saihesteko, izen logiko bat eta eremu-izen bat bete ezean. |
| Azpikontratazioa | 2677485 | Saltzaileen faktura-lerroen helburuko bertsioa eguneratu da idazketa bikoitzeko mapa. |
| Denbora eta gastua | 2700428 | Onarpen-logika hobetu da, proiekturako beste onarpen-multzo batzuk prozesatu daitezkeela ziurtatzeko, nahiz eta onarpen-multzo bat sistemako lanetan itsatsita egon. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuen kudeaketa eta kontabilitatea Finantzetan

Eguneratze honetan sartzen diren akatsen konponketei buruzko informazioa lortzeko, hasi saioa hemen Microsoft Dynamics Lifecycle Services (LCS) eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=673271).
