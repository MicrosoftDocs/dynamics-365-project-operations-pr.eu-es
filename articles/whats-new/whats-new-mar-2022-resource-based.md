---
title: 2022ko martxoko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Gai honek informazioa eskaintzen du 2022ko martxoan Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruz, baliabideetan / stockean oinarritutako egoeretarako.
author: sigitac
ms.date: 03/31/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 986d0652ed502873085259fef5ad40aba99c278d
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8910891"
---
# <a name="whats-new-march-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>2022ko martxoko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.30.0.99
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.25 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Egunkariak gaur egun gastuen lan-espazio moderno berrian eta birimaginatuan onartzen dira. Egunkariak erabiltzen dituzten enpresek eginbide hau gaitu dezakete erabiltzaileei bidaltzeko eta eguneko gastuak itzultzeko modu erraz bat emateko. Informazio gehiago lortzeko, ikusi [Eguneko dieten gastuak](../expense/per-diem-expenses.md).

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo zerrendan 2022ko martxoko Project Operations aldatu edo gehitu diren idazketa bikoitzeko mapak agertzen dira.

| **Entitate-esleipena** | **Eguneratutako bertsioa** | **Iruzkinak** |
| --- | --- | --- |
| Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn\_projectvendorinvoicelines) | 1.0.0.3 | Mapaketak eguneratu dira hornitzaileen faktura-lerroaren entitatearekin lerrokatzeko Dataverse. <br>Ez aktibatu mapen bertsioa 1.0.0.4. Finantza ingurunearen 10.0.26 bertsioarekin batera erabiltzeko prest egongo da hurrengo hileko eguneratzean. |

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Denbora eta gastua | 2388011 | Erakutsi ukatzeko iruzkinak denbora-sarrerak bidaltzen dituztenei masiboki onartzean. |
| Proiektuaren antolaketa eta jarraipena | 2495294 | Proiektuaren xehetasunak ezin dira editatu **Zereginaren xehetasunak** orrialdea. |
| Fakturazioa eta prezioak | 2499605 | Eskaintza-mugarrietatik sortzen diren kontratuaren mugarriak gaizki markatuta daude irakurtzeko soilik gisa. |
| Proiektuaren antolaketa eta jarraipena | 2506050 | Eragiketa multzoa ordubetez geratzen da gordetzeko aldaketarik ez badago. Ondoren, multzoa modu faltsuan markatzen da **Huts egin du**, berriz, berehala osatu beharko litzateke. |
| Fakturazioa eta prezioak | 2507401 | Kontratazio-unitate lehenetsiak gaizki sartzen dira proiektuetan, cachean oker dagoelako. |
| Fakturazioa eta prezioak | 2541660 | **Salmenta-eskaerak sortzearen baliozkotzea** idazkera bikoitzean proiektuetan oinarritutako eskaeretarako soilik izan behar da. |
| Fakturazioa eta prezioak | 2552745 | Zerga ez da banatzen fakturazio arauak ezarri dituzten bezeroen artean. |
| Fakturazioa eta prezioak | 2558859 | Errore-mezuak hobetu dira prezioen dimentsioak konfiguratzen direnean. |
| Fakturazioa eta prezioak | 2558933 | **Inportatu proiektuaren kalkuluetatik** huts egiten duenean **msdyn\_project** prezioen dimentsio gisa gehitzen da. |
| Fakturazioa eta prezioak | 2559101 | Proiektuaren parametroa ezabatzea ez dago blokeatuta eta arazoak sortzen ditu. |
|   Abaguneen kudeaketa | 2570390 | Idazketa bikoitzeko plug-in-ak aurrekontuen, eskaeren eta aukeretan kontu mota izatera behartzen du **Bezeroa**, nahiz eta kontu mota hori zuzena ez izan. |
| Fakturazioa eta prezioak | 2586097 | Zatitutako fakturatutako kostu errealak ez dira alderantzikatzen proiektu bat proiektuaren kontratu-lerro batetik kentzen denean. |
| Fakturazioa eta prezioak | 2589619 | Idatzitako materialaren gaineko zerga fakturatu gabeko salmenta errealetara eta fakturara hedatzen da. |
|   Abaguneen kudeaketa | 2594015 | Eskaintza bat ezin da itxi irabazi gisa duten bezeroentzat **Net60** ordainketa baldintzak. |
| Proiektuaren antolaketa eta jarraipena | 2595841 | Project for the Web-en, erabiltzaileek falta den baten inguruko errore-mezu bat jasotzen dute **msdyn\_actualstart** baliabide eskaera berri bat sortzen dutenean. |
| Denbora eta gastua | 2602511 | **Errefusatua** ordua sartzeko eremua erakusten du **Sistema** errefusatzaile gisa izendatutako erabiltzaile baten ordez. |
| Denbora eta gastua | 2602528 | Proiektuaren onartzaileak denbora onar dezake onartzaile gisa zerrendatuta ez dauden proiektuetan. |
| Fakturazioa eta prezioak | 2608550 | Zuzenketa-faktura berretsi daiteke jatorrizkoan aldaketarik egon ez arren. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Project Management and Accounting Dynamics 365 Finance-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [606759](https://fix.lcs.dynamics.com/Issue/Details/?bugId=606759) | Finantza eta Project Operations artean desegokia dago baimendutako iraupenean **Kategoriaren IDa** eremua. |
| Proiektuaren kudeaketa eta kontabilitatea | [617806](https://fix.lcs.dynamics.com/Issue/Details/?bugId=617806) | Prezio finkoko proiektuak ezin dira kendu **Konturako fakturazioa** eremuan ezarrita dago **Irabaziak eta galerak** eta **Osatutako ehunekoa** printzipioa erabiltzen da. |
| Proiektuaren kudeaketa eta kontabilitatea | [620979](https://fix.lcs.dynamics.com/Issue/Details/?bugId=620979) | Salmenta-zergaren talde lehenetsi oker bat sartzen da proiektuaren konfiguraziotik proiektuaren eragiketen integrazio aldizkariko gastu-lerroetan. |
| Proiektuaren kudeaketa eta kontabilitatea | [623014](https://fix.lcs.dynamics.com/Issue/Details/?bugId=623014) | Ezin dituzu editatu proiektuaren faktura-proposamenaren goiburuko dimentsioak Project Operations-en inplementazio integratuan. |
| Proiektuaren kudeaketa eta kontabilitatea | [624283](https://fix.lcs.dynamics.com/Issue/Details/?bugId=624283) | Enpresaren arteko hornitzaileen fakturak ezin dira bateratu Dataverse-rekin. |
| Proiektuaren kudeaketa eta kontabilitatea | [634156](https://fix.lcs.dynamics.com/Issue/Details/?bugId=634156) | Desberdintasun bat dago bezeroen saldoen moneta eta txosteneko moneta. |
| Proiektuaren kudeaketa eta kontabilitatea | [641612](https://fix.lcs.dynamics.com/Issue/Details/?bugId=641612) | Proiektu-faktura bat argitaratu dezakezu, nahiz eta bezeroa faktura guztietarako zain egon. |
| Proiektuaren kudeaketa eta kontabilitatea | [642945](https://fix.lcs.dynamics.com/Issue/Details/?bugId=642945) | **Ezabatu lerro guztiak** botoia falta da hau duten proiektuen faktura-proposamenetan **Goiburua** eta **Lerroak** bistak. |
| Proiektuaren kudeaketa eta kontabilitatea | [637760](https://fix.lcs.dynamics.com/Issue/Details/?bugId=637760) | Saltzaileen faktura bat argitaratzen duzunean, errore hau gertatzen da: "Fakturaren kontabilitate-data erlazionatutako erosi-eskaeraren kontabilitate-urte berean egon behar da. Exekutatu erosketa-eskaeraren urte amaierako prozesua edo aldatu data uneko kontabilitate ekitaldira". |
| Bidaia eta gastua | [604128](https://fix.lcs.dynamics.com/Issue/Details/?bugId=604128) | Proiektu baten kostu konprometitua ez da kaleratzen bidaia eskaera kostu konprometituarekin argitaratu ondoren. |
| Bidaia eta gastua | [620803](https://fix.lcs.dynamics.com/Issue/Details/?bugId=620803) | Gastuen txostena bidaltzen duzunean errore hau gertatzen da "Stack Trace: konpainia ez da existitzen." |
| Bidaia eta gastua | [622465](https://fix.lcs.dynamics.com/Issue/Details/?bugId=622465) | Lehenetsia **Proiektuaren IDa** ez da gastu-txostenetan sartzen denean **Aldizkaria egiteko jarduera eskatu** parametroa hautatzen da proiektuan. |
| Bidaia eta gastua | [626781](https://fix.lcs.dynamics.com/Issue/Details/?bugId=626781) | **Posta gastuak** botoiak ez du behar bezala funtzionatzen Project Operations-n baliabide/hornituta ez dauden agertokietarako. |
| Bidaia eta gastua | [635348](https://fix.lcs.dynamics.com/Issue/Details/?bugId=635348) | Arazo bat dago **Tasa kilometro bakoitzeko** bidaiariak barne hartzen dituen kilometro-gastuen txosten baterako. |
| Bidaia eta gastua | [638019](https://fix.lcs.dynamics.com/Issue/Details/?bugId=638019) | Langileen gastuen kilometraje-tasak ez dira behar bezala biltzen bi ibilgailu mota desberdin erabiltzen direnean **Kilometraje-tasa mailak** gastuen kategoria. |
| Bidaia eta gastua | [641272](https://fix.lcs.dynamics.com/Issue/Details/?bugId=641272) | Bilaketa **Proiektua** Bidaia-eskaeraren lerroko eremuak ez du proiektuen zerrenda zuzena itzultzen. |
| Bidaia eta gastua | [645905](https://fix.lcs.dynamics.com/Issue/Details/?bugId=645905) | **Kilometrajea berrikusten** gastuen txostenei buruzko abisua erakusten du. |
| Bidaia eta gastua | [647819](https://fix.lcs.dynamics.com/Issue/Details/?bugId=647819) | Ordainagiriaren karaktereak ezagutzeko (OCR) zerbitzuak ez du funtzionatzen gastuaren OCR zerbitzuaren URLarekin arazo bat dagoelako. |
| Bidaia eta gastua | [648684](https://fix.lcs.dynamics.com/Issue/Details/?bugId=648684) | Noiz **Aldizkako gastuak azkar banatzeko gaitasuna** Ezaugarritasuna gaituta dago, gastu-txostenetako elementu-lerroetako zenbatekoak zenbatekoak aldatzen ditu **Bihurtu elementu** orria irekitzen da. |
| Bidaia eta gastua | [651899](https://fix.lcs.dynamics.com/Issue/Details/?bugId=651899) | Ezin duzu gastuen txosten bat ezabatu behin-behineko zerrendak onartzaile bat baino gehiago dituenean. |

## <a name="removed-and-deprecated-features"></a>Kendu eta zaharkitutako ezaugarriak

[Project Operations-en eginbideak kendu edo zaharkituta](removed-depreciated-features-project.md) artikuluak ezabatu edo zaharkitu diren ezaugarriak deskribatzen ditu Dynamics 365 Project Operations.

- Kendu eginbidea dagoeneko ez dago eskuragarri produktuan.
- Zaharkitua funtzioa ez dago garapen aktiboan eta baliteke etorkizuneko eguneratze batean ezabatzea.

Zaharberritze-iragarkia agertuko da [Project Operations-en eginbideak kendu edo zaharkituta](removed-depreciated-features-project.md) artikulua produktuari edozein ezaugarri kendu baino 12 hilabete lehenago.

Konpilazio-denborari bakarrik eragiten dioten baina sandbox eta ekoizpen-inguruneekin bitar bateragarriak diren aldaketetarako, zaharkitze-denbora 12 hilabete baino txikiagoa izango da. Normalean, aldaketa hauek konpilatzaileari egin behar zaizkion eguneratze funtzionalak dira.
