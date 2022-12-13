---
title: Proiektuko eskaintzen kontzeptu bakarrak
description: Gai honek Project Operations-eko proiektu-eskaintzak erabiltzeari buruzko informazioa ematen du.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 7f0a33f1d7d77f3b5aebfdcf8e6aeb14072cd596
ms.sourcegitcommit: e0cbbe7c6f03d4978134405cf04bd8bc1d019f65
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/05/2022
ms.locfileid: "9825878"
---
# <a name="concepts-unique-to-project-quotes"></a>Proiektuko eskaintzen kontzeptu bakarrak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_


Dynamics 365 Project Operations-en proiektu-eskaintzak erabiltzen hasi baino lehen kontuan hartu behar dira kontzeptu-gako hauek:

## <a name="contracting-unit"></a>Kontratazio-unitatea

Kontratazio unitateak proiektua entregatzeko jabea den zatiketa edo praktika adierazten du. Kontratazio unitate bakoitzerako baliabide kostuak konfigura ditzakezu. Kontratazio unitatean baliabide baten baliabideen kostua zehazten duzunean, kostu tasa desberdinak ezarri ahal izango dituzu kontratazio unitate honek maileguan hartzen dituen baliabideetarako edo enpresako beste zatiketa edo praktiketarako. Hauek transferentzia prezioak, baliabideen zorpetzea edo truke prezioak dira. Beste dibisio batzuetako baliabideak mailegatzearen kostua konfiguratzen duzunean, kostu-tasa horiek mailegu-dibisioaren monetan konfiguratzea ere aukera dezakezu.

## <a name="cost-currency"></a>Kostua dibisa

Project Operations-en eragiketen kostuen moneta kostuak jakinarazi diren moneta da. Moneta hau eranskinari erantsitako monetatik eratorria da **Kontratazio unitatea** aurrekontua, kontratua eta proiektuaren eremua. Kostuak edozein monetan erregistratu daitezke proiektu batekin. Hala ere, moneta-kostuak erregistratu ziren proiektuaren kostu-monetara bihurtzeko aukera dago.

CDS plataformako truke-tasak ezin baitira data eraginkorrak izan, kostuaren guztizko pantailak aldatu egin daitezke denborarekin moneta-truke tasak eguneratzen badituzu. Hala ere, datu-basean erregistratutako kostuak ez dira aldatu, zenbatekoak jasan zituzten monetan gordetzen direlako.

## <a name="sales-currency"></a>Salmenten moneta

Salmenten moneta Project Operations-en salmenten zenbateko estimatuak eta benetakoak erregistratu eta erakusten diren moneta da. Bezeroari fakturatuko zaion moneta ere tratua. Proiektuaren aurrekontuan, bezeroaren edo kontuaren erregistroaren salmenten moneta lehenetsita dago eta aurrekontua sortzen denean alda daitezke. Aurrekontua gorde ondoren, salmenten moneta ezin da aldatu. Produktuen eta proiektuen prezioen zerrenden balio lehenetsia eskaintzaren salmenta-monetan oinarrituta.

Kostuak ez bezala, salmenten balioak salmenten monetan soilik erregistratu daitezke.

## <a name="billing-method"></a>Fakturazio-metodoa

Proiektuek normalean kuota finkoak eta kontsumoan oinarritutako kontratazio ereduak dituzte. Project Operations-en adierazten da **Fakturazio metodoa** eta bi balio ditu, denbora eta materiala eta prezio finkoa.

- **Denbora eta materiala:** Kontsumoan oinarritutako kontratu-eredua da, non sortutako kostu bakoitzari dagozkion diru-sarreren bermea dagoen. Kostu gehiago kalkulatzen edo sortzen dituzunean, dagokien salmenta estimatuak eta errealak ere handitu egingo dira. Fakturazio metodo hau duten aurrekontu lerroen mugak ez gainditzeko zehaztu dezakezu. Horrek benetako diru sarrerak mugatuko ditu. Aurreikusitako diru-sarrerek ez dituzte mugak gainditu beharrik eragiten.
- **Prezio finkoa:** Kuota finkoen kontratuaren eredua da, salmenten balioak sortutako kostuetatik independenteak izango direla adierazten duena. Salmenten balioa finkoa da eta ez da aldatzen kostu gehiago kalkulatu edo sortzen dituzunean.

## <a name="project-price-lists"></a>Proiektuaren prezio-zerrendak

Proiektuen prezioen zerrendak prezio lehenetsietarako erabiltzen diren prezioen zerrendak dira, ez kostuen tasak, denbora, gastua eta proiektuarekin lotutako beste osagai batzuetarako. Hainbat prezio zerrenda egon daitezke, eta zerrenda bakoitzak bere data eraginkortasuna izan dezake proiektuaren aurrekontu bakoitzerako. Proiektuaren prezio-zerrendetako data-eraginkortasuna gainjartzea ez da onartzen Project Operations-en.

