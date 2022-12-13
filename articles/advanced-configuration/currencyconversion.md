---
title: Konfiguratu moneta bihurketa kostu-tasetatik salmenten prezioak kalkulatzeko
description: Artikulu honek Microsoft Dynamics 365 Project Operations n erabiliko den moneta bihurtzeko portaera nola konfiguratu azaltzen du kostu-transakzioetatik salmenten transakzioak sortzen direnean.
author: rumant
ms.date: 11/01/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 3fa8077deb18f1a54e7f0f5e6dc4491a830df45b
ms.sourcegitcommit: 95e52fcf012a51229f3f6ae7dbf7b0fa56072a85
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/01/2022
ms.locfileid: "9816684"
---
# <a name="set-up-currency-conversion-to-calculate-sales-prices-from-cost-rates"></a>Konfiguratu moneta bihurketa kostu-tasetatik salmenten prezioak kalkulatzeko

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Microsoft Dynamics 365 Project Operations n, gastu-kategorien salmenta-prezioak zenbakizko balio gisa ezar daitezke, edo sortutako kostuaren arabera kalkulatu ahal izateko.

Sortutako kostuaren arabera kalkulatzeko konfiguratuta daudenean, aukera hauek daude eskuragarri:

- Kostuan
- Markatu kostuaren gaineko ehunekoa

Gastuaren kostua proiektuaren kontratuaren salmenta-monetatik desberdina den moneta batean sortzen den agertokietan, moneta-bihurketa beharrezkoa da salmenta-prezioa kostuaren arabera kalkulatzeko.

## <a name="currency-conversion-behavior-that-uses-native-dataverse-exchange-rates"></a>Bertako Dataverse truke-tasak erabiltzen dituen moneta bihurtzeko portaera

Modu lehenetsian, Project Operations-ek Moneta taulan gordeta dauden moneta-truke-tasak erabiltzen ditu Dataverse. Proiektu-eragiketak konfiguratzeko berezko truke-tasak erabiltzeko kostuaren arabera salmenta-prezioak kalkulatzeko, jarraitu urrats hauek.

1. Joan **Proiektuaren Eragiketak \> Ezarpenak \> Parametroak**.
1. Ireki **Proiektuaren parametroa** xehetasun orria.
1. Ezarri  **Moneta bihurtzeko logika** eremua balio huts batean.

## <a name="currency-conversion-behavior-that-uses-exchange-rates-from-finance-and-operations-apps"></a>Finantza- eta operazio-aplikazioetako truke-tasak erabiltzen dituen moneta bihurtzeko portaera

 Dataverse n berez eskuragarri dauden Moneta taulako truke-tasak ez dira datan indarrean. Hori dela eta, baliteke beti ez eskalatzea kostu-tasetatik salmenta-prezioak kalkulatzeko dituzun eskakizunetara.

Finantza eta eragiketen inguruneko truke-tasak erabil ditzakezu salmenta-dibisan salmenta-prezioa kalkulatzeko kostu-dibisako kostu-tasa batetik. Moneta bihurtzeko portaera hau konfiguratzeko, jarraitu urrats hauek.

1.  **Proiektuaren parametroak** orrian, gehitu **Moneta bihurtzeko logika** eremua. Ondoren, gorde eta argitaratu pertsonalizazioa.
1. Joan **Proiektuaren Eragiketak \> Ezarpenak \> Parametroak**.
1. Ireki **Proiektuaren parametroa** xehetasun orria. 
1. Ezarri **Dibisa bihurtzeko portaera** eremua **Lehenetsitako atzerapenarekin hedatua**.
1. Eman **Idazketa bikoitzeko aplikazioaren erabiltzaileari** segurtasun-funtzio **Irakurketa globala** baimena taula hauei:

    - msdyn\_ moneta-trukeak
    - msdyn\_ currencyexchangeratepairs
    - msdyn\_ truke motak

1. Zure finantza eta eragiketen ingurunean, exekutatu idazketa bikoitzeko mapa hauek hasierako sinkronizazioarekin:

    - Truke-tasa mota (msdyn\_ truke-tipoak)
    - Truke-tasaren moneta bikotea (msdyn\_ currencyexchangeratepairs)
    - CDS truke-tasak (msdyn\_ moneta-trukeak)

Aldaketa hauek osatu ondoren, idazketa bikoitzak finantza eta eragiketen inguruneko truke-tasak eskuragarri jarriko ditu Dataverse n. Ondoren, Project Operations-ek truke-tasa horiek erabiliko ditu kostu-tasak kontratuaren salmenta-moneta bihurtzeko.

> [!NOTE]
> Moneta bihurtzeko portaera hau kostu-tasetatik salmenten prezioak kalkulatzeko soilik aplikatzen da. Ez da erabiliko oinarrizko moneta-balioak modu orokorrean kalkulatzeko. Oinarrizko moneta balioek jatorrizko Dataverse truke-tasa erabiliko dituzte beti, prozedura hau betetzen duzun ala ez.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
