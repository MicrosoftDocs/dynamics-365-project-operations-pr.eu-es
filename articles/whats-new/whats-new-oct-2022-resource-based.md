---
title: Berriak 2022ko urrian - Baliabideetan/hornituta ez dauden agertokietarako proiektu-eragiketak
description: Artikulu honek Microsoft Dynamics 365 Project Operations ren 2022ko urriko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du baliabideetan edo hornituta ez dauden agertokietarako.
author: ramagadu
ms.date: 11/17/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 392a12d6954c2390e5bad8e8e36cf58b7a1d0749
ms.sourcegitcommit: 1f162707ac342343fb5390fb9ae335e4cea4f3f2
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/29/2022
ms.locfileid: "9806711"
---
# <a name="whats-new-october-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Berriak 2022ko urrian - Baliabideetan/hornituta ez dauden agertokietarako proiektu-eragiketak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.57.0.176
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.30 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

| Ezaugarrien eremua | Eginbidearen izena | Informazio gehiago |
| --- | --- | --- |
| Proiektuaren antolaketa eta jarraipena | **Proiektuaren Eragiketak Kanpoko Programazioa**<br>Kanpoko programazio moduari esker, bezeroek modu natiboan sortu, eguneratu eta ezaba ditzakete lanaren banaketa egiturekin (WBS) zerikusia duten entitateak Dataverse API natiboak erabiliz, Project for the Web-ek ezartzen dituen egungo mugarik gabe. . | [Kanpoko Programazioa](/dynamics365/project-operations/project-management/external-scheduling) |
| Inplementazioa eta konfigurazioa | <p>**Eman bezeroei inplementazio mota aukeratzeko**<br>Project Operations-en produktuak gidatutako eguneraketak (PDU) Project Operations Dual-write soluzioa automatikoki instalatzeko erabiltzen dira, Dual-write core eta orkestrazio soluzioak ingurunean instalatuta daudenean.</p><p>Eginbide honek **soluzio berritze portaera** parametro berri bat aurkezten du Proiektuaren parametroetan. Parametro hau **Lite soilik** gisa ezartzen denean, PUDek ez dute automatikoki instalatuko Project Operations Dual-write soluzioa, nahiz eta Dual-write core eta orkestrazio soluzioak ingurunean instalatuta egon. . Jokabide honek Idazte bikoitzeko soluzioak erabiltzeko asmoa duten bezeroei mesede egingo die salmenta-eskaerak finantza- eta operazio-aplikazioetan integratzeko, baina Project Operations Lite moduan erabili nahi duten bezeroei (hau da, finantza- eta operazio-aplikazioetan integratu gabe).</p> | |
| Fakturazioa eta prezioak | <p>**Ingurune Integratuetan fakturatu gabeko salmenta-transakziorako moneta bihurtzea**<br>Finantza- eta eragiketa-aplikazioekin integratuta dauden Project Operations (hau da, baliabideak/hornitutako inplementazio motan) erabiltzen dituzten bezeroentzat, normalean, truke-tasak finantza- eta operazio-aplikazioetan menperatzen dira. However, if an expense category should be priced by using the "at cost" or "markup over cost" price calculation method when the customer is billed, the exchange rate that's used to calculate sales amount uses the exchange rates in Dataverse, not the exchange rates from finance and operations apps.</p><p>Eginbide honek **Moneta bihurtzeko portaera** parametro berri bat aurkezten du Proiektuaren parametroetan. Parametro hau **Erreserbarekin hedatua** gisa ezartzen denean, fakturatu gabeko salmenten zenbatekoak gastu-transakzioetan finantza- eta operazio-aplikazioetako kanbio-tasak erabiliz kalkulatzen dira.</p> | |

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2316317 | Sistemari esker, kobratu beharreko transakziorik ez duten fakturak sortu daitezke. |
| Fakturazioa eta prezioak | 2737300 | Egiaztatu **Bezeroa** eremuen erabilgarritasuna inprimakia sartu aurretik. |
| Fakturazioa eta prezioak | 2744948 | Gehitu egiaztapen nulua Fakturazio metodorako. |
| Fakturazioa eta prezioak | 2763515 | Erreferentzia hutsaren errorearen kudeatzailea fakturaren salmenta-kontratua falta denean. |
| Fakturazioa eta prezioak | 2844301 | Batch fakturak sortzeak huts egin du errore baten ondorioz. |
| Fakturazioa eta prezioak | 2845869 | Antolakuntza Zerbitzuaren biltegiratzea okerra. |
| Fakturazioa eta prezioak | 2853729 | Rolaren eta prezioaren xehetasunak fakturazio mota aldatzen direnean eguneratzen dira. |
| Fakturazioa eta prezioak | 2940350 | Benetako prezioak tasatzen direnean, prezioen zerrenda aktiboak soilik sartu behar dira automatikoki. |
| Inplementazioa eta konfigurazioa | 3001206 | msdyn\_ replaylogheader entitatea Bezeroen Erakundeen bertsio berritzea eragozten ari da. |
| Abaguneen kudeaketa | 2755582 | Erreferentzia nuluen salbuespenen kudeatzailea Split Billing Rule Helper-en. |
| Abaguneen kudeaketa | 2761477 | Zatitutako fakturazioa erabiltzen denean, mugarri bat (goiburua) ezabatzeak mugarri umezurtz uzten ditu. |
| Abaguneen kudeaketa | 2767595 | Materialaren erabilera-erregistro bat inprimaki nagusian irekitzen denean, erregistrorako erreserba daitekeen baliabidea une honetan saioa hasita dagoen erabiltzailera aldatzen da. |
| Proiektuaren antolaketa eta jarraipena | 2790384 | Pending OperationSet denbora-muga laburregia da. |
| Proiektuaren antolaketa eta jarraipena | 2957840 | Ezin dira atazak gorde eta zutabeak ezin dira gehitu proiektu integratuko Eragiketak ataleko **Zereginak** orrian. |
| Baliabideen kudeaketa | 2751560 | Baliabide-eskakizunean hobetsitako antolakuntza-unitate ez-koherenteak. |
| Azpikontratazioa | 2853245 | Saltzaileen faktura-lerroen benetako bat etortzeak ez du egiaztapen-egoera eguneratzen kontratu-lerro bat dagoeneko saltzaile-faktura-lerroarekin lotuta badago. |
| Azpikontratazioa | 2907231 | Saltzaileen fakturen prozesua ezin da aurreratu. |
| Denbora eta gastua | 2867363 | Erregistroak ez dira onartzeko faltak/oporrak ikuspegitik ateratzen onartzeko ilaran daudenean. |
| Denbora eta gastua | 2894405 | TESA: Erabiltzen ez den POC direktorioa betetze arazoak sortzen ari da. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Finantzan

Eguneratze honetan jasotako arazoen konponketen inguruko informazioa lortzeko, hasi saioa Microsoft Dynamics Lifecycle Services-en eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=745468).
