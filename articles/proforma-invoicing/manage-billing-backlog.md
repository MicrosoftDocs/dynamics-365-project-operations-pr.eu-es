---
title: Kudeatu fakturazio atzeratua
description: Gai honek Project Operations-en fakturazio-zorroa ikusi eta nola lan egin jakiteko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ec77f3911a460b96414a61bc44ea254f1b7da660
ms.sourcegitcommit: f8edff6422b82fdf2cea897faa6abb51e2c0c3c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/21/2020
ms.locfileid: "4087795"
---
# <a name="manage-the-billing-backlog"></a>Kudeatu fakturazio atzeratua

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek bi ikuspegi eskaini ditu fakturazio-zorroarekin lan egiten eta kudeatzen laguntzeko. **Prezio finkoaren mugarriak** eta **Denboraren eta materialaren fakturazio-zorroa** Ikuspegia hautatzeko, **Salmentak** proiektuaren eragiketen eremua, ezkerreko nabigazio orrian, hautatu **Fakturazioa**. Fakturazioaren atzerapen estekak bertan gordetzen dira.

## <a name="fixed-price-milestones"></a>Prezio finkoaren mugarriak

Ikuspegi honek sistemako proiektuen kontratu lerro guztietako prezio finkoen mugarri guztiak zerrendatzen ditu. Mugarri bakar edo anitz gisa markatu daitezke **Fakturatzeko prest** edo **Ez dago fakturatzeko prest** ikuspegi honetatik. Mugarri gisa markatzen duzunean **Fakturatzeko prest** , mugarria faktura zirriborro baterako eskuragarri egongo da.

Bezero anitzeko kontratu lerroek prezio finkoko fakturazio metodoa dutenean, mugarri bat sortzen da kontratu lerroan bezero bakoitzarentzat. Erabiltzaileak mugarri bat sortzen du eta mugarri hori bezeroaren arabera = mugarri zehatzen erregistroetan banatzen da, kontratuaren lerroan bezero bakoitzarentzat zehaztutako fakturazio ehunekoaren arabera. **Prezio finkoaren mugarriak** ikuspegian, bezeroaren berariazko mugarrien erregistroak ikusiko dituzu. Mugarrien erregistro horietako bakoitza honela markatu daiteke **Fakturatzeko prest** ikuspegi honetatik bereizita. Lotutako mugarrietako bat edo gehiago honela markatzen direnean **Fakturatzeko prest** , goiburua egoera batera pasatzen da **Eraikitzen** aukeratik **Ez da hasi** aukerara. Mugarri banaketa guztiak fakturatu direnean, goiburuaren mugarri egoera bihurtzen da **Osatuta**.

Fakturaren zirriborroaren mugarria erakusten da ikuspegi honetan fakturazio egoerarekin **Bezeroaren faktura sortu da**. Faktura zirriborroa baieztatzen denean, erregistro honetako fakturazio egoera eguneratzen da **Faktura argitaratua**. Ez da gomendagarria egoera balio hori eguneratzea kode pertsonalizatua erabiliz. Proiektuaren eragiketek ez dute behar bezala funtzionatuko egoera balio horiek kode pertsonalizatuarekin eguneratzen badira.

## <a name="time-and-material-billing-backlog"></a>Denbora eta materialen fakturazioaren lana

Ikuspegi honek sistemako proiektuen kontratu guztietan fakturatu ez diren fakturatu gabeko salmenten faktore guztiak zerrendatzen ditu. Fakturatu gabeko salmenta bakarraren edo anitzen benetako datu gisa markatu daitezke **Fakturatzeko prest** edo **Ez dago fakturatzeko prest** ikuspegi honetatik. Fakturarik gabeko salmenten gisa markatzen da **Fakturatzeko prest** eskuragarri jartzen du faktura zirriborroan jartzeko.

A duten fakturatutako salmenten benetakoak **Ez gainditzeko** egoera **Huts egin du** ezin da gisa markatu **Fakturatzeko prest**. Benetako hauek horrela markatu behar badira, berrezarri konpromisoa hartu duten kontratuaren lineako beste benetako egoera, eta gero ebaluatu **Ez gainditzeko** egoera.

Denbora eta materialen fakturazio metodoa duten bezero anitzeko kontratu lerroen kasuan, denbora eta gastuak onartzen direnean, fakturatu gabeko salmenta erreal bat sortzen da kontratu lerroan bezero bakoitzarentzat, bezero bakoitzerako zehaztutako fakturazio ehunekoaren arabera. kontratu lerroa. **Denboraren eta materialaren fakturazio-zorroa** ikuspegian, bezeroaren berariazko fakturaziorik gabeko salmenta errealak ikusiko dituzu. Faktura gabeko salmenten benetako datuen erregistro horietako bakoitza honela markatu daiteke **Fakturatzeko prest** ikuspegi honetatik bereizita.

Fakturatu gabeko salmenten benetako datuak zirriborroaren mugarria erakusten da ikuspegi honetan **Fakturazio egoerarekin** **Bezeroaren faktura sortu da**. Faktura zirriborroa baieztatzen denean, erregistro honetako fakturazio egoera eguneratzen da **Bezeroaren faktura argitaratua**. Egoera horretan dagoenean, ez da gomendagarria egoera balio hori eguneratzea kode pertsonalizatua erabiliz. Proiektuaren eragiketek ez dute behar bezala funtzionatuko egoera balio horiek kode pertsonalizatuarekin eguneratzen direnean.
