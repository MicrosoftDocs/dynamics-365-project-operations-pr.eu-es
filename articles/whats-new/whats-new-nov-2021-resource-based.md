---
title: 2021eko azaroko berrikuntzak - Baliabideetan oinarritutako eszenatokietarako proiektu-eragiketak/biltegiratu gabeak
description: Artikulu honetan, 2021eko Project Operations-en 2021eko azaroko bertsioan eskuragarri dauden kalitate-eguneratzeei buruzko informazioa ematen da, baliabideetan oinarritutako edo biltegiratu gabeko agertokietarako.
author: sigitac
ms.date: 11/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d5b58965f728321cc30d4e476b0dacf621fdec71
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8932879"
---
# <a name="whats-new-november-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko azaroko berrikuntzak - Baliabideetan oinarritutako eszenatokietarako proiektu-eragiketak/biltegiratu gabeak

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Artikulu hau Microsoft-en osagai eta bertsio hauei aplikatzen zaie Dynamics 365 Project Operations:

- Proiektu-eragiketak ingurune 4.26.0.145, 4.26.0.148, 4.26.0.150, 4.26.0.155 bertsio batean Dataverse
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.22 bertsioa

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- Project Scheduling aplikazioen programaziorako interfazeek (API) Project-en bucket-ak sortzeko eta ezabatzeko gaitasuna onartzen dute orain.

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](/dynamics365/project-operations/environment/resource-dual-write-maps).

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta Finantza irtenbidearen bertsioa. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa bat pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa bikoitzeko arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-in-dataverse"></a>Proiektuaren eragiketak Dataverse

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2240080 | Ordaintzeko baldintzak **ez dira** bikoiztu behar fakturan. |
| Fakturazioa eta prezioak | 2358236 | Fakturak zuzentzeak zero prezioko lineak dituzten zuzenketak ahalbidetu behar ditu. |
| Baliabideen kudeaketa | 2410072 | Lanari proiektu-kudeatzaile gisa esleitutako baliabide bat eratzeko aukera ematea. |
| Fakturazioa eta prezioak | 2430234 | Kostuen errendimendua kalkulatzeko arazo bat konpontzea. |
| Denbora eta gastua | 2436978 | Utzi denbora hh: mm formatuan sartzen. |
| Fakturazioa eta prezioak | 2448623 | Prezioen zerrendak antolaketa-unitate bati lotuta egon ondoren eguneratzen uztea. |
| Denbora eta gastua | 2460396 | Utzi denbora-sarrera bat ezabatzen gela ezabatuz. |
| Fakturazioa eta prezioak | 2467386 | Lan bat duen proiektu bat ezabatzea, baita lana irabazitako kotizazio bati lotuta dagoenean ere. |
| Denbora eta gastua | 2461744 | **Nire onarpen** hutsa ikusita, bidalitako etapan **proiektuak onartu besterik ez dago**. |
| Denbora eta gastua | 2464082 | Kendu proiektuaren onarpenen eta onarpenen arteko lotura, helmuga-egoera bat bat datorrenean. |
| Denbora eta gastua | 2468108 | Programatze lanak ez du **prozesatze-egoerarik** ezarri behar onarpen osorako. |
| Denbora eta gastua | 2471503 | Ezabatu zazpi eguneko antzinatasuna duten onarpen-multzoak. |
| Fakturazioa eta prezioak | 2480687 | Kotizazio-lerroaren erreferentzia ez da ezabatu behar kotizazio-lerroaren mugarri bat sortzen denean. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuen kudeaketa eta kontabilitatea Finantzetan

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [584732](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584732) | Hornitzaileak proiektuaren gastu-transakzioetan atxikitako zenbatekoak ez dira transakzioen zerrendan agertzen. |
| Proiektuaren kudeaketa eta kontabilitatea | [593068](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593068) | Hornitzaile-faktura eten egiten da enpresen artean, hornitzaileen fakturen integrazioa aktibatzen denean. |
| Proiektuaren kudeaketa eta kontabilitatea | [593382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593382) | Proiektuen fakturak ordaintzeko baldintzek ez dute espero bezala funtzionatzen. |
| Proiektuaren kudeaketa eta kontabilitatea | [596263](https://fix.lcs.dynamics.com/Issue/Details/?bugId=596263) | Hornitzaileen atxikipena askatzen denean, kupoien kontabilizatuak lerro gehigarriak ditu, eta horiek okerrak dira. |
| Proiektuaren kudeaketa eta kontabilitatea | [598758](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598758) | Project Operations-en integrazio-egunkaria argitaratzen denean, akats bat gertatzen da argitaratzen ari ez den kontu baterako dimentsiorik ez dagoelako. |
| Proiektuaren kudeaketa eta kontabilitatea | [602650](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602650) | Proiektua **ezin** da argitaratu ordaintzeke dagoen hornitzaile-faktura batean, artikuluari eskuratze-kategoria esleitzen zaionean. |
| Proiektuaren kudeaketa eta kontabilitatea | [605121](https://fix.lcs.dynamics.com/Issue/Details/?bugId=605121) | Nabigazio-panela falta da, proiektu-eragiketetan Dataverse saiorik hasi ez badu. |
| Proiektuaren kudeaketa eta kontabilitatea | [602728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602728) | Aplikatutako atxikipen kasu batean, proiektu-faktura baten diru-sarrerak kontabilizatuz gero, arazo bat sortzen da, egiaztapeneko transakzioak ez direlako orekatzen. |
| Proiektuaren kudeaketa eta kontabilitatea | [603624](https://fix.lcs.dynamics.com/Issue/Details/?bugId=603624) | Faktura-proposamen bat kontabilizatu ondoren aurrekontu bat sortzeak inportazioaren zuzenketa-lerroak blokeatzen ditu. |
| Proiektuaren kudeaketa eta kontabilitatea | [606083](https://fix.lcs.dynamics.com/Issue/Details/?bugId=606083) | Ezingo litzateke bere osotasunean fakturatutako mugarrien erregistro bat aldatu. |
| Bidaia eta gastua | [575305](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575305) | Gastuen txosten guztiak ikusgai daude aplikazio mugikorrean kategoria bat bilatzen duenean. |
| Bidaia eta gastua | [583101](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583101) | Hornitzaileen transakzioetako diru-kopuru okerrak eta salmenten gaineko zergen transakzioak kreditu-txarteldun transakzio batetik sortzen den gastu batetik abiatuta kontabilizatzen dira. |
| Bidaia eta gastua | [583760](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583760) | Garrantzirik gabeko ohartarazpena gertatzen da gastuen **txostena eguneratzean**. |
| Bidaia eta gastua | [598656](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598656) | Behin-behineko onartzailea behin-behineko onargailu bat ezabatzen denean erabiltzen da, eta, ondoren, gastuei buruzko txosten bat bidaltzen da lan-fluxuaren bidez. |
| Bidaia eta gastua | [612742](https://fix.lcs.dynamics.com/Issue/Details/?bugId=612742) | Kontabilizatzeko akats bat gertatzen da, kilometroaren konfigurazioarekin lotuta. |
