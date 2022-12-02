---
title: 2022eko abuztuko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations
description: Artikulu honek 2022eko abuztuko baliabideetan/izakinik ezan oinarritutako egoeretarako Microsoft Dynamics 365 Project Operations bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 4042dca72a33f48e04e51af2a3cfd2da83146afd
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/02/2022
ms.locfileid: "9403841"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>2022eko abuztuko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.45.0.53
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.28 bertsioan

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
|   Abaguneen kudeaketa | 2762089 | Akatsa kudeatzea kontratua ixtean galdutzat jotzea erakundean gordetze automatikoa desgaituta badago.|
|Proiektuaren antolaketa eta jarraipena | 2767841 | Telemetria eguneratzeak Proiektuaren entitatea Sortu edo Eguneratu eszenatokiak.|
|Fakturazioa eta prezioak | 2771072 | Erreferentzia nuluaren salbuespenen kudeaketa aurrekontua irabazten duzun bitartean.|
|Fakturazioa eta prezioak | 2844181 |Korrelazio-id bat lortzean eta faktura bat sortzea blokeatzea.|
|Fakturazioa eta prezioak | 2852836 | CEn sortu eta onartutako enpresen arteko gastuak falta dira.|


### <a name="project-management-and-accounting-in-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Finantzan

Eguneratze honetan jasotako arazoen konponketen inguruko informazioa lortzeko, hasi saioa Microsoft Dynamics Lifecycle Services-en (LCS) eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
