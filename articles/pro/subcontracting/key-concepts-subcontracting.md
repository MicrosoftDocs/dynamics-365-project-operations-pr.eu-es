---
title: Azpikontratazioko kontzeptu nagusiak
description: Gai honek azpikontratazioari aplika dakizkiokeen funtsezko kontzeptu batzuk azaltzen ditu Microsoft Dynamics 365 Project Operations-en.
author: rumant
ms.date: 08/03/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 01d2e57b99015c346be15e3504440c14cb9a54e24215c0b1c052c5112f4b940a
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994261"
---
# <a name="key-concepts-in-subcontracting"></a>Azpikontratazioko kontzeptu nagusiak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gaiak azpikontratazio funtzionalitatea erabiltzen hasi aurretik ezagutu behar zenituzkeen zenbait gako kontzeptu azaltzen ditu Microsoft Dynamics 365 Project Operations-en.

## <a name="contracting-unit-on-the-subcontract"></a>Azpikontrataren kontratazio unitatea

Kontratazio unitateak proiektua entregatzearen jabe den zatiketa edo praktika adierazten du. Kontratazio unitatea saltzailearekin kontratu harremana egiten duen zatiketa ere bada.

## <a name="purchase-currency"></a>Ordainketa-moneta

Project Operations-en, erosketa moneta azpikontratua sortzen den moneta da. Proiektu batean azpikontratisten kostuak erregistratzen diren moneta ere bada. Erosketa moneta proiektuaren moneta desberdina izan daiteke, eta proiektuaren moneta salmenten moneta desberdina izan daiteke.

## <a name="billing-methods-on-subcontract-lines"></a>Fakturazio metodoak azpikontratazio lerroetan

Proiektuetarako, normalean kuota finkoak eta kontsumoan oinarritutako kontratazio ereduak daude. Project Operations-ek fakturazio metodo hauek onartzen ditu salmenta eta erosketa testuinguruetan. Erosketa egiteko, fakturazio metodoek honela funtzionatzen dute:

- **Denbora eta materiala**: azpikontratazio lerro batek **Denbora eta materiala** fakturazio metodoa, denboraren kostua proiektuan erregistratzen da azpikontratatzaileek proiektu horretan lan egiten duten bitartean eta denbora erregistratzen duten bitartean. Azpikontratatzaileen kostu transakzio hauek saltzailearen fakturetako lerro-elementuekin lotzen dira. Eredu honetan, Project Operations erabiltzen dituzten proiektuen zuzendariek hornitzaileen faktura-lerroak erregistratu eta onartzen dituzten azpikontratisten denborarekin lotu eta egiaztatu ditzakete. Egiaztapena amaitu ondoren, onartu ondoren erregistratu ziren aurreko kostuen fakturak alderantzikatu egiten dira eta saltzailearen fakturan oinarritutako kostu berrien egitasmoak sortzen dira proiektuan.
- **Prezio finkoa**: kuota finkoen kontratazio eredu honetan, saltzailearen fakturak mugarri finkoetan oinarritzen dira. Hala ere, azpikontratatutako baliabideek denbora jakinarazi dezakete. Ordua proiektuaren zuzendariak berrikusi eta onartu egiten du. Onartzen denean, Project Operations-ek aldi baterako kostuen errealitatea sortzen du proiektuan. Saltzaileak mugarri baten faktura bidali ondoren, proiektuaren zuzendariak aurrez erregistratutako kostuen errealitatearekin bat egin dezake. Egiaztapena amaitutakoan, kostuen benetako gauzak alderantzikatu egiten dira eta mugarrian oinarritutako kostua erregistratzen da.

## <a name="project-price-lists-on-subcontracts"></a>Proiektuaren prezio-zerrendak azpikontratuetan

Proiektuen prezioen zerrendak denbora, gastu eta proiektuarekin lotutako beste osagai batzuetarako erosketa prezioak ezartzeko erabiltzen diren prezioen zerrendak dira. Hainbat prezio zerrenda egon daitezke, eta horietako bakoitzak bere data eraginkorra den azpikontrata izan dezake Project Operations-en. Project Operations-ek ez dute azpikontratako proiektuen prezioen zerrendetan data eraginkorrak gainjartzea onartzen.

## <a name="transaction-classes-on-subcontracts"></a>Azpikontratetako transakzio klaseak

Project Operations-ek lau transakzio klase mota onartzen ditu:

- Denbora
- Gastua
- Materiala
- Tasa

Erosketa kostuak soilik kalkulatu eta sor daitezke **Denbora**, **Gastua**, eta **Materiala** transakzio klaseak. **Kuota** diru-sarrerak soilik dituzten transakzio klasea da eta ez dago eskuragarri erosketaren edukian.

## <a name="purchase-pricing-dimensions"></a>Erosketa-prezioen dimentsioak

Prezioen dimentsioek erosketa prezioa konfiguratzeko eta denborako transakzioetan lehenetsitakoak zer atributu erabakitzen dituzun. Erosketari dagokionez, Project Operations-ek dimentsio finko multzoak soilik onartzen ditu erosketa prezioa konfiguratzeko eta lehenetsitakoak. Erosketaren prezioa konfiguratzeko eta azpikontratazio lerroetan eta azpikontratazio denborako transakzioetan lehenespenez egiteko, atributuak hauek dira **Funtzioa** eta **Erreserbatzeko Baliabidea**.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
