---
title: Erosketa-kategoriak erabili proiektuak erosteko aginduekin eta hornitzaileen fakturekin
description: Artikulu honetan, proiektuak erosteko eskariekin eta oraindik hornitzaileen fakturekin erabil daitezkeen erosketa-kategoriak nola konfiguratu azaltzen da.
author: sigitac
ms.date: 04/07/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 7d774631a4712de9b29ddedfee2ea3fc4a2d436f
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927405"
---
# <a name="use-procurement-categories-with-project-purchase-orders-and-pending-vendor-invoices"></a>Erosketa-kategoriak erabili proiektuak erosteko aginduekin eta hornitzaileen fakturekin

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Erosketa-profesionalek proiektuak erosteko aginduetan eta hornitzaileek ordaintzeke dauden fakturetan erabil daitezkeen artikulu eta zerbitzuen katalogoak sortu eta mantendu ditzakete. [Erosketa-katalogoek](/dynamics365/supply-chain/procurement/procurement-catalogs) erraz eskaintzen diote erosketak kategorizatzeko, argitaratutako produktuen katalogo bat konfiguratu eta erabili behar izan gabe. Erosketa-kategoria bakoitza proiektu-kategoria bati esleitu ahal zaio, denbora-transakzioetarako, gastuetarako edo artikuluetarako. Eskuratze-kategoria bat erabiltzen duen hornitzaile-faktura bat kontabilizatu ondoren, sistemak denbora-proiektuen, gastuen edo materialen, proiektuen transakzioen eta sublibroen sarreren datu errealak sortuko ditu.

## <a name="minimum-version-requirements"></a>Gutxieneko bertsio-betekizunak

Honako bertsio hauek beharrezkoak dira Microsoften Dynamics 365 Project Operations baliabideetan biltegiratu gabeko/oinarririk gabeko agertokietarako proiektuak erosteko aginduak dituzten erosketa-kategoriak erabiltzeko:

- Project Operations-en Dataverse soluzioaren bertsioa 4.41.0.45 edo geroago
- Finance and Operations ingurua 10.0.26 bertsioa edo ondorengoa

## <a name="run-dual-write-maps-for-procurement-category-support"></a>Eskritura dualeko mapak egitea, erosketa-kategoriekin bateragarria izan dadin

Ziurtatu Project Operations msdyn **projectvendorinvoicelines integrazio-proiektuaren hornitzailearen faktura-lerroa esportatzeko erakundeak faktura-lerroa esleitzeak \_** 1.0.0.4 edo ondorengo bertsioa erabiltzen duela.

## <a name="enable-the-feature-key-for-procurement-categories"></a>Erosketa-kategorietarako ezaugarri-gakoa gaitzea

Jarraitu urrats horiek, proiektuak erosteko aginduak dituzten erosketa-kategoriak erabiltzeko funtzionaltasuna gaitzeko.

1. Dynamics 365 Finance-n, ezaugarriak dituen **administrazioaren lan-arloa** irekitzen du.
1. Ezaugarrien zerrendan, bilatu **proiektu-eragiketetan erosketa-kategoriak erabiltzea, biltegiratutako** baliabideetan oinarritutako agertokietarako, eta, ondoren, aukeratu **·**.

> [!IMPORTANT]
> Aldez aurretik, proiektu-eragiketetan hornitzailearen **fakturak gaitzea ere gaitu behar du, biltegiratu** gabeko baliabideetan oinarritutako agertokietarako.

## <a name="map-project-categories-in-the-procurement-category-hierarchy"></a>Proiektuen kategoriak esleitu Erosketak kategorien hierarkian

Jarraitu urrats horiek erosketa-kategorien hierarkian erosketa-kategoriei **proiektu-kategoriak** esleitzeko:

1. **Zoaz erosketa eta \> hornikuntza kategorietara**.
1. Hautatu **Kategorien** hierarkia.
1. Aukeratu nahi den kategorien hierarkia-nodoa, eta, ondoren, proiektu-kategoriak esleitu fitxatu **, nodoa proiektu-kategoriarekin lotu denbora** **,** gastu **edo elementu-proiektua** kategoriatik (hau da, **aurrez zehaztutako denbora** edo **aurrez zehaztutako gastua** kategoriatik **).**
1. Sakatu **Gorde**.
1. Itxi orria.

> [!NOTE]
> Proiektu-kategoria bati eskuratze-kategoria bat esleitzea aukerakoa da. Erosketa-kategoria bat esleitu ezean, sistemak proiektuen administrazio- eta kontabilitate-parametroen Dynamics 365 Customer Engagement **orriko proiektu-eragiketaren** proiektuaren kategoriako Balio aurrez zehaztuak **atalaren** **elementuan** **ezartzen den balioa erabiliko du.**
