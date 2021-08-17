---
title: Konfiguratu aurrerapenaren antolaketa
description: Gai honek Project Operations-en atxikipen-egutegia nola konfiguratu jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a1cfd83837a91a8d1b3db6df688da6e216a90ada4735e5909a7e8cb26b87247d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994351"
---
# <a name="set-up-a-retainer-schedule"></a>Konfiguratu aurrerapenaren antolaketa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Atxikitzaileen ordutegiak **Proiektuaren kontratua** orria Dynamics 365 Project Operations-en.

1. **Proiektuaren kontratua** orrialdean, **Aurrerakinak eta gordailuak** fitxa, hautatu **Konfiguratu atxikitze ordutegia**.
2. Irekitzen den elkarrizketa-orrian, hurrengo taulan agertzen diren eremuak agertzen dira. Taulan sartutako balioek sortuko den atxikitze programan nola eragiten duten edo nola eragiten duten azaltzen da.

| Eremua | Deskribapena | Downstream eragina |
| --- | --- | --- |
| Proiektuaren kontratuaren bezeroa | Atxikipen edo aurrerakin hori fakturatuko zaion kontratuko bezeroak. | Kontratuan hainbat bezero badituzu eta horietako bakoitzari atxikipen zehatz bat edo aurrerakinaren zenbatekoa fakturatu behar badiozu, sortu eskuz faktura bat bezero bakoitzarentzat. |
| Aurrerapenaren antolaketaren hasiera | Idatzi aurrerakinaren antolaketaren hasiera-data. | Baliteke data hori ez izatea lehen atxikipena edo aurrerakina sortzen den eguna. Lehenengo atxikipena edo aurrerakina sortzen den datak fakturazioaren maiztasunaren eragina du. |
| Aurrerapenaren antolaketaren amaiera | Idatzi aurrerakinaren antolaketaren amaiera-data. | Baliteke data hori ez izatea lehen atxikipena edo aurrerakinaren azken eguna. Lehenengo atxikipena edo aurrerakinaren azken datak fakturazioaren maiztasunaren eragina du. |
| Sortzeko aurrerapen kopurua | Sortu beharreko atxikitzaile kopurua sartzen duzunean, sistemak hasiera-data eta maiztasuna erabiltzen ditu eremuko zenbakia sortzeko. | Eremu hau eskuz eguneratzen denean, sistemak ez dio jaramonik egiten **Atxikitzaileen ordutegiaren amaiera** eremuan eta horren ordez atxikipen edo aurrerapen kopuru zehatza sortzen du. |
| Fakturen maiztasuna | Aplikazioak zenbat aldiz sortuko dituen atxikipenak eta aurrerakuntzak. | Balio horrek zuzenean eragiten du atxikipen eta aurrerapen kopuruan eta sortutako datetan. |
| Zenbatekoa guztira | Zenbateko osoa sortuko den atxikipen indibidualean edo aurrerakinetan banatzen den zenbatekoa da. | Ez dago alor honen beherako eraginik. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]