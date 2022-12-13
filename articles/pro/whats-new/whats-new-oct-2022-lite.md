---
title: Zer berri 2022ko urrian - Project Operations lite inplementatzea
description: Artikulu honek Microsoft Dynamics 365 Project Operations lite inplementazioaren 2022ko urriko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: ramagadu
ms.date: 11/17/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: b6975e1f8645721fc03239b355b117eb664785f0
ms.sourcegitcommit: 1f162707ac342343fb5390fb9ae335e4cea4f3f2
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/29/2022
ms.locfileid: "9806712"
---
# <a name="whats-new-october-2022---project-operations-lite-deployment"></a>Zer berri 2022ko urrian - Project Operations lite inplementatzea

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.57.0.176

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

| Ezaugarrien eremua | Eginbidearen izena | Informazio gehiago |
| --- | --- | --- |
| Proiektuaren antolaketa eta jarraipena | **Proiektuaren Eragiketak Kanpoko Programazioa**<br>Kanpoko programazio moduari esker, bezeroek modu natiboan sortu, eguneratu eta ezaba ditzakete lanaren banaketa egiturekin (WBS) zerikusia duten entitateak Dataverse API natiboak erabiliz, Project for the Web-ek ezartzen dituen egungo mugarik gabe. . | [Kanpoko Programazioa](/dynamics365/project-operations/project-management/external-scheduling) |
| Inplementazioa eta konfigurazioa | <p>**Eman bezeroei inplementazio mota aukeratzeko**<br>Project Operations-en produktuak gidatutako eguneraketak (PDU) Project Operations Dual-write soluzioa automatikoki instalatzeko erabiltzen dira, Dual-write core eta orkestrazio soluzioak ingurunean instalatuta daudenean.</p><p>Eginbide honek **soluzio berritze portaera** parametro berri bat aurkezten du Proiektuaren parametroetan. Parametro hau **Lite soilik** gisa ezartzen denean, PUDek ez dute automatikoki instalatuko Project Operations Dual-write soluzioa, nahiz eta Dual-write core eta orkestrazio soluzioak ingurunean instalatuta egon. . Jokabide honek Idazte bikoitzeko soluzioak erabiltzeko asmoa duten bezeroei mesede egingo die salmenta-eskaerak finantza- eta operazio-aplikazioetan integratzeko, baina Project Operations Lite moduan erabili nahi duten bezeroei (hau da, finantza- eta operazio-aplikazioetan integratu gabe).</p> | |

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2316317 | Sistemari esker, kobratu beharreko transakziorik ez duten fakturak sortu daitezke. |
| Fakturazioa eta prezioak | 2737300 | Egiaztatu Bezeroaren eremuaren erabilgarritasuna inprimakia sartu aurretik. |
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
| Baliabideen kudeaketa | 2751560 | Baliabide-eskakizunean hobetsitako antolakuntza-unitate ez-koherenteak. |
| Azpikontratazioa | 2907231 | Saltzaileen fakturen prozesua ezin da aurreratu. |
| Denbora eta gastua | 2867363 | Erregistroak ez dira onartzeko faltak/oporrak ikuspegitik ateratzen onartzeko ilaran daudenean. |
| Denbora eta gastua | 2894405 | TESA: Erabiltzen ez den POC direktorioa betetze arazoak sortzen ari da. |
