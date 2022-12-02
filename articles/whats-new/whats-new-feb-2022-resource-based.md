---
title: 2022eko otsaileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Gai honek informazioa eskaintzen du 2022ko otsailean Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruz, baliabideetan / stockean oinarritutako egoeretarako.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: b036c0a3c39c52cb15277293679ef88906cae2c4
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8932971"
---
# <a name="whats-new-february-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>2022eko otsaileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.28.0.120
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.24 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

- Argitalpen honetatik aurrera, 300 taldekide gehi ditzakezu proiektu bakarrean. Lehen, taldekide kopuruaren muga 150 zen. Informazio gehiagorako, ikusi [Proiektu-mugak](../project-management/create-wbs.md#project-limitations).

## <a name="project-operations-dual-write-map-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo zerrendan 2022eko otsaileko Project Operations aldatu edo gehitu diren idazketa bikoitzeko mapak agertzen dira.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| --- | --- | --- |
| Project Operations-ek integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn\_expenses) | 1.0.0.3 | Proiektuaren jarduerak sinkronizatzeko hedatua Dataverse. |

Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2415109 | Balio lehenetsia **Eragiketak ordaintzeko baldintzak** eremuak proiektuaren kontratuaren bezeroaren erregistroa eta proformako fakturaren erregistroa izan behar du. |
| Fakturazioa eta prezioak | 2497369 | Materialaren zuzenketak data-balioari jarraitu behar dio **Zuzenketa** parametroak. |
| Fakturazioa eta prezioak | 2498697 | Segurtasun-konfigurazioa hobetu da **Denboraren sarrera gogoratzea**. |
| Fakturazioa eta prezioak | 2513824 | Baliabideetan oinarritutako agertokietarako, transakzio-kategoriaren IDak ez du 28 karaktere baino gehiago izan behar Project Operations-en. |
| Fakturazioa eta prezioak | 2517455 | **Freskatu faktura lerroko transakzioak** Ez da onartu behar ekintza aldi berean hainbat aldiz abiarazteko faktura berdinerako. |
| Fakturazioa eta prezioak | 2517465 | **Desaktibatu faktura-lerroaren xehetasunak** ekintza blokeatuta dago, onartzen ez delako. |
| Fakturazioa eta prezioak | 2556660 | Proiektuaren parametroen erregistroari atxikita dagoen prezio-zerrendan egiten den data-eraginkortasunaren egiaztapena konpondu da. |
|   Abaguneen kudeaketa | 2369202 | Proiektu-kontratu berari eragingarritasun-datak gainjarritako prezio-zerrendak erantsi daitezkeela egiaztatzen duen negozio-logika zuzendu da. |
|   Abaguneen kudeaketa | 2385965 | Portaera zuzendu du **Bezeroak** fitxan **Proiektuaren kontratua** orrialdea hautatzen duzunean **Gorde eta itxi**. |
| Denbora eta gastua | 2538503 | Proiektu-zeregin bat eskuragarri egon behar da **Proiektu errealak** entitatea gastuen txostena argitaratu ondoren. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Project Management and Accounting Dynamics 365 Finance-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [615496](https://fix.lcs.dynamics.com/Issue/Details/?bugId=615496) | Saltzaileen kreditu-oharrak inportatzean, errore bat gertatzen da. Errore-mezuak honakoa dio: "Atxikipenaren zenbatekoa ezin da izan gainerako kopuru garbia baino gehiago". |
| Proiektuaren kudeaketa eta kontabilitatea | [619391](https://fix.lcs.dynamics.com/Issue/Details/?bugId=619391) | Faktura-proposamen batek fakturatu gabeko salmenten benetako transakziorik gabeko kuoten transakziorik badakar, ezin da fakturatu. |
| Proiektuaren kudeaketa eta kontabilitatea | [624423](https://fix.lcs.dynamics.com/Issue/Details/?bugId=624423) | Argitaratzen den kostua ez da zuzena erosketa prezioa eta **Aldaketen kudeaketa aktibatu** gaitu ondoren.|
| Proiektuaren kudeaketa eta kontabilitatea | [628386](https://fix.lcs.dynamics.com/Issue/Details/?bugId=628386) | Prezio finkoko proiektu baten bidalketa-kalkuluak dirua eta zenbatekoa okerrak erabiltzen ditu aurrekontu-bonuan, nahiz eta **Gaitu proiektuaren kontratuaren moneta estimazioa kalkulatzeko** funtzioa gaituta dago. |
| Proiektuaren kudeaketa eta kontabilitatea | [629239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=629239) | **ProjDMFDataPopulation\_Extension** ez luke deirik egin aldaketaren jarraipena gaitzeko, gaituta ez dauden konfigurazio-gakoak dituzten entitateen salbuespenak aurkitu gabe. |
| Proiektuaren kudeaketa eta kontabilitatea | [623818](https://fix.lcs.dynamics.com/Issue/Details/?bugId=623818) | Sortako lana konpondu egiten da hainbat aldizkari aurreratu argitaratzen direnean eta errore bat gertatzen denean. |
| Bidaia eta gastua | [616805](https://fix.lcs.dynamics.com/Issue/Details/?bugId=616805) | Gastu-txostenen diru-aurrerakinekin zerikusia duen likidazio-arazo bat dela eta, zerga-kopurua ez da diru-aurrerakinaren zati gisa estaltzen. |
| Bidaia eta gastua | [616959](https://fix.lcs.dynamics.com/Issue/Details/?bugId=616959) | Salmenten gaineko zergaren informazioa ez dago sartuta **Gastua - Argitaratutako eragiketak** txostena. |
| Bidaia eta gastua | [618943](https://fix.lcs.dynamics.com/Issue/Details/?bugId=618943) | **Beharrezko ordainagiriak** gastu-politika urratzeak gaizki erakusten du gastu-txostenetan abisua. |
| Bidaia eta gastua | [633470](https://fix.lcs.dynamics.com/Issue/Details/?bugId=633470) | Proiektuaren transakzio batek ez du salmenten gaineko zerga berreskuraezina sartzen salmenten zenbatekoan, transakzioa kilometraje-gastu baten ondorio denean. |
| Bidaia eta gastua | [642979](https://fix.lcs.dynamics.com/Issue/Details/?bugId=642979) | Elementu-lerro batek zergak dituenean, ezin duzu elementu-lerroaren data aldatu eta iturburu-dokumentuaren egoera-errore bat gertatzen da. |

## <a name="removed-and-deprecated-features"></a>Kendu eta zaharkitutako ezaugarriak

[Project Operations-en eginbideak kendu edo zaharkituta](removed-depreciated-features-project.md) artikuluak ezabatu edo zaharkitu diren ezaugarriak deskribatzen ditu Dynamics 365 Project Operations.

- Kendu eginbidea dagoeneko ez dago eskuragarri produktuan.
- Zaharkitua funtzioa ez dago garapen aktiboan eta baliteke etorkizuneko eguneratze batean ezabatzea.

Zaharberritze-iragarkia agertuko da [Project Operations-en eginbideak kendu edo zaharkituta](removed-depreciated-features-project.md) artikulua produktuari edozein ezaugarri kendu baino 12 hilabete lehenago.

Konpilazio-denborari bakarrik eragiten dioten baina sandbox eta ekoizpen-inguruneekin bitar bateragarriak diren aldaketetarako, zaharkitze-denbora 12 hilabete baino txikiagoa izango da. Normalean, aldaketa hauek konpilatzaileari egin behar zaizkion eguneratze funtzionalak dira.
