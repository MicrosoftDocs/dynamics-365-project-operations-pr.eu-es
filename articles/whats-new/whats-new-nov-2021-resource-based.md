---
title: 2021eko azaroko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Artikulu honek informazioa eskaintzen du 2021eko azaroan Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruz, baliabideetan / stockean oinarritutako egoeretarako.
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
# <a name="whats-new-november-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko azaroko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations 4.26.0.145, 4.26.0.148, 4.26.0.150, 4.26.0.155 bertsioko Dataverse ingurunean
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.22 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- Project Scheduling aplikazioen programazio-interfazeek (API) orain proiektuaren kuboak sortzeko eta ezabatzeko gaitasuna onartzen dute.

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](/dynamics365/project-operations/environment/resource-dual-write-maps).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-in-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2240080 | **Ordainketa baldintzak** eremua ez da bikoiztu behar pro formako fakturan. |
| Fakturazioa eta prezioak | 2358236 | Fakturaren zuzenketak zero prezio-lerroak dituzten zuzenketak ahalbidetu behar ditu. |
| Baliabideen kudeaketa | 2410072 | Proiektuaren kudeatzaile gisa zeregin bati esleitutako baliabidearen erabilera-unitateak onartu |
| Fakturazioa eta prezioak | 2430234 | Konpondu kostuen errendimendua kalkulatzeko arazo bat. |
| Denbora eta gastua | 2436978 | Baimendu denbora hh:mm formatuan sartzeko. |
| Fakturazioa eta prezioak | 2448623 | Onartu prezioen zerrendak eguneratzea antolakuntza-unitate batekin erlazionatu ondoren. |
| Denbora eta gastua | 2460396 | Erabiltzaileek ordu-sarrera bat sartzea onartu gelaxka garbituz. |
| Fakturazioa eta prezioak | 2467386 | Baimendu zeregin bat duen proiektu bat ezabatzea, baita zeregina irabazitako aurrekontu batekin lotuta dagoenean ere. |
| Denbora eta gastua | 2461744 | **Nire onarpen hutsa** ikuspegiak egoera duten proiektuen onarpenak baino ez ditu **Bidalita** fasean. |
| Denbora eta gastua | 2464082 | Kendu proiektuaren onarpenetatik onarpen multzorako esteka helburu-egoera bat datorrenean. |
| Denbora eta gastua | 2468108 | Programazio lanak ez du ezarri behar **Tramitazioa** onarpen multzoaren egoera. |
| Denbora eta gastua | 2471503 | Ezabatu zazpi egun dituzten onarpen-multzoak. |
| Fakturazioa eta prezioak | 2480687 | Aipamen-lerroaren erreferentzia ez da kendu behar aurrekontu-lerroaren mugarri bat sortzen denean. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Finantzan

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [584732](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584732) | Atxikitako saltzaileen zenbatekoak proiektuko gastu transakzioetan ez dira transakzioen zerrendan erakusten. |
| Proiektuaren kudeaketa eta kontabilitatea | [593068](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593068) | Enpresaren arteko hornitzaileen faktura hautsi egiten da hornitzaileen fakturaren integrazioa aktibatuta dagoenean. |
| Proiektuaren kudeaketa eta kontabilitatea | [593382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593382) | Proiektuaren fakturen ordainketa-baldintzek ez dute espero bezala funtzionatzen. |
| Proiektuaren kudeaketa eta kontabilitatea | [596263](https://fix.lcs.dynamics.com/Issue/Details/?bugId=596263) | Saltzaileen atxikipena askatzen denean, bonuaren bidalketak lerro gehigarri okerrak ditu. |
| Proiektuaren kudeaketa eta kontabilitatea | [598758](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598758) | Project Operations integrazio-egunkariak huts egiten du argitaratzen duzunean, kontu bati dimentsioak falta zaizkiolako. |
| Proiektuaren kudeaketa eta kontabilitatea | [602650](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602650) | Ezin da editatu **Proiektua** fitxa zain dagoen saltzailearen fakturan prokurazio-kategoria esleituta dagoenean elementuari. |
| Proiektuaren kudeaketa eta kontabilitatea | [605121](https://fix.lcs.dynamics.com/Issue/Details/?bugId=605121) | Nabigazio-panela falta da Project Operations-en saioa hasi ez baduzu Dataverse-n. |
| Proiektuaren kudeaketa eta kontabilitatea | [602728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602728) | Bonuen transakzioak ez dira behar bezala orekatzen aplikatutako atxikipen kasuetan proiektuaren fakturatutako diru sarrerak bidaltzeagatik. |
| Proiektuaren kudeaketa eta kontabilitatea | [603624](https://fix.lcs.dynamics.com/Issue/Details/?bugId=603624) | Faktura-proposamena argitaratu ondoren estimazio bat sortzeak zuzenketa-lerroak blokeatzen ditu inportaziotik. |
| Proiektuaren kudeaketa eta kontabilitatea | [606083](https://fix.lcs.dynamics.com/Issue/Details/?bugId=606083) | Ezin izango litzateke guztiz fakturatutako mugarrien erregistroa aldatzea. |
| Bidaia eta gastua | [575305](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575305) | Gastuen txosten guztiak ikus daitezke Expense mugikorreko aplikazioan kategoria bat bilatzen duzunean. |
| Bidaia eta gastua | [583101](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583101) | Kreditu txartelaren transakzio batetik sortutako gastu batetik erregistratutako saltzaileen eta salmenten gaineko zergaren transakzioen zenbatekoak ez dira zuzenak. |
| Bidaia eta gastua | [583760](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583760) | Garrantzirik gabeko abisu-mezu bat erakusten da **gastu-txosten** orriak freskatzen dituzunean. |
| Bidaia eta gastua | [598656](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598656) | Behin-behineko onartzaile okerra erabiltzen da behin-behineko onartzaile bat ezabatzen duzunean eta gastu-txostena lan-fluxuaren bidez berriro bidaltzen duzunean. |
| Bidaia eta gastua | [612742](https://fix.lcs.dynamics.com/Issue/Details/?bugId=612742) | Kilometrajearen konfigurazioarekin lotutako errore bat dago. |
