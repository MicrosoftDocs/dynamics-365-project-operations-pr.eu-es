---
title: Eguneko dietaren gastuak
description: Artikulu honek eguneko dietekin lana egiteko moduari buruzko informazioa ematen du.
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
> Artikulu honetan zehaztutako funtzionaltasuna helburuko erabiltzaile guztientzat erabilgarri dago aurreargitalpen-bertsioaren zati gisa.

Eguneko dieten ordainketa finkoa da, enpresa batek bere langileei ostatua (hotelak), otorduak eta langile horiek lanera bidaiatzen duten bitartean sortzen dituzten gastu osagarriak ordaintzen dizkie. Enpresak hobari hori langileei ordaintzen die benetako bidaia-gastuak ordaindu beharrean. Langileek beren erabil dezakete **Gorabeherak/Besteak** eguneko dietak, negozio-bilera garrantzitsuetarako aholkuak, gela-zerbitzua, arropa garbiketa edo lehor-garbiketa zerbitzuak estaltzeko. Eguneko dieta alda daiteke, enplegatzaileak ostatuaren eta otorduen kostu bateratua itzultzea edo otorduen eta gorabeheraren kostua soilik itzultzea aukeratzen duenaren arabera.

Eguneko tasak urteko garaian, bidaiaren kokapenean edo bietan oinarrituta egon daitezke. Eguneko araua sortzen duzunean, eguneko tasaren ehuneko bat gordeko dela zehaztu dezakezu langileak osagarriak diren otorduak edo zerbitzuak jasotzen baditu. Halaber, eguneko tasak langilearen bidaiari aplikatu ahal izateko gutxieneko eta gehieneko ordu kopurua ere ezar dezakezu.

Eguneko dieta langileari ematen zaion otorduen murrizketa (otordu osagarrien kostua) egunean eskaintzen den guztizko diru-laguntza gisa kalkulatzen da.

## <a name="configure-per-diems"></a>Konfiguratu eguneko dietak

Eguneko dieten gastuak konfiguratzeko, jarraitu urrats hauek.

1. Joan **Gastuen kudeaketa** \> **Konfigurazioa** \> **Orokorra** \> **Gastuak kudeatzeko parametroak**.
2. **Eguneko dietak** fitxan, **Kalkulatu otorduen murrizketa arabera** eremuan, hautatu dietak nola kalkulatu behar diren:

    - **Otordu mota bidaia bakoitzeko** – Kalkulatu eguneko dietan sartzen den otordu motaren arabera (gosaria, bazkaria edo afaria) eta bidaiak irauten duen bitartean otordu mota bakoitzerako zehazten den otordu-murrizketaren arabera.
    - **Otordu mota egun bakoitzeko** – Kalkulatu eguneko dietan sartzen den otordu motaren arabera eta otordu mota bakoitzerako zehazten den otordu-murrizketaren arabera.
    - **Eguneko otordu kopurua** – Kalkulatu dieta egunean sartzen diren otordu kopuruaren eta egun bakoitzean ematen diren otordu kopuruaren otordu-murrizketaren arabera.

3. Joan **Gastuen kudeaketa** \> **Konfigurazioa** \> **Kalkuluak eta kodeak** \> **Eguneko dieten kokapenak**.
4. Gehitu dietak erabil daitezkeen kokapenak.
5. Gehitutako kokapen bakoitzerako, **eguneko dietak** fitxan, hautatu hasiera- eta amaiera-daten artean baliozkoak diren eguneko dieten tasa eta moneta hotelerako, otorduetarako eta bestelako gastuetarako. Eguneko dieten tasak eta monetak konfiguratzeko, joan **Gastuen kudeaketa** \> **Konfigurazioa** \> **Kalkuluak eta kodeak** \> **Eguneko dietak**.

## <a name="per-diems-in-the-reimagined-expense-interface"></a>Eguneko dietak berregituratutako gastuen interfazean

Eguneko dieten funtzioa berregituratutako **Gastuen Kudeaketa** laneko arean Microsoft Dynamics 365 Finance-ren 10.0.25 bertsioa eta berriagoan onartzen da.

Egunek dietak gaitzeko, jarraitu urrats hauei.

1. **Ezaugarrien kudeaketa** lan-eremua, bilatu eta hautatu **Gastuen txostenak berriro irudikatuta** zerrendako eginbidea, eta, ondoren, hautatu **Gaitu orain**.
2. Bilatu eta aurkitu **Eguneko dietak gastuen txostenetarako interfaze berregituratua** eginbidea zerrendan eta hautatu **Gaitu orain**.

## <a name="how-the-feature-works"></a>Nola funtzionatzen du eginbideak

Atal honek hiru konfigurazio agertokiren adibideak eskaintzen ditu. Adibide bakoitzeko, **Kalkulatu otorduen murrizketaren arabera** eremua beste balio batean ezarrita dago. Hiru adibideetarako, ordaindu beharreko zenbateko osoa berdina da otorduen murrizketa aplikatu arte. Une horretatik aurrera, ordaindu beharreko zenbateko osoa desberdina da adibide bakoitzeko.

Hiru adibideetarako erabiltzen den eguneko gastua sortzeko, jarraitu urrats hauek.

1. Joan **Laneko areak** \> **Gastuen kudeaketa** atalera.
2. Aukeratu **Gastuen txosten berria** edo hautatu dagoen gastuen txostena.
3. Gehitu gastuen aurreikuspen berria. **Kategoria** eremuan, hautatu **Eguneko dieta**. Hautatu kokapena eta bidaiaren hasiera eta amaiera datak. Ostatua, otorduak eta gorabeherak (beste gastu batzuk) hautatutako tokirako ezartzen den eguneko dietaren diru-laguntzaren arabera kalkulatzen da.

    Adibidez, zuk hautatzen duzu **Redmond (AEB)** kokapena gisa. Kokapen horretarako eguneko diru-laguntza 150 dolar (150 USD) da ostaturako, USD 75 otorduetarako eta USD 5 gorabeherak egiteko. Hasiera-data urtarrilaren 10a da, eta amaiera-data urtarrilaren 14a. Hori dela eta, aukeratutako iraupena bost egunekoa da, hautatutako konfigurazioa egun naturalak denborarekin daudenean, eta hautatutako ordua goizeko 12:00etan hasi eta amaitzen da hasiera eta amaiera egunetan. Hona hemen kalkuluak:

    - Ordaindu beharreko kopuru osoa = 5 × (150 + 75 + 5) = 5 × 230 = USD 1.150
    - Otordua eta kopuru osoaren zati bat = 5 × (75 + 5) = USD 400

Bidaian zehar gosaria, bazkaria eta afaria eman baziren, otordu horiek otorduen murrizketa gisa kontabilizatu beharko dira.

### <a name="example-1-per-diem-where-meal-reductions-are-based-on-meal-type-per-trip"></a>1. adibidea: eguneko dietak, non otorduen murrizketak bidaia bakoitzeko otordu motaren araberakoak diren

Adibide honetan, otorduen murrizketa ehuneko 30ekoa da gosaltzeko, ehuneko 30eko bazkarirako eta ehuneko 40ko afarirako. **Gastuak kudeatzeko parametroak** orrialdea, **Kalkulatu otorduen murrizketaren arabera** eremuan ezarrita dago **Otordu mota bidaia bakoitzeko**. Hona hemen langileari hiru gosari, bi bazkari eta zero afari emango balitu kalkuluak:

- Otorduen murrizketa = (3 × \[75 × 30%\]) + (2 × \[75 × 30%\]) + 0 = (3 × 22.50) + (2 × 22.50) + 0 = 67.50 + 45 + 0 = USD 112,50
- Otorduak eta gorabeherak = 400 – 112,50 = USD 287,50
- Ordaindu beharreko zenbateko osoa = Hobari osoa – Bazkariaren murrizketa = 1.150 – 112,50 = USD 1.037,50

![Eguneko dieten gastua, non otorduen murrizketa bidaia bakoitzeko otordu motaren araberakoa den.](media/1-meal-type-per-trip.png)

### <a name="example-2-per-diem-where-meal-reductions-are-based-on-meal-type-per-day"></a>2. adibidea: eguneko dietak, non otorduen murrizketak egun bakoitzeko otordu motaren araberakoak diren

Adibide honetan, otorduen murrizketa ehuneko 30ekoa da gosaltzeko, ehuneko 30eko bazkarirako eta ehuneko 40ko afarirako. **Gastuak kudeatzeko parametroak** orrialdea, **Kalkulatu otorduen murrizketaren arabera** eremuan ezarrita dago **Otordu mota egun bakoitzeko**. Kasu honetan, **Otorduak** saretan **Editatu gastua** elkarrizketa-koadroan, kontrol-laukiak garbitzen dituzu bidaian zehar zein otordu eman zizkizun adierazteko.

Adibidez, hona hemen bidaiaren lehen hiru egunetan gosaria eman bazen kalkuluak:

- Lehen hiru egunetako eguneko otorduen murrizketa = 75 × % 30 = USD 22,50
- Otorduen murrizketa totala = 3 × 22,50 = USD 67,50
- 1etik 3 egunera bitarteko otorduak eta gorabeherak = 75 – 22,50 = USD 57,50
- Otorduak eta gorabeherak guztira = bost egunetan zehar otorduen eta gorabeheraren batura = 400 – 67,50 = USD 332,50
- Ordaindu beharreko zenbateko osoa = Kopuru osoa – Bazkariaren murrizketa = 1.150 – 67,50 = USD 1.082,50

![Eguneko dieten gastua, non otorduen murrizketa egun bakoitzeko otordu motaren araberakoa den.](media/2-meal-type-per-day.png)

### <a name="example-3-per-diem-where-meal-reductions-are-based-on-number-of-meals-per-day"></a>3. adibidea: eguneko dietak, non otorduen murrizketak egun bakoitzeko otordu kopuruaren araberakoak diren

Adibide honetan, otorduen murrizketa egunean emandako otordu kopuruaren arabera kalkulatzen da (hau da, **Kalkulatu otorduen murrizketa honen arabera** eremuan **Gastuak kudeatzeko parametroak** orrialdea ezarrita dago **Eguneko otordu kopurua**). **Otorduak** saretan **Editatu gastua** elkarrizketa-koadroan, kontrol-laukiak garbitzen dituzu eman zizkizun adierazteko.
Kasu honetan, # otorduen murrizketa emandako otordu kopuruan soilik oinarritzen da, eta ez emandako otordu motan (Gosaria/bazkaria/afaria).

Hona hemen eguneko diru-laguntzaren kalkuluak ostaturako USD 150, otorduetarako USD 75 eta USD 5 gorabeherak direnean:

- **Ordaindu beharreko kopuru osoa** = 5 × (150 + 75 + 5) = 5 × 230 = USD 1.150
- **Otordu bat:** Otorduen murrizketa = % 20 = USD 15
- **Bi otordu:** Otorduen murrizketa = % 50 = USD 37.50
- **Hiru otordu:** Otorduen murrizketa = % 100 = USD 75

Hona hemen **otorduak eta gorabeheren**, USD 5 barne hartzen dituen gorabeherak egiteko:

- 1. eguna - Bi otordu eman dira = (75 – 37,50) + 5 = 37,50 + 5 = USD 42,50
- 2. eguna - Bi otordu eman dira = (75 – 37,50) + 5 = 37,50 + 5 = USD 42,50
- 3. eguna - Otordu bat ematen da = (75 – 15) + 5 = 60 + 5 = USD 65
- 4. eguna - Zero otordu eman dira = (75 – 0) + 5 = 75 + 5 = USD 80
- 5. eguna - Hiru otordu eman dira = (75 – 75) + 5 = 0 + 5 = USD 5

- Otorduak eta gorabeherak guztira = 1. eguneko otorduak eta gorabeherak + 2. eguna + 3. eguna + 4. eguna + 5. eguna = USD 235
- Otorduen murrizketa totala = 1. eguna, 2. eguna + 3. eguna + 4. eguna + 5. eguneko otorduen murrizketak= 37,5+ 37,5+ 15 + 0+ 75 = USD 165
- Ordaindu beharreko zenbateko osoa = Hobari osoa – Otorduen murrizketa, guztira = USD 1.150 – USD 165 = USD 985

![Eguneko dieten gastua, non otorduen murrizketa egun bakoitzeko otordu kopuruaren araberakoa den.](media/3-number-of-meals-per-day.png)

> [!NOTE]
> Finance-ren 10.0.23 bertsiotik aurrera, berriro imajinatutako gastuen interfazea erabiltzen baduzu, ezin dituzu sortu datak gainjarri dituzten eguneko gastuak. Hori egiten saiatzen bazara, errore-mezu bat jasoko duzu.
