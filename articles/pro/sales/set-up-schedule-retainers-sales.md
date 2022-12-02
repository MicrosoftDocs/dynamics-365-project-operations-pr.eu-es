---
title: Konfiguratu aurrerapenaren antolaketa
description: Gai honek Project Operations-en atxikipen-egutegia nola konfiguratu jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 077961d2f649754149315438252970609c246555
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927727"
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