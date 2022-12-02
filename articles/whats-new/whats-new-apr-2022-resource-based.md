---
title: 2022ko apirileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Artikulu honek 2022eko apirileko baliabideetan/izakinik ezan oinarritutako egoeretarako Microsoft Dynamics 365 Project Operations bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 04/08/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 999006b2c2fe2b31d6e47910a3f1a55cab415f0e
ms.sourcegitcommit: 5c971b15295046b3c92ff6638dd1352129f1c390
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/01/2022
ms.locfileid: "9110869"
---
# <a name="whats-new-april-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>2022ko apirileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.41.0.45
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.26 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Erosketa-kategoriak erabili daitezke proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin. Informazio gehiago [Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin](../procurement/configure-procurement-categories.md).

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo taulan 2022ko martxoko Project Operations aldatu edo gehitu diren idazketa bikoitzeko mapak agertzen dira.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| -------------- | ------------------- | ------------|
| Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn\_projectvendorinvoicelines) | 1.0.0.4 | Mapa honek onartzen du erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin erabiltzea. |

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| ------------ | ---------------- | -------------- |
| Denbora eta gastua | 2573900 | **Onarpen Modernoa** funtzioak lehenespenez gaituta egon behar du. |
| Fakturazioa eta prezioak | 2603313 | Bikoiztutako erregistro-errore bat konpondu da, produktu bat duten aurrekontu eta kontratu lerroak gehitzea eragozten zuena. |
| Inplementazioa eta konfigurazioa | 2611368 | Bezeroek soluzioan bost entitate pertsonalizatu gehitzeko gai izan behar dute aplikazioen diseinatzaile modernoa erabiliz. |
| Denbora eta gastua | 2628285 | Denbora-sarrera inportatzean baliabide-kategoria egokia ezartzeko gaitasunari eragiten zion arazo bat konpondu da. |
|   Abaguneen kudeaketa| 2628815 | Eguneratu aipu-lerroaren xehetasunen deskribapenaren karaktere-muga ataza-gaiaren karaktere-mugarekin bat etor dadin, gaiak 100 karaktere baino luzeagoak diren zereginetarako inportazioak arrakasta izan dezan. |
| Denbora eta gastua| 2629547 | **Nork bidalia** proiektuaren onespenen eremuak erregistroa aurkeztu duen erabiltzailea adierazi behar du. |
| Denbora eta gastua| 2629865 | **Kopiatu kategoria** proiektuak kopiatzen direnean zereginei buruzko eremua. |
| Denbora eta gastua| 2636463 | Onarpenen iragazkiak onarpen-inprimaki modernoetan konpondu dira. |
| Proiektuaren antolaketa eta jarraipena | 2648300 | Proiektuaren jabea aldatzea eragozten duen arazo bat konpondu da. |
| Fakturazioa eta prezioak | 2563000 | Ez dira onartu behar fakturatu gabeko salmenta baterako egunkari-lerroak, moneta kontratuaren moneta desberdina den. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Project Management and Accounting Dynamics 365 Finance-n

Eguneratze honetan jasotako arazoen konponketen inguruko informazioa lortzeko, hasi saioa Microsoft Dynamics Lifecycle Services-en (LCS) eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864).
