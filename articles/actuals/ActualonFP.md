---
title: Benetako datuen eragina prezio finkoko elkarrekintza batean
description: Artikulu honek prezio finkoaren parte-hartzearen bizitza-zikloko hainbat gertakaritan Errealak taulan duen eraginari buruzko informazioa eskaintzen du Microsoft Dynamics 365 Project Operations-en.
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
ms.openlocfilehash: 50819d77d56935bfe5438d7d9dae99562bcc0b49
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8918113"
---
# <a name="actuals-impact-in-a-fixed-price-engagement"></a>Benetako datuen eragina prezio finkoko elkarrekintza batean

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Ondorengo taulak prezio finkoaren konpromisoan hainbat gertaeratan sortzen diren transakzio mota desberdinen benetakoak zerrendatzen ditu.

| Gertaera | Benetako kostua | Fakturatu gabeko benetako salmentak | Fakturatutako benetako salmentak | Adibidez |
|---|---|---|---|---|
| Denbora sortu da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | <p>Bob Kozack, Fabrikam AEBetako antolakuntza-unitatekoa, 100 dolar (100 USD) orduko kostu-tasa duena, "Arm Installation at Adatum" izeneko proiektuan ari da lanean. Proiektu hau prezio finkoko fakturazio-metodo batera dago mapatuta kontratuaren lerroan. Hona hemen Bob Kozak-en denboraren lagin bat:</p><p>Bob Kozack - 8 ordu</p> |
| Bidali da denbora. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | Kostuen egunkari-lerro bat sartzen da denbora sarrerarako. Lehenetsitako kostu-tasa aldizkariko sarreran sartzen dira. |
| Denbora-sarrera gogoratzen da onartu baino lehen. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | |
| Onartu da ordua. | Benetako kostu bat sortzen da. | Ez da aplikagarria | Ez da aplikagarria | <p>Erreal berria sortutakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Denbora onarpena bertan behera utzi da. | <p>Kostuen jatorrizko salmenten benetako doikuntza-egoera eguneratzen da **Egokitua** modura.</p><p>Salmenten kostuen erreal itzulketa bat sortzen da, doikuntza-egoera duena **Ezin da egokitu**.</p> | Ez da aplikagarria | Ez da aplikagarria | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *doituta*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 ordu), (USD 800), *ezin da doitu*</li></ul> |
| Denbora-sarrera gogoratzen da onartu ondoren. | <p>Kostuen jatorrizko salmenten benetako doikuntza-egoera eguneratzen da **Egokitua** modura.</p><p>Salmenten kostuen erreal itzulketa bat sortzen da, doikuntza-egoera duena **Ezin da egokitu**.</p> | Ez da aplikagarria | Ez da aplikagarria | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *doituta*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 ordu), (USD 800), *ezin da doitu*</li></ul> |
| Kontratu berretsi da. | <p>Kostu erreal zaharren doikuntza-egoera eguneratzen da hona: **Doituta**.</p><p>Salmenten kostuen erreal itzulketa bat sortzen da, doikuntza-egoera duena **Ezin da egokitu**.</p><p>Kostu-arauak berriro ebaluatu ondoren, kostu erreal berriak sortzen dira.</p> | Ez da aplikagarria | Ez da aplikagarria | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *doituta*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 ordu), (USD 800), *ezin da doitu*</li></ul><p>Berriro ebaluatutako finantza-eraginerako sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Faktura bat sortzen da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | |
| Faktura mugarri batekin berresten da. | Ez da aplikagarria | Ez da aplikagarria | Mugarrietan oinarritutako fakturatutako salmenta erreal berriak sortzen dira. | <p>Aldaketarik gabe geratzen den lehendik dagoen erreala:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul><p>Fakturatutako salmenten balioak erregistratzeko sortzen den erreal berria:</p><ul><li>**Fakturatutako salmenten benetako:** Mugarria, USD 5.000</li></ul> |
| Faktura zuzentzen da mugarria kreditatzeko. | Ez da aplikagarria | Ez da aplikagarria | Fakturatutako alderantzikatze-salmenta errealak sortzen dira. | <p>Aldaketarik gabe geratzen den lehendik dagoen erreala:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul><p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Fakturatutako salmenten benetako:** Mugarria, USD 5.000, *doituta*</li></ul><p>Aurrez fakturatutako salmenten balioak alderantzikatzeko sortzen den erreal berria:</p><ul><li>**Fakturatutako salmenten benetako:** Mugarria, USD 5.000,*ezin doitu*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
