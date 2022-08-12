---
title: Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin
description: Artikulu honek proiektuko erosketa-aginduekin eta saltzaileen zain dauden fakturekin erabil daitezkeen kontratazio-kategoriak nola konfiguratu deskribatzen du.
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

Erosketa profesionalek proiektuko erosketa-aginduetan eta saltzaileen zain dauden fakturetan erabil daitezkeen elementu eta zerbitzuen katalogoak sortu eta mantendu ditzakete. [Kontratazio katalogoak](/dynamics365/supply-chain/procurement/procurement-catalogs) erosketak sailkatzeko modu erraz bat emango dizu kaleratutako produktuen katalogoa konfiguratu eta erabili beharrik gabe. Kontratazio-kategoria bakoitza proiektu-kategoria batera eslei daiteke denbora, gastu edo elementuen transakzioetarako. Kontratazio-kategoria erabiltzen duen hornitzaileen zain dagoen faktura bat argitaratu ondoren, sistemak denbora, gastu edo material-proiektuaren benetako datuak, proiektu-transakzioak eta azpiliburuko sarrerak sortuko ditu.

## <a name="minimum-version-requirements"></a>Gutxieneko bertsio-eskakizunak

Microsoft-en proiektuko erosketa-aginduekin kontratazio-kategoriak erabiltzeko hurrengo bertsioak behar dira Dynamics 365 Project Operations hornitu gabeko/baliabideetan oinarritutako eszenatokiak:

- Proiektuaren Eragiketak Dataverse irtenbide-bertsioa 4.41.0.45 edo geroago
- Finantza eta eragiketen ingurunea 10.0.26 bertsioa edo berriagoa

## <a name="run-dual-write-maps-for-procurement-category-support"></a>Exekutatu idazketa bikoitzeko mapak kontratazio kategorien laguntzarako

Ziurtatu mapak egiteko **Project Operations integrazio proiektua hornitzaile faktura lerro esportatzeko entitatea msdyn\_ proiektuenhornitzailefakturalerroak** 1.0.0.4 edo ondorengo bertsioa erabiltzen du.

## <a name="enable-the-feature-key-for-procurement-categories"></a>Gaitu erosketa kategorietarako eginbide-gakoa

Jarraitu urrats hauek proiektuko erosketa-eskaerekin kontratazio-kategoriak erabiltzeko funtzionaltasuna gaitzeko.

1. Dynamics 365 Finance atalean, ireki **Ezaugarrien kudeaketa** lan-eremua.
1. Ezaugarrien zerrendan, bilatu **Erabili kontratazio-kategoriak Proiektu-eragiketetan baliabideetan oinarritutako/hornituta ez dauden agertokietarako** eginbidea eta, ondoren, hautatu **Gaitu**.

> [!IMPORTANT]
> Aurrebaldintza gisa, ere gaitu behar duzu **Gaitu zain dauden saltzaileen fakturak Project Operations-en baliabideetan oinarritutako edo hornituta ez dauden agertokietarako** ezaugarria.

## <a name="map-project-categories-in-the-procurement-category-hierarchy"></a>Mapeatu proiektuen kategoriak Kontratazio kategorien hierarkian

Jarraitu urrats hauek proiektuen kategoriak kontratazio kategoriekin mapatzeko **Kontratazio kategoria** hierarkia:

1. Joan **Kontratazioa eta hornidura \> Kontratazio kategoriak**.
1. Hautatu **Editatu kategorien hierarkia**.
1. Hautatu nahi duzun kategoriaren hierarkia-nodoa, eta, ondoren, atalean **Proiektuen kategoriak esleitu** fitxan, lotu nodoa proiektuaren kategoriarekin **Denbora**, **·**, edo, **Item Proiektua** kategoria (hau da **Lehenetsitako ordua** edo **Lehenetsia-Gastuak** kategoria).
1. Sakatu **Gorde**.
1. Itxi orria.

> [!NOTE]
> Kontratazio-kategoria bat proiektu-kategoria batekin mapatzea aukerakoa da. Kontratazio-kategoria bat mapatzen ez bada, sistemak atalean ezarritako balioa erabiliko du **Elementua** eremuan **Proiektuaren kategoria lehenetsiak** atala **Project Operations on Dynamics 365 bezeroen konpromisoa** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.