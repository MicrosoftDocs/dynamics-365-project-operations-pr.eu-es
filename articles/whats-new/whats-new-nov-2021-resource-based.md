---
title: 2021eko azaroko berritasunak - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak
description: Gai honek 2021eko azaroko Project Operations-en bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du baliabideetan edo hornituta ez dauden agertokietarako.
author: sigitac
ms.date: 11/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 20f277bc9b6f571c0144eaaa867bb97c0cf30ddb
ms.sourcegitcommit: 04ebe764afa22742b3fbf8f12af31e8eea93682e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/23/2021
ms.locfileid: "7827310"
---
# <a name="whats-new-november-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko azaroko berritasunak - Baliabideetan edo hornituta ez dauden agertokietarako proiektuen eragiketak

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Dynamics 365 Project Operations Microsoft-en osagai eta bertsio hauei dagokie:

- Proiektuaren Eragiketak Dataverse inguruneko bertsioan 4.26.0.145, 4.26.0.148, edo 4.26.0.150
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.22 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- Project Scheduling aplikazioen programazio-interfazeek (API) orain proiektuaren kuboak sortzeko eta ezabatzeko gaitasuna onartzen dute.

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](/dynamics365/project-operations/environment/resource-dual-write-maps).

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure Project Operations Dataverse soluzioa eta Finantza irtenbidearen bertsioa eguneratzen dituzun bitartean. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa bat pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa bikoitzeko arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-in-dataverse"></a>Proiektuaren eragiketak Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2240080 | The **Ordainketa baldintzak** eremua ez da bikoiztu behar proformako fakturan. |
| Fakturazioa eta prezioak | 2358236 | Fakturaren zuzenketak zero prezio-lerroak dituzten zuzenketak ahalbidetu behar ditu. |
| Baliabideen kudeaketa | 2410072 | Baimendu proiektu-kudeatzaile gisa zereginari esleitutako baliabidea konfiguratzea. |
| Fakturazioa eta prezioak | 2430234 | Konpondu kostuen errendimendua kalkulatzeko arazo bat. |
| Denbora eta gastua | 2436978 | Baimendu denbora hh:mm formatuan sartzeko. |
| Fakturazioa eta prezioak | 2448623 | Onartu prezioen zerrendak eguneratzea antolakuntza-unitate batekin erlazionatu ondoren. |
| Denbora eta gastua | 2460396 | Baimendu denbora-sarrera bat ezabatzeko gelaxka garbituz. |
| Fakturazioa eta prezioak | 2467386 | Baimendu zeregin bat duen proiektu bat ezabatzea, baita zeregina irabazitako aurrekontu batekin lotuta dagoenean ere. |
| Denbora eta gastua | 2461744 | The **Nire onarpen hutsa** ikuspegian proiektuaren onarpenak soilik ditu **Aurkeztua** etapa. |
| Denbora eta gastua | 2464082 | Kendu proiektuaren onarpenetatik onarpen multzorako esteka helburu-egoera bat datorrenean. |
| Denbora eta gastua | 2468108 | Programazio lanak ez du ezarri behar a **Tramitazioa** onarpen multzoaren egoera. |
| Denbora eta gastua | 2471503 | Ezabatu zazpi egun dituzten onarpen-multzoak. |
| Fakturazioa eta prezioak | 2480687 | Aipamen-lerroaren erreferentzia ez da kendu behar aurrekontu-lerroaren mugarri bat sortzen denean. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuen kudeaketa eta kontabilitatea Finantzetan

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [584732](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584732) | Atxikitako saltzaileen zenbatekoak proiektuko gastu transakzioetan ez dira transakzioen zerrendan erakusten. |
| Proiektuaren kudeaketa eta kontabilitatea | [593068](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593068) | Enpresaren arteko hornitzaileen faktura hautsi egiten da hornitzaileen fakturaren integrazioa aktibatuta dagoenean. |
| Proiektuaren kudeaketa eta kontabilitatea | [593382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593382) | Proiektuaren fakturen ordainketa-baldintzek ez dute espero bezala funtzionatzen. |
| Proiektuaren kudeaketa eta kontabilitatea | [596263](https://fix.lcs.dynamics.com/Issue/Details/?bugId=596263) | Saltzaileen atxikipena askatzen denean, bonoaren bidalketak okerrak diren lerro gehigarriak ditu. |
| Proiektuaren kudeaketa eta kontabilitatea | [598758](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598758) | Project Operations integrazio aldizkaria argitaratzen denean, huts egiten du argitaratzen ez den kontu baten dimentsioak falta direlako. |
| Proiektuaren kudeaketa eta kontabilitatea | [602650](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602650) | The **Proiektua** fitxa ezin da editatu zain dagoen saltzaileen faktura batean kontratazio-kategoria elementuari esleitzen zaionean. |
| Proiektuaren kudeaketa eta kontabilitatea | [605121](https://fix.lcs.dynamics.com/Issue/Details/?bugId=605121) | Nabigazio-panela falta da ez bazaude saioa hasi Project Operations Dataverse. |
| Proiektuaren kudeaketa eta kontabilitatea | [602728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602728) | Proiektu-faktura baten diru-sarrerak aplikatutako atxikipen-kasu batean argitaratzen dituzunean, arazo bat gertatzen da bonoaren transakzioak ez direlako orekatzen. |
| Proiektuaren kudeaketa eta kontabilitatea | [603624](https://fix.lcs.dynamics.com/Issue/Details/?bugId=603624) | Faktura-proposamena argitaratu ondoren estimazio bat sortzeak zuzenketa-lerroak blokeatzen ditu inportaziotik. |
| Proiektuaren kudeaketa eta kontabilitatea | [606083](https://fix.lcs.dynamics.com/Issue/Details/?bugId=606083) | Ezin izan beharko litzateke guztiz fakturatutako mugarrien erregistroa aldatzea. |
| Bidaia eta gastua | [575305](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575305) | Gastu-txosten guztiak ikusgai daude Expense aplikazio mugikorrean kategoria bat bilatzen duzunean. |
| Bidaia eta gastua | [583101](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583101) | Hornitzaileen transakzioen eta salmenten gaineko zergaren transakzioen kopuru okerrak kreditu-txartelaren transakzio batetik sortutako gastu batetik argitaratzen dira. |
| Bidaia eta gastua | [583760](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583760) | Garrantzirik gabeko abisu bat gertatzen da freskatzen duzunean **Gastuen txostena** orrialdea. |
| Bidaia eta gastua | [598656](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598656) | Behin-behineko onartzaile okerra erabiltzen da behin-behineko onartzaile bat ezabatzen duzunean eta, ondoren, lan-fluxuaren bidez gastu-txostena berriro bidaltzen duzunean. |
| Bidaia eta gastua | [612742](https://fix.lcs.dynamics.com/Issue/Details/?bugId=612742) | Kilometrajearen konfigurazioarekin erlazionatutako argitalpen-errore bat gertatu da. |
