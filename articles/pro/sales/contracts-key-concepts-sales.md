---
title: Proiektu-kontratuak - Kontzeptu nagusiak - arina
description: Gai honek proiektuaren kontratuaren kontzeptu nagusiei buruzko informazioa ematen du.
author: rumant
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a797a4fef6276f6ed008b0e58eed4c7480ba3492bcc166a362d4ff2816acf777
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6991426"
---
# <a name="concepts-unique-to-project-contracts"></a>Proiektuko kontratuen kontzeptu bakarrak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Gai honek Project kontratuak erabiltzen hasi aurretik ezagutu beharreko kontzeptu nagusiak eskaintzen ditu Dynamics 365 Project Operations:

## <a name="contracting-unit"></a>Kontratatzailea

Kontratazio unitateak proiektua entregatzeko jabea den zatiketa edo praktika adierazten du. Kontratazio unitate bakoitzerako baliabide kostuak konfigura ditzakezu. Baliabide baten baliabideen kostua zehazten duzunean, baliabideen kostu tasa desberdinak ere ezar ditzakezu. Kontratazio unitate honek baliabide horiek enpresako beste dibisio edo praktika batzuetatik hartzen ditu. Baliabideen kostu-tarifak transferentzia prezioak, baliabideen zorpetzea edo truke prezioak dira. Beste dibisio batzuetako baliabideak mailegatzearen kostua konfiguratzen duzunean, mailegu-dibisioaren moneta erabil dezakezu.

## <a name="cost-currency"></a>Kostu-dibisa

Eragiketen kostuen moneta kostuak pantailan jakinarazi diren moneta da. Moneta hau eranskinari erantsitako monetatik eratorria da **Kontratazio unitatea** kontratuan eta proiektuaren eremuan. Kostuak edozein monetan erregistratu daitezke proiektu batekin. Hala ere, moneta-kostuak erregistratu ziren proiektuaren kostu-monetara bihurtzeko aukera dago, pantailan erakustean.

Common Data Service (CDS) plataformako truke-tasak ezin baitira data eraginkorrak izan, kostuaren guztizko pantailak aldatu egin daitezke denborarekin moneta-truke tasak eguneratzen badituzu. Hala ere, datu-basean erregistratutako kostuak ez dira aldatu, zenbatekoak jasan zituzten monetan gordetzen direlako.

## <a name="sales-currency"></a>Salmenten moneta

Salmenten moneta Project Operations-en salmenten zenbateko estimatuak eta benetakoak erregistratu eta erakusten diren moneta da. Bezeroari fakturatuko zaion moneta ere bada salmenten dibisa. Proiektuaren kontratuan, bezeroaren edo kontuaren erregistroaren salmenten moneta lehenetsita dago eta kontratua sortzen denean alda daitezke. Aurrekontua irabazitako moduan itxiz kontratua sortzen denean, kontratuko moneta aurrekontuaren monetan lehenetsita dago.

Proiektu kontratua hutsetik sortzen duzunean, **Salmenten moneta** eremua ezin da editatu. Produktuen eta proiektuen prezioen zerrenden balio lehenetsia kontratuko monetan oinarrituta.

Kostuak ez bezala, salmenten balioak salmenten monetan soilik erregistratu daitezke.

## <a name="billing-method"></a>Fakturazio-metodoa

Proiektuen kontratu-ereduen bi mota dira, kuota finkoak eta kontsumoan oinarritutakoa. Eredu horiek Project Operations-en bi balio posible dituzten fakturazio metodo gisa irudikatzen dira:

- Denbora eta materiala: Kontsumoan oinarritutako kontratu-eredua da, non sortutako kostu bakoitzari dagozkion diru-sarreren bermea dagoen. Kostu gehiago kalkulatzen edo sortzen dituzunean, dagokien salmenta estimatuak eta errealak ere handitu dira. Zehaztu fakturazio-metodo hori duten fakturazio-metodo hori duten diru-sarrerak gainditzen dituzten kontratu-lerroen mugak ez gainditzeko. Aurreikusitako diru-sarrerek ez dituzte mugak gainditu beharrik eragiten.
- Prezio finkoa: Kuota finkoen kontratuaren eredua da, salmenten balioak sortutako kostuetatik independenteak izango direla adierazten duena. Salmenten balioa finkoa da eta ez da aldatzen kostu gehiago kalkulatu edo sortzen dituzunean.

