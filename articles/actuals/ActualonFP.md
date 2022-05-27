---
title: Benetako eragina prezio finko batean
description: Gai honek Microsoft-en prezio finkoko engaiamendu baten bizitza-zikloko hainbat gertakaritan Errealak taulan duen eraginari buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
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
ms.openlocfilehash: 222e7c5eefd7c619e4d7389cdaff2f96176ff275
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8579213"
---
# <a name="actuals-impact-in-a-fixed-price-engagement"></a>Benetako eragina prezio finko batean

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Ondorengo taulak prezio finkoko konpromiso batean gertaera ezberdinetan sortzen diren transakzio mota ezberdinen errealak zerrendatzen ditu.

| Gertaera | Benetako kostua | Fakturatu gabeko benetako salmentak | Fakturatutako salmentak benetakoak | Adibidez |
|---|---|---|---|---|
| Denbora sortzen da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | <p>Bob Kozack, orduko 100 dolar (100 USD) kostu-tasa duen Fabrikam AEBko antolakuntza-unitatekoa, "Arm Installation at Adatum" izeneko proiektuan ari da lanean. Proiektu hau kontratu-lerroan prezio finkoko fakturazio-metodo batera lotzen da. Hona hemen Bob Kozak-en denboraren lagin bat:</p><p>Bob Kozack - 8 ordu</p> |
| Denbora aurkeztu da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | Kostuen egunkari-lerro bat sortzen da denbora-sarrerarako. Kostu-tasa lehenetsia aldizkariko sarreran sartzen da. |
| Denbora-sarrera gogoratzen da onartu baino lehen. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | |
| Ordua onartu da. | Benetako kostu bat sortzen da. | Ez da aplikagarria | Ez da aplikagarria | <p>Sortzen den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Denbora onarpena bertan behera utzi da. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | Ez da aplikagarria | Ez da aplikagarria | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |
| Ordu-sarrera gogoratzen da onartu ondoren. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | Ez da aplikagarria | Ez da aplikagarria | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul> |
| Kontratua berresten da. | <p>Kostu erreal zaharren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu errealak sortzen dira, doikuntza-egoera dutenak **Egoki ezina**.</p><p>Kontratu-arauak berriro ebaluatu ondoren, kostu erreal berriak sortzen dira.</p> | Ez da aplikagarria | Ez da aplikagarria | <p>Eguneratzen den egungo benetakoa:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li></ul><p>Aurreko finantza-eragina atzera botatzeko sortu den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li></ul><p>Berriz ebaluatutako finantza-inpaktuagatik sortzen den erreal berria:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul> |
| Faktura bat sortzen da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | |
| Faktura mugarri batekin berresten da. | Ez da aplikagarria | Ez da aplikagarria | Mugarrietan oinarritutako fakturatutako salmenta erreal berriak sortzen dira. | <p>Aldaketarik gabe geratzen den lehendik dagoen erreala:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul><p>Fakturatutako salmenten balioak erregistratzeko sortzen den erreal berria:</p><ul><li>**Fakturatutako salmentak:** Mugarria, USD 5,000</li></ul> |
| Faktura zuzentzen da mugarria kreditatzeko. | Ez da aplikagarria | Ez da aplikagarria | Alderantzikatu fakturatutako salmenta errealak sortzen dira. | <p>Aldaketarik gabe geratzen den lehendik dagoen erreala:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, 800 USD</li></ul><p>Eguneratzen den egungo benetakoa:</p><ul><li>**Fakturatutako salmenta errealak:** Mugarria, USD 5,000, *Egokitua*</li></ul><p>Aurreko fakturatutako salmenten balioak alderantzikatzeko sortu den erreal berria:</p><ul><li>**Fakturatutako salmentak:** Mugarria, (5.000 USD), *Egoki ezina*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
