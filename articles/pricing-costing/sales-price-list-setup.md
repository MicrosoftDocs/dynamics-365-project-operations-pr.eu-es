---
title: Salmenten prezio-zerrendaren konfigurazioa
description: Gai honek proiektu-prezioaren salmenten prezio-zerrendak buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1d2c797b72666123eb0a18d2d0c1df9fe3d207f7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071091"
---
# <a name="sales-price-list-setup"></a>Salmenten prezio-zerrendaren konfigurazioa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuen eskaintzen eta kontratuen kasuan, proiektuen prezio-zerrendak produktuen prezio-zerrenda baino beste prezio eredu bat du. Produktuen katalogoan oinarritutako eskaintzaren lerroan, prezioa zuzendu eta funtzioetara zuzendu daiteke eskaintzaren lerroan. Eskaintzaren lerro bakoitzak katalogoko elementu bat besterik ez duelako. Dena den, proiektuan oinarritutako eskaintzaren lerroan, ezin duzu prezioa zuzendu eskaintzaren lerroan eta kategorietan zuzenean. Proiektuaren prezioen zerrenda bi gainidazketa eredu desberdinekin funtzionatzeko erabil dezakezu.

> [!NOTE]
> Zure proiektuaren baliabideen eta katalogoko elementuen prezio-zerrenda berezi bat izatea gomendatzen dugu, prezioak baliogabetzen dituzunean bien arteko portaera desberdintasunak direla eta.

Erakunde hauetako bakoitzak salerosketako prezioe-zerrenda bat edo gehiago izan ditzake proiektuaren prezioetarako:

- Bezeroa (kontua) 
- Abagunea 
- Eskaintza 
- Proiektu-kontratua

Prezio-zerrenda duten entitate horien elkartea proiektuaren prezio-zerrendek adierazten dute. Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu.

Lehenetsitako proiektuen prezio-zerrenda ez da automatikoki sartu bezeroaren erregistroan. Hala ere, proiektuaren prezio-zerrenda eskuz erantsi dezakezu bezeroaren erregistroan. Nolanahi ere, proiektuaren prezio-zerrenda eskuz erantsi behar zenuke bezeroarekin prezioen akordio pertsonalizatua denean. 

Proiektuen prezioen zerrenda salmenta erakunde bati atxikitakoan, informazio hau balioztatzen du:

- Prezio-zerrenda testuinguru bat da **Salmentak**. 
- Monetak prezio-zerrendaren monetarekin bat dator. 

Proiektu baten kontratuan, lehentasun hurrenkera hau proiektuaren inguruko prezioen zerrendak automatikoki ezartzeko:

1. Eskaintza
2. Abagunea
3. Bezeroa 
4. Ezarpen orokorrak 

Proiektuen prezio-zerrenda lehenespenez sartzen denean, sistemak balioztatzen du moneta bezeroaren monetarekin bat datorrela eta sartu diren prezio-zerrenden lehenetsiak testuinguruan **salmentak**.

Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu. Gaitasun honek iraupen luzeko proiektu kontratuetarako zehaztutako prezioak onartzen ditu, non prezio-zerrenda bat baino gehiago eska dezakezun inflazioaren ondorioz gertatzen diren prezioen eguneratzeak kontatzeko. Hala ere, bezeroa, abagunea, eskaintza edo proiektu-kontratuaren entitatearekin lotzen dituzun prezioen zerrendek data eraginkortasun bat badute, baliteke prezio lehenetsiak okerrak izatea. Hori dela eta, ziurtatu behar duzu data eraginkortasuna bata bestearen gainjartzen duten proiektuen prezio-zerrendak ez daudela entitate horiekin lotuta.