## <a name="project-price-lists"></a>Proiektuaren prezio-zerrendak

Proiektuen prezioen zerrendak prezio lehenetsietarako erabiltzen dira, ez kostuen tasak, denbora, gastua eta proiektuarekin lotutako beste osagai batzuetarako. Hainbat prezio zerrenda egon daitezke. Prezio zerrenda bakoitzak proiektuaren kontratu bakoitzerako data eraginkortasuna du. Proiektuaren prezio-zerrendetako data-eraginkortasuna gainjartzea ez da onartzen Project Operations-en.

Proiektuaren kontratua proiektuaren aurrekontua irabazita sortzen denean, proiektuaren prezioen zerrendak kontratuaren izenarekin eta datarekin kopiatzen dira. Informazio hau kopiatzeak proiektu kontratu honetako proiektuen osagaien prezio pertsonalizatua suposatzen du.

## <a name="product-price-lists"></a>Produktuaren prezio-zerrendak

Produktuen prezioen zerrendak prezio lehenetsietarako erabiltzen dira, ez kostuen tasak, kontratuko produktuetan oinarritutako lerroetarako. Kontratu bakoitzeko produktuen prezioen zerrenda bakarra dago.

## <a name="transaction-classes"></a>Transakzio-klaseak

Project Operations-ek lau transakzio klase mota onartzen ditu:

- Ordua
- Gastua
- Materiala
- Prezioa

Kostuen eta salmenten balioak Denbora, Gastu eta Material transakzio klaseetan kalkula eta sor daitezke. Kuota diru-sarrerak soilik transakzio klasea da.

## <a name="work-entities-and-billing-entities"></a>Lan entitateak eta fakturazio entitateak

Lana irudikatzen duten entitateak proiektuak eta zereginak dira. Fakturazio-aspektuak adierazten dituzten entitateak kontratuaren lerroak dira. Laneko entitate desberdinak fakturazio aukerekin lotu ditzakezu kontratuaren lerroekin lotuz.

## <a name="multi-customer-deals"></a>Bezero anitzeko eskaintzak

Bezero anitzeko akordioak fakturatzeko bezero bat baino gehiago dauzkate. Adibide arruntak hauek dira:

- OEM enpresak eta haien bazkideak: bazkideek eta saltzaileek produktu bat balio erantsiko zerbitzu batzuekin saltzen dute, normalean bezeroarekin tratu jakin bat izanez. OEM-ek proiektuaren zati bat finantzatzea eskaintzen du. 

- Sektore publikoko proiektuak: Tokiko gobernu bateko sail anitzek proiektu bat finantzatzea onartzen dute eta aurrez adostutako zatiketaren arabera fakturatzen dira. Adibidez, eskola-barruti batek eta tokiko gobernu sailak igerileku baten eraikuntza finantzatzea adosten dute.

## <a name="invoice-schedules"></a>Fakturazio-antolaketak

Fakturen ordutegiak kontratu lerro bakoitzari dagozkio eta fakturazio automatikoa funtzionatzeko beharrezkoak dira. Fakturen ordutegiak hasiera eta amaiera data jakin batzuen eta fakturazio maiztasunaren arabera sortzen dira. Ordutegiak kontratuaren fasean erabiltzen dira fakturak automatikoki sortzeko prozesua konfiguratzen denean. Aurrekontu batetik proiektuaren kontratua sortzen denean, fakturaren egutegia aurrekontutik proiektuaren kontratura kopiatzen da.

## <a name="changes-from-the-dynamics-365-sales-contract"></a>Dynamics 365 Sales kontratuaren aldaketak

Project Operations-en kontratuak Dynamics 365 Sales-en kontraktuen gainean eraikitzen dira. Hala ere, funtzionaltasunean desbideratze eta desberdintasun garrantzitsu batzuk jakin behar dituzu:

- Project Operations-en kontratuek bi linea mota desberdin dituzte, bata proiektuetarako eta bestea produktuetarako.
- Project Operations-en kontratuek beren forma eta interfazeko elementu propioak dituzte, negozio arauak, negozio logika plug-inetan eta bezeroen aldeko scriptak, Salmenten kontratuetatik bakarrak bihurtzen dituztenak.

Arrazoi horiek direla eta, ez zenuke salmenta kontratua eta proiektu kontratua erabili beharrik izango.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
