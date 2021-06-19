---
title: Konfiguratu proiektuko kontratuaren lerro bateko kobra daitezkeen osagaiak
description: Gai honek kontratuaren lerrokako aurrekontu lerro batean barne dauden, kargagarriak eta kargagarriak ez diren osagaiei buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/12/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d42dd180dacc45e72eddcac70ae9ede38d4c36c6
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013606"
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
