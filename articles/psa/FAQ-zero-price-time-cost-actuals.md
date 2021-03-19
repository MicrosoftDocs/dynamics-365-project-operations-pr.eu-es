---
title: Zergatik da prezio lehenetsia zero uneko denbora kostuan?
description: Uneko denboraren kostuan prezio lehenetsia 0 izatea arazoa konpontzeko.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 65f2bc773a376800928cc3746691061d8e290f74
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285783"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a>Zergatik da prezio lehenetsia zero uneko denbora kostuan?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Hau ri buruzko FAQ aplikatzen denbora emaitzetan non transakzio heredatzen da denbora eta transakzio mota ez dago Kostua. Hurrengo egiaztapenak hiru dira lagun konpontzeko zergatik prezio denbora salmenta benetako zenbatekoak kalkulatu, 0 defaulting da.
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a>1. egiaztatu: Identifikatu kostuaren prezio-zerrenda proiekturako

Bilaketa proiektua orrira benetako eta deskonektatu proiektua eremu proiektua. Sakatu eremuan unitate esteka contracting. Unitate Contracting orrian, egiaztatu contracting unitate duela prezio-zerrenda bat Kostua Prezio-Zerrendak saretan.

Prezio-zerrenda bat baino gehiago badago, arazoa isolated izan. Project Service bakarrik onartzen prezio-zerrenda bat bakoitzeko antolakuntza unitatea. Kendu prezio-zerrendak entitate honen prezio-zerrenda bakarra Antolakuntza Unitatea-Kostua Prezio-Zerrendak azpisaretan erantsita arte.

Erantsitako Antolakuntza Unitatea ez dago prezio-zerrendak badira, egin Antolakuntza unitatea moneta-oharra. Joan Project Service-ra eta, ondoren, Parametroak eta Prezio-Zerrendak fitxa Kontrol prezio-zerrendak edozein Kostua eta Antolakuntza Unitatea moneta bat datorren moneta-testuinguru badaude, ireki.
 
Horren irizpideekin bat datozen prezio-zerrendak ez badira, arazoak isolated izan. Ziurtatu gutxienez prezio-zerrendaren Kostua ezarrita testuinguru kontrolatzen dute eta moneta kontrolatzen Antolakuntza Unitatea moneta bat.

Horren irizpideekin bat datozen prezio-zerrenda bat baino gehiago badago, jarraitu irakurketa-dokumentuaren egiaztapenak gehiago egiteko.

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a>2. egiaztatu: bada beste prezio-zerrendarik identifikatuta zehaztutako datu benetako denbora-kostuan?

Project Service hartu prezio defaulting prezio-zerrenda bat, prezio-zerrenda horren behar da aplikagarria salmentak denbora-kostua benetako data. Egiaztatu hauek ikus gaineko identifikatutako prezio-zerrendak aplikagarria dira:

- Egiaztatu hasiera- eta amaiera-datak orokorra fitxan erantsita prezio-zerrendak hutsik ez. Hasiera eta amaiera-datak prezioa zerrendak gaineko identifikatu dira hutsik, arazoa isolated izan. 
- Egin ohar bat denbora-kostuaren hasiera-data eremua benetako eta egiaztatu identifikatutako prezio-zerrendak-da aplikagarria data. Adibidez, benetako denbora-kostuaren data behar daude hasiera-data eta amaiera-data ere prezio-zerrendan. 
    - Horri buruzko eremu zehatzera salmentak denbora-kostuaren benetako data horren prezio-zerrendarik ez badago, arazoa isolated izan. Aldatu, hasiera- eta amaiera-datak prezio-zerrenda, prezio-zerrenda benetako denbora-kostuaren data estaltzen dela ziurtatzeko. 
    - Benetako denbora-kostuko data estaltzen duen prezio-zerrenda bat baino gehiago badaude, arazo bakan bat duzu. Konpondu arazoa editatu hasiera- eta amaiera-datetan prezio-zerrendak-horri buruzko eremu zehatzera benetako denbora-kostuaren prezio-zerrenda bakarra dago daitezen. 
    - Horri buruzko eremu zehatzera kostuaren ordua benetako data prezio-zerrenda bat badago, mugitu begiratu hurrengo dokumentua.
Beharrezko konponketez egin ditzakezu, baina denbora-sarrera sortu berriro, onartu da eta egiaztatu fakturatu gabeko denbora-kostuaren prezio baliogabea.

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a>3. egiaztatu: Badago prezio bat prezio-zerrendaren, prezioen neurriak dira ordua kostuaren benetako?

Behar bezala osatu Egiaztatu 1 eta 2 Egiaztatu, baduzu orain koadrorako proiektua prezio-zerrenda bakarra denbora-kostua benetako data honetan aplikagarria den. Ireki Prezio-zerrenda eta joan Funtzio-prezioak fitxara. Ziurtatu errenkada bat dagoela prezio-dimentsioaren saretan benetako denbora-kostuan.

Badago errenkada ez dago prezio-prezioen neurriak dira ordua kostuaren-saretan funtzioa benetako, ondoren, duzu izan isolated arazoa. Sortu errenkada bat Funtzioa prezioak saretan, prezioen neurriak dira ordua zure kostuaren-benetako. Amaieran, beharrezko konponketez egin ditzakezu, baina denbora-sarrera sortu berriro, onartu da eta egiaztatu balio-kostua fakturatu gabeko prezio baliogabea.
 
Oraindik ikusten ez baduzu baliozko denbora-kostua benetako atalean egiten egiaztapenak hiru goiko ondoren, itxaron saioa laguntza tiketa, gertaera bat.





[!INCLUDE[footer-include](../includes/footer-banner.md)]