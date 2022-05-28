---
title: Kudeatu fakturazio atzeratua
description: Gai honek Project Operations-en fakturazio-zorroa ikusi eta nola lan egin jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 9837af0d3c0b2476edab35a53092cf95a44e5244
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8599957"
---
# <a name="manage-billing-backlog"></a>Kudeatu fakturazio atzeratua

**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations

Dynamics 365 Project Operations-ek ikuspegiak eskaintzen ditu fakturazio-zorroa kudeatzen laguntzeko. Fakturazio-zorroa kudeatzeko, hautatu estekak **Salmentak** area, **Fakturazioa** eremuan. 

Ikuspegi hauek daude erabilgarri:

- Aurrerapenak eta aurrerakinak
- Erabilgarri dauden aurrerapenak eta aurrerakinak
- Prezio finkoaren mugarriak
- Denbora eta materialen fakturazioaren lana

## <a name="retainers-and-advances"></a>Aurrerapenak eta aurrerakinak

**Atxikitzaileak eta aurrerakinak** ikuspegiak proiektuen kontratu guztien atxikipenak eta aurrerapenak zerrendatzen ditu. Atxikipena edo aurrerakina fakturatu ondoren, aurrerakinaren zenbatekoa erabilgarri egongo da.

## <a name="available-retainers-and-advances"></a>Erabilgarri dauden aurrerapenak eta aurrerakinak

**Atxikitzaile eta aurrerakin erabilgarriak** ikuspegiak proiektuen kontratu guztien erabilgarri dauden atxikipenak eta aurrerapenak zerrendatzen ditu. Atxikipena edo aurrerakina fakturatu ondoren, aurrerakinaren zenbatekoa erabilgarri egongo da eta zerrendan gehitzen da. Atxikipenaren edo aurrerakinaren kopurua erabat erabili ondoren, zerrendatik kentzen da.

## <a name="fixed-price-milestones"></a>Prezio finkoaren mugarriak

**Prezio finkoaren mugarriak** Ikusi proiektuaren kontratu lerro guztietako prezio finkoen mugarri guztiak zerrendatzen ditu. Ikuspegi honetatik, mugarri bakar edo anitz gisa markatu daitezke **Fakturatzeko prest** edo **Ez dago fakturatzeko prest**. Mugarri gisa markatzea **Fakturatzeko prest** faktura zirriborroan jartzeko erabilgarri jartzen du.

Bezero anitzeko kontratu lerroek prezio finkoko fakturazio metodoa dutenean, kontratu lerroan bezero bakoitzarentzat mugarri bat sortzen da. Mugarri bat sor daiteke eta gero bezeroaren berariazko mugarrien erregistro banatu daiteke. Zatiketa hori barnekoa da eta kontratuaren lerroan bezero bakoitzarentzat zehaztutako fakturazio ehunekoaren arabera. **Prezio finkoaren mugarriak** ikuspegian, bezeroaren berariazko mugarrien erregistroak ikusiko dituzu. Mugarrien erregistro horietako bakoitza honela markatu daiteke **Fakturatzeko prest** ikuspegi honetatik bereizita. Lotutako mugarrietako bat edo gehiago honela markatzen direnean **Fakturatzeko prest**, goiburuaren egoera eguneratu da **Eraikitzen** **Ez da hasi**. Mugarri banaketa guztiak fakturatzen direnean, goiburuaren mugarri egoera eguneratu egiten da **Osatuta**.

Fakturaren zirriborroaren mugarria erakusten da ikuspegi honetan fakturazio egoerarekin **Bezeroaren faktura sortu da**. Faktura zirriborroa baieztatzen denean, erregistroan fakturazio egoera eguneratzen da **Bezeroaren faktura argitaratua**. 

> [!NOTE] 
> Ez eguneratu egoera balio hau kode pertsonalizatua erabiliz. Project Operations-ek ez du ondo funtzionatzen egoera balio horiek kode pertsonalizatuarekin eguneratzen direnean.

## <a name="time-and-material-billing-backlog"></a>Denbora eta materialen fakturazioaren lana

**Denboraren eta materialaren fakturazio-zorroa** ikuspegian fakturatu gabeko sistemako proiektuen kontratu guztietan fakturatu gabeko salmenten faktore guztiak zerrendatzen dira. Fakturatu gabeko salmenta bakarraren edo anitzen benetako datu gisa markatu daitezke **Fakturatzeko prest** edo **Ez dago fakturatzeko prest** ikuspegi honetatik. Fakturarik gabeko salmenten gisa markatzen da **Fakturatzeko prest** eskuragarri jartzen du faktura zirriborroan jartzeko.

Fakturatu gabeko salmenten benetakoak **Ez gainditzeko** egoera **Huts egin du** ezin da gisa markatu **Fakturatzeko prest**. Egiazkoak honela markatu behar badira **Fakturatzeko prest**, berrezarri konpromisoa hartu duten kontratuaren lineako beste datu batzuen egoera eta, ondoren, berriro ebaluatu **Ez gainditzeko** egoera.

Bezero anitzeko kontratu lerroek denbora eta materialen fakturazio metodoa baldin badute, denbora eta gastuak onartzen direnean, fakturatu gabeko salmenta erreal bat sortzen da kontratu lerroan bezero bakoitzarentzat, bezero bakoitzarentzat zehaztutako fakturazio ehunekoaren arabera. **Denboraren eta materialaren fakturazio-zorroa** ikuspegian, bezeroaren berariazko fakturaziorik gabeko salmenta errealak ikusiko dituzu. Faktura gabeko salmenten benetako datuen erregistro horietako bakoitza honela markatu daiteke **Fakturatzeko prest** ikuspegi honetatik bereizita.

Fakturaren zirriborroan jasotako fakturaziorik gabeko salmentak erakusten dira ikuspegi honetan fakturazio egoerarekin **Bezeroaren faktura sortu da**. Faktura zirriborroa baieztatzen denean, erregistro honetako fakturazio egoera eguneratzen da **Bezeroaren faktura argitaratua**. 

> [!NOTE] 
> Ez eguneratu egoera balio hau kode pertsonalizatua erabiliz. Project Operations-ek ez du ondo funtzionatzen egoera balio horiek kode pertsonalizatuarekin eguneratzen direnean.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
