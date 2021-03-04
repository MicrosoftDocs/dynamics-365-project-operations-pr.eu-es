---
title: Proiektuen txantiloiak
description: Gai honek proiektuaren txantiloiak proiektuaren konfigurazio bizkorra egiteko erabiltzeko moduari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: db42c9ea7280274cdc9cc90f1487f27e08f892e5
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148043"
---
# <a name="project-templates"></a>Proiektuen txantiloiak 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuen txantiloia aurrez zehaztutako markoa da, proiektu bat azkar eta erraz hasten laguntzeko. Klik bakar batekin beste proiektu bat sortzeko aurrez definitutako txantiloia erabil dezakezu. Proiektuei dagokienez, proiektuaren txantiloietarako baldintzak zehaztu beharko dituzu. Proiektuaren egutegia zehaztu behar duzu proiektuaren txantiloi bakoitzerako, eta funtzioak eta prezio-zerrendak lehenetsi behar dira antolakuntzan, txantiloiaren osagaiek datu baliagarriak izan ditzaten.

Proiektuaren txantiloia hiru osagaik osatzen dute: antolaketak, proiektuaren kalkuluek eta proiektuaren taldekideek.

## <a name="schedule"></a>Antolaketa

Proiektu baten txantiloiaren antolaketak proiektuko antolaketako elementu multzo bera du. Zereginen hierarkia bat sor dezakezu, funtzioak zereginekin esleitu ditzakezu, antolaketa atributuak zehaztu ditzakezu eta mendekotasunak ezarri ditzakezu. Proiektuaren txantiloiaren antolaketak zeregin bakoitzerako zeregin moduak ere onartzen ditu. Beraz, programazio motorra onartzen du. Proiektuaren egutegia proiektuarekin lotu behar duzu. Lan-antolaketa sortzen duzunean, ez dago alderik proiektua txantiloi baten eta proiektua baten artean.

## <a name="project-estimates"></a>Proiektuaren aurreikuspenak

Proiektuaren txantiloieko aurreikuspenek proiektuko aurreikuspenek bezala funtzionatzen dute. Hala ere, kostu- eta salmenta-prezioak parametroetan zehazten diren kostu lehenetsien eta salmenta prezioen zerrendetatik ateratzen dira.

## <a name="creating-a-project-from-a-template"></a>Sortu proiektua txantiloitik
 
Proiektuen txantiloi batetik proiektu bat sortzeko hainbat modu daude:

- Eskaintza batetik proiektua bat sortzen duzunean, proiektu-txantiloi bat aukera dezakezu **Sorrera bizkorra: proiektua** elkarrizketa-koadroan.

> ![Sorrera bizkorra: proiektuaren elkarrizketa-koadroa](media/project-11.png)

- Proiektua sortzen duzunean **Proiektu berria** hautatuta, **Proiektua** orria agertzen da erregistroa gorde aurretik. **Aukeratu txantiloia** eremuan, hautatu aurrez definitutako proiektuen txantiloiak antolakuntzan.
- Erabili **Sortu Proiektua txantiloi batetik** aukera **Txantiloiaren entitatea** orrian.

## <a name="copying-components-of-template-to-project"></a>Txantiloiko osagaiak proiektuan kopiatzea

Proiektuaren txantiloiaren osagaiak proiektu batean kopiatzean, zenbait birbidalketa gerta daitezke, proiektuaren ezarpenen arabera.

### <a name="copying-the-schedule"></a>Kopiatu antolaketa

Proiektuen txantiloi batetik antolaketa koipiatzen duzunean, proiektuaren egutegia txantilokoaren desberdina bada, proiektuko eguteko lanorduak aplikatzen dira zereginaren antolaketan. Horrela, antolaketa doitzen da backing proiektua egutegiarekin bat etortzeko. Era berean, antolaketako lehenengo zereginak proiektuaren hasiera-data hartzen du, eta gainerako hierarkiaren antolaketa eguneratu egiten da txantiloian zehaztutako iraupenean eta mendekotasunean oinarrituta. 

### <a name="copying-project-estimates"></a>Kopiatu proiektuaren aurreikuspenak 

Proiektuen aurreikuspenaren lerroetan kopiatzean, prezio-zerrendak eguneratzen dira. Kostuen prezio-zerrendarako, eguneratze horiek proiektuaren unitate jabetzan oinarritzen dira. Salmenten prezio-zerrendarako, bezeroan oinarritzen dira. Salmenta entitate bati esleitutako proiektuetarako, unitate-kostua eta salmenta-prezioak prezio-zerrenden arabera zehazten dira.

### <a name="copying-a-project-team"></a>Kopiatu proiektuaren taldea

Proiektu-talde bat proiektuaren txantiloitik proiektura kopiatzen denean, baliabideak orokorrak kopiatzen dira txantiloian zehaztutako gaitasun eta trebetasunekin batera. Baliabide orokorren esleipenak ere mantendu egiten dira proiektuaren txantiloian zeudelako. Baliabide izendatuak ez dira onartzen proiektuaren txantiloietan.


[!INCLUDE[footer-include](../includes/footer-banner.md)]