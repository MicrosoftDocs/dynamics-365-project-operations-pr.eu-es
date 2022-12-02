---
title: Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin
description: Artikulu honek proiektuko erosketa-aginduekin eta saltzaileen zain dauden fakturekin erabil daitezkeen erosketa-kategoriak nola konfiguratu deskribatzen du.
author: sigitac
ms.date: 04/07/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: f71c6bfcd183613471a4cc10e16a5a54571fac31
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028595"
---
# <a name="use-procurement-categories-with-project-purchase-orders-and-pending-vendor-invoices"></a>Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Erosketa profesionalek proiektuko erosketa-aginduetan eta saltzaileen zain dauden fakturetan erabil daitezkeen elementu eta zerbitzuen katalogoak sortu eta mantendu ditzakete. [Kontratazio katalogoak](/dynamics365/supply-chain/procurement/procurement-catalogs) erosketak sailkatzeko modu erraz bat emango dizu kaleratutako produktuen katalogoa konfiguratu eta erabili beharrik gabe. Kontratazio-kategoria bakoitza proiektu-kategoria batera eslei daiteke denbora, gastu edo elementuen transakzioetarako. Kontratazio-kategoria erabiltzen duen saltzaileen zain dagoen faktura bat argitaratu ondoren, sistemak denbora, gastu edo material-proiektuaren benetako datuak, proiektu-transakzioak eta liburu azpiko sarrerak sortuko ditu.

## <a name="minimum-version-requirements"></a>Bertsioaren gutxieneko eskakizunak

Proiektuko erosketa-aginduekin kontratazio-kategoriak erabiltzeko hurrengo bertsioak behar dira Microsoft Dynamics 365 Project Operations hornitu gabeko/baliabideetan oinarritutako eszenatokiak:

- Project Operations Dataverse irtenbide-bertsioa 4.41.0.45 edo geroago
- Finantza eta eragiketen ingurunea 10.0.26 bertsioa edo berriagoa

## <a name="run-dual-write-maps-for-procurement-category-support"></a>Exekutatu idazketa bikoitzeko mapak kontratazio kategorien laguntzarako

Ziurtatu **Project Operations integrazioa proiektuaren saltzailearen fakturen lerroa esportatzeko entitatea msdyn\_projectvendorinvoicelines** 1.0.0.4 bertsioa edo geroagokoa erabiltzen duela.

## <a name="enable-the-feature-key-for-procurement-categories"></a>Gaitu erosketa kategorietarako eginbide-gakoa

Jarraitu urrats hauek proiektuko erosketa-eskaerekin kontratazio-kategoriak erabiltzeko funtzionaltasuna gaitzeko.

1. Dynamics 365 Finance-n, ireki **Ezaugarrien kudeaketa** lan eremua.
1. Ezaugarrien zerrendan, bilatu **Gaitu Project Operations-en erabili prokurazio-kategoriak, baliabideetan oinarritutako / gordeta ez dauden eszenatokietarako** eginbidea eta hautatu **Gaitu**.

> [!IMPORTANT]
> Eskakizun gisa, gaitu behar duzu **Gaitu Project Operations-en saltzailearen fakturak zain, baliabideetan oinarritutako / gordeta ez dauden eszenatokietarako eginbidea**.

## <a name="map-project-categories-in-the-procurement-category-hierarchy"></a>Esleitu proiektuen kategoriak Kontratazio kategorien hierarkian

Jarraitu urrats hauek proiektuen kategoriak kontratazio kategoriekin mapatzeko **Kontratazio kategoria** hierarkia:

1. Joan **Kontratazioa eta hornidura \> Kontratazio kategoriak**.
1. Hautatu **Editatu kategorien hierarkia**.
1. Hautatu nahi duzun kategoriaren hierarkia-nodoa, eta, ondoren, atalean **Proiektuen kategoriak esleitu** fitxan, lotu nodoa proiektuaren kategoriarekin **Denbora**, **Gastua**, edo, **elementuaren Proiektua** kategoria (hau da **Lehenetsitako ordua** edo **Lehenetsia-Gastuak** kategoria).
1. Sakatu **Gorde**.
1. Itxi orria.

> [!NOTE]
> Kontratazio-kategoria bat proiektu-kategoria batekin mapatzea aukerakoa da. Kontratazio-kategoria ez badago esleituta, sistemak erabiliko du **elementua** eremua **proiektuaren kategoriaren lehenespenak** sekzioa **Project Operations Dynamics 365 Customer engagement** fitxan **Proiektuen kudeaketa eta kontabilitatea** orrian.
