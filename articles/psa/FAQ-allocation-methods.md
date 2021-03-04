---
title: Erreserbak esleitzeko metodoak Project Service Automation-en
description: Gai honek esleipenak erreserbatzeko modu desberdinei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: e1ceb7ea5484a1d099c4709eda48d34ecd9bac2e
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5151598"
---
# <a name="booking-allocation-methods-in-project-service-automation"></a>Erreserbak esleitzeko metodoak Project Service Automation-en

[!include [banner](../includes/psa-now-project-operations.md)]

Gehitu taldeko kide zuzenean proiektua **Taldea** fitxan, edo antolaketa-panel batetik proiektua edo eskakizun baliabide erreserbatutako, gutxi beste erreserbatu guztirako baldintza kopuruak metodo daude erabil dezakezu. Gai honen arrazoi metodo bakoitzean funtzionamendua eta metodoak zer overbooking baliabideak, sorraraz ditzaketela.

## <a name="full-capacity"></a>Ahalmen osoa 
Gaitasun osoa metodoa aukerarek erreserbatzen du baliabidearen ahalmena osoa. Adibidez, baliabide bat ezarri egunaren lanorduak zortzi egutegi bat badu, bost egun asteko, horri buruzko eremu zehatzera bost lanegunetan hasierako eta amaierako data ezartzen books baliabidea 40 ordu. Ahalmena geratzen diren baliabidearen erreserba egiten da. Baliabide bat dagoeneko badago booked beste projects, tarte hori, 40 ordu da booked ordu gehigarriak, potentzialki arriskutsua gidatzen erreserba gehiegi, gisa.

## <a name="remaining-capacity"></a>Geratzen den ahalmena
Geratzsen den ahalmena metodo hori soilik dago erabilgarri antolaketa-panela erabiliz proiektua zuzenean erreserbatutako duzu. Metodo honek baliabideen erabilgarritasun-gaitasuna erreserbatzen du zehaztutako data-tarte jakin batean. Adibidez, baliabide bat asteko bakoitzeko ordu 40 ahalmena eta dagoeneko booked asteko ordu 10, erreserbatu erabiltzen bera asteko emaitzak-30 orduetan gainerako erreserbatu asteko.

## <a name="percentage-capacity"></a>Ehuneko ahalmena
Ehunekoaren gaitasuna metodoa aukerak erreserbatzen du baliabidearen ahalmenaren ehuneko batean baliabidea zehaztutako daten artean. Adibidez, baliabide bat ezarri egunaren lanorduak zortzi egutegi bat badu, bost egun asteko, horri buruzko eremu zehatzera bost lanegunetan hasierako eta amaierako data ezartzen books baliabidea 20 ordu. Egunaren banakako bookings dira spread tratatzen, denbora-tarte zehar adibidez adibide hau egunaren ordu lau. Ahalmena geratzen diren baliabidearen erreserba egiten da. Baliabide bat dagoeneko badago booked, tarte hori, 20 ordu da booked ordu gehigarriak, potentzialki arriskutsua gidatzen erreserba gehiegi, gisa.

## <a name="evenly-distribute-hours"></a>Banatu orduak modu uniformean
Berdin banatu aukerak epe jakin batean zehaztatutako orduak erreserbatzen ditu, zehaztatutako hasiera- eta amaiera-daten artean berdin banatuz, egunen arabera. Adibidez, baliabide- bost eguneko tarte jakin batean zehar ordu 20 erreserbatutako baduzu metodo hau distributes uniformeki aldi eguneko ordu 20 ordu. Ahalmena geratzen diren baliabidearen erreserba egiten da. Baliabide bat dagoeneko badago booked, tarte hori, 20 ordu da booked ordu gehigarriak, potentzialki arriskutsua gidatzen erreserba gehiegi, gisa.

## <a name="front-load-hours"></a>Ordainketa goiztiarraren orduak
Aurreikusitako orduaren metodoaren arabera ordu jakin baterako erreserbatzen du baliabidea, egunean ordu jakin batzuk zehaztutako datetan. Baliabidearen ahalmena erabilgarri "lehenengo-n-lehenengo-hartzen duten lekua askatu" ordena consumes front-loading. Adibidez, eguneko, asteko, bakoitzeko egun bost 8 zortzi ordu bada baliabideen lan-antolaketa eta bookings uneko ez duten, baliabidea booking bost lanegun tarte jakin batean zehar 20 ordu-ondorio, hurrengo eguneko erreserbatu maiztasuna: 

|         Erreserbak          |    1. eguna    |    2. eguna    |    3. eguna    |    4. eguna    |    5. eguna    |    Totala    |
|---------------------------|-------------|-------------|-------------|-------------|-------------|-------------|
|    Lehendik dauden erreserbak    |    0        |    0        |    0        |    0        |    0        |    0        |
|    Erreserba berria          |    8        |    8        |    4        |    0        |    0        |    20       |

Kargatu front metodoa ez ditu irauten detekzioaren dagoen bookings eta ahalmena erabilgarri. Adibidez, baliabidea bera dagoeneko orduak bookings aplikazioan lan-astearen 20 badu, bookings berria darabil ahalmena gelditzen diren honela:

|   Erreserbak          | 1. eguna | 2. eguna | 3. eguna | 4. eguna | 5. eguna | Totala |
|---------------------|-------|-------|-------|-------|-------|-------|
| Lehendik dauden erreserbak | 8     | 8     | 4     | 0     | 0     | 20    |
| Erreserba berria       | 0     | 0     | 4     | 8     | 8     | 20    |

Erabilgarri dagoen ahalmena hartzen delako jaso dezakezu errore-mezu bat baliabidea erreserbatu, arabera absorbed ahalmena gelditzen diren ez badu. Metodo honekin, ezin da gainerreserbatu.

## <a name="none"></a>Bat ere ez
Metodo hori soilik dago erabilgarri **Taldea** xede proiektuaren barruan fitxa erreserbatutako duzu. Metodo hori baliabidea proiektuan lanean taldearen kide gisa gehitzen, baina ez du sortu edozein bookings absorb baliabidearen ahalmena. Metodo hori lehenetsia proiektua kudeatzailea taldeko kide proiektua bat sortzen denean gehitzen zaionean erabiltzen da. Proiektua kudeatzailea sortu zuen erabiltzailearen proiektuan gehitzen da modu lehenetsian, proiektua proiektua entitate-erregistroaren jabea da eta proiektuan lanean approver bat dago. Erabiltzaile honek ez duelako bookings edozein baliabidea erreserbatutako nahi izanez gero ditzakezu ezabatu eta ondoren berriro gehitu bidez kopuruan beste metodo bat, edo gehitu baliabidea zereginak eta ondoren, **Luzatu erreserbak** **Kontziliazioa fitxan** sortzeko erabili-bookings. esleipenetan.

## <a name="allocation-methods-that-lead-to-overbooking"></a>Bezerogaiaren overbooking guztirako baldintza kopuruak metodoak
Laburtu, ondorengo esleipen metodoak bezerogaia overbooking baliabidea dagoeneko badago balidatu beste projects (edo beste lan-eskaera edo antola daitezkeen entitateak):

- Ahalmen osoa
- Ehuneko ahalmena
- Banatu orduak modu uniformean

Metodoetako horiek hiru guztirako baldintza kopuruak erabiliz gero duzun ez jakinaraztea baliabidea overbooked da. Gehiegizko erreserbak zuzentzeko, antolaketa-panela erabili beharko duzu.
