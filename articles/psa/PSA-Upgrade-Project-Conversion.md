---
title: Project Service Automation-etik Project Operations proiektuen antolaketa bihurtzeko prozesua
description: Artikulu honek Microsoft Dynamics 365 Project Service Automation-etik Dynamics 365 Project Operations-erako eginbide-aldaketen ikuspegi orokorra eskaintzen du.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/07/2022
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
ms.openlocfilehash: 84a40fcc9a8561c4ade0be175b08f701f3196508
ms.sourcegitcommit: 28004d38800782540fa5642d41f8fe0f6e2d9fa5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/08/2022
ms.locfileid: "9642553"
---
# <a name="project-service-automation-to-project-operations-project-scheduling-conversion-process"></a>Project Service Automation-etik Project Operations proiektuen antolaketa bihurtzeko prozesua

Proiektu bat berritu ondoren Microsoft Dynamics 365 Project Service Automation 3.X-tik Dynamics 365 Project Operations Lite-ra, ezinezkoa da ataza-sareko lanaren banaketa egituran (WBS) proiektuko zereginak editatzea. Bezeroek WBSak berrikusi ahal izango dituzte jarraipen-sareko eremu berriak gehitu diren zereginarekin zerikusia duten xehetasun guztiak emateko. WBSren aldaketak behar diren proiektuetarako, hautagarri diren proiektuak proiektu berrira bihur ditzakezu Project for the web antolatzeko esperientziarako.

## <a name="project-conversion-process"></a>Proiektuaren bihurketa prozesua

Jarraitu urrats hauek proiektua bihurtzeko.

1. Ireki proiektuaren orri nagusia eta hautatu **Bihurtu** Ekintza panelean.
1. Berrespen-mezuen koadroan, hautatu **Ados** proiektuaren bihurketa hasteko. Ekintza hauek gertatzen dira:

    1. Proiektuaren orri nagusian agertzen den mezu-barra batek honela dio: "Proiektuaren egutegia bihurtzen ari da. Bihurketa burutu arte ezingo duzu aldaketarik egin proiektuan".
    1. Proiektuen zerrendara birbideratuko zara.

    Proiektuaren bihurketa amaitu ondoren, ekintza hauek gertatzen dira:

    1. Esleitutako proiektuaren kudeatzaileak jakinarazpen bat jasotzen du aplikazioaren eskuinaldean.
    1. Bihurketa abian dela adierazten duen mezu-barra kendu da.
    1. **Ordutegia** fitxak Project for the web-ekin programazio esperientzia berria erakusten du. Lizentzia eta segurtasun funtzio egokiak dituen edozein erabiltzailek edita dezake WBS.
    1. **Programazio motorra** eremua eguneratzen da **Project for the web-era**.
    1. **Bihurtu** botoia Ekintza Paneletik kenduko da.

> [!IMPORTANT]
> Ez da onartzen proiektuak masiboki bihurtzea. Proiektu bolumen handia aldi berean eguneratzeko edozein saiakera zapaldu egingo da. Muga honek bezero guztien errendimendu handia bermatzen laguntzen du.

## <a name="manual-tasks-vs-automatic-tasks"></a>Eskuzko zereginak eta zeregin automatikoak

Ingurune bat Project Service Automation-etik Project Operations-era eguneratzen denean, WBSko zeregin guztiak automatikoki programatuta hartzen dira. Eskuz programatutako zereginen kontzeptua ez dago erabilgarri Project for the web-en. Hala ere, zure proiektuen programazio-portaera hobetsia defini dezakezu [programazio modua](/project-management/scheduling-modes.md) ezarpena erabiliz proiektu berriak sortzen dituzunean.

## <a name="restricted-operations-for-pre-conversion-projects"></a>Bihurketa aurreko proiektuetarako eragiketa mugatuak

Atal honek proiektuak bihurtu ez direnean espero ditzakezun desberdintasun funtzionalak zehazten ditu.

### <a name="copy-project"></a>Kopiatu proiektua

**Kopiatu** eragiketa bihurtutako proiektuetan soilik onartzen da. Berritutako proiektuak ezin dira kopiatu bihurtu aurretik.

### <a name="move-project"></a>Aldatu proiektua lekuz

Proiektu baten hasiera data aldatzeak ez du proportzionalki zereginen hasiera mugituko, proiektua bihurtu ez bada.

## <a name="frequently-asked-questions"></a>Ohiko galderak

### <a name="what-are-the-differences-between-converted-projects-and-new-projects-that-are-created-after-the-upgrade-has-been-completed"></a>Zein dira bertsio berritu ondoren sortzen diren proiektu bihurtutako eta proiektu berrien arteko aldeak?

Ingurunea berritu ondoren bihurtzen diren proiektuetarako, programazioari proiektuaren egutegia soilik errespetatzeko agintzen dion marka bat ezarriko da. Portaera hau Project Service Automation-en portaerarekin bat dator. Hala ere, marka ez da ezarriko bertsio berritu ondoren sortzen diren proiektu berrietarako. Beraz, antolaketak baliabideen lanaldia errespetatuko du zeregin bati esleitzen zaizkionean.

### <a name="what-should-i-do-if-my-project-fails-to-be-converted"></a>Zer egin behar dut nire proiektua bihurtzen ez bada?

Zure proiektua ez bada bihurtzen, lehen urratsa erroreen erregistroak berrikustea da, zure WBSarekin erlazionatutako arazo arruntak identifikatzeko. Erregistroek ez badute ekintzarik egin dezakezun errore zehatzik adierazten, jarri harremanetan Bezeroarentzako laguntza-zerbitzuarekin zure kasua gehiago berrikusteko.

### <a name="how-are-business-closures-handled-in-project-for-the-web"></a>Nola kudeatzen dira negozioen itxierak Project for the web-en?

Project for the web-ek ez ditu errespetatzen enpresak erakunde mailan definitzen dituen negozioen itxierak. Hala ere, lan-orduaren txantiloi jakin batean definitutako beste atsedenaldi mota batzuk errespetatuko ditu.

### <a name="what-are-the-limitations-of-project-for-the-web"></a>Zein dira Project for the web-en mugak?

Ikusi [Sortu zereginen xehetasunen egitura: proiektuaren mugak](/project-management/create-wbs#project-limitations.md).

### <a name="can-i-expect-changes-to-my-cost-and-sales-estimates"></a>Espero al dezaket nire kostuen eta salmenten kalkuluen aldaketak?

Baliabideen esleipenaren sestrak birkalkulatzen diren kasu bakanetan edo sorburu-proiektuaren beste data-muga batean daudenean, baliteke salmenten eta kostuen estimazioen desberdintasunak ikustea. Berritze-prozesuaren barruan, bezeroek proiektuen lagin-multzo adierazgarri bat probatzea espero da, programazio-aldaketak uler ditzaten.
