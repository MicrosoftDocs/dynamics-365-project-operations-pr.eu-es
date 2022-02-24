---
title: Zergatik da prezioaren lehenetsia zero benetako gastuen salmenta?
description: Hurrengo egiaztapenak hiru dira lagun konpontzeko zergatik prezio expense salmenta benetako zenbatekoak kalkulatu, 0 defaulting da.
author: rumant
ms.prod: ''
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
ms.openlocfilehash: 92b507d8e5605c01f1a9235233b3cd2885070749
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5992996"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-sales-actuals"></a>Zergatik da prezioaren lehenetsia zero benetako gastuen salmenta?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Hau ri buruzko FAQ aplikatzen expense emaitzetan non transakzio heredatzen da Expense eta transakzio mota ez dago Fakturatu gabeko salmentak. Hurrengo egiaztapenak hiru dira lagun konpontzeko zergatik prezioa (fakturazio-tasa) expense salmenta benetako zenbatekoak kalkulatu, 0 defaulting da.

## <a name="check-1-identify-the-sales-price-list-for-project"></a>1. egiaztatu: Identifikatzeko proiektua salmenta prezio-zerrenda

Bilaketa proiektua orrira benetako eta deskonektatu proiektua eremu proiektua. Ondoren, joan Salmentak fitxan aurki daiteke. Saretan Proiektua Kontratu lineak, sakatu esteka Proiektua Kontratu eremuan. Orri Proiektua Kontratua ireki egingo da. Kontratu Proiektua orrian, joan Proiektua Prezio-Zerrendak fitxa Kontrol gutxienez prezio-zerrenda bat erantsita hemen baldin badago.

Prezio-zerrendarik ez badago erantsita Proiektu-kontratuaren Proiektuaren prezio-zerrendak saretan:

- Prezio-zerrenda bat erantsi Proiektua Prezio-zerrendak saretan. Prezio-zerrendetako eransteko hemen koadrorako salmentak ezarri testuinguru eremua eta prezio-zerrendako moneta-eremu bat etorri behar dute, Proiektua kontratuaren moneta-eremu onartzen. Beharrezko konponketez egin ditzakezu, baina expense-sarrera sortu berriro, onartu da eta egiaztatu salmentak unbilled benetako-erakusten prezio baliogabea.
- Gutxienez prezio-zerrendak Proiektua kontratuaren Proiektua Prezio-Zerrendak saretan erantsita baduzu, joan Kontrol-2.

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-expense-actual"></a>2. egiaztatu: Dira gaineko identifikatutako prezio-zerrendak-benetako expense data jakin baliozko?

Project Service hartu prezio defaulting prezio-zerrenda bat, prezio-zerrenda horren behar da aplikagarria salmentak expense benetako data. Egiaztatu hauek ikus gaineko identifikatutako prezio-zerrendak aplikagarria dira:

- Egiaztatu arabera hasi hasiera- eta amaiera-datak orokorra fitxan erantsita prezio-zerrendak hutsik ez. Hasiera eta amaiera-datak prezioa zerrendak gaineko identifikatu dira hutsik, arazoa isolated izan. 
- Egin ohar bat expense salmentak hasiera-data eremua benetako eta egiaztatu identifikatutako prezio-zerrendak-da aplikagarria data. Adibidez, benetako expense data behar daude hasiera-data eta amaiera-data ere prezio-zerrendan. 
    - Horri buruzko eremu zehatzera salmentak expense benetako data horren prezio-zerrendarik ez badago, arazoa isolated izan. Aldatu, hasiera- eta amaiera-datak prezio-zerrenda, prezio-zerrenda benetako expense data estaltzen dela ziurtatzeko. 
    - Benetako gastuen salmentako data estaltzen duen prezio-zerrenda bat baino gehiago badaude, arazo bakan bat duzu. Editatu hasiera- eta amaiera-datetan prezio-zerrendak-horri buruzko eremu zehatzera benetako gastuen data prezio-zerrenda bakarra dago daitezen. 
    - Horri buruzko eremu zehatzera benetako expense data horren prezio-zerrenda bakarra bada, Begiratu 3 mugitzeko.
Beharrezko konponketez egin ditzakezu, baina expense-sarrera sortu berriro, onartu da eta egiaztatu salmentak unbilled benetako-erakusten prezio baliogabea.

## <a name="check-3-is-there-a-valid-price-for-the-expense-category-in-the-applicable-project-price-list"></a>3. egiaztatu: Ez Da baliozko prezio bat prezio-zerrendaren aplikagarria proiektua expense kategoria? 

Behar bezala osatu Egiaztatu 1 eta 2 Egiaztatu, baduzu orain koadrorako proiektua prezio-zerrenda bakarra salmentak expense benetako data honetan aplikagarria den. Ireki Proiektua Prezio-Zerrenda eta Kategoria Prezioak fitxa joan Ziurtatu dela errenkada bat tresna-barran, Expense jakin expense kategoria saretan benetako.
 
- Errenkada ez bada, ondoren, duzu izan isolated arazoa. Sortu errenkada bat expense zure kategoria-Kategoria prezio sareta benetako. Ondoren, beharrezko konponketez egin ditzakezu, baina expense-sarrera sortu berriro, onartu da eta egiaztatu salmentak unbilled benetako-erakusten prezio baliogabea. 
- Kategoria prezioak saretan expense kategoria-errenkada bat bada, kontrol-prezio baliogabea da.

Zer ulertzeko prezio baliogabea da, hauek metodoak erabili:

- Kategoria prezio ilaran Prezio-Metodoa eremu gisa ezarrita badago Une Kostua, salmentak Expense benetako atalean unitate tasa Expense sarrera balioa defaulted izango da gero.
- Prezio-Metodoa Kategoria prezio ilaran eremua prezio-Igoeraren Ehunekoa gisa ezarrita badago, ondoren, egiaztatu eremu Ehunekoa baliozko balio bat esleitzeko ezartzen da. Tresna-barran salmentak Expense benetako unitate tasa Expense sarrera prezioa hau prezio-igoeraren ehunekoa aplikatuz defaulted da.
- Kategoriaren prezio-lerroko Prezio-metodoaren eremua Prezioa unitateko gisa ezarrita dago, eta egiaztatu Prezio-eremua baliozko balio gisa ezarrita badago. Tresna-barran salmentak Expense benetako unitate tasa moneta-zenbatekoaren Prezio eremuan zehaztutako defaulted da.

Kategoria expense instalazio-programak prezio baliogabea ez, ondoren, duzu izan isolated arazoa. Urratsak eremu egokira arauak in accordance with expense kategoria-prezio baliogabea dituen kategoria prezio linea editatzeko da soluzioa. Amaieran, beharrezko konponketez egin ditzakezu, baina expense-sarrera sortu berriro, onartu da eta egiaztatu salmentak unbilled benetako-erakusten prezio baliogabea.

Oraindik ikusten ez baduzu baliozko prezio salmentak expense benetako atalean egiten egiaztapenak hiru goiko ondoren, itxaron saioa laguntza tiketa, gertaera bat.




[!INCLUDE[footer-include](../includes/footer-banner.md)]