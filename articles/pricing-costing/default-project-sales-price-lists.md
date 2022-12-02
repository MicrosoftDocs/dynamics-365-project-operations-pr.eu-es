---
title: Prezio-zerrenda lehenetsiak
description: Artikulu honek salmenten eta kostuen prezio-zerrenda lehenetsiei buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 09/01/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 50dbf74e31b9eb8d63c378e5fd718dc17c9691f4
ms.sourcegitcommit: 16c9eded66d60d4c654872ff5a0267cccae9ef0e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/07/2022
ms.locfileid: "9410247"
---
# <a name="default-price-lists"></a>Prezio-zerrenda lehenetsiak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

## <a name="sales-price-lists"></a>Salmenten prezio-zerrendak

Dynamics 365 Project Operations-eko proiektuaren eskaintza eta kontratu bakoitzak salmenten prezio-zerrenda lehenetsia dauka. 

### <a name="price-list-default-on-project-quotes"></a>Prezioen zerrenda lehenetsia proiektuaren aurrekontuetan
Sistemak prozesu hau burutzen du proiektuaren aurrekontuan lehenetsitako prezio zerrenda zehazteko:

1. Sistemak kontuaren proiektuaren prezio zerrendetan erantsitako prezio zerrendak begiratzen ditu. 
1. Kontuaren erregistroan proiektuen prezioen zerrendak ez badaude, sistemak proiektuaren aurrekontuaren monetarekin bat datozen proiektuaren parametroei atxikitako salmenta prezioen zerrendak begiratzen ditu.
1. Ondoren, sistemak proiektuaren aurrekontuaren data tartearekin bat datozen prezio zerrenden data eraginkortasuna egiaztatzen du. Zehazki, eskaintza sortu zen data.
1. Proiektuaren aurrekontuaren datarako eraginkorrak diren prezioen zerrenda bat baino gehiago badira, prezioen zerrenda guztiak proiektuaren aurrekontuan lehenetsita daude.
1. Proiektuaren aurrekontuaren datarako indarrean dagoen prezio zerrendarik ez badago, proiektuaren aurrekontuan ez dago lehenetsitako proiektuen zerrendarik. Abisu mezu bat agertuko da proiektuaren aurrekontuan. Mezuan esaten da proiektuaren prezioen zerrendarik ez dagoenez, zure proiektuaren eta kalkulatutako egiazko eta lanaren kostuak ez direla tasatuko.

### <a name="price-list-default-on-project-contracts"></a>Prezioen zerrenda lehenetsia proiektuaren kontratuetan 
Sistemak prozesu hau burutzen du proiektuaren kontratuen lehenetsitako prezio zerrenda zehazteko:

1. Kontratua aurrekontu batetik sortuz gero, aurrekontuaren proiektuaren prezioen zerrendak banan-banan kopiatzen dira eta proiektuaren kontratuari eransten zaizkio.
1. Kontratua hutsetik sortzen bada, sistemak kontuko proiektuaren prezioen zerrendei atxikitako prezioen zerrendak begiratzen ditu. Kontuaren erregistroan proiektuen prezioen zerrendak badaude, sistemak proiektuaren kontratuaren monetarekin bat datozen proiektuaren parametroei atxikitako salmenta prezioen zerrendak begiratzen ditu.
1. Ondoren, sistemak proiektuaren kontratuaren data tartearekin bat datozen prezio zerrenden data eraginkortasuna egiaztatzen du. Zehazki, kontratua sortu zen data.
1. Kontratuaren datarako eraginkorrak diren prezioen zerrenda bat baino gehiago badira, prezioen zerrenda guztiak kontratuaren lehenetsita daude.
1. Kontratuaren datarako indarrean dagoen prezio zerrendarik ez badago, kontratuaren ez dago lehenetsitako proiektuen zerrendarik. Abisu mezu bat agertuko da proiektuaren kontratuan. Mezuan esaten da proiektuaren prezioen zerrendarik ez dagoenez, zure proiektuaren eta kalkulatutako egiazko eta lanaren kostuak ez direla tasatuko.

## <a name="cost-price-lists"></a>Kostuaren prezio-zerrendak

Kostuen prezioen zerrendek ez dituzte lehenetsitako proiektuen eragiketetako entitateak. Proiektuaren kostuetarako erabili beharreko kostuen prezioen zerrenda zehazteko transakzioen arabera egiten da. Sistemak prozesu hau burutzen du proiektuaren kostuen lehenetsitako prezio zerrenda zehazteko:

