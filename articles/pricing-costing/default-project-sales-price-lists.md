---
title: Prezio-zerrenda lehenetsiak
description: Gai honek salmenten eta kostuen prezio-zerrenda lehenetsiei buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 275ef9b9706d212a6da0dc7c060081c3226572f3
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070915"
---
# <a name="default-price-lists"></a>Prezio-zerrenda lehenetsiak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

## <a name="sales-price-lists"></a>Salmenten prezio-zerrendak

Dynamics 365 Project Operations proiektuaren aurrekontu eta kontratu guztiek salmenta prezioen zerrenda lehenetsia dute. 

### <a name="price-list-default-on-project-quotes"></a>Prezioen zerrenda lehenetsia proiektuaren aurrekontuetan
Sistemak prozesu hau burutzen du proiektuaren aurrekontuan lehenetsitako prezio zerrenda zehazteko:

1. Sistemak kontuaren proiektuaren prezio zerrendetan erantsitako prezio zerrendak begiratzen ditu. 
2. Kontuaren erregistroan proiektuen prezioen zerrendak badaude, sistemak proiektuaren aurrekontuaren monetarekin bat datozen proiektuaren parametroei atxikitako salmenta prezioen zerrendak begiratzen ditu.
3. Ondoren, sistemak proiektuaren aurrekontuaren data tartearekin bat datozen prezio zerrenden data eraginkortasuna egiaztatzen du. Zehazki, eskaintza sortu zen data.
4. Proiektuaren aurrekontuaren datarako eraginkorrak diren prezioen zerrenda bat baino gehiago badira, prezioen zerrenda guztiak proiektuaren aurrekontuan lehenetsita daude.
5. Proiektuaren aurrekontuaren datarako indarrean dagoen prezio zerrendarik ez badago, proiektuaren aurrekontuan ez dago lehenetsitako proiektuen zerrendarik. Abisu mezu bat agertuko da proiektuaren aurrekontuan. Mezuan esaten da proiektuaren prezioen zerrendarik ez dagoenez, zure proiektuaren eta kalkulatutako egiazko eta lanaren kostuak ez direla tasatuko.

### <a name="price-list-default-on-project-contracts"></a>Prezioen zerrenda lehenetsia proiektuaren kontratuetan 
Sistemak prozesu hau burutzen du proiektuaren kontratuen lehenetsitako prezio zerrenda zehazteko:

1. Kontratua aurrekontu batetik sortuz gero, aurrekontuaren proiektuaren prezioen zerrendak banan-banan kopiatzen dira eta proiektuaren kontratuari eransten zaizkio.
2. Kontratua hutsetik sortzen bada, sistemak kontuko proiektuaren prezioen zerrendei atxikitako prezioen zerrendak begiratzen ditu. Kontuaren erregistroan proiektuen prezioen zerrendak badaude, sistemak proiektuaren kontratuaren monetarekin bat datozen proiektuaren parametroei atxikitako salmenta prezioen zerrendak begiratzen ditu.
4. Ondoren, sistemak proiektuaren kontratuaren data tartearekin bat datozen prezio zerrenden data eraginkortasuna egiaztatzen du. Zehazki, kontratua sortu zen data.
5. Kontratuaren datarako eraginkorrak diren prezioen zerrenda bat baino gehiago badira, prezioen zerrenda guztiak kontratuaren lehenetsita daude.
6. Kontratuaren datarako indarrean dagoen prezio zerrendarik ez badago, kontratuaren ez dago lehenetsitako proiektuen zerrendarik. Abisu mezu bat agertuko da proiektuaren kontratuan. Mezuan esaten da proiektuaren prezioen zerrendarik ez dagoenez, zure proiektuaren eta kalkulatutako egiazko eta lanaren kostuak ez direla tasatuko.

## <a name="cost-price-lists"></a>Kostuaren prezio-zerrendak

Kostuen prezioen zerrendek ez dituzte lehenetsitako proiektuen eragiketetako entitateak. Proiektuaren kostuetarako erabili beharreko kostuen prezioen zerrenda zehazteko momentuan egiten da beti. Sistemak prozesu hau burutzen du proiektuaren kostuen lehenetsitako prezio zerrenda zehazteko:

1. Sistemak proiektuaren kontratazio antolamendu unitateari atxikitako prezio zerrendak aztertzen ditu lehenik eta behin.
2. Sistemak sarrerako estimazioaren edo benetako lerroaren datarekin bat datozen prezio zerrenden dataren eraginkortasuna aztertzen du. Egoera horretan, *kalkulatzeko lerroa* Project Operations-eko zenbatespenaren hiru testuinguruak aipatzen ditu:

    - Proiektuaren aurreikuspen-lerroa
    - Eskaintzaren lerroaren xehetasunak
    - Kontratuaren lerroaren xehetasuna
  
3. Sarrerako estimazioan edo benetako egunean eraginkorrak diren prezio zerrenda bat baino gehiago badira, azkenaldian sortutako prezio zerrenda hautatuko da.
4. Proiektuaren erakunde-unitatearen kontratuari proiektuen prezioen zerrendak badaude, sistemak proiektuaren aurrekontuaren monetarekin bat datozen proiektuaren parametroei atxikitako salmenta prezioen zerrendak begiratzen ditu.
5. Hurrena, sistemak sarrerako estimazioaren edo benetako lerroaren datarekin bat datozen prezio zerrenden dataren eraginkortasuna aztertzen du. 
6. Sarrerako estimazioan edo benetako egunean eraginkorrak diren prezio zerrenda bat baino gehiago badira, azkenaldian sortutako prezio zerrenda hautatuko da.
7. Proiektuaren parametroei moneta eta efektibitate datarekin bat datozen kostu prezioen zerrendarik ez badago, sistemak kostu tasa zero (0) lehenetsiko du sarrerako estimazioan edo benetako lerroan.