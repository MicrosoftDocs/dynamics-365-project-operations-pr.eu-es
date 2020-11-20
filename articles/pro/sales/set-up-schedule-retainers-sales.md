---
title: Konfiguratu aurrerapenen antolaketa - arina
description: Gai honek Project Operations-en atxikipen-egutegia nola konfiguratu jakiteko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5e0312b89d9969f140146b6aaaa9bdcfde702c0b
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181257"
---
# <a name="set-up-a-retainer-schedule---lite"></a>Konfiguratu aurrerapenen antolaketa - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

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
