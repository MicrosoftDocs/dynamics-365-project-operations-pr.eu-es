---
title: Konfiguratu proiektuko kontratuaren lerro bateko kobra daitezkeen osagaiak
description: Artikulu honetan, kontratu-lerroetan sartutako osagaiei, ordainketa-osagaiei eta kobratu ezin direnei buruzko informazioa ematen da.
author: rumant
ms.date: 10/12/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 175b25dbcc43a5954fbbf2d54efdd73e19395907
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928279"
---
# <a name="configure-chargeable-components-of-a-project-contract-line"></a>Konfiguratu proiektuko kontratuaren lerro bateko kobra daitezkeen osagaiak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuetan oinarritutako kontratuaren lerroak barne dauden, kobragarriak diren eta kroba ezin daitezkeen osagaiak kontzeptuak ditu.

Sartutako osagaiak fakturazio metodoaren, bezeroen zatitzeen, mugak gainditu behar ez direnen eta proiektuan oinarritutako kontratu lerroan zehaztutako fakturen maiztasunaren menpe daude.

Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua eguneratuz.

Osagai kargagarriak roletan eta transakzio kategorietan defini daitezke.

Kontratuaren lerro batean, funtzio batean definitutako kargagarritasuna **Denbora** transakzio klaseari soilik aplikatzen zaio. **Gehitu denbora** eremua **Ez** gisa ezarrita badago kontratuaren lerroan, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.

Proiektuaren kontratuaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea. **Gehitu gastuak** eremua **Ez** gisa ezarrita badago kontratuaren lerroan, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a>Eguneratu funtzioa kargagarria edo kargagarria ez den moduan

Eginkizun bat kargagarria edo ez kargagarria izan daiteke proiektuan oinarritutako kontratu-lerro jakin batean.

Proiektuetan oinarritutako kontratuaren lerroko **Funtzio kargagarriak** fitxan, **Kategoria kargagarriak** azpisarean, **Fakturazio mota** eremuan, eguneratu funtzio baten fakturazio mota.

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a>Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan

Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke proiektuetan oinarritutako kontratu-lerro jakin batean.

Proiektuetan oinarritutako kontratuaren lerroko **Kategoria kargagarriak** fitxan, **Kategoria kargagarriak** azpisarean, **Fakturazio mota** eremuan, eguneratu funtzio baten fakturazio mota.

### <a name="resolve-chargeability"></a>Kargagarritasuna ebatzi

Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da denbora kontratu-lerroan sartzen da, eta bada funtzioa kontratu-linean kargatzeko moduan konfiguratuta daude.

Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da gastua kontratu-lerroan sartzen da, eta bada transakzioa kategoriaren kontratu-linean kargatzeko moduan konfiguratuta dago.

| Denbora barne | Gastua barne | Funtzioa | Kategoria | Ataza |
| --- | --- | --- | --- | --- |
| Yes | Yes | Kobra daiteke | Kobra daiteke | Fakturazioa denbora errealean: Kargagarria </br>Fakturazio mota benetako gastuan: Kargagarria |
| Yes | Yes | Ezin da kargatu | Kobra daiteke | Fakturazioa denbora errealean: Ez-kargagarria </br>Fakturazio mota benetako gastuan: Kargagarria |
| Yes | Yes | Ezin da kargatu | Ezin da kargatu | Fakturazioa denbora errealean: Ez-kargagarria </br>Fakturazio mota benetako gastuan: Ez-kargagarria |
| +Ez | Yes | Ezin da ezarri | Kobra daiteke | Fakturazioa denbora errealean: Ez dago erabilgarri </br>Fakturazio mota benetako gastuan: Kargagarria |
| +Ez | Yes | Ezin da ezarri | Ezin da kargatu | Fakturazioa denbora errealean: Ez dago erabilgarri </br>Fakturazio mota benetako gastuan: Ez-kargagarria |
| Yes | +Ez | Kobra daiteke | Ezin da ezarri | Fakturazioa denbora errealean: Kargagarria </br>Fakturazio mota benetako gastuan: Ez dago erabilgarri |
| Yes | +Ez | Ezin da kargatu | Ezin da ezarri | Fakturazioa denbora errealean: Ez-kargagarria </br> Fakturazio mota benetako gastuan: Ez dago erabilgarri |


[!INCLUDE[footer-include](../includes/footer-banner.md)]
