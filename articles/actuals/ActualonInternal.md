---
title: Barneko proiektu baten benetako datuen eragina
description: Artikulu honek barne-proiektu baten gertakari ezberdinetan Errealak taulan duen eraginari buruzko informazioa eskaintzen du Microsoft Dynamics 365 Project Operations.
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
# <a name="actuals-impact-for-an-internal-project"></a>Barneko proiektu baten benetako datuen eragina

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Ondorengo taulak barruko proiektuaren konpromisoan hainbat gertaeratan sortzen diren transakzio mota desberdinen benetakoak zerrendatzen ditu.

| Gertaera | Benetako kostua | Adibidez |
|---|---|---|
| Denbora sortu da. | Ez da aplikagarria | <p>Bob Kozack, Fabrikam AEBetako antolakuntza-unitatekoa, 100 dolar (100 USD) orduko kostu-tasa duena, "Arm Installation at Adatum" izeneko proiektuan ari da lanean. Proiektu hau prezio finkoko fakturazio-metodo batera dago mapatuta kontratuaren lerroan. Hona hemen Bob Kozak-en denboraren lagin bat:</p><p>Bob Kozack - 8 ordu</p> |
| Bidali da denbora. | Ez da aplikagarria | Kostuen egunkari-lerro bat sartzen da denbora sarrerarako. Lehenetsitako kostu-tasa aldizkariko sarreran sartzen dira. |
| Denbora-sarrera gogoratzen da onartu baino lehen. | Ez da aplikagarria | |
| Onartu da ordua. | Benetako kostu bat sortzen da. | <p>Erreal berria sortutakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Denbora onarpena bertan behera utzi da. | <p>Kostuen jatorrizko salmenten benetako doikuntza-egoera eguneratzen da **Egokitua** modura.</p><p>Salmenten kostuen erreal itzulketa bat sortzen da, doikuntza-egoera duena **Ezin da egokitu**.</p> | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *doituta*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 ordu), (USD 800), *ezin da doitu*</li></ul> |
| Denbora-sarrera gogoratzen da onartu ondoren. | <p>Kostuen jatorrizko salmenten benetako doikuntza-egoera eguneratzen da **Egokitua** modura.</p><p>Salmenten kostuen erreal itzulketa bat sortzen da, doikuntza-egoera duena **Ezin da egokitu**.</p> | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *doituta*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 ordu), (USD 800), *ezin da doitu*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
