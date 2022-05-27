---
title: Konpromiso baten salmenta aurreko fasean benetako eragina
description: Gai honek Errealitateak taulan izandako eraginari buruzko informazioa eskaintzen du hainbat ekitalditan konpromiso bat Microsoft-en salmenta aurreko fasean dagoen bitartean Dynamics 365 Project Operations.
author: rumant
ms.date: 02/22/2022
ms.topic: overview
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: ad62639b345d5519b103d4bde3fbb033b9a7a519
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8577221"
---
# <a name="actuals-impact-during-the-pre-sales-stage-of-an-engagement"></a>Konpromiso baten salmenta aurreko fasean benetako eragina

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Ondorengo taulak proiektuko konpromiso baten salmenta-aurreko fasean hainbat ekitalditan sortzen diren transakzio mota desberdinen errealak zerrendatzen ditu.

| Gertaera | Benetako kostua | Adibidez |
|---|---|---|
| Denbora sortzen da. | Ez da aplikagarria | <p>Bob Kozack, orduko 100 dolar (100 USD) kostu-tasa duen Fabrikam AEBko antolakuntza-unitatekoa, "Arm Installation at Adatum" izeneko proiektuan ari da lanean. Proiektu hau kontratu-lerroan prezio finkoko fakturazio-metodo batera lotzen da. Hona hemen Bob Kozak-en denboraren lagin bat:</p><p>Bob Kozack - 8 ordu</p> |
| Denbora aurkeztu da. | Ez da aplikagarria | Kostuen egunkari-lerro bat sortzen da denbora-sarrerarako. Kostu-tasa lehenetsia aldizkariko sarreran sartzen da. |
| Denbora-sarrera gogoratzen da onartu baino lehen. | Ez da aplikagarria | |
| Ordua onartu da. | Benetako kostu bat sortzen da. | <p>Sortzen den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Denbora onarpena bertan behera utzi da. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |
| Ordu-sarrera gogoratzen da onartu ondoren. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |
| Aurrekontua irabazi, eta kontratua sortzen da. | <p>Kostu erreal zaharren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu errealak sortzen dira, doikuntza-egoera dutenak **Egoki ezina**.</p><p>Kontratu-arauak berriro ebaluatu ondoren, kostu erreal berriak sortzen dira.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul><p>Aurrekontua irabazten denean eta kontratua sortzen denean berrebaluatutako inpaktu finantzariorako sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