## <a name="product-price-lists"></a>Produktuaren prezio-zerrendak

Produktuen prezioen zerrendak prezio lehenetsietarako erabiltzen diren prezioen zerrendak dira, ez kostuen tasak, aurrekontu bateko produktuetan oinarritutako lerroetarako. Aurrekontu bakoitzeko produktuen prezioen zerrenda bakarra dago.

## <a name="transaction-classes"></a>Transakzio-klaseak

Project Operations-ek lau transakzio klase mota onartzen ditu:

- Ordua
- Gastua
- Materiala
- Prezioa

Kostuen eta salmenten balioak Denbora, Gastu eta Material transakzio klaseetan kalkula eta sor daitezke. Kuota diru-sarrerak soilik transakzio klasea da.

## <a name="work-entities-and-billing-entities"></a>Lan entitateak eta fakturazio entitateak

Lana irudikatzen duten entitateak Proiektuak eta Zereginak dira. Fakturazioa adierazten duten entitateak Aurrekontu lerroak eta Kontratu lerroak dira. Laneko entitate desberdinak fakturazio aukerekin lotu ditzakezu Aurrekontuaren edo Kontratuaren lerroekin lotuz.

## <a name="multi-customer-deals"></a>Bezero anitzeko eskaintzak

Bezero anitzeko akordioak fakturatzeko bezero bat baino gehiago daudenean gertatzen dira. Honelako adibideek hauek dituzte barne:

- **OEM enpresak eta haien bazkideak:** Bazkideek eta saltzaileek produktu bat balio erantsiko zerbitzuekin saltzen dute. Normalean, bezero batekin tratu jakin batean OEMak proiektuaren zati bat finantzatzea eskaintzen duen agertokia da. 

- **Sektore publikoko proiektuak:** Tokiko gobernu bateko sail anitzek proiektu bat finantzatzea onartzen dute eta aurrez adostutako zatiketaren arabera fakturatzen dira. Adibidez, eskola-barruti batek eta udalak edo tokiko gobernu sailak igerileku baten eraikuntza finantzatzea adosten dute.

## <a name="invoice-schedules"></a>Fakturazio-antolaketak

Fakturen ordutegiak aurrekontu lerro bakoitzari dagozkio eta aukerakoak dira. Fakturen ordutegiak hasiera eta amaiera data jakin batzuen eta fakturazio maiztasunaren arabera sortzen dira. Fakturen ordutegiak kontratuaren fasean erabiltzen dira fakturak automatikoki sortzeko prozesua konfiguratzen denean. Aurrekontuaren fasean, ordutegiak aukerakoak dira. Fitxategien fakturak programan sortzen direnean **Aurrekontua** etapa, proiektuaren aurrekontua irabazten denean sortzen den proiektuaren kontratuan kopiatzen dira.

## <a name="changes-from-dynamics-365-sales-quote"></a>Dynamics 365 Sales-en aurrekontuaren aldaketak:

Project Operations-en aurrekontuak Dynamics 365 Sales-en aurrekontuen gainean eraikitzen dira. Hala ere, funtzionaltasunean desberdintasun garrantzitsu batzuk jakin behar dituzu:


- Project Operations-en aurrekontuek bi lerro mota dituzte. Bat proiektuetarako da eta bestea produktuetarako.
- Project Operations-en aurrekontuek beren forma eta interfazeko elementu propioak dituzte, negozio arauak, negozio logika plug-inetan eta bezeroen aldeko scriptak, Salmenten aurrekontuetatik bakarrak bihurtzen dituztenak.
- Salmenta aurrekontuei esker, hainbat eskaera eransteko aukera ematen dizu salmenta aurrekontu bati. Proiektu Eragiketetan, proiektu-kontratu bakarra erantsi ahal izango zaio proiektuaren aurrekontuari.
- Salmenta aurrekontua irabazten duzunean, erlazionatutako aukera zabalik egon daiteke. Proiektu-eskaintza irabazi ondoren, erlazionatutako abagunea itxita dago.
- Salmenta aurrekontuak ez ditu proiektuaren aurrekontuan sartzen diren eremu eta kontzeptu batzuk barne hartzen. Eremuek **Kontratazio-unitatea**, **Kontuen kudeatzailea**, eta **Harreman-izenaren faktura** dituzte.  
- **Mota**: Salmenta-eskaintzak eta proiektu-eskaintzak multzoan oinarritutako eremua moduan, **Mota**, ere identifikatzen dira. Salmenta-eskaintzak lortzeko, eremuak balio hau du: **Elementuan oinarritutakoa**. Proiektu-eskaintza lortzeko, balio hau du: **Lanean oinarritutakoa**.

Arrazoi hauengatik, ez da gomendagarria Salmenten aurrekontua eta Project Operations-en aurrekontua modu aldakorrean erabiltzea.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
