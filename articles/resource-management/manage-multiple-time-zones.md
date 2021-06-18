---
title: Kudeatu ordu-zonak
description: Proiektu bat sortzen denean, bere ordu-zona aplikatutako lan-ordu txantiloian definitutako ordu-eremuan oinarritzen da.
author: ruhercul
ms.date: 10/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1480d68105be1041e791de567b180178b330d71e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997721"
---
# <a name="manage-time-zones"></a>Kudeatu ordu-zonak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


## <a name="projects"></a>Proiektuak

Proiektu bat sortzen denean, bere ordu-zona aplikatutako lan-ordu txantiloian definitutako ordu-eremuan oinarritzen da. **Proiektua** izan ere, datak beti daude fitxa bakoitzean saioa hasita duen erabiltzailearen ordu-zonaren aldean, **Zeregina** fitxa. Lanaren banakako egitura ikusten duzunean, datak proiektuaren ordu-eremuan erakutsiko dira beti.

## <a name="tasks"></a>Zereginak

Zeregin bat sortzen denean, hasiera ordua, amaiera ordua eta eguneko orduak proiektuaren lan orduek kontrolatzen dituzte. Adibidez, zeregin bat ordu-zona -8 PST duen eta laneko ordutegia duen proiektu batekin sortzen bada: 9:00etatik 17:00etara astelehenetik ostiralera, esleipenik gabe sortutako edozein zereginek hasiera ordua errespetatuko dute eta proiektuaren egutegiaren amaiera ordua.

## <a name="manage-resources-with-time-zones"></a>Kudeatu baliabideak ordu-zonekin

Erabiltzean emaitza zehatzak eta aurresatekoak lortzeko **Luzatu erreserba**, funtsezko bi baldintza bete behar dira:  

- Erabiltzaileak bere gailuaren ordu-eremua sisteman zehaztutako ordu-zonarekin bat etor dadin konfiguratu behar du **Pertsonalizazio-ezarpenak**.
 
  ![Ordu-eremuaren ezarpenak Windows 10-en](media/reconcile-assignments-03.png)

  ![Ordutegi-eremuaren ezarpenak pertsonalizazio-ezarpenetan](media/reconcile-assignments-04.png)
 
- Baliabide erreserbagarriak eskatutako luzapena definitzeko erabilitako sarrerak gainjartzen den lanaldiko minutu bat izan behar du gutxienez. Adibidez, goizeko 9:00etatik 19:00etara bitarteko lanorduekin honako baliabide hauek. 

  ![Baliabideen sarrerak alderatzea](media/reconcile-assignments-05.png)

Taula honek hau erakusten du:

- Proiektuaren egutegi-txantiloi bat
- A baliabidea: baliabide honek egutegi bera du eta proiektuaren ordu-eremu berean dago. Erreserbaren hasiera-ordua goizeko 09:00etan izango da.
- B Baliabidea: Baliabide hau proiektuarekiko beste ordu-zona batean dago eta goizeko 7:00etan hasten da haien ordu-gunean. Hala ere, erreserbak goizeko 09:00etan hasiko dira, esleipen-sarreraren hasiera-ordu goiztiarrena delako.
- C eta D baliabideak: baliabideak ordu-zona desberdinetan daude, bata bestearekin eta proiektuarekin desberdinak, eta erreserbak dagozkien hasiera-orduak baino lehenago hasten dira.

|Entitatea  |Egutegia  |
|-|-|
|Proiektuaren egutegi-txantiloia   | ![proiektuaren egutegia](media/reconcile-assignments-06.png) |
|A baliabidea  | ![A baliabidearen egutegia](media/reconcile-assignments-06.png) |
|B baliabidea  |  ![B baliabidearen egutegia](media/reconcile-assignments-07.png) |
|C baliabidea  |  ![C baliabidearen egutegia](media/reconcile-assignments-08.png) |
|D baliabidea  | ![D baliabidearen egutegia](media/reconcile-assignments-09.png)  |
 
Helbidera nabigatzen duzunean **Adiskidetzea** ikuspegia, baliabideen esleipenak eta horrekin lotutako erreserba eskasia bistaratzen dira.

![Bateratze-ikuspegia hedapenaren aurretik](media/reconcile-assignments-10.png)

Baliabide bakoitzerako hedapenaren erreserbaren funtzionalitatea erabili ondoren, erreserbak baliabide bakoitzerako behar bezala hedatzen dira, baliabide bakoitzaren lan orduak gabeziaren sestrarekin gainjartzen direlako.

![Bateratze-ikuspegia erreserba luzatu ostean](media/reconcile-assignments-11.png) 

Kontuan izan erreserben xehetasunak aztertuz gero, erreserbak hasteko orduaren aldeak erakusten dituela. Erreserbak esleipenaren sestra hasierako ordua baino lehenago hasten dira eta baliabidearen erabilgarri dagoen ordua baino lehenago hasten dira.

![Antolaketa-taulako baliabideen erreserba berriak](media/reconcile-assignments-12.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]