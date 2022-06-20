---
title: Saltzaileen fakturen integrazioa
description: Artikulu honetan, hornitzailearen fakturak proiektu-eragiketetan integratzeari buruzko informazioa ematen da.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d1e41638b6fe827e9e577860a78a84a9948053e4
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912041"
---
# <a name="vendor-invoice-integration"></a>Saltzaileen fakturen integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuarekin lotutako kontratazioa Dynamics 365 Project Operations ra joan daiteke **Ordaintzeko kontuak** > **Fakturak** > **Saltzailearen fakturak zain** eta zain dagoen saltzailearen faktura dokumentua erabiliz. Informazio gehiagorako, ikusi [Erosi ez dauden materialak saltzailearen faktura pendiente baten bidez](../procurement/pending-vendor-invoices.md).

> [!IMPORTANT]
> Artikulu honetan deskribatutako funtzionalitateak erabili aurretik, berrikusi eta aplikatu behar diren konfigurazioak. Informazio gehiagorako, ikusi [Gaitu ez dauden materialak eta saltzailearen faktura pendienteak](../procurement/configure-materials-nonstocked.md).

Project Operations-en, proiektuari lotutako saltzaileen fakturak argitaratzeko arau bereziak erabiliz argitaratzen dira:

- Proiektuarekin lotutako kostua (berreskuraezina den zerga barne) ez da berehala kontabilitate proiektuan liburu nagusian. Horren ordez, kostua **Kontratazioen integrazio kontua**. **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** aukeran dago konfiguratuta kontua **Dynamics 365 Customer Engagement-en Project Operations** fitxan.
- Idazketa bikoitzak saltzailearen fakturen datuak sinkronizatzen ditu Microsoft Dataverse taula taula hauek erabiliz:

     - **Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices)**: Taula mapa honek saltzailearen fakturen goiburuko informazioa sinkronizatzen du. Proiektuaren IDa duen gutxienez lerro bat duten saltzaileen fakturak soilik sinkronizatzen dira Dataverse.
     - **Project Operations integrazioa proiektuaren saltzailearen fakturen lerroa esportatzeko entitatea (msdyn_projectvendorinvoicelines)**: Taula mapa honek saltzailearen fakturen lerroko informazioa sinkronizatzen du. Proiektuaren IDa duten lerroak soilik sinkronizatzen dira Dataverse.

     > [!NOTE]
     > Saltzailearen faktura xehetasunak hemen Dataverse ez dira editagarriak.

Zergen sublibrotea, hornitzailearen sublibrotea eta beste finantza-kontabilizazio batzuk Dynamics 365 Finance-n aplikagarri gisa erregistratzen dira, hornitzailearen faktura kontabiltzen denean.

![Saltzaileen fakturen integrazioa.](media/DW7VendorInvoice.png)

Erregistroak a-ra idazten direnean **Saltzailearen faktura** entitatea Dataverse-n, erregistroen onespen prozesu automatikoa hasten da. Behar izanez gero, onartutako prozesuen egoera automatikoa berrikusi daiteke Dataverse-n, **Ezarpen aurreratuak** > **Sistema** > **Sistemako lanak** aukerara joanda. Onarpena amaitu ondoren, sistemak transakzio materialen erregistroak sortzen ditu **Benetako datuak** entitatea.

Materialarekin lotutako errealitateak idazketa bikoitzeko taulako mapa erabiliz prozesatzen dira, **Project Operations-en integrazioaren benetako datuak (msdyn_actuals)**. Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md).

Aldizkako prozesua, **Inportatu eszenaratzetik** saltzailearen fakturarekin lotutako Project Operations integrazioko egunkari lerroak sortzen ditu. Desplazatutako kontuak lehenespenez kontratazio integrazio kontua. Integrazio egunkaria argitaratzen denean, saltzailearen faktura transakzioaren kontuaren saldoa garbituko da eta lerroaren zenbatekoa proiektuaren kostu kontura eramango da. Proiektuen azpiegituren transakzioak fakturazio downstream eta diru-sarrerak ezagutzeko helburuetarako ere sortzen dira.
