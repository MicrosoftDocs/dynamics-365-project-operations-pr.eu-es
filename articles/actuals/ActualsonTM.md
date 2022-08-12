---
title: Benetako eragina denboran eta materialen konpromisoan
description: Artikulu honek Microsoft-en denbora eta materialen engaiamenduaren bizitza-zikloko hainbat gertakaritan Errealak taulan duen eraginari buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
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
ms.openlocfilehash: 039700e61796bf77c7661e5269b6923101139a1e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923311"
---
# <a name="actuals-impact-in-a-time-and-materials-engagement"></a>Benetako eragina denboran eta materialen konpromisoan

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Ondorengo taulak denbora eta materialen konpromisoan hainbat ekitalditan sortzen diren transakzio mota desberdinen benetakoak zerrendatzen ditu.

| Gertaera | Benetako kostua | Fakturatu gabeko benetako salmentak | Fakturatutako salmentak benetakoak | Adibidez |
|---|---|---|---|---|
| Denbora sortzen da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | <p>Bob Kozack, orduko 100 dolar (100 USD) kostu-tasa duen Fabrikam AEBko antolakuntza-unitatekoa, "Arm Installation at Adatum" izeneko proiektuan ari da lanean. Proiektu honetarako, kontratatutako fakturaren tarifa orduko USD 200 da. Hona hemen Bob Kozak-en denboraren lagin bat:</p><p>Bob Kozack, 8 ordu</p> |
| Denbora aurkeztu da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | Kostuen egunkari-lerroa eta Fakturatu gabeko salmenta-aldizkariak sortzen dira denbora-sarrerarako. Lehenetsitako prezioa eta kostu-tasa aldizkariko sarreran sartzen dira. |
| Denbora-sarrera gogoratzen da onartu baino lehen. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | |
| Ordua onartzen da: aurkeztutako orduak faktura daitezkeen orduak dira. | Benetako kostu bat sortzen da. | Fakturatu gabeko salmenta erreal bat sortzen da. | Ez da aplikagarria | <p>Sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600</li></ul> |
| Denbora onartu da: faktura daitezkeen orduak aurkeztutako orduen azpitik murrizten dira. | Benetako kostu bat sortzen da. | <p>Fakturatu gabeko bi salmenta erreal sortzen dira:</p><ul><li>Fakturatu gabeko salmenta kobragarriak faktura daitezkeen orduetarako</li><li>Kobratu gabeko fakturatu gabeko salmentak gainontzeko kantitateari dagokionez</li></ul> | Ez da aplikagarria | <p>Sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 6 ordu, USD 1,200, *Kobragarria*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 2 ordu, USD 400, *Kobratu gabea*</li></ul> |
| Denbora onartu da: faktura daitezkeen orduak bidalitako orduen gainetik igotzen dira. | Benetako kostu bat sortzen da. | Fakturatu gabeko salmenta erreal bat sortzen da. | Ez da aplikagarria | <p>Sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 10 ordu, USD 2,000</li></ul> |
| Denbora onarpena bertan behera utzi da. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Fakturatu gabeko jatorrizko salmentaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Fakturatu gabeko salmenten erreal itzulketa bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | Ez da aplikagarria | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Egokitua*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 ordu), (1.600 USD), *Egoki ezina*</li></ul> |
| Ordu-sarrera gogoratzen da onartu ondoren. | <p>Jatorrizko kostu errealaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu erreal bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | <p>Fakturatu gabeko jatorrizko salmentaren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Fakturatu gabeko salmenten erreal itzulketa bat sortzen da, doikuntza-egoera duena **Egoki ezina**.</p> | Ez da aplikagarria | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Egokitua*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 ordu), (1.600 USD), *Egoki ezina*</li></ul> |
| Kontratua berresten da. | <p>Kostu erreal zaharren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Berraztertzeko kostu errealak sortzen dira, doikuntza-egoera dutenak **Egoki ezina**.</p><p>Kontratu-arauak berriro ebaluatu ondoren, kostu erreal berriak sortzen dira.</p> | <p>Fakturatu gabeko salmenta erreal zaharren doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Fakturatu gabeko salmenten errealak itzultzeko doikuntza-egoera dutenak sortzen dira **Egoki ezina**.</p><p>Fakturatu gabeko salmenta erreal berriak kontratu-arauak berriro ebaluatu ondoren sortzen dira.</p> | Ez da aplikagarria | <p>Eguneratzen diren lehendik dauden datuak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800, *Egokitua*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Egokitua*</li></ul><p>Aurreko finantza-eragina alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, (8 h), (800 USD), *Egoki ezina*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 ordu), (1.600 USD), *Egoki ezina*</li></ul><p>Berriz ebaluatutako finantza-inpaktuagatik sortzen diren erreal berriak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600</li></ul> |
| Faktura bat sortzen da. | Ez da aplikagarria | Ez da aplikagarria | Ez da aplikagarria | |
| Faktura baieztatzen da. Ez dago aldaketarik faktura-lerroaren xehetasunak fakturatu gabeko salmenten kopurutik. | Ez da aplikagarria | <p>Fakturatu gabeko salmenta zaharren benetako fakturaren egoera eguneratzen da.</p><p>Fakturatu gabeko salmenten errealak itzultzeko doikuntza-egoera dutenak sortzen dira **Egoki ezina**. | Fakturatutako salmenta erreal bat sortzen da. | <p>Aldaketarik gabe geratzen den lehendik dagoen erreala:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul><p>Eguneratzen den egungo benetakoa:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Bezeroaren faktura argitaratua*</li></ul>Abian dauden finantza-lanak (WIP) alderantzikatzeko sortzen den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 h), (1.600 USD)</li></ul><p>Fakturatutako salmenten balioak erregistratzeko sortzen den erreal berria:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, 8 ordu, USD 1,600</li></ul> |
| Faktura berresten da faktura-lerroaren xehetasuna fakturatu gabeko salmenten kopurutik txikitu ondoren. | Ez da aplikagarria | <p>Fakturatu gabeko jatorrizko salmenten errealen doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Fakturatu gabeko salmenten errealak itzultzeko fakturatu gabeko salmenten errealetarako sortzen dira. Egokitzapen egoera dute **Egoki ezina**.</p><p>Fakturatu gabeko bi salmenta erreal berri sortzen dira:</p><ul><li>Fakturatu gabeko salmenta kobragarriak faktura daitezkeen orduetarako</li><li>Kobratu gabeko fakturatu gabeko salmentak gainontzeko kantitateari dagokionez</li></ul><p>Fakturatu gabeko salmenten errealak itzultzeko fakturatu gabeko bi salmenta erreal berrietarako sortzen dira.</p> | <p>Fakturatutako bi salmenta erreal sortzen dira:</p><ul><li>Fakturatutako salmenten errealak faktura daitezkeen orduetarako</li><li>Kobratu gabeko fakturatutako salmentak gainontzeko kantitatearen errealak</li></ul> | <p>Aldaketarik gabe geratzen den lehendik dagoen erreala:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul><p>Eguneratzen den egungo benetakoa:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Egokitua*</li></ul><p>Aurreko finantza-WIPa bueltatzeko sortu den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 ordu), (1.600 USD), *Egoki ezina*</li></ul><p>Salmenten WIP eguneratua erregistratzeko sortzen diren erreal berriak:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, 6 ordu, USD 1,200, *Kobragarria*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 2 ordu, USD 400, *Kobratu gabea*</li></ul><p>Salmenten WIP eguneratua alderantzikatzeko sortzen diren erreal berriak:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, (6 ordu), (1.200 USD), *Kobragarria*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, (2 ordu), (400 USD), *Kobratu gabea*</li></ul><p>Fakturatutako salmenten balioak erregistratzeko sortzen diren erreal berriak:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, 6 ordu, USD 1,200, *Kobragarria*</li><li>**Fakturatutako salmenta errealak:** Bob Kozack, 2 ordu, USD 400, *Kobratu gabea*</li></ul> |
| Faktura berresten da faktura-lerroko xehetasuna fakturatu gabeko salmenten kopurutik handitu ondoren. | Ez da aplikagarria | <p>Fakturatu gabeko jatorrizko salmenten errealen doikuntza-egoera eguneratzen da **Egokitua**.</p><p>Fakturatu gabeko salmenten errealak itzultzeko fakturatu gabeko salmenten errealetarako sortzen dira. Egokitzapen egoera dute **Egoki ezina**.</p><p>Fakturatu gabeko salmenta erreal berriak sortzen dira kantitate berrirako.</p><p>Fakturatu gabeko salmenten errealak itzultzeko fakturatu gabeko salmenta erreal berrietarako sortzen dira.</p> | Fakturatutako salmenta errealak kantitate berrirako sortzen dira. | <p>Aldaketarik gabe geratzen den lehendik dagoen erreala:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li></ul><p>Eguneratzen den egungo benetakoa:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Egokitua*</li></ul><p>Aurreko finantza-WIPa bueltatzeko sortu den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 ordu), (1.600 USD), *Egoki ezina*</li></ul><p>Salmenten WIP eguneratua erregistratzeko sortu den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, 10 ordu, USD 2,000, *Kobragarria*</li></ul><p>Salmenten WIP eguneratua aldatzeko sortu den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, (10 ordu), (2.000 USD), *Kobragarria*, *ezina*</li></ul><p>Fakturatutako salmenten balioak erregistratzeko sortzen den erreal berria:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, 10 ordu, USD 2,000, *Kobragarria*</li></ul> |
| Faktura zuzentzen da kargatu beharreko kantitatea edo prezioa murrizteko. | Ez da aplikagarria | <p>Fakturatu gabeko bi salmenta erreal sortzen dira:</p><ul><li>Fakturatu gabeko salmenta kobragarriak faktura zuzentzailean dagoen kantitateagatik</li><li>Fakturatu gabeko salmenta kobragarriak gainontzeko kantitateagatik</li></ul><p>Fakturatu gabeko salmenten errealak itzultzeko fakturatu gabeko bi salmenta erreal berrietarako sortzen dira.</p> | <p>Alderantzikatu fakturatutako salmenta errealak sortzen dira.</p><p>Fakturatutako salmenta erreal berriak sortzen dira kantitate berrirako. | <p>Aldaketarik gabe geratzen diren lehendik dauden benetakoak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Bezeroaren faktura argitaratua*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 h), (1.600 USD)</li></ul><p>Eguneratzen den egungo benetakoa:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, (8 h), (1.600 USD) *Egokitua*</li></ul><p>Aurreko fakturatutako salmenten balioak alderantzikatzeko sortu den erreal berria:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, (8 h), (1.600 USD) *Egoki ezina*</li></ul><p>Salmenten WIP zuzendua erregistratzeko sortzen diren erreal berriak:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, 6 ordu, USD 1,200, *Kobragarria*, *faktura argitaratuta*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 2 ordu, USD 400, *Kobragarria*</li></ul><p>Salmenten WIP zuzendua alderantzikatzeko sortu den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, (6 ordu), (1.200 USD), *Kobragarria*, *ezina*</li></ul><p>Zuzendutako fakturatutako salmenten balioak erregistratzeko sortu den erreal berria:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, 6 ordu, USD 1,200, *Kobragarria*</li></ul> |
| Faktura zuzentzen da ordaindu beharreko kantitatea edo prezioa handitzeko. | Ez da aplikagarria | <p>Fakturatu gabeko salmenta erreal berriak sortzen dira kantitate berrietarako.</p> <p>Fakturatu gabeko salmenten errealak itzultzeko fakturatu gabeko salmenta erreal berrietarako sortzen dira.</p> | <p>Alderantzikatu fakturatutako salmenta errealak sortzen dira.</p>Fakturatutako salmenta erreal berriak sortzen dira kantitate berrirako.</p> | <p>Aldaketarik gabe geratzen diren lehendik dauden benetakoak:</p><ul><li>**Benetako kostua:** Bob Kozack, 8 ordu, USD 800</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, 8 ordu, USD 1,600, *Bezeroaren faktura argitaratua*</li><li>**Fakturatu gabeko salmentak:** Bob Kozack, (8 h), (1.600 USD)</li></ul><p>Eguneratzen den egungo benetakoa:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, (8 h), (1.600 USD) *Egokitua*</li></ul><p>Aurreko fakturatutako salmenten balioak alderantzikatzeko sortu den erreal berria:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, (8 h), (1.600 USD) *Egoki ezina*</li></ul><p>Salmenten WIP zuzendua erregistratzeko sortu den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, 10 ordu, USD 2,000, *Kobragarria*, *faktura argitaratu da*</li></ul><p>Salmenten WIP zuzendua alderantzikatzeko sortu den erreal berria:</p><ul><li>**Fakturatu gabeko salmentak:** Bob Kozack, (10 ordu), (2.000 USD), *Kobragarria*</li></ul><p>Zuzendutako fakturatutako salmenten balioak erregistratzeko sortu den erreal berria:</p><ul><li>**Fakturatutako salmenta errealak:** Bob Kozack, 10 ordu, USD 2,000, *Kobragarria*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]