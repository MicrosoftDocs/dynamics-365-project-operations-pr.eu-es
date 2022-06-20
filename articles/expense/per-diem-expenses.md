---
title: Eguneko dietaren gastuak
description: Artikulu honek eguneko gastuekin lan egiteko informazioa ematen du.
author: suvaidya
ms.date: 03/18/2022
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.search.region: ''
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 0d2f95b677720726049d7d010e9738ad8c513802
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923173"
---
# <a name="per-diem-expenses"></a>Eguneko dietaren gastuak

> [!IMPORTANT] 
> Artikulu honetan deskribatzen den funtzionaltasuna aurrebista-argitalpen baten barruan dago erabilgarri zuzendutako erabiltzaileentzat.

Eguneko ordainketa enpresa batek bere langileei ordaintzen dien eguneko diru-laguntza finko bat da, ostatua (hotelak), otorduak eta langile horiek lanera bidaiatzen duten bitartean egiten dituzten gorabehera-gastuengatik. Enpresak hobari hori langileei ordaintzen die benetako bidaia-gastuak ordaindu beharrean. Langileek beren erabil dezakete **Gorabeherak/Besteak** eguneko diru-laguntza, negozio bilera garrantzitsuetarako aholkuak, gela-zerbitzua, arropa garbiketa edo lehorreko garbiketa zerbitzuak estaltzeko. Eguneko tasa alda daiteke, enplegatzaileak ostatuaren eta otorduen kostu konbinatua itzultzea edo otorduen eta gorabeheraren kostua soilik itzultzea aukeratzen duenaren arabera.

Eguneko tasak urteko garaian, bidaiaren kokapenean edo bietan oinarrituta egon daitezke. Eguneko arau bat sortzen duzunean, eguneko tasaren ehuneko bat atxikiko dela zehaztu dezakezu langile batek otorduak edo zerbitzuak osagarriak jasotzen baditu. Halaber, eguneko tasa langile baten bidaietan aplika daitekeen gutxieneko ordu-kopurua eta gehienezko ordu-kopurua ezar ditzakezu.

Egunekoa, langileari ematen zaion otorduen murrizketa (otordu osagarrien kostua) egunean eskaintzen den guztizko diru-laguntza gisa kalkulatzen da.

## <a name="configure-per-diems"></a>Konfiguratu dietak

Eguneko gastuak konfiguratzeko, jarraitu urrats hauek.

1. Joan **Gastuen kudeaketa** \> **Konfigurazioa** \> **Orokorra** \> **Gastuak kudeatzeko parametroak**.
2. Gainean **Egunekoa** fitxan, **Kalkulatu otorduen murrizketa arabera** eremuan, hautatu dietak nola kalkulatu behar diren:

    - **Otordu mota bidaia bakoitzeko** – Kalkulatu dieta sartzen den otordu motaren arabera (gosaria, bazkaria edo afaria) eta bidaiak irauten duen otordu-mota bakoitzerako zehazten den otordu-murrizketaren arabera.
    - **Bazkari mota eguneko** – Kalkulatu dieta, sartzen den otordu-motaren eta otordu-mota bakoitzerako zehazten den otordu-murrizketaren arabera, eguneko diru-laguntzaren arabera.
    - **Eguneko otordu kopurua** – Kalkulatu dieta egunean sartzen den otordu kopuruaren eta egun bakoitzean ematen diren otordu kopuruaren otordu-murrizketaren arabera.

3. Joan **Gastuen kudeaketa** \> **Konfigurazioa** \> **Kalkuluak eta kodeak** \> **Eguneko kokapenak**.
4. Gehitu dietak erabil daitezkeen kokapenak.
5. Gehitzen duzun kokapen bakoitzeko, atalean **Egunkariak** fitxan, hautatu ostatu, otordu eta bestelako gastuetarako hasiera eta amaiera data zehatzen artean balio duten eguneko tasa eta moneta. Eguneko tasak eta monetak konfiguratzeko, joan hona **Gastuen kudeaketa** \> **Konfigurazioa** \> **Kalkuluak eta kodeak** \> **Egunkariak**.

## <a name="per-diems-in-the-reimagined-expense-interface"></a>Eguneko gastu-interfazea berriro irudikatuta

Eguneko funtzioa berraztertutakoan onartzen da **Gastuen Kudeaketa** lantokian Microsoft Dynamics 365 Finance 10.0.25 bertsioa eta berriagoa.

Egunkariak gaitzeko, jarraitu urrats hauek.

1. urtean **Ezaugarrien kudeaketa** lan-eremua, bilatu eta hautatu **Gastuen txostenak berriro irudikatuta** zerrendako eginbidea, eta, ondoren, hautatu **Gaitu orain**.
2. Bilatu eta hautatu **Gastu-txostenaren eguneroko interfazea berriro irudikatuta** zerrendako eginbidea, eta, ondoren, hautatu **Gaitu orain**.

## <a name="how-the-feature-works"></a>Ezaugarriak nola funtzionatzen duen

Atal honek hiru konfigurazio agertokiren adibideak eskaintzen ditu. Adibide bakoitzeko, **Kalkulatu otorduen murrizketa arabera** eremua beste balio batean ezarrita dago. Hiru adibideetarako, ordaindu beharreko zenbateko osoa berdina da otorduen murrizketa aplikatu arte. Une horretatik aurrera, ordaindu beharreko zenbateko osoa desberdina da adibide bakoitzeko.

Hiru adibideetarako erabiltzen den eguneko gastua sortzeko, jarraitu urrats hauek.

1. Joan **Lan-eremuak** \> **Gastuen Kudeaketa**.
2. Hautatu **Gastuen txosten berria**, edo hautatu lehendik dagoen gastu-txosten bat.
3. Gehitu gastu berri bat. urtean **Kategoria** eremua, hautatu **Egunekoa**. Hautatu kokapena eta bidaiaren hasiera eta amaiera datak. Ostatua, otorduak eta gorabeherak (beste gastu batzuk) hautatutako tokirako ezartzen den eguneko diru-laguntzaren arabera kalkulatzen da.

    Adibidez, zuk hautatzen duzu **Redmond (AEB)** kokapena gisa. Kokapen horretarako eguneko diru-laguntza 150 dolar (150 USD) da ostaturako, USD 75 otorduetarako eta USD 5 gorabeherak egiteko. Hasiera-data urtarrilaren 10a da, eta amaiera-data urtarrilaren 14a. Hori dela eta, hautatutako iraupena bost egunekoa da, hautatutako konfigurazioa egun naturalak denborarekin daudenean, eta hautatutako ordua goizeko 12:00etan hasi eta amaitzen da hasiera eta amaiera egunetan. Hona hemen kalkuluak:

    - Ordaindu beharreko kopuru osoa = 5 × (150 + 75 + 5) = 5 × 230 = USD 1,150
    - Otordua eta kopuru osoaren zati bat = 5 × (75 + 5) = USD 400

Bidaian zehar gosaria, bazkaria eta afaria eman baziren, otordu horiek otorduen murrizketa gisa kontabilizatu beharko dira.

### <a name="example-1-per-diem-where-meal-reductions-are-based-on-meal-type-per-trip"></a>1. adibidea: eguneko otorduen murrizketak bidaia bakoitzeko otordu motaren araberakoak diren

Adibide honetan, otorduen murrizketa ehuneko 30ekoa da gosaltzeko, ehuneko 30eko bazkarirako eta ehuneko 40eko afarirako. Gainean **Gastuak kudeatzeko parametroak** orrialdea, du **Kalkulatu otorduen murrizketa arabera** eremuan ezarrita dago **Otordu mota bidaia bakoitzeko**. Hona hemen langileari hiru gosari, bi bazkari eta zero afari emango balitu kalkuluak:

- Otorduen murrizketa = (3 ×\[ % 75 × 30\]) + (2 ×\[ % 75 × 30\]) + 0 = (3 × 22,50) + (2 × 22,50) + 0 = 67,50 + 45 + 0 = USD 112.50
- Otorduak eta gorabeherak = 400 – 112,50 = USD 287.50
- Ordaindu beharreko zenbateko osoa = Hobari osoa – Bazkariaren murrizketa = 1.150 – 112,50 = USD 1,037.50

![Eguneko gastua, non otorduen murrizketa bidaia bakoitzeko otordu motaren araberakoa den.](media/1-meal-type-per-trip.png)

### <a name="example-2-per-diem-where-meal-reductions-are-based-on-meal-type-per-day"></a>2. adibidea: eguneko otorduen murrizketak eguneko otordu motaren araberakoak diren

Adibide honetan, otorduen murrizketa ehuneko 30ekoa da gosaltzeko, ehuneko 30eko bazkarirako eta ehuneko 40eko afarirako. Gainean **Gastuak kudeatzeko parametroak** orrialdea, du **Kalkulatu otorduen murrizketa arabera** eremuan ezarrita dago **Bazkari mota eguneko**. Kasu honetan, urtean **Otorduak** sarean **Editatu gastua** elkarrizketa-koadroa, kontrol-laukiak garbitzen dituzu bidaian zehar zein otordu eman zizkizun adierazteko.

Esaterako, hona hemen bidaiaren lehen hiru egunetan gosaria eman bazen kalkuluak:

- Lehen hiru egunetako eguneko otorduen murrizketa = 75 × % 30 = USD 22.50
- Otorduen murrizketa totala = 3 × 22,50 = USD 67.50
- 1etik 3ra bitarteko egunetarako otorduak eta gorabeherak = 75 – 22.50 = USD 57.50
- Otorduak eta gorabeherak guztira = bost egunetan zehar otorduen eta gorabeheraren batura = 400 – 67,50 = USD 332.50
- Ordaindu beharreko zenbateko osoa = Zenbateko osoa – Bazkariaren murrizketa = 1.150 – 67,50 = USD 1,082.50

![Eguneko gastua, non otorduen murrizketa eguneko otordu motaren araberakoa den.](media/2-meal-type-per-day.png)

### <a name="example-3-per-diem-where-meal-reductions-are-based-on-number-of-meals-per-day"></a>3. adibidea: eguneko otorduen murrizketak eguneko otordu kopuruan oinarritzen diren

Adibide honetan, otorduen murrizketa egunean emandako otordu kopuruaren arabera kalkulatzen da (hau da, **Kalkulatu otorduen murrizketa arabera** eremuan **Gastuak kudeatzeko parametroak** orrialdea ezarrita dago **Eguneko otordu kopurua**). urtean **Otorduak** sarean **Editatu gastua** elkarrizketa-koadroan, kontrol-laukiak garbitzen dituzu zein otordu eman diren adierazteko.
Kasu honetan, otorduen murrizketa emandako otordu kopuruan bakarrik oinarritzen da, eta ez emandako otordu motan (Gosaria/bazkaria/afaria).

Hona hemen eguneko diru-laguntzaren kalkuluak ostaturako USD 150, otorduetarako USD 75 eta USD 5 gorabeherak direnean:

- **Ordaindu beharreko zenbateko osoa** = 5 × (150 + 75 + 5) = 5 × 230 = USD 1,150
- **Bazkari bat:** Otorduen murrizketa = % 20 = USD 15
- **Bi otordu:** Otorduen murrizketa = % 50 = USD 37.50
- **Hiru otordu:** Otorduen murrizketa = % 100 = USD 75

Hona hemen kalkuluak **otorduak eta gorabeherak**, USD 5 barne hartzen dituen gorabeherak egiteko:

- 1. eguna - Bi otordu eman = (75 – 37,50) + 5 = 37,50 + 5 = USD 42.50
- 2. eguna - Bi otordu eskaintzen dira = (75 – 37,50) + 5 = 37,50 + 5 = USD 42.50
- 3. eguna - Otordu bat ematen da = (75 – 15) + 5 = 60 + 5 = USD 65
- 4. eguna - Zero otorduak ematen = (75-0) + 5 = 75 + 5 = USD 80
- 5. eguna - Hiru otordu ematen dira = (75 – 75) + 5 = 0 + 5 = USD 5

- Guztira otorduak eta gorabeherak = 1. eguneko otorduak eta gorabeherak + 2. eguna + 3. eguna + 4. eguna + 5. eguna = USD 235
- Otorduen murrizketa totala = 1. eguneko otorduen murrizketa
- Ordaindu beharreko zenbateko osoa = Hobari osoa – Otorduen murrizketa osoa = USD 1,150 - USD 165 = USD 985

![Eguneko gastua, otorduen murrizketa eguneko otordu kopuruan oinarritzen den.](media/3-number-of-meals-per-day.png)

> [!NOTE]
> Finantza 10.0.23 bertsiotik aurrera, berriro irudikaturiko gastuen interfazea erabiltzen baduzu, ezin dituzu sortu datak gainjarri dituzten eguneko gastuak. Saiatzen bazara, errore-mezu bat jasoko duzu.
