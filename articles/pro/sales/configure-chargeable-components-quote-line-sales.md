---
title: Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak
description: Gai honek proiektuan oinarritutako aurrekontu lerro batean kargagarriak eta kargagarriak ez diren osagaiak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e0b64d7edb21df127bf7544f044de7f3c496dfe3
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071157"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a>Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuetan oinarritutako eskaintzaren lerroak *barne* osagaiak eta *kargagarriak* osagaiak kontzeptuak ditu.

Sartutako osagaien menpe daude:

  - Fakturazio metodoa eta bezeroen banaketak
  - Ez gainditzeko mugak 
  - Proiektuan oinarritutako eskaintzaren lerroan zehaztutako fakturen maiztasun ezarpenak

Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua. **Fakturazio mota** eremua eskaintzaren lerro baten testuinguruan balio hauek onartzen dituen aukera multzoa da:

  - Kobra daiteke
  - Ezin da kargatu

Osagai kargagarriak zereginetan, roletan eta transakzio kategorietan defini daitezke.

Kargagarritasuna eskaintzaren kontratu lerro bateko zereginetan definitzen da eta lerroan sartutako transakzio klase guztiei aplikatzen zaie. **Gehitu zereginak** eremua **Proiektu osoa** bada edo hutsik badago, **Kobratzeko zereginak** fitxa ez da erabilgarri egongo.

Eskaintzaren lerro bateko roletan definitutako kargagarritasuna **Denbora** transakzio klasea. Eremuan, **Gehitu denbora** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.

Eskaintzaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea. Eremuan, **Gehitu gastuak** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a>Eguneratu proiektuaren zeregina kargagarria edo kargagarria ez den moduan

Proiektuaren zeregina proiektuetan oinarritutako eskaintzaren lerro zehatz baten testuinguruan kargagarria edo ez kargagarria izan daiteke eta horrek konfigurazio hau posible egiten du:

Proiektuan oinarritutako aurrekontu lerroak biltzen badu **Denbora** eta zeregina **T1**, zeregina aurrekontu lerroarekin lotzen da kobratzeko moduan. Horrek barne hartzen duen bigarren eskaintzaren lerro bat badago **Gastuak**, **T1** zeregina eskaintzaren lerroan lotu dezakezu kobratzeko moduan. Emaitza da zereginean grabatutako denbora guztia kargagarria dela eta kargagarriak ez diren zereginetako gastu guztiak ez direla erregistratzen.

Ataza baten fakturazio mota konfiguratu daiteke **Zeregin kargagarriak** proiektuetan oinarritutako eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Eskaintzaren lerroaren zereginak** azpi-saretan. Bestela, **Fakturazio mota** eremuko proiektuaren fakturazio mota egunera dezakezu zereginaren azpi-saretako zeregin bati lotutako eskaintzaren lerroak erakusten dituen proiektu baten fakturazio konfigurazioa.

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a>Eguneratu funtzioa kargagarria edo kargagarria ez den moduan

Eginkizun bat kargagarria edo ez kargagarria izan daiteke proiektuan oinarritutako aurrekontu lerro jakin baten testuinguruan.

Funtzio baten fakturazio mota konfiguratu daiteke **Funtzio kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Funtzio kargagarriak** azpi-saretan.

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a>Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan

Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke eskaintzaren lerro jakin batean.

Transakzio baten fakturazio mota konfiguratu daiteke **Kategoria kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Kategoria kargagarriak** azpi-saretan.

### <a name="resolve-chargeability"></a>Kargagarritasuna ebatzi
Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da **Denbora** eskaintzaren lerroan sartzen da, eta bada **Egitekoa** eta **Rola** eskaintzaren lerroan kargatzeko moduan konfiguratuta daude.

Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da **Gastua** eskaintzaren lerroan sartzen da, eta bada **Egitekoa** eta **Transakzioaren kategoria** eskaintzaren linean kargatzeko moduan konfiguratuta daude.

| Denbora barne | Gastua barne | Gehitutako zereginak | Funtzioa | Kategoria | Ataza | Fakturazioa |
| --- | --- | --- | --- | --- | --- | --- |
| Yes | Yes | Proiektu osoa | Kobra daiteke | Kobra daiteke | Ezin da ezarri | Fakturazioa denbora errealean: Kargagarria </br>Fakturazio mota benetako gastuan: Kargagarria |
| Yes | Yes | Hautatutako zereginak soilik | Kobra daiteke | Kobra daiteke | Kobra daiteke | Fakturazioa denbora errealean: Kargagarria</br>Fakturazio mota benetako gastuan: Kargagarria |
| Yes | Yes | Hautatutako zereginak soilik | Ezin da kargatu | Kobra daiteke | Kobra daiteke | Fakturazioa denbora errealean: Ez-kargagarria</br>Fakturazio mota benetako gastuan: Kargagarria |
| Yes | Yes | Hautatutako zereginak soilik | Kobra daiteke | Kobra daiteke | Ezin da kargatu | Fakturazioa denbora errealean: Ez-kargagarria</br> Fakturazio mota benetako gastuan: Ez-kargagarria |
| Yes | Yes | Hautatutako zereginak soilik | Ezin da kargatu | Kobra daiteke | Ezin da kargatu | Fakturazioa denbora errealean: Ez-kargagarria</br> Fakturazio mota benetako gastuan: Ez-kargagarria |
| Yes | Yes | Hautatutako zereginak soilik | Ezin da kargatu | Ezin da kargatu | Kobra daiteke | Fakturazioa denbora errealean: Ez-kargagarria</br> Fakturazio mota benetako gastuan: Ez-kargagarria |
| +Ez | Yes | Proiektu osoa | Ezin da ezarri | Kobra daiteke | Ezin da ezarri | Fakturazioa denbora errealean: Ez dago erabilgarri </br>Fakturazio mota benetako gastuan: Kargagarria |
| +Ez | Yes | Proiektu osoa | Ezin da ezarri | Ezin da kargatu | Ezin da ezarri | Fakturazioa denbora errealean: Ez dago erabilgarri </br>Fakturazio mota benetako gastuan: Ez-kargagarria |
| Yes | +Ez | Proiektu osoa | Kobra daiteke | Ezin da ezarri | Ezin da ezarri | Fakturazioa denbora errealean: Kargagarria</br>Fakturazio mota benetako gastuan: Ez dago erabilgarri |
| Yes | +Ez | Proiektu osoa | Ezin da kargatu | Ezin da ezarri | Ezin da ezarri | Fakturazioa denbora errealean: Ez-kargagarria </br>Fakturazio mota benetako gastuan: Ez dago erabilgarri |
