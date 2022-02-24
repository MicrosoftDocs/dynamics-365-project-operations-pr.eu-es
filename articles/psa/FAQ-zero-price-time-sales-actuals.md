---
title: Zergatik da prezio lehenetsia zero uneko denbora salmentan?
description: Uneko denboraren salmentan prezio lehenetsia 0 izatea arazoa konpontzeko.
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
ms.openlocfilehash: 5f72e0db94392a35fee9fdcf2c4adb8a08feef13
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146198"
---
# <a name="why-is-price-defaulting-to-zero-on-time-sales-actuals"></a>Zergatik da prezio lehenetsia zero uneko denbora salmentan?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Hau ri buruzko FAQ aplikatzen expense emaitzetan non transakzio heredatzen da Denbora eta transakzio mota ez dago Fakturatu gabeko salmentak. Hurrengo egiaztapenak hiru dira lagun konpontzeko zergatik prezioa (fakturazio-tasa) denbora salmenta benetako zenbatekoak kalkulatu, 0 defaulting da.

## <a name="check-1-identify-the-sales-price-list-for-the-project"></a>1. egiaztatu: Identifikatzeko proiektua salmenta prezio-zerrenda

Bilaketa proiektua orrira benetako eta deskonektatu proiektua eremu proiektua. Ondoren, joan Salmentak fitxan aurki daiteke eta saretan Proiektua Kontratu lineak, sakatu esteka Proiektua Kontratu eremuan. Orri Proiektua Kontratua ireki egingo da. Kontratu Proiektua orrian, joan Proiektua Prezio-Zerrendak fitxa Kontrol gutxienez prezio-zerrenda bat erantsita hemen baldin badago. Proiektuaren prezio-zerrendaren saretako prezio-zerrendarik ez badago Proiektu-kontraktua isolatutako arazoa. Prezio-zerrenda bat erantsi Proiektua Prezio-zerrendak saretan. Prezio-zerrendetako eransteko hemen koadrorako salmentak ezarri testuinguru eremua eta prezio-zerrendako moneta-eremu bat etorri behar dute, Proiektua kontratuaren moneta-eremu onartzen. Beharrezko konponketez egin ditzakezu, baina denbora-sarrera sortu berriro, onartu da eta egiaztatu salmentak unbilled benetako-erakusten prezio baliogabea. 

Prezio-zerrenda bat baino gehiago badituzu Proiektu-kontratuaren Proiektuaren Prezio-zerrenden saretan, joan hurrengo dokumentura.

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-sales-actual"></a>2. egiaztatu: bada beste prezio-zerrendarik identifikatuta zehaztutako datu benetako salmenta-kostuan?

Project Service hartu prezio defaulting prezio-zerrenda bat, prezio-zerrenda horren behar da aplikagarria salmentak denbora-salmenta benetako data. Egiaztatu hauek ikus gaineko identifikatutako prezio-zerrendak aplikagarria dira:
- Egiaztatu hasiera- eta amaiera-datak orokorra fitxan erantsita prezio-zerrendak hutsik ez. Hasiera eta amaiera-datak prezioa zerrendak gaineko identifikatu dira hutsik, arazoa isolated izan. 
- Egin ohar bat denbora-salmentaren hasiera-data eremua benetako eta egiaztatu identifikatutako prezio-zerrendak-da aplikagarria data. Adibidez, benetako denbora-salmentaren data behar daude hasiera-data eta amaiera-data ere prezio-zerrendan. 
    - Horri buruzko eremu zehatzera salmentak denbora-salmentaren benetako data horren prezio-zerrendarik ez badago, arazoa isolated izan. Aldatu, hasiera- eta amaiera-datak prezio-zerrenda, prezio-zerrenda benetako denbora-salmentaren data estaltzen dela ziurtatzeko. 
    - Benetako denbora-salmenta data estaltzen duen prezio-zerrenda bat baino gehiago badaude, arazo bakan bat duzu. Konpondu arazoa editatu hasiera- eta amaiera-datetan prezio-zerrendak-horri buruzko eremu zehatzera benetako denbora-salmentaren prezio-zerrenda bakarra dago daitezen. 
    - Horri buruzko eremu zehatzera benetako denbora-salmenten data horren prezio-zerrenda bakarra bada, joan 3. egiaztapenera.
Beharrezko konponketez egin ditzakezu, baina denbora-sarrera sortu berriro, onartu da eta egiaztatu fakturatu gabeko denbora-salmenten prezio baliogabea.

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-sales-actual"></a>3. egiaztatu: Badago prezio bat prezio-zerrendaren, prezioen neurriak dira benetako denbora-salmetan?

Behar bezala osatu Egiaztatu 1 eta 2 Egiaztatu, baduzu orain koadrorako proiektua prezio-zerrenda bakarra denbora-salmenta benetako data honetan aplikagarria den. Ireki Prezio-zerrenda eta joan Funtzio-prezioak fitxara. Ziurtatu errenkada bat dagoela prezio-dimentsioaren saretan benetako denbora-salmentan.

Badago errenkada ez dago prezio-prezioen neurriak dira benetako denbora-salmentaren funtzioa benetako, ondoren, duzu izan isolated arazoa. Sortu errenkada bat Funtzioa prezioak saretan, prezioen neurriak dira ordua zure benetako denbora-salmentan. Amaieran, beharrezko konponketez egin ditzakezu, baina denbora-salmenta sortu berriro, onartu da eta egiaztatu balio-kostua fakturatu gabeko prezio baliogabea.

Oraindik ikusten ez baduzu baliozko prezio benetako denbora salmenta atalean egiten egiaztapenak hiru goiko ondoren, itxaron saioa laguntza tiketa, gertaera bat. 

