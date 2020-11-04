---
title: Proiektuetan oinarritutako kontratuaren lerro baten osagai kargagarriak konfiguratzea
description: Gai honetan Project Operations-eko kontratuaren lerroetan osagai kargagarriak gehitzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4d665a6351d2315d185e64e4eb6b0b8859f7bbc4
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070943"
---
# <a name="configuring-chargeable-components-of-a-project-based-contract-line"></a>Proiektuetan oinarritutako kontratuaren lerro baten osagai kargagarriak konfiguratzea

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako kontratuaren lerroak osagaiak eta osagai *kargagarriak* *ditu barne*.

Osagai hauek honako hauen menpeko osagaiak dira:

  - Fakturazio metodoa eta bezeroen banaketak
  - Ez gainditzeko mugak 
  - Proiektuan oinarritutako kontratu lerroan zehaztutako fakturen maiztasun ezarpenak

Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua. **Fakturazio mota** eremua kontratu lerro baten testuinguruan balio hauek onartzen dituen aukera multzoa da:

  - Kobra daiteke
  - Ezin da kargatu

Osagai kargagarriak zereginetan, roletan eta transakzio kategorietan defini daitezke.

Kargagarritasuna proiektuko kontratu lerro bateko zereginetan definitzen da eta lerroan sartutako transakzio klase guztiei aplikatzen zaie. Kontratuaren lerroko **Gehitu zereginak** eremua hutsik badago edo **Proiektu osoa** gisa ezarrita badago, **Kobratzeko zereginak** fitxa ez da erabilgarri egongo.

Proiektuaren kontratu lerro bateko roletan definitutako kargagarritasuna **Denbora** transakzio klasea. Kontratuaren lerroko **Gehitu denbora** eremua **Ez** gisa ezarrita badago, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.

Proiektuaren kontratuaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea. Kontratuaren lerroko **Gehitu gastuak** eremua **Ez** gisa ezarrita badago, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a>Eguneratu proiektuaren zeregina kargagarria edo kargagarria ez den moduan

Proiektuaren zeregina kontratu-lerro zehatz batean kargagarria edo ez kargagarria izan daiteke eta horrek konfigurazio hau posible egiten du:

Proiektuetan oinarritutako kontratu lerroak barne hartzen badu **Denbora** eta zeregin jakin bat, **T1** kargagarri gisa lotzen zaio. Horrek barne hartzen duen bigarren kontratu linea bat badago **Gastua** , T1 zeregina kontratu-lerroan lotu dezakezu kobratzeko moduan. Emaitza da zereginean grabatutako denbora guztia kargagarria dela eta gastu guztiak ez direla kobratzen.

Ataza baten fakturazio mota konfiguratu daiteke **Zeregin kargagarriak** kontratuaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua kontratu-lerroaren atazen azpi-saretan. Bestela, **Fakturazio mota** eremua egunera dezakezu zereginaren azpi-saretako Zeregin bati lotutako kontratu lerroak erakusten dituen proiektu baten fakturazio konfigurazioa.

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a>Eguneratu funtzioa kargagarria edo kargagarria ez den moduan

Eginkizun bat kargagarria edo ez kargagarria izan daiteke kontratu-lerro jakin batean.

Rol baten fakturazio mota konfiguratu daiteke **Kargatzeko rolak** kontratu lerro baten fitxa. Horretarako, eguneratu **Fakturazio mota** eremuan **Kargatzeko rolak** azpi-sareta.

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a>Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan

Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke kontratu-lerro jakin batean.

Transakzio baten fakturazio mota konfiguratu daiteke **Kargatzeko kategoriak** kontratuaren lerro batean oinarritutako proiektatearen fitxa. Horretarako, eguneratu **Fakturazio mota** eremuan **Kargatzeko kategoriak** azpi-sareta.

### <a name="resolve-chargeability"></a>Kargagarritasuna ebatzi

Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da **Denbora** kontratu-lerroan sartzen da, eta bada **Egitekoa** eta **Rola** kontratu-linean kargatzeko moduan konfiguratuta daude.

Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da **Gastua** kontratu-lerroan sartzen da, eta bada **Egitekoa** eta **Transakzioa** kategorien kontratu-linean kargatzeko moduan konfiguratuta daude.


| Denbora barne | Gastua barne | Zereginak barne | Funtzioa           | Kategoria       | Ataza                                                                                                      |
|---------------|------------------|----------------|----------------|----------------|-----------------------------------------------------------------------------------------------------------|
| Yes           | Yes              | Proiektu osoa | Kobra daiteke     | Kobra daiteke     | Fakturazioa denbora errealean: **Kargagarria** </br> Fakturazio mota benetako gastuan: **Kargagarria**           |
| Yes           | Yes              | Hautatutako zereginak | Kobra daiteke     | Kobra daiteke     | Fakturazioa denbora errealean: **Kargagarria** </br> Fakturazio mota benetako gastuan: **Kargagarria**           |
| Yes           | Yes              | Hautatutako zereginak | Ezin da kargatu | Kobra daiteke     | Fakturazioa denbora errealean: **Ez-kargagarria** </br> Fakturazio mota benetako gastuan: **Kargagarria**       |
| Yes           | Yes              | Hautatutako zereginak | Kobra daiteke     | Kobra daiteke     | Fakturazioa denbora errealean: **Ez-kargagarria** </br> Fakturazio mota benetako gastuan: **Ez-kargagarria** |
| Yes           | Yes              | Hautatutako zereginak | Ezin da kargatu | Kobra daiteke     | Fakturazioa denbora errealean: **Ez-kargagarria** </br> Fakturazio mota benetako gastuan: **Ez-kargagarria** |
| Yes           | Yes              | Hautatutako zereginak | Ezin da kargatu | Ezin da kargatu | Fakturazioa denbora errealean: **Ez-kargagarria** </br> Fakturazio mota benetako gastuan: **Ez-kargagarria** |
| +Ez            | Yes              | Proiektu osoa | Ezin da ezarri   | Kobra daiteke     | Fakturazioa denbora errealean: **Ez dago erabilgarri**</br>Fakturazio mota benetako gastuan: **Kargagarria**          |
| +Ez            | Yes              | Proiektu osoa | Ezin da ezarri   | Ezin da kargatu | Fakturazioa denbora errealean: **Ez dago erabilgarri**</br> Fakturazio mota benetako gastuan: **Ez-kargagarria**     |
| Yes           | +Ez               | Proiektu osoa | Kobra daiteke     | Ezin da ezarri   | Fakturazioa denbora errealean: **Kargagarria** </br> Fakturazio mota benetako gastuan: **Ez dago erabilgarri**        |
| Yes           | +Ez               | Proiektu osoa | Ezin da kargatu | Ezin da ezarri   | Fakturazioa denbora errealean: **Ez-kargagarria** </br>Fakturazio mota benetako gastuan: **Ez dago erabilgarri**   |
