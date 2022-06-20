---
title: Benetako eragina konpromiso baten aurresalmenta-aldian
description: Artikulu honetan, egungo taulak hainbat ekitalditan izango duen eraginari buruzko informazioa ematen da, Microsoften aurresalmenta-garaian konpromiso bat dagoen bitartean Dynamics 365 Project Operations.
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
ms.openlocfilehash: d03d6ac2154806189d0d9d0b232bb317f51071ba
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922345"
---
# <a name="actuals-impact-during-the-pre-sales-stage-of-an-engagement"></a>Benetako eragina konpromiso baten aurresalmenta-aldian

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Hurrengo taulan, proiektu-konpromiso baten aurresalmenta-aldian hainbat ekitalditan sortzen diren transakzio moten benetako datuak zerrendatzen dira.

| Gertaera | Benetako kostua | Adibidez |
|---|---|---|
| Denbora sortzen da. | Ez da aplikagarria | <p>Bob Kozack, orduko 100 dolar (100 USD) kostu-tasa duen Fabrikam AEBko antolakuntza-unitatekoa, "Arm Installation at Adatum" izeneko proiektuan ari da lanean. Proiektu hau kontratu-lerroan prezio finkoko fakturazio-metodo batera lotzen da. Hona hemen Bob Kozak-en denboraren lagin bat:</p><p>Bob Kozack - 8 ordu</p> |
| Denbora aurkeztu da. | Ez da aplikagarria | Kostuen egunkari-lerro bat sortzen da denbora-sarrerarako. Kostu-tasa lehenetsia aldizkariko sarreran sartzen da. |
| Denbora-sarrera gogoratzen da onartu baino lehen. | Ez da aplikagarria | |
| Ordua onartu da. | Benetako kostu bat sortzen da. | <p>Sortzen den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Denbora onarpena bertan behera utzi da. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |
| Ordu-sarrera gogoratzen da onartu ondoren. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |
| Kotizazioa irabazten da eta kontratu bat sortzen da. | <p>Kostu erreal zaharren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu errealak sortzen dira, doikuntza-egoera dutenak **Egoki ezina**.</p><p>Kontratu-arauak berriro ebaluatu ondoren, kostu erreal berriak sortzen dira.</p> | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul><p>Kotizazioa irabazten denean eta kontratua sortzen denean, finantza-inpaktu berrirabatzeko sortzen diren datu erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
