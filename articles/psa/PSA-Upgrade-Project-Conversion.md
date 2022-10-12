---
title: Project Service Automation-en eginbide-aldaketak Project Operations-era
description: Artikulu honek ezaugarrien aldaketen ikuspegi orokorra eskaintzen du Microsoft Dynamics 365 Project Service Automation to Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 9869b3ad0fb6429484a26f367e06a0996f110ed8
ms.sourcegitcommit: a2d720ac6d7ddb20a0967fe87992a376b2478208
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/04/2022
ms.locfileid: "9621300"
---
# <a name="feature-changes-for-project-service-automation-to-project-operations"></a>Project Service Automation-en eginbide-aldaketak Project Operations-era

Proiektu bat berritu ondoren Microsoft Dynamics 365 Project Service Automation 3.X to Dynamics 365 Project Operations Lite, ezinezkoa da ataza-sareko lanaren banaketa egituran (WBS) proiektuko zereginak editatzea. Bezeroek WBSak berrikusi ahal izango dituzte jarraipen-sareko eremu berriak gehitu diren zereginarekin zerikusia duten xehetasun guztiak emateko. WBSren aldaketak behar diren proiektuetarako, hautagarri diren proiektuak proiektu berrira bihur ditzakezu web antolatzeko esperientziarako.

## <a name="project-conversion-process"></a>Proiektua bihurtzeko prozesua

Proiektu bat bihurtzeko, jarraitu urrats hauek.

1. Ireki proiektuaren orri nagusia eta hautatu **Bihurtu** Ekintza panelean.
1. Berrespen-mezuen koadroan, hautatu **Ados** proiektuaren bihurketa hasteko. Ekintza hauek gertatzen dira:

    1. Proiektuaren orri nagusian agertzen den mezu-barra batek honela dio: "Proiektuaren egutegia bihurtzen ari da. Ezin duzu proiektuan aldaketarik egin bihurketa amaitu arte".
    1. Proiektuen zerrendara birbideratuko zara.

    Proiektuaren bihurketa amaitu ondoren, ekintza hauek gertatzen dira:

    1. Esleitutako proiektuaren kudeatzaileak jakinarazpen bat jasotzen du aplikazioaren eskuinaldean.
    1. Bihurketa abian dela adierazten duen mezu-barra kendu da.
    1. The **Ordutegia** fitxak Weberako Project-ekin programazio esperientzia berria erakusten du. Lizentzia eta segurtasun rol egokiak dituen edozein erabiltzailek edita dezake WBS.
    1. The **Programazio motorra** eremua eguneratzen da **Weberako proiektua**.
    1. The **Bihurtu** botoia Ekintza Paneletik kenduko da.

> [!IMPORTANT]
> Ez da onartzen proiektuak masiboki bihurtzea. Proiektu bolumen handia aldi berean eguneratzeko edozein saiakera zapaldu egingo da. Muga honek bezero guztien errendimendu handia bermatzen laguntzen du.

## <a name="manual-tasks-vs-automatic-tasks"></a>Eskuzko zereginak versus zeregin automatikoak

Ingurune bat Project Service Automation-etik Project Operations-era eguneratzen denean, WBSko zeregin guztiak automatikoki programatuta hartzen dira. Eskuz programatutako zereginen kontzeptua ez dago erabilgarri Weberako Project-en. Hala ere, zure proiektuen programazio-portaera hobetsia defini dezakezu [programazio modua](/project-management/scheduling-modes.md) ezarpena proiektu berriak sortzen dituzunean.

## <a name="restricted-operations-for-pre-conversion-projects"></a>Bihurketa aurreko proiektuetarako eragiketa mugatuak

Atal honek proiektuak bihurtu ez direnean espero ditzakezun desberdintasun funtzionalak zehazten ditu.

### <a name="copy-project"></a>Kopiatu proiektua

The **Kopiatu** eragiketa bihurtutako proiektuetan soilik onartzen da. Berritutako proiektuak ezin dira kopiatu bihurtu aurretik.

### <a name="move-project"></a>Mugitu proiektua

Proiektu baten hasiera data aldatzeak ez du proportzionalki zereginen hasiera mugituko, proiektua bihurtu ez bada.

## <a name="frequently-asked-questions"></a>Ohiko galderak

### <a name="what-are-the-differences-between-converted-projects-and-new-projects-that-are-created-after-the-upgrade-has-been-completed"></a>Zein dira bertsio berritu ondoren sortzen diren proiektu bihurtutako eta proiektu berrien arteko aldeak?

Ingurumena berritu ondoren bihurtzen diren proiektuetarako, programazioari proiektuaren egutegia soilik errespetatzeko agintzen dion bandera bat ezarriko da. Portaera hau Project Service Automation-en portaerarekin bat dator. Hala ere, bandera ez da ezarriko bertsio berritu ondoren sortzen diren proiektu berrietarako. Beraz, ordutegiak baliabideen lanaldia errespetatuko du zeregin bati esleitzen zaizkionean.

### <a name="what-should-i-do-if-my-project-fails-to-be-converted"></a>Zer egin behar dut nire proiektua bihurtzen ez bada?

Zure proiektua ez bada bihurtzen, lehen urratsa erroreen erregistroak berrikustea da, zure WBSarekin erlazionatutako arazo arruntak identifikatzeko. Erregistroek ez badute ekintzarik egin dezakezun errore zehatzik adierazten, jarri harremanetan Bezeroarentzako laguntza-zerbitzuarekin zure kasua gehiago berrikusteko.

### <a name="how-are-business-closures-handled-in-project-for-the-web"></a>Nola kudeatzen dira negozioen itxierak Project for web-en?

Weberako proiektuak ez ditu errespetatzen enpresak erakunde mailan definitzen dituen negozioen itxierak. Hala ere, lan-orduaren txantiloi jakin batean definitutako beste atsedenaldi mota batzuk errespetatuko ditu.

### <a name="what-are-the-limitations-of-project-for-the-web"></a>Zeintzuk dira Project weberako mugak?

Ikusi [Sortu lanaren banaketa egitura: Proiektuaren mugak](/project-management/create-wbs#project-limitations.md).

### <a name="can-i-expect-changes-to-my-cost-and-sales-estimates"></a>Espero al dezaket nire kostuen eta salmenten kalkuluen aldaketak?

Baliabideen esleipenaren sestrak birkalkulatzen diren kasu bakanetan edo sorburu-proiektuaren beste data-muga batean daudenean, baliteke salmenten eta kostuen estimazioen desberdintasunak ikustea. Berritze-prozesuaren barruan, bezeroek proiektuen lagin-multzo adierazgarri bat probatzea espero da, programazio-aldaketak uler ditzaten.
