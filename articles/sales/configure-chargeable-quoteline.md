---
title: Konfiguratu proiektuetan oinarritutako eskaintzaren lerro bateko kobra daitezkeen osagaiak
description: Gai honek proiektuan oinarritutako aurrekontu lerroetan sartutako, kargatzeko eta kargatu ezin diren osagaiei buruzko informazioa eskaintzen du.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a9febf305e3cd29bab42cd6c83a941f7b494fa56
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013561"
---
# <a name="configure-the-chargeable-components-of-a-project-based-quote-line"></a>Konfiguratu proiektuetan oinarritutako eskaintzaren lerro bateko kobra daitezkeen osagaiak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuan oinarritutako aurrekontu lerro batek osagaiak eta kargagarriak diren osagaiak izan ditzake.

Sartutako osagaiak fakturazio metodoaren, bezeroen zatitzeen, mugak gainditu behar ez direnen eta proiektuan oinarritutako aurrekontu lerroan zehaztutako fakturen maiztasunaren menpe daude.
Sartutako osagaien azpimultzo bat kargagarritzat marka daiteke erabilita **Fakturazio mota**. Aukera hauetako bat hauta dezakezu **Fakturazio mota** eremua aurrekontu lerro baten testuinguruan:

   - Kobra daiteke
   - Ezin da kargatu

Osagai kargagarriak roletan eta transakzio kategorietan defini daitezke.

Proiektuaren aurrekontu lerro bateko roletan definitzen den kargagarritasuna **Denbora** transakzio klasea. Proiektuaren aurrekontu lerroak badu **Sartu denbora** = **Ez**, **Kargatzeko rolak** fitxa ez dago erabilgarri.

Proiektuaren aurrekontu lerro bateko transakzio-kategoriek definitzen den kargagarritasuna **Gastuak** transakzio klasea. Proiektuaren aurrekontu lerroak badu **Sartu gastuak** = **Ez**, **Kargatzeko kategoriak** fitxa ez dago erabilgarri.

## <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a>Eguneratu funtzioa kargagarria edo kargagarria ez den moduan
Eginkizun bat kargagarria edo kargagarria izan daiteke proiektuan oinarritutako aurrekontu lerro batean. Rol batean fakturazio mota konfiguratu daiteke **Kargatzeko rolak** proiektuan oinarritutako aurrekontu lerroaren fitxa. Horretarako, eguneratu **Fakturazio mota** **Kargatzeko rolak** azpisarea. 

## <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a>Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan
Transakzio-kategoria bat kargagarria edo kargagarria izan daiteke proiektuan oinarritutako aurrekontu lerro batean. Transakzio batean fakturazio mota konfiguratu daiteke **Kargatzeko kategoriak** proiektuan oinarritutako aurrekontu lerroaren fitxa. Horretarako, eguneratu **Fakturazio mota** eremuan **Kargatzeko kategoriak** azpisarea. 

## <a name="resolve-chargeability"></a>Kargagarritasuna ebatzi

Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da denbora aurrekontuaren lerroan sartzen bada eta eginkizuna kargatzeko moduan konfiguratuta badago.
Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da gastua aurrekontuaren lerroan sartzen bada eta eginkizuna kargatzeko moduan konfiguratuta badago. Hurrengo taulan kargagarritasuna benetako bakoitzean nola lehenesten den erakusten da. Lehenespenak barne dauden osagaietan eta aurrekontu lerroan konfiguratutako fakturazio motan oinarritzen dira.

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