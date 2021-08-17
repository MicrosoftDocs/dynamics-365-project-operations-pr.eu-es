---
title: Produktuetan oinarritutako kontratuaren lerroen ikuspegi orokorra - arina
description: Gai honek kontratu eta produktuetan oinarritutako lerroei buruzko informazioa ematen du.
author: rumant
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 79b4f6355afb7472f843eda06bf33a3fe732274d6f2566bd23000aa11cbfdce1
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007536"
---
# <a name="product-based-contract-lines-overview---lite"></a>Produktuetan oinarritutako kontratuaren lerroen ikuspegi orokorra - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Produktuetan oinarritutako kontratuaren lerroak sor ditzakezu Dynamics 365 Project Operations-en. Produktuen araberako kontratuaren lerroak eskuz sortutako lerroak izan daitezke, edo produktuen katalogoko elementuak izan daitezke.

## <a name="product-catalog"></a>Produktuen katalogoa

Produktuen katalogoko produktuek unitate eta unitate multzo lehenetsiak dituzte. Hainbat produktuk atributu multzo bera partekatzen badute, ezaugarri horiek ere badituen produktuen familia sor dezakezu. Produktu familia bateko produktu guztiek ezaugarri berdinak heredatzen dituzte.

Adibidez, enpresa batek harpidetzako lizentziak saltzen ditu software askotarako. Harpidetza software guztiek bi atributu hauek dituzte:

- Erabiltzaile kopurua
- Harpidetzaren iraupena (hilabeteetan)

Katalogo mota hau mantentzeko, sortu izena duen produktu familia **Harpidetza softwarea**. Gehitu atributuak, **Erabiltzaile kopurua** eta **Harpidetzaren iraupena** produktuen familiari. Ondoren, gehitu produktu indibidualak **Harpidetza softwarea** produktuen familia.

## <a name="add-product-catalog-items-to-a-project-contract"></a>Gehitu produktuen katalogoko elementuak proiektuaren kontratuan

Proiektuen kontratuek bi lerro mota dituzte ataletan: proiektuan oinarritutakoak eta produktuetan oinarritutakoak. Produktuan oinarritutako lerroek produktu eta unitate guztiak biltzen dituzte kontratuko produktuen prezioen zerrendan. Kontratuaren produktu-zerrendako zati ez diren produktuak gehi ditzakezu.

Produktuak beste prezio zerrendetatik edo zuzenean produktuen katalogotik hauta ditzakezu. Produktuak katalogo batetik zuzenean hautatzen dituzunean, produktu horren prezioen zerrenda lehenetsia erabiltzen da produktuaren salmenta prezioa lortzeko. Lehenetsitako prezioen zerrenda zehazten ez bada, prezioa 0 (zero) izango da.

Kontratuaren lerro bat produktuen katalogoan oinarrituta badago, salmenta-prezioa zuzenean alda dezakezu lerroan. Kontratu linea batek du **Prezioak** bi balioekin eremua:

- **Gainidatzi prezioa**
- **Erabili balio lehenetsiak**

**Prezioak** eremua **Gainidatzi prezioa** gisa ezartzen baduzu, ez da prezio lehenetsirik zehazten. Idatzi kontratuaren lerroko produktuaren prezioa. Eremua ezartzen baduzu **Erabili lehenetsia**, salmenta prezio lehenetsia erabiltzen da eta eremua ezin da editatu.

Project Operations instalatu ondoren, salmenta prezio lehenetsiak produktuaren araberako lerroetan sartzen dira kontratu batean. **Prezioa** eremua, eremuan ezarri behar da **Gainidatzi prezioak** kontratuaren lerroetan prezio lehenetsia editatu ahal izateko. Project Operations-ek produktuan oinarritutako lerroen portaera berraztertzen dute Dynamics 365 Sales-en.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]