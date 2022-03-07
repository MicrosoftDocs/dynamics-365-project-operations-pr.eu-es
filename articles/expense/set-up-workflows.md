---
title: Konfiguratu Gastuak kudeatzeko lan-fluxuak
description: Bidaia eta gastuen dokumentuak berrikusi eta onartzeko erabiltzen den lan-fluxuaren prozesua konfigura dezakezu.
author: suvaidya
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 883e871b434c910747e45904cc9dc0c46bb4e2df788f503b848ad41984884edd
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6997726"
---
# <a name="set-up-workflows-for-expense-management"></a>Konfiguratu Gastuak kudeatzeko lan-fluxuak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Bidaia eta gastuen dokumentuak berrikusi eta onartzeko lan-fluxuaren prozesua konfigura dezakezu. Gastuen txostenak, bidaia eskakizunak eta dirua aurreratzeko eskaeren fluxuak defini ditzakezu.

Lan-fluxuak negozio-prozesua adierazten du eta dokumentu bat sisteman zehar nola igarotzen den definitzen du. Lan-fluxuak ere adierazten du nork bete behar duen edo dokumentu bat onartu behar duen. Zure erakundeko lan-fluxuaren sistema erabiltzearen abantaila ugari daude:

- **Prozesu koherenteak**: Dokumentu zehatzen onarpen prozesua defini dezakezu, hala nola erosketa eskaerak eta gastuen txostenak. Lan-fluxuaren sistema erabiliz dokumentuak modu koherentean eta eraginkorrean prozesatu eta onartzen direla ziurtatzen da.
- **Prozesuaren ikusgaitasuna**: Lan-fluxu instantzia jakin baten egoera, historia eta errendimendu-metrikak jarrai ditzakezu. Horrek lan-fluxuan aldaketak egin behar diren ala ez zehazten lagunduko dizu eraginkortasuna hobetzeko.
- **Lan zerrenda zentralizatua**: Erabiltzaileek lan zerrenda zentralizatua ikus dezakete esleitutako lan fluxuen zereginak eta onarpenak ikusteko. 

## <a name="workflow-types"></a>Lan-fluxua motak

Ondorengo taulan sortu ditzakezun lan-fluxu motak zerrendatzen dira **Gastuen kudeaketa**.


|              <strong>Mota</strong>              |                   <strong>Erabili mota hau</strong>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <strong>Gastuen txostenen onespen automatikoa</strong> |            Sortu onespen lan-fluxuak gastuen txostenetarako.             |
|  <strong>Gastuen txostenen argitaratze automatikoa</strong>   |        Sortu argitalpen automatikoko lan-fluxuak gastuen txostenetarako.        |
|       <strong>Gastuen lerroko elementua</strong>        |     Sortu onespen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.      |
| <strong>Gastuen lineako elementuak automatikoki argitaratzea</strong> | Sortu argitalpen automatikoen lan-fluxuak gastuen txosteneko lerroaren elementuetarako. |
|       <strong>Bidaiatzeko eskakizuna</strong>       |          Sortu onarpen-fluxuak bidaia-eskakizunetarako.           |
|      <strong>Diru-aurrerakinaren eskaera</strong>      |         Sortu onarpen-fluxuak dirua aurreratzeko eskaeretarako.          |
|        <strong>BEZ zergaren berreskurapena</strong>        | Balio erantsiaren gaineko zerga (BEZ) berreskuratzeko onarpen-fluxuak sortu.  |


[!INCLUDE[footer-include](../includes/footer-banner.md)]