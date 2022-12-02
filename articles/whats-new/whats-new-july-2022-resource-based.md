---
title: 2022eko uztaileko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations
description: Artikulu honek 2022eko uztaileko baliabideetan/izakinik ezan oinarritutako egoeretarako Microsoft Dynamics 365 Project Operations bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: e63b29741dbaa400a2176ff8b4c35c6d64dfeab4
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/02/2022
ms.locfileid: "9403936"
---
# <a name="whats-new-july-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>2022eko uztaileko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.44.0.22
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.28 bertsioan

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Inplementazioa eta konfigurazioa | 2761472 | Project Operations instalazio-errore bat kudeatzen da. |
| Fakturazioa eta prezioak | 2746940 | Azpikontratuaren lerroaren izenak gehienez 100 karaktere izan behar ditu. |
| Fakturazioa eta prezioak | 2739162 | Bezeroek zinta-botoiak ikusteko gai izan behar dute benetako sareta-ikuspegian. |
| Proiektuaren antolaketa eta jarraipena | 2730318 | Proiektuaren gaian onartzen ez diren karaktereen baliozkotze eguneratua. |
| Fakturazioa eta prezioak | 2705361 | Mugarrian fakturatutako salmenta errealak proiektuaren jarraipenaren eremuetan sartu behar dira. |
| Fakturazioa eta prezioak | 2675880 | Proiektu bat lan-oinarritutako ez den kontratu-lerro bati lotzea eragotzi. |
| Fakturazioa eta prezioak | 2664396 | Aurrekontu prezioen zerrenda aurrekonturik gabe gordetzen bada, aurrekontua ezin dela hutsik egon dioen errore bat egon behar da. |
| Fakturazioa eta prezioak | 2184019 | **Zereginen Oinarritutako Fakturazioa** fitxa ez da agertu behar babes-kontraturik edo aurrekonturik ez duten proiektuetarako. |
| Denbora eta gastua | 2754459 | Hodei-fluxua errepikatzen den programazioa inaktibo dagoenean, erakutsi bannerra eta saihestu prozesamendu asinkronikoa. |
| Fakturazioa eta prezioak | 2724391 | Salbuespen okerra botatzen da proiektuaren kontratuaren zatiketaren fakturazio-arau bezeroaren balio bat falta denean. |
| Fakturazioa eta prezioak | 2708638 | Erregistrorik ez da aurkitu sareta-bilaketa erabiliz Materialen erabilerak eta Materialen erabilerak onartzeak atalean.|
| Fakturazioa eta prezioak | 2686977 | Saihestu faktura-lerroaren baliozkotzea fakturak sortzean. |
| Fakturazioa eta prezioak | 2683032 | Kobratzeko rolak eta kategoriak kopiatzea ez da 5.000 erregistrotik gora eskalatzen.|
| Fakturazioa eta prezioak | 2673363 | Proiektuko kostu-kontsumoaren % hondatuta dago proiektu baterako esfortzuak eta gastuak estimazioak eta benetakoak daudenean. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Finantzan

Eguneratze honetan jasotako arazoen konponketen inguruko informazioa lortzeko, hasi saioa Microsoft Dynamics Lifecycle Services-en (LCS) eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).

## <a name="features-turned-on-by-default-in-upcoming-release"></a>Eginbideak lehenespenez aktibatuta daude hurrengo bertsioan

Hurrengo taulan 10.0.29 bertsioan lehenespenez aktibatuta dauden funtzioak zerrendatzen dira. Automatikoki aktibatu diren eginbide gehienak desaktibatu daitezke [Ezaugarrien kudeaketan](/dynamics365/fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview). Etorkizunean, baliteke automatikoki aktibatu diren eginbide batzuk Eginbideen kudeaketatik kendu eta derrigorrezko bihurtzea. Aldaketa honek bezeroek egungo funtzionalitateak erabiltzen dituztela ziurtatzen du, hobekuntzak gehitu ahala uneko funtzionalitatean oinarritu daitezen. Eginbideak ez dira inoiz automatikoki gaituko urtebete baino gutxiagoan, ezinbestekoak direla erabakitzen ez bada.

| Eginbidearen izena | Gaitu data | Eginbidea gehitu da | Eginbidearen egoera | Modulua |
| --- | --- | --- |--- |--- |
| Gaitu orduko transakzioaren doikuntza finantzaketa-arauen esleipenaren aldaketaren arabera | 2022ko irailaren 16an | 2020ko urriak 7 | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Proiektuaren erosketa-eskaera aldez aurretik ordaintzeko fakturak itzultzeko eginbidea | 2022ko irailaren 16an | 2021eko urriak 6 | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Ezabatu fakturaren proposamen-lerroak Project Operations erabiltzean baliabideetan onarritutako / artxiboan ez dauden agertokietan | 2022ko irailaren 16an | 2021eko urriak 6 | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Doitu kontabilitatea argitaratutako proiektuaren transakzio batean | 2022ko irailaren 16an | 2020ko maiatzaren 10a | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Gaitu proiektuaren kontabilitate-konfigurazio lehenetsia | 2022ko irailaren 16an | 2020ko otsailaren 19a | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Gaitu proiektu baterako hainbat kontratu lerro | 2022ko irailaren 16an | 2020ko ekainaren 29a | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Egin proiektuaren orduen egunkariak irakurtzeko soilik, oraingo onespen-egoerak ez badu editatzen uzten | 2022ko irailaren 16an | 2021eko urriak 6 | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Gaitu erosketa-lerroetatik sinkronizatzeko salmenta-lerroak erosketa-lerroak eguneratzen direnean eta erosketa-eskaeraren aldaketak kudeatzeko parametroa aktibatuta dagoenean | 2022ko irailaren 16an | 2020ko urriak 7 | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Gaitu Project Operations Dynamics 365 Customer Engagement-en | 2022ko irailaren 16an | 2020ko ekainaren 29a | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |
| Proiektuaren transakzioen itzulera zuzentzeko eginbidea | 2022ko irailaren 16an | 2020ko uztailaren 13a | Lehenespenez aktibatuta | Proiektuaren kudeaketa eta kontabilitatea |

## <a name="features-that-become-mandatory-in-the-upcoming-release"></a>Datorren bertsioan derrigorrezko bihurtzen diren eginbideak

Hurrengo taulan 10.0.29 bertsioaren ondoren derrigorrezkoak diren funtzioak zerrendatzen dira.

| Eginbidearen izena | Gaitu data | Eginbidea gehitu da | Eginbidearen egoera | Modulua |
| --- | --- | --- | --- | --- |
| Kalkulatu finantzaketa-iturriaren konprometitutako balioa truke-tasa biribildu gabe | 2022ko irailaren 16an | 2020ko ekainaren 14a | Derrigorrezkoa | Proiektuaren kudeaketa eta kontabilitatea |
| Gaitu proiektuaren doikuntzaren argitalpena jatorrizko transakzioaren liburuko kontu berarekin | 2022ko irailaren 16an | 2020ko ekainaren 14a | Derrigorrezkoa | Proiektuaren kudeaketa eta kontabilitatea |
| Proiektuaren kontratuaren konpromisoaren zenbatekoaren xehetasuna | 2022ko irailaren 16an | 2019ko abuztuak 31 | Derrigorrezkoa | Proiektuaren kudeaketa eta kontabilitatea |
| Gaitu baliabideen arabera sailkatzea proiektuaren faktura-proposamena sortzean | 2022ko irailaren 16an | 2019ko abuztuak 31 | Derrigorrezkoa | Proiektuaren kudeaketa eta kontabilitatea |
