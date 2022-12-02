---
title: Erosi izakinik gabeko materialak edo kontratazio kategoriak ordaindu gabeko saltzaileen faktura bat erabiliz
description: Gai honetan azaltzen diren saltzaileen fakturak nola grabatu azaltzen da.
author: sigitac
ms.date: 09/13/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: b1c05755f6759e90e031a11261f15a2c4b6b716e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921977"
---
# <a name="purchase-non-stocked-materials-or-procurement-categories-using-a-pending-vendor-invoice"></a>Erosi izakinik gabeko materialak edo kontratazio kategoriak ordaindu gabeko saltzaileen faktura bat erabiliz

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Enpresa batek material baterako material edo kontratazio kategoriak ez hornituak proiektu baterako, kostuak berehala erregistratu daitezke proiektuaren aurka. 

Adibidez, Contoso Robotics US ekipoak berritzeko proiektua egiten ari da eta software lizentziak behar ditu. Lizentzia horiek hirugarrenen saltzaile batek eskuratzen ditu.  Dynamics 365 Finance erabiliz, Ordaintzeko kontuetako idazkariak saltzailearen faktura dokumentu bat erregistratzen du eta lizentziaren kostuak ekipamendua berritzeko proiektuari zuzenean egozten dizkio. 

> [!IMPORTANT]
> Gai honetan azaldutako funtzionalitatea erabili aurretik, berrikusi eta aplikatu beharrezko konfigurazioak. Informazio gehiagorako, ikus [Gaitu hornituta ez dauden materialak eta zain dauden saltzaileen fakturak](configure-materials-nonstocked.md) eta [Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin](configure-procurement-categories.md)

## <a name="post-a-project-related-pending-vendor-invoice"></a>Bidali proiektuari lotutako saltzailearen faktura zain 

Saltzailearen fakturak zain daude **Saltzailearen fakturak zain** orrialdea (**Ordaintzeko kontuak** > **Fakturak** > **Saltzailearen fakturak zain**). Bete urrats hauek proiektuari lotutako saltzailearen faktura pendiente bat bidaltzeko:

1. Joan **Ordaintzeko kontuak** > **Fakturak** aukerara eta hautatu **Berria**. 
1. **Faktura kontua** eremuan, hautatu saltzailea eta **Zenbakia** eremuan, sartu saltzailearen faktura identifikazioa.
1. Gehitu lerro bat saltzailearen fakturan eta **Elementuaren zenbakia** eremuan, hautatu saltzailearengandik erositako stockik gabeko elementua. Bestela, **Kontratazio kategoria** eremuan, hautatu hornitzaileari erositako erosketa-kategoria.   
1. Gehitu erositako kantitatea. Sistemak unitateko prezioa beteko du hornitu gabeko elementuen prezioaren konfigurazioan oinarrituta. 
1. Egiaztatu zenbateko osoa eta beharrezko gainerako xehetasunak linean.
1. Linearen xehetasunetan, **Proiektua** fitxan, hautatu elementu hau grabatuko den proiektuaren IDa.
1. Aukeran, hautatu jardueraren zenbakia eta eguneratu proiektuaren kategoria eta lerroaren propietatea.
1. Bidali zain dagoen saltzailearen faktura. Sistemak fakturaren egutegia sortzen du eremuko informazio honekin:
    
    - Saltzailearen saldoaren zenbatekoa.
    - Salmenten zergen zenbatekoa.
    - Proiektuaren kostua kontratazioen integrazio kontuan erregistratzen da.
    - Urtean proiektuaren kostu transakzioa Dataverse-n.  Transakzio hau gehiago prozesatzen da [Project Operations integrazio-aldizkaria](../project-accounting/project-operations-integration-journal.md) erabiliz. Aldizkari hau argitaratzeak zenbatekoa kontratazioen integrazio kontutik proiektuaren kostu kontura mugitzen du. 
    - Proiektuaren bezeroari fakturatutako erosketak denbora eta materialen fakturazio metodoa erabiliz. Gainera, fakturatu gabeko salmenta transakzioak sortzen dira hemengo erosketetarako Dataverse-n. Produktuaren prezioen zerrenda Dataverse-n salmenta prezioetarako eta fakturatu gabeko salmenta eragiketetarako zenbatekoetarako erabiltzen da.