1. Sistemak proiektuaren kontratazio antolamendu unitateari atxikitako prezio zerrendak aztertzen ditu lehenik eta behin.
1. Hurrena, sistemak sarrerako estimazioaren edo benetako testuinguruarekin datarekin bat datozen prezio zerrenden dataren eraginkortasuna aztertzen du.

    - *Testuinguru estimatua lerroa* Project Operations-eko zenbatespenaren hiru testuinguruetako bat aipatzen du:

        - Proiektuaren aurreikuspen-lerroa
        - Eskaintzaren lerroaren xehetasunak
        - Kontratuaren lerroaren xehetasuna

    - *Testuinguru benetakoa* Project Operations-eko benetako datuen hiru iturburuetako bat aipatzen du:

       - Eskuz sortzen diren sarrera-egunkari-lerroak edo zuzenketa-egunkari batean sortzen diren zuzenketa-egunkari-lerroak
       - Denbora, gastu edo material erabileraren erregistroak bidaltzean sortzen diren aldizkari-lerroak
       - Fakturaren lerroaren xehetasunak

    Project Operations-en sarrerako egunkari-lerroaren data-eraginkortasuna edo faktura-lerroaren xehetasunarekin bat datozenean *benetako testuingurua*, erabiltzen du **Transakzio data** eremua.

    - Sarrerako estimazioko edo benetako testuinguruan eraginkorrak diren prezio zerrenda bat baino gehiago badira, azkenaldian sortutako prezio zerrenda hautatuko da.
    - Proiektuaren erakunde-unitatearen kontratuari proiektuen prezioen zerrendak badaude, sistemak proiektuaren aurrekontuaren monetarekin bat datozen proiektuaren parametroei atxikitako salmenta prezioen zerrendak begiratzen ditu.

## <a name="enable-multi-currency-cost-price-list"></a>Gaitu moneta ugariko kostuaren prezio-zerrenda

Ezarpen hau helbidean aurki daiteke **Ezarpenak** \> **Parametroak**. Balio lehenetsia **Ez** da.

Ezarpen hau gaituta dagoenean (hau da, balioa ezarrita dago **Bai**), sistemak honela jokatzen du:

- Kostu prezioen zerrendak edozein monetatan antolakuntza-unitatearekin lotzea ahalbidetzen du. Esaterako, kostu-prezioen zerrenda bat USD monetan erants daiteke antolakuntza-unitate bati. Sistemak baliozkotzen jarraituko du antolakuntza-unitate bati atxikitako kostu-prezio-zerrendek ez dutela data-eraginkortasun gainjarririk.
- Proiektuaren parametroei erantsitako kostu-prezio-zerrendek ez dutela data-eraginkortasun gainjarririk, moneta desberdinak izan arren. Portaera hau lehenetsitako portaeratik desberdina da (hau da, portaera balioa ezarrita dagoenean **Ez**). Portaera lehenetsian, kostu-prezioen zerrendak bakarrik daukaten **bera** moneta balioztatuta dago gainjartzen ez den dataren eragingarritasunerako.
- Sarrerako transakzio-testuinguru baterako, kostu-prezioen zerrenda zehazten du data-eraginkortasunean soilik oinarrituta. Portaera hau lehenetsitako portaeratik desberdina da, non sistemak proiektuaren moneta eta data-eraginkortasunarekin bat datorren kostu-prezio zerrenda hautatzen baitu.

Portaera aldaketa hauek direla eta, Project Operations bezeroek kostu-prezioen zerrenda global bat mantendu ahal izango dute, enpresa osoarentzat garrantzitsua izango dena. Ez dute prezio-zerrendarik izan beharko operazio-moneta bakoitzean. Prezio-zerrenda globalak data-eraginkortasuna izango du eta kostu-tasak edozein monetan ezartzea ahalbidetuko du prezioen dimentsio-balioen konbinazio zehatz baterako. Kostu prezioen zerrendako moneta balio lehenetsiak sartzeko soilik erabiltzen da **Rolen prezioak**, **Kategorien prezioak**, eta **Prezioen zerrenda** elementuen erregistroak sortzen dira. Ez da prezioen zerrenda zehazteko erabiliko.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
