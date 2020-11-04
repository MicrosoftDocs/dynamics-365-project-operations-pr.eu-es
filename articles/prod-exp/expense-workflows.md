---
title: Konfiguratu gastuak kudeatzeko lan-fluxuak
description: Bidaia eta gastuen dokumentuak berrikusi eta onartzeko lan-fluxuaren prozesua konfigura dezakezu.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0af23ed2cf172e4c90de72f5db389c349303c039
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071190"
---
# <a name="set-up-expense-management-workflows"></a>Konfiguratu gastuak kudeatzeko lan-fluxuak

[!include [banner](../includes/banner.md)]

Bidaia eta gastuen dokumentuak berrikusi eta onartzeko erabiltzen den lan-fluxuaren prozesua konfigura dezakezu. Lan-fluxuak definitzeko dokumentuek gastuen txostenak, bidaia eskakizunak eta dirua aurreratzeko eskaerak defini ditzakete.

Lan-fluxuak negozio-prozesua adierazten du. Dokumentu bat sisteman zehar nola igarotzen den zehazten du eta zeregin bat nork bete edo dokumentu bat onartu behar duen adierazten du. Zure erakundeko lan-fluxuaren sistema erabiltzearen abantaila ugari daude:

-   **Prozesu koherenteak** : Dokumentu zehatzen onarpen prozesua defini dezakezu, hala nola erosketa eskaerak eta gastuen txostenak. Lan-fluxuaren sistema erabiliz dokumentuak modu koherentean eta eraginkorrean prozesatu eta onartzen direla ziurtatzen da.

-   Prozesuaren ikusgaitasuna: Lan-fluxu instantzia jakin baten egoera, historia eta errendimendu-metrikak jarrai ditzakezu. Horrek lan-fluxuan aldaketak egin behar diren ala ez zehazten lagunduko dizu eraginkortasuna hobetzeko.

-   Lan zerrenda zentralizatua: Erabiltzaileek lan zerrenda zentralizatua ikus dezakete esleitutako lan fluxuen zereginak eta onarpenak ikusteko. 

**Sor ditzakezun la-fluxuen motak**

Ondorengo taulan sortu ditzakezun lan-fluxu motak zerrendatzen dira **Gastuak**.


|              <strong>Mota</strong>              |                   <strong>Erabili mota hau</strong>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <strong>Gastuen txostena</strong>         |            Sortu onespen lan-fluxuak gastuen txostenetarako.             |
|  <strong>Gastuen txostenen argitaratze automatikoa</strong>   |        Sortu argitalpen automatikoko lan-fluxuak gastuen txostenetarako.        |
|       <strong>Gastuen lerroko elementua</strong>        |     Sortu onespen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.      |
| <strong>Gastuen lineako elementuak automatikoki argitaratzea</strong> | Sortu argitalpen automatikoen lan-fluxuak gastuen txosteneko lerroaren elementuetarako. |
|       <strong>Bidaiatzeko eskakizuna</strong>       |          Sortu onarpen-fluxuak bidaia-eskakizunetarako.           |
|      <strong>Diru-aurrerakinaren eskaera</strong>      |         Sortu onarpen-fluxuak dirua aurreratzeko eskaeretarako.          |
|        <strong>BEZ zergaren berreskurapena</strong>        | Balio erantsiaren gaineko zerga (BEZ) berreskuratzeko onarpen-fluxuak sortu.  |

