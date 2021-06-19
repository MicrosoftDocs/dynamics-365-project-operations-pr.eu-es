---
title: Saltzaileen fakturen integrazioa
description: Gai honek saltzaileen fakturen integrazioaren inguruko informazioa eskaintzen du Project Operations-en.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d4f1b0ad94b71dc4adc5b2b3423340c5fdb171eb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002235"
---
# <a name="vendor-invoice-integration"></a>Saltzaileen fakturen integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuarekin lotutako kontratazioa Dynamics 365 Project Operations ra joan daiteke **Ordaintzeko kontuak** > **Fakturak** > **Saltzailearen fakturak zain** eta zain dagoen saltzailearen faktura dokumentua erabiliz. Informazio gehiagorako, ikusi [Erosi ez dauden materialak saltzailearen faktura pendiente baten bidez](../procurement/pending-vendor-invoices.md).

> [!IMPORTANT]
> Gai honetan azaldutako funtzionalitatea erabili aurretik, berrikusi eta aplikatu beharrezko konfigurazioak. Informazio gehiagorako, ikusi [Gaitu ez dauden materialak eta saltzailearen faktura pendienteak](../procurement/configure-materials-nonstocked.md).

Project Operations-en, proiektuari lotutako saltzaileen fakturak argitaratzeko arau bereziak erabiliz argitaratzen dira:

- Proiektuarekin lotutako kostua (berreskuraezina den zerga barne) ez da berehala kontabilitate proiektuan liburu nagusian. Horren ordez, kostua **Kontratazioen integrazio kontua**. **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** aukeran dago konfiguratuta kontua **Dynamics 365 Customer Engagement-en Project Operations** fitxan.
- Idazketa bikoitzak saltzailearen fakturen datuak sinkronizatzen ditu Microsoft Dataverse taula taula hauek erabiliz:

     - **Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices)**: Taula mapa honek saltzailearen fakturen goiburuko informazioa sinkronizatzen du. Proiektuaren IDa duen gutxienez lerro bat duten saltzaileen fakturak soilik sinkronizatzen dira Dataverse.
     - **Project Operations integrazioa proiektuaren saltzailearen fakturen lerroa esportatzeko entitatea (msdyn_projectvendorinvoicelines)**: Taula mapa honek saltzailearen fakturen lerroko informazioa sinkronizatzen du. Proiektuaren IDa duten lerroak soilik sinkronizatzen dira Dataverse.

     > [!NOTE]
     > Saltzailearen faktura xehetasunak hemen Dataverse ez dira editagarriak.

Zerga azpiegitura, saltzailearen azpiegitura eta bestelako finantza bidalketak hemen aplikatzen diren moduan erregistratzen dira Dynamics 365 Finance saltzailearen faktura argitaratzen denean.

![Saltzaileen fakturen integrazioa](media/DW7VendorInvoice.png)

Erregistroak a-ra idazten direnean **Saltzailearen faktura** entitatea Dataverse-n, erregistroen onespen prozesu automatikoa hasten da. Behar izanez gero, onartutako prozesuen egoera automatikoa berrikusi daiteke Dataverse-n, **Ezarpen aurreratuak** > **Sistema** > **Sistemako lanak** aukerara joanda. Onarpena amaitu ondoren, sistemak transakzio materialen erregistroak sortzen ditu **Benetako datuak** entitatea.

Materialarekin lotutako errealitateak idazketa bikoitzeko taulako mapa erabiliz prozesatzen dira, **Project Operations-en integrazioaren benetako datuak (msdyn_actuals)**. Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md).

Aldizkako prozesua, **Inportatu eszenaratzetik** saltzailearen fakturarekin lotutako Project Operations integrazioko egunkari lerroak sortzen ditu. Desplazatutako kontuak lehenespenez kontratazio integrazio kontua. Integrazio egunkaria argitaratzen denean, saltzailearen faktura transakzioaren kontuaren saldoa garbituko da eta lerroaren zenbatekoa proiektuaren kostu kontura eramango da. Proiektuen azpiegituren transakzioak fakturazio downstream eta diru-sarrerak ezagutzeko helburuetarako ere sortzen dira.
