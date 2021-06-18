---
title: Erosi izakinik gabeko materialak ordaindu gabeko saltzaileen faktura bat erabiliz
description: Gai honetan azaltzen diren saltzaileen fakturak nola grabatu azaltzen da.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b5e6632d73c8a211b1f0d568be8e10ef47be77e2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993763"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a>Erosi izakinik gabeko materialak ordaindu gabeko saltzaileen faktura bat erabiliz

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Enpresa batek material baterako material ez hornituak proiektu baterako, kostuak berehala erregistratu daitezke proiektuaren aurka. 

Adibidez, Contoso Robotics US ekipoak berritzeko proiektu bat egiten ari da eta software lizentziak behar ditu. Lizentzia horiek hirugarrenen saltzaile batek eskuratzen ditu.  Dynamics 365 Finance erabiliz, Ordaintzeko kontuetako idazkariak saltzailearen faktura dokumentu bat erregistratzen du eta lizentziaren kostuak ekipamendua berritzeko proiektuari zuzenean egozten dizkio. 

> [!IMPORTANT]
> Gai honetan azaldutako funtzionalitatea erabili aurretik, berrikusi eta aplikatu beharrezko konfigurazioak. Informazio gehiagorako, ikusi [Gaitu ez dauden materialak eta saltzailearen faktura pendienteak](configure-materials-nonstocked.md). 

## <a name="post-a-project-related-pending-vendor-invoice"></a>Bidali proiektuari lotutako saltzailearen faktura zain 

Saltzailearen fakturak zain daude **Saltzailearen fakturak zain** orrialdea (**Ordaintzeko kontuak** > **Fakturak** > **Saltzailearen fakturak zain**). Bete urrats hauek proiektuari lotutako saltzailearen faktura pendiente bat bidaltzeko:

1. Joan **Ordaintzeko kontuak** > **Fakturak** aukerara eta hautatu **Berria**. 
2. **Faktura kontua** eremuan, hautatu saltzailea eta **Zenbakia** eremuan, sartu saltzailearen faktura identifikazioa.
3. Gehitu lerro bat saltzailearen fakturan eta **Elementuaren zenbakia** eremuan, hautatu saltzailearengandik erositako stockik gabeko elementua. 

    > [!NOTE]
    > Kontratazio kategoria batean oinarritutako saltzaileen faktura lerroak ezin dira proiektuaren aurka erregistratu. 
    
5. Gehitu erositako kantitatea. Sistemak unitateko prezioa beteko du hornitu gabeko elementuen prezioaren konfigurazioan oinarrituta. 
6. Egiaztatu zenbateko osoa eta beharrezko gainerako xehetasunak linean.
7. Linearen xehetasunetan, **Proiektua** fitxan, hautatu elementu hau grabatuko den proiektuaren IDa.
8. Aukeran, hautatu jardueraren zenbakia eta eguneratu proiektuaren kategoria eta lerroaren propietatea.
9. Bidali zain dagoen saltzailearen faktura. Faktura argitaratzen denean, sistemak erregistratzen du:
    
    - Saltzailearen saldoaren zenbatekoa.
    - Salmenten zergen zenbatekoa.
    - Proiektuaren kostua kontratazioen integrazio kontuan erregistratzen da.
    - Proiektuaren benetako transakzioa Dataverse-n. Transakzio hau gehiago prozesatzen da [Project Operations integrazio-aldizkaria](../project-accounting/project-operations-integration-journal.md) erabiliz. Aldizkari hau argitaratzeak zenbatekoa kontratazioen integrazio kontutik proiektuaren kostu kontura mugitzen du.
