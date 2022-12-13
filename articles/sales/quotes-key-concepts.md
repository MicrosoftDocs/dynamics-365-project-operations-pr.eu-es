---
title: Proiektuetan oinarritutako eskaintzen kontzeptu bakarrak
description: Artikulu honek Microsoft-en proiektuen aurrekontuei buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 12/02/2022
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 89867cfbe92f47d58b16da40b62d3d9dd6a15b64
ms.sourcegitcommit: e0cbbe7c6f03d4978134405cf04bd8bc1d019f65
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/05/2022
ms.locfileid: "9824312"
---
# <a name="concepts-unique-to-project-based-quotes"></a>Proiektuetan oinarritutako eskaintzen kontzeptu bakarrak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Microsoft Dynamics 365 Project Operations-n proiektuaren aurrekontuak erabiltzen hasi baino lehen, ondoko kontzeptu gakoez jabetu beharko zenituzke.

## <a name="owning-company"></a>Jabetzadun enpresa

Enpresa jabeak proiektuaren entregaren jabe den pertsona juridikoa ordezkatzen du. Aurrekontuko bezeroak entitate juridiko horretan baliozko bezero bat izan behar du finantza eta eragiketa aplikazioetan. Enpresa jabearen moneta eta proiektuetan oinarritutako aurrekontuan hautatutako kontratazio-unitatearen moneta bat etorri behar dira.

## <a name="contracting-unit"></a>Kontratazio-unitatea

Kontratazio-unitateak proiektuaren entregaren jabe den dibisioa edo praktika adierazten du. Kontratazio unitate bakoitzerako baliabide kostuak konfigura ditzakezu. Kontratazio-unitate bateko baliabide baterako baliabide-kostuak zehazten dituzunean, kostu-tasa desberdinak konfigura ditzakezu kontratazio-unitateak maileguan hartzen dituen baliabideetarako, edo enpresaren beste dibisio edo praktika batzuetarako. Kostu-tasa horiei transferentzia-prezioak, baliabideen mailegua edo truke-prezioak esaten zaie. Beste dibisio batzuetako baliabideak hartzeko kostua konfiguratzen duzunean, kostu-tasak mailegu-dibisioaren monetan konfigura ditzakezu.

## <a name="cost-currency"></a>Kostua dibisa

Proiektuaren Eragiketetako kostu-moneta kostuen berri ematen den moneta da. Moneta hau aurrekontuaren, kontratuaren eta proiektuaren **Kontratazio-unitatea** eremuari atxikitako monetatik eratorria da. Proiektu baten kostuak edozein monetan erregistratu daitezke. Hala ere, kostuak erregistratu ziren monetatik proiektuaren kostuen moneta bihurtzea dago.

 Dataverse plataformako truke-tasak ezin direnez data-eraginkorra izan, baliteke pantailako kostuaren guztizkoak denboran zehar aldatzea moneta-tasak eguneratzen badituzu. Hala ere, datu-basean erregistratzen diren kostuak ez dira aldatu, zenbatekoak sortu ziren monetan gordetzen direlako.

## <a name="sales-currency"></a>Salmenten moneta

Project Operations-en salmenta-moneta zenbatetsitako eta benetako salmenta-kopuruak erregistratu eta erakusten diren dibisa da. Era berean, bezeroari akordiorako fakturatzen zaion moneta da. Proiektuko aurrekontu baterako, salmenta-moneta lehenetsi bat ezartzen da bezeroaren edo kontuaren erregistrotik, eta aurrekontua sortzen denean alda daiteke. Hala ere, salmenta-moneta ezin da aldatu aurrekontua gorde ondoren. Produktu eta proiektuen prezioen zerrenda lehenetsiak aurrekontuaren salmenta-monetan oinarrituta ezartzen dira.

Kostuak ez bezala, salmenten balioak **soilik** salmentetako monetan erregistra daitezke.

## <a name="billing-method"></a>Fakturazio-metodoa

Proiektuek normalean kuota finkoko eta kontsumoan oinarritutako kontratazio ereduak dituzte. Proiektuaren Eragiketetan, proiektu baten kontratazio-eredua fakturazio-metodoaren bidez adierazten da. Fakturazio metodoak bi balio ditu: denbora eta materiala eta prezio finkoa.

- **Denbora eta materiala** – Kontsumoan oinarritutako kontratazio-eredua, non sortzen den kostu bakoitza dagokion diru-sarrerak babesten dituen. Kostu gehiago kalkulatzen edo sortzen dituzunean, dagokien salmenta estimatuak eta errealak ere handitu dira. Fakturazio metodo hau duten aurrekontu lerroen mugak ez gainditzeko zehaztu dezakezu. Horrela, benetako diru-sarrerak muga ditzakezu. Aurreikusitako diru-sarrerak ez du gainditzeko mugak eragiten.
- **Prezio finkoa** – Kuota finkoko kontratazio eredua, non salmenta-balioak sortzen diren kostuetatik independenteak diren. Salmenten balioa finkoa da eta ez da aldatzen kostu gehiago kalkulatu edo sortzen dituzunean.

## <a name="project-price-lists"></a>Proiektuaren prezio-zerrendak

Proiektuen prezio-zerrendak prezio lehenetsiak sartzeko erabiltzen diren prezio-zerrendak dira, ez kostu-tasak, denbora, gastu eta proiektuarekin lotutako beste osagai batzuetarako. Hainbat prezio zerrenda egon daitezke, eta zerrenda bakoitzak bere data eraginkortasuna izan dezake proiektuaren aurrekontu bakoitzerako. Project Operations-ek ez du onartzen proiektuaren prezio-zerrendetan data-eraginkortasuna gainjartzea.

## <a name="product-price-lists"></a>Produktuaren prezio-zerrendak

Produktuen prezioen zerrendak prezio lehenetsiak sartzeko erabiltzen diren prezio zerrendak dira, ez kostu-tasak, produktuetan oinarritutako lerroetarako aurrekontu batean. Produktuen prezioen zerrenda bakarra dago aurrekontu bakoitzeko.

## <a name="transaction-classes"></a>Transakzio-klaseak

Project Operations-ek lau transakzio klase mota onartzen ditu:

- Ordua
- Gastua
- Materiala
- Prezioa

Kostuen eta salmenten balioak **Denboran**, **Gastuak** eta **tan izan daitezke. Material** transakzio-klaseak. **Tasa** diru-sarrerak soilik jasotzen dituen transakzio klasea da.

## <a name="work-entities-and-billing-entities"></a>Lan entitateak eta fakturazio entitateak

Proiektuak eta Zereginak lana ordezkatzen duten entitateak dira. Aurrekontu lerroak eta Kontratu lerroak fakturazioa adierazten duten entitateak dira. Lan-entitate desberdinak fakturazio-aukerekin lotu ditzakezu aurrekontu-lerroekin edo Kontratu-lerroekin lotuz.

## <a name="multi-customer-deals"></a>Bezero anitzeko eskaintzak

Bezero anitzeko akordioak faktura bakoitzeko bezero bat baino gehiago daudenean gertatzen dira. Hona hemen adibide tipiko batzuk:

- **Jatorrizko ekipamenduen fabrikatzaileen (OEM) enpresek eta haien bazkideek** – Bazkideek eta saltzaileek balio erantsiko zerbitzuak biltzen dituen produktua saltzen dute. Bezero batekin akordio batean, OEMak normalean proiektuaren zati bat finantzatzea eskaintzen du.
- **Sektore publikoko proiektuak** – Tokiko gobernu bateko hainbat sailek proiektu bat finantzatzea adosten dute eta aurrez adostutako zatiketaren arabera fakturatzen dira. Adibidez, eskola-barruti batek eta udalak edo tokiko gobernu sailak igerileku baten eraikuntza finantzatzea adosten dute.

## <a name="invoice-schedules"></a>Fakturazio-antolaketak

Fakturen ordutegiak aurrekontu-lerro bakoitzeko espezifikoak dira eta aukerakoak dira. Fakturen programazioak hasiera eta amaiera data zehatzetan eta fakturaren maiztasunean oinarrituta sortzen dira. Kontratuaren fasean erabiltzen dira, fakturak sortzeko prozesu automatikoa konfiguratzen denean. Aurrekontu fasean, fakturen ordutegiak aukerakoak dira. Aurrekontu fasean sortzen badira, proiektuaren aurrekontua irabazten denean sortzen den proiektu-kontratuan kopiatzen dira.

## <a name="differences-from-dynamics-365-sales-quotes"></a>Dynamics 365 Sales aurrekontuekiko desberdintasunak

Project Operations aurrekontuak Dynamics 365 Sales aurrekontuetan eraikitzen dira. Hala ere, funtzionaltasunean desberdintasun garrantzitsu batzuk jakin behar dituzu:

- Project Operations aurrekontuek bi lerro mota dituzte: bata proiektuetarako eta bestea produktuetarako.
- Project Operations-ek bere orrialde eta erabiltzaile-interfazearen (UI) elementuak, negozio-arauak, negozio-logika plug-inetan eta bezeroen alboko script-ak dituzte, Salmenten aurrekontuetatik bereizten direnak.
- Salmentetan, hainbat eskaera erantsi ditzakezu salmenta-aurrekontu bakar bati. Proiektu-eragiketetan, proiektu-kontratu bakarra erantsi diezaiokezu proiektuaren aurrekontuari.
- Salmenta aurrekontua irabazten duzunean, erlazionatutako aukera zabalik egon daiteke. Proiektu-eskaintza irabazi ondoren, erlazionatutako abagunea itxita dago.
- Salmenta aurrekontu batek ez ditu proiektuaren aurrekontuak barne hartzen dituen eremu eta kontzeptu batzuk barne hartzen. Eremuek **Kontratazio-unitatea**, **Kontuen kudeatzailea**, eta **Harreman-izenaren faktura** dituzte.
- Salmenta aurrekontuak eta proiektuen aurrekontuak aukera multzo-en oinarritutako **Mota** eremuaren bidez identifikatzen dira. Salmenta aurrekontu baterako, eremu honen balioa **Elementuetan oinarritutakoa da**. Proiektuaren aurrekonturako, balioa **Lanean oinarritutakoa da**.

Desberdintasun hauek direla eta, ez dugu gomendatzen Salmenta-aurrekontuak eta Proiektu-eragiketen aurrekontuak elkarren artean erabiltzea.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
