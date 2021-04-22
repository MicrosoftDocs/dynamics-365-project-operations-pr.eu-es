---
title: Kudeatu proiektuaren fakturazioaren lan atzeratua
description: Gai honek proiektuetan fakturazio-zorroa kudeatzeko erabilgarri dauden hainbat ikuspegiri buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 25dc9cff6aeb6daed9a27ba843a74b892ca4751c
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/07/2021
ms.locfileid: "5866981"
---
# <a name="manage-project-billing-backlog"></a>Kudeatu proiektuaren fakturazioaren lan atzeratua 

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Dynamics 365 Project Operations-ek ikuspegiak eskaintzen ditu fakturazio-zorroa kudeatzen laguntzeko. Fakturazio-zorroa kudeatzeko, hautatu estekak **Salmentak** area, **Fakturazioa** eremuan. 

Ikuspegi hauek daude erabilgarri:

- Aurrerapenak eta aurrerakinak
- Erabilgarri dauden aurrerapenak eta aurrerakinak
- Prezio finkoaren mugarriak
- Produktuaren fakturazioaren lana
- Denbora eta materialen fakturazioaren lana

## <a name="retainers-and-advances"></a>Aurrerapenak eta aurrerakinak

**Atxikitzaileak eta aurrerakinak** ikuspegiak sistemako proiektuen kontratu guztien atxikipen eta aurrerapen guztiak zerrendatzen ditu. Atxikipena edo aurrerakina fakturatu ondoren, aurrerakinaren zenbatekoa erabilgarri egongo da.

## <a name="available-retainers-and-advances"></a>Erabilgarri dauden aurrerapenak eta aurrerakinak

**Erabilgarri dauden Atxikitzaileak eta aurrerakinak** ikuspegiak sistemako proiektuen kontratu guztien atxikipen eta aurrerapen guztiak zerrendatzen ditu. Atxikipena edo aurrerakina fakturatu ondoren, aurrerakinaren zenbatekoa erabilgarri egongo da eta zerrendan gehitzen da. Atxikipenaren edo aurrerakinaren kopurua erabat erabili ondoren, zerrendatik kentzen da.

## <a name="fixed-price-milestones"></a>Prezio finkoaren mugarriak

**Prezio finkoaren mugarriak** ikuspegiak sistemako proiektuen kontratu lerro guztietako prezio finkoen mugarri guztiak zerrendatzen ditu. Mugarri bakar edo anitz gisa markatu daitezke **Fakturatzeko prest** edo **Ez dago fakturatzeko prest** ikuspegi honetatik. Mugarri gisa markatzea **Fakturatzeko prest** faktura zirriborroan jartzeko erabilgarri jartzen du.

Bezero anitzeko kontratu lerroek prezio finkoko fakturazio metodoa dutenean, kontratu lerroan bezero bakoitzarentzat mugarri bat sortzen da. Mugarri bat sor daiteke eta gero bezeroaren berariazko mugarrien erregistro banatu daiteke. Zatiketa hori barnekoa da eta kontratuaren lerroan bezero bakoitzarentzat zehaztutako fakturazio ehunekoaren arabera. **Prezio finkoaren mugarriak** ikuspegian, bezeroaren berariazko mugarrien erregistroak ikusiko dituzu. Mugarrien erregistro horietako bakoitza honela markatu daiteke **Fakturatzeko prest** ikuspegi honetatik bereizita. Lotutako mugarrietako bat edo gehiago honela markatzen direnean **Fakturatzeko prest**, goiburuaren egoera eguneratu da **Abian** **Ez da hasi** aukeratik. Mugarri banaketa guztiak fakturatzen direnean, goiburuaren mugarri egoera eguneratu egiten da **Osatuta**.

Fakturaren zirriborroaren mugarria erakusten da ikuspegi honetan fakturazio egoerarekin **Bezeroaren faktura sortu da**. Faktura zirriborroa baieztatzen denean, erregistroan fakturazio egoera eguneratzen da **Bezeroaren faktura argitaratua**. Ez eguneratu egoera balio hau kode pertsonalizatua erabiliz. Project Operations-ek ez du ondo funtzionatzen egoera balio horiek kode pertsonalizatuarekin eguneratzen direnean.

## <a name="product-billing-backlog"></a>Produktuaren fakturazioaren lana

**Produktuen fakturazio-zorroa** ikuspegia sistemako proiektuen kontratu guztietan produktuetan oinarritutako kontratu lerro guztiak zerrendatzen ditu. Produktuetan oinarritutako kontratuaren lerro bakar edo anitz gisa markatu daitezke **Fakturatzeko prest** edo **Ez dago fakturatzeko prest** ikuspegi honetatik. Produktuan oinarritutako kontratuaren lerroak **Fakturatzeko prest** faktura zirriborroan jartzeko erabilgarri jartzen du.

Fakturaren zirriborroan agertzen den produktuan oinarritutako kontratu lerroa fakturazio egoerarekin erakusten da ikuspegi honetan **Bezeroaren faktura sortu da**. Faktura zirriborroa baieztatzen denean, erregistro honetako fakturazio egoera eguneratzen da **Bezeroaren faktura argitaratua**. Ez eguneratu egoera balio hau kode pertsonalizatua erabiliz. Project Operations-ek ez du ondo funtzionatzen egoera balio horiek kode pertsonalizatuarekin eguneratzen direnean.

## <a name="time-and-material-billing-backlog"></a>Denbora eta materialen fakturazioaren lana

**Denboraren eta materialaren fakturazio-zorroa** ikuspegian fakturatu gabeko sistemako proiektuen kontratu guztietan fakturatu gabeko salmenten faktore guztiak zerrendatzen dira. Fakturatu gabeko salmenta bakarraren edo anitzen benetako datu gisa markatu daitezke **Fakturatzeko prest** edo **Ez dago fakturatzeko prest** ikuspegi honetatik. Fakturarik gabeko salmenten gisa markatzen da **Fakturatzeko prest** eskuragarri jartzen du faktura zirriborroan jartzeko.

Fakturatu gabeko salmenten benetakoak **Ez gainditzeko** egoera **Huts egin du** ezin da gisa markatu **Fakturatzeko prest**. Egiazkoak honela markatu behar badira **Fakturatzeko prest**, berrezarri konpromisoa hartu duten kontratuaren lineako beste datu errealetan. eta berrebaluatu **Ez gainditzekoa** egoeran.

Bezero anitzeko kontratu lerroek denbora eta materialen fakturazio metodoa baldin badute, denbora eta gastuak onartzen direnean, fakturatu gabeko salmenta erreal bat sortzen da kontratu lerroan bezero bakoitzarentzat, bezero bakoitzarentzat zehaztutako fakturazio ehunekoaren arabera. **Denboraren eta materialaren fakturazio-zorroa** ikuspegian, bezeroaren berariazko fakturaziorik gabeko salmenta errealak ikusiko dituzu. Faktura gabeko salmenten benetako datuen erregistro horietako bakoitza honela markatu daiteke **Fakturatzeko prest** ikuspegi honetatik bereizita.

Fakturatu gabeko salmenten benetako datuen zirriborroan agertzen den produktuan oinarritutako kontratu lerroa fakturazio egoerarekin erakusten da ikuspegi honetan **Bezeroaren faktura sortu da**. Faktura zirriborroa baieztatzen denean, erregistro honetako fakturazio egoera eguneratzen da **Bezeroaren faktura argitaratua**. Ez eguneratu egoera balio hau kode pertsonalizatua erabiliz. Project Operations-ek ez du ondo funtzionatzen egoera balio horiek kode pertsonalizatuarekin eguneratzen direnean.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
