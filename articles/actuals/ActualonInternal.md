---
title: Barne proiektu baten benetako eragina
description: Artikulu honek Microsoft-en barne-proiektu baten gertakari ezberdinetan Errealak taulan duen eraginari buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
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
ms.openlocfilehash: de05714c079fe121ef68e28b1acb82c24bce095e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921333"
---
# <a name="actuals-impact-for-an-internal-project"></a>Barne proiektu baten benetako eragina

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Hurrengo taulak barne proiektuko konpromiso batean gertaera ezberdinetan sortzen diren transakzio mota ezberdinen benetakoak zerrendatzen ditu.

| Gertaera | Benetako kostua | Adibidez |
|---|---|---|
| Denbora sortzen da. | Ez da aplikagarria | <p>Bob Kozack, orduko 100 dolar (100 USD) kostu-tasa duen Fabrikam AEBko antolakuntza-unitatekoa, "Arm Installation at Adatum" izeneko proiektuan ari da lanean. Proiektu hau kontratu-lerroan prezio finkoko fakturazio-metodo batera lotzen da. Hona hemen Bob Kozak-en denboraren lagin bat:</p><p>Bob Kozack - 8 ordu</p> |
| Denbora aurkeztu da. | Ez da aplikagarria | Kostuen egunkari-lerro bat sortzen da denbora-sarrerarako. Kostu-tasa lehenetsia aldizkariko sarreran sartzen da. |
| Denbora-sarrera gogoratzen da onartu baino lehen. | Ez da aplikagarria | |
| Ordua onartu da. | Benetako kostu bat sortzen da. | <p>Sortzen den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Denbora onarpena bertan behera geratzen da. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |
| Ordu-sarrera gogoratzen da onartu ondoren. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
