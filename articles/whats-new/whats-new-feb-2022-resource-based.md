---
title: Berriak 2022ko otsaila - Baliabideetan/hornituta ez dauden agertokietarako proiektu-eragiketak
description: Gai honek Project Operations-en 2022ko otsaileko bertsioan eskuragarri dauden kalitate-eguneratzeei buruzko informazioa eskaintzen du baliabideetan edo hornituta ez dauden agertokietarako.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 76ae00517c857415c89d7a03f421686dad28da93
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8600819"
---
# <a name="whats-new-february-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Berriak 2022ko otsaila - Baliabideetan/hornituta ez dauden agertokietarako proiektu-eragiketak

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Microsoft-en osagai eta bertsio hauei dagokie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.28.0.120
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.24 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

- Argitalpen honetatik aurrera, 300 taldekide gehi ditzakezu proiektu bakarrean. Lehen, taldekide kopuruaren muga 150 zen. Informazio gehiagorako, ikus [Proiektuaren mugak](../project-management/create-wbs.md#project-limitations).

## <a name="project-operations-dual-write-map-updates"></a>Project Operations idazketa bikoitzeko mapen eguneraketak

Hurrengo zerrendak Project Operations 2022ko otsaileko bertsioan aldatu edo gehitu diren idazketa bikoitzeko mapak erakusten ditu.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| --- | --- | --- |
| Project Operations integrazio proiektuaren gastuak esportatzeko entitatea (msdyn\_ gastuak) | 1.0.0.3 | Proiektuaren jarduerak sinkronizatzeko hedatua Dataverse. |

Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikus [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta Finantza irtenbidearen bertsioa. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa bat pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Dual Write arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2415109 | Balio lehenetsia **Eragiketak ordaintzeko baldintzak** eremuak proiektuaren kontratuaren bezeroaren erregistroa eta proformako fakturaren erregistroa izan behar du. |
| Fakturazioa eta prezioak | 2497369 | Materialaren zuzenketak data-balioari jarraitu behar dio **Zuzenketa** parametroak. |
| Fakturazioa eta prezioak | 2498697 | Segurtasun-konfigurazioa hobetu da **Denboraren sarrera gogoratzea**. |
| Fakturazioa eta prezioak | 2513824 | Baliabideetan oinarritutako agertokietarako, transakzio-kategoriaren IDak ez du 28 karaktere baino gehiago izan behar Project Operations-en. |
| Fakturazioa eta prezioak | 2517455 | The **Freskatu faktura lerroko transakzioak** Ez da onartu behar ekintza aldi berean hainbat aldiz abiarazteko faktura berdinerako. |
| Fakturazioa eta prezioak | 2517465 | The **Desaktibatu faktura-lerroaren xehetasunak** ekintza blokeatuta dago, onartzen ez delako. |
| Fakturazioa eta prezioak | 2556660 | Proiektuaren parametroen erregistroari atxikita dagoen prezio-zerrendan egiten den data-eraginkortasunaren egiaztapena konpondu da. |
|   Abaguneen kudeaketa | 2369202 | Proiektu-kontratu berdinari eragingarritasun-datak gainjarritako prezio-zerrendak erantsi daitezkeela egiaztatzen duen negozio-logika zuzendu da. |
|   Abaguneen kudeaketa | 2385965 | Portaera zuzendu du **Bezeroak** fitxan **Proiektuaren kontratua** orrialdea hautatzen duzunean **Gorde eta itxi**. |
| Denbora eta gastua | 2538503 | Proiektu-zeregin bat eskuragarri egon behar da **Proiektuaren benetakoak** entitatea gastuen txostena argitaratu ondoren. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance-en

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [615496](https://fix.lcs.dynamics.com/Issue/Details/?bugId=615496) | Saltzaileen kreditu-oharrak inportatzean, errore bat gertatzen da. Errore-mezuak honakoa dio: "Erretenimenduaren zenbatekoa ezin da izan gainerako kopuru garbia baino gehiago". |
| Proiektuaren kudeaketa eta kontabilitatea | [619391](https://fix.lcs.dynamics.com/Issue/Details/?bugId=619391) | Faktura-proposamen batek fakturatu gabeko salmenten benetako transakziorik gabeko kuoten transakziorik badakar, ezin da fakturatu. |
| Proiektuaren kudeaketa eta kontabilitatea | [624423](https://fix.lcs.dynamics.com/Issue/Details/?bugId=624423) | Argitaratutako kostua ez da zuzena erosketa prezioa eguneratu ondoren eta **Aldaketen kudeaketa aktibatu** gaituta dago.|
| Proiektuaren kudeaketa eta kontabilitatea | [628386](https://fix.lcs.dynamics.com/Issue/Details/?bugId=628386) | Prezio finkoko proiektu baten bidalketa-kalkuluak okerreko dirua eta zenbatekoa erabiltzen ditu aurrekontu-bonuan, nahiz eta **Gaitu proiektuaren kontratuaren moneta aurrekontua kalkulatzeko** funtzioa gaituta dago. |
| Proiektuaren kudeaketa eta kontabilitatea | [629239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=629239) | **ProjDMFDataPopulation\_ Luzapena** ez luke deirik egin aldaketaren jarraipena gaitzeko, gaituta ez dauden konfigurazio-gakoak dituzten entitateen salbuespenak aurkitu gabe. |
| Proiektuaren kudeaketa eta kontabilitatea | [623818](https://fix.lcs.dynamics.com/Issue/Details/?bugId=623818) | Batch lana konpondu egiten da hainbat aldizkari aurreratu argitaratzen direnean eta errore bat gertatzen denean. |
| Bidaia eta gastua | [616805](https://fix.lcs.dynamics.com/Issue/Details/?bugId=616805) | Gastu-txostenetako diru-aurrerakinekin zerikusia duen likidazio-arazo bat dela eta, zerga-kopurua ez da diru-aurrerakinaren zati gisa estaltzen. |
| Bidaia eta gastua | [616959](https://fix.lcs.dynamics.com/Issue/Details/?bugId=616959) | Salmenten gaineko zergaren informazioa ez dago sartuta **Gastua - Argitaratutako eragiketak** txostena. |
| Bidaia eta gastua | [618943](https://fix.lcs.dynamics.com/Issue/Details/?bugId=618943) | The **Beharrezko ordainagiriak** gastu-politika urratzeak gaizki erakusten du gastu-txostenetan abisua. |
| Bidaia eta gastua | [633470](https://fix.lcs.dynamics.com/Issue/Details/?bugId=633470) | Proiektu-transakzio batek ez du salmenten gaineko zerga-zergarik sartzen salmenten kopuru osoan, transakzioa kilometraje-gastu baten ondoriozkoa denean. |
| Bidaia eta gastua | [642979](https://fix.lcs.dynamics.com/Issue/Details/?bugId=642979) | Elementu-lerro batek zergak dituenean, ezin duzu elementu-lerroaren data aldatu eta iturburu-dokumentuaren egoera-errore bat gertatzen da. |

## <a name="removed-and-deprecated-features"></a>Ezaugarriak kendu eta zaharkituta

The [Project Operations-en eginbideak kendu edo zaharkituta](removed-depreciated-features-project.md) gaiak ezabatu edo zaharkitu diren ezaugarriak deskribatzen ditu Dynamics 365 Project Operations.

- Kendu eginbidea dagoeneko ez dago eskuragarri produktuan.
- Zaharkitutako eginbide bat ez dago garapen aktiboan eta baliteke etorkizuneko eguneratze batean kentzea.

Zaharberritze-iragarkia agertuko da [Project Operations-en eginbideak kendu edo zaharkituta](removed-depreciated-features-project.md) gaia produktutik eginbideren bat kendu baino 12 hilabete lehenago.

Konpilazio-denboran bakarrik eragiten duten baina sandbox eta ekoizpen-inguruneekin bitar bateragarriak diren aldaketetarako, zaharkitze-denbora 12 hilabete baino txikiagoa izango da. Normalean, aldaketa hauek konpilatzaileari egin beharreko eguneratze funtzionalak dira.
