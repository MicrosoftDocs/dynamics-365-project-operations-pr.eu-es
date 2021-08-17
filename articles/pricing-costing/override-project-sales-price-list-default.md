---
title: Gainidatzi proiektuaren salmenten prezio-zerrendak
description: Gai honek salmenta prezioen zerrenda pertsonalizatuak sortzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b26947822eb8e87b3b36fcde9c99c6ee69375aa942a5641112b9b1109dcaa26c
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7009561"
---
# <a name="override-project-sales-price-lists"></a>Gainidatzi proiektuaren salmenten prezio-zerrendak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

## <a name="customer-specific-project-price-lists"></a>Bezeroarentzako proiektuaren prezioen zerrendak

Bezeroen berariazko prezioen akordioak proiektuaren prezioen zerrenda gisa konfigura daitezke Dynamics 365 Project Operations-eko kontu erregistro batean.

Bezeroaren proiektuaren prezioen zerrenda konfiguratzeko, **Salmentak** eremuan, nabigatu kontuaren erregistroa.

1. Ireki **Kontuak** zerrenda orria.
2. Aurkitu eta egin klik bikoitza bezeroaren erregistroan fitxategia irekitzeko **Kontua** xehetasunen orria.
3. **Proiektuaren prezio-zerrendak** fitxan, hautatu **+ Proiektuaren prezio-zerrenda berria**.
4. **Proiektuaren prezio-zerrenda berrian** orrialdean, hautatu goitibeherako prezioen zerrenda. Testuingurua ezarrita duten prezioen zerrendak soilik **Salmentak** eta zeinen moneta bat datorren kontuaren moneta barne.
5. Elkarketaren izena, eta ondoren egin klik **Gorde** botoian. Bezeroarentzako proiektuaren prezioen zerrenda sortzen da. Prezio zerrenda hau proiektu honen aurrekontuak edo bezero honentzat sortutako kontratuetan proiektuaren prezio lehenetsiak erabiliko dira, aurrekontuaren edo proiektuaren kontratuaren sortutako data prezioen zerrendaren eraginkortasun dataren barruan kokatzen bada.

## <a name="custom-pricing-on-project-quotes"></a>Prezio pertsonalizatuak proiektuaren aurrekontuetan

Proiektuen aurrekontuetan, bezeroaren edo proiektuaren parametroen arabera lehenetsitako prezio zerrenda lehenetsi batekin hasten den proiektuaren prezioak izan ditzakezu.

Aurrekontu jakin batean proiektuarekin lotutako lanaren prezio pertsonalizatuak behar dituzunean, proiektuaren prezioen zerrendekin lotutako erakundetik lor dezakezu.

Osatu urrats hauek aurrekontuaren araberako proiektuaren prezioak konfiguratzeko.

1. Ireki proiektuaren eskaintza eta hautatu **Proiektuen prezioen zerrendak** fitxa.
2. Azpisaretan, sakatu **Sortu prezio pertsonalizatuak**.

Aurrekontuari erantsitako proiektuen prezio zerrenda guztiak prezio zerrenda berrietara kopiatzen dira. Prezio zerrenda berrien izenek aurrekontuaren izena islatzen dute prezio zerrenda hauek sortu zireneko data-ordu zigiluarekin.

Prezio zerrenda horietako bakoitza erabil dezakezu eta eskulanaren (rolaren prezioa) eta gastuen (kategoriaren prezioa) prezioen eguneratzeak egin ditzakezu. Prezio hauek proiektuaren eskaintza honi soilik aplikatuko zaizkio.

## <a name="price-lists-on-a-project-contract"></a>Proiektu-kontratuko prezio-zerrendak

Proiektuaren kontratu batean, proiektuaren prezioak beti lehenetsitako prezioen zerrenda pertsonalizatu gisa kontratuaren izenarekin eta sortutako data-ordu zigilua izenarekin erantsita daude. Egia da kontratua aurrekontua irabazi zenean sortu zen edo kontratua hutsetik sortu zen. Behar izanez gero, elkarte hau pertsonalizatutako prezioen zerrendara ken dezakezu eta horren ordez prezio zerrenda estandarra proiektuaren kontratuarekin lotu.

Prezio zerrenda estandar bat aurrekontuan edo kontratuan proiektuaren prezio zerrendekin lotzen duzunean, prezio zerrendako prezioetan egindako aldaketek eragina izango dute prezio zerrenda erabiltzen duten aurrekontu eta kontratu guztietan.


[!INCLUDE[footer-include](../includes/footer-banner.md)]