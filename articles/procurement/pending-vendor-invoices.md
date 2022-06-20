---
title: Erosi hornituta ez dauden materialak edo erosketa-kategoriak zain dagoen saltzaileen faktura erabiliz
description: Artikulu honek zain dauden saltzaileen fakturak nola erregistratu azaltzen du.
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
# <a name="purchase-non-stocked-materials-or-procurement-categories-using-a-pending-vendor-invoice"></a>Erosi hornituta ez dauden materialak edo erosketa-kategoriak zain dagoen saltzaileen faktura erabiliz

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Enpresa batek hornituta ez dauden materialak edo kontratazio kategoriak proiektu baterako eskuratzen dituenez, kostuak berehala erregistratu daitezke proiektuaren aurka. 

Adibidez, Contoso Robotics US ekipoak berritzeko proiektua egiten ari da eta software lizentziak behar ditu. Lizentzia horiek hirugarrenen saltzaile batek eskuratzen ditu.  Dynamics 365 Finance erabiliz, Ordainketa-bulegoak saltzaileen zain dagoen faktura-dokumentua erregistratzen du eta lizentzia-kostuak zuzenean egozten dizkio ekipamenduak berritzeko proiektuaren aurka. 

> [!IMPORTANT]
> Artikulu honetan deskribatutako funtzionalitateak erabili aurretik, berrikusi eta aplikatu behar diren konfigurazioak. Informazio gehiagorako, ikus [Gaitu hornituta ez dauden materialak eta zain dauden saltzaileen fakturak](configure-materials-nonstocked.md) eta [Erabili erosketa-kategoriak proiektuko erosketa-aginduekin eta zain dauden saltzaileen fakturekin](configure-procurement-categories.md)

## <a name="post-a-project-related-pending-vendor-invoice"></a>Bidali proiektuari lotutako saltzailearen faktura zain 

Saltzailearen fakturak zain daude **Saltzailearen fakturak zain** orrialdea (**Ordaintzeko kontuak** > **Fakturak** > **Saltzailearen fakturak zain**). Bete urrats hauek proiektuari lotutako saltzailearen faktura pendiente bat bidaltzeko:

1. Joan **Ordaintzeko kontuak** > **Fakturak**, eta hautatu **Berria**. 
1. urtean **Faktura kontua** eremuan, hautatu hornitzaile bat eta, ondoren, atalean **Zenbakia** eremuan, idatzi saltzailearen fakturaren identifikazioa.
1. Gehitu lerro bat saltzaileen fakturan, eta gero, atalean **Elementu zenbakia** eremuan, hautatu hornitu gabeko elementua saltzaileari erositakoa. Bestela, en **Kontratazio kategoria** eremuan, hautatu hornitzaileari erositako erosketa-kategoria.   
1. Gehitu erositako kantitatea. Sistemak unitateko prezioa betetzen du, salgai ez dagoen elementuaren prezioaren konfigurazioan oinarrituta. 
1. Egiaztatu zenbateko osoa eta beharrezko gainerako xehetasunak linean.
1. Lerroaren xehetasunetan, aldean **Proiektua** fitxan, hautatu elementu hau grabatuko den proiektuaren IDa.
1. Aukerakoa: hautatu jarduera-zenbakia eta eguneratu proiektuaren kategoria eta lerro-propietatea.
1. Argitaratu zain dagoen saltzaileen faktura. Faktura argitaratzen denean, sistemak informazio hau erregistratzen du:
    
    - Saltzailearen saldoaren zenbatekoa.
    - Salmenten zergen zenbatekoa.
    - Proiektuaren kostua kontratazioen integrazio kontuan erregistratzen da.
    - Urtean proiektuaren kostu transakzioa Dataverse-n.  Transakzio hau gehiago prozesatzen da [Project Operations integrazio-aldizkaria](../project-accounting/project-operations-integration-journal.md) erabiliz. Aldizkari hau argitaratzeak zenbatekoa kontratazioen integrazio kontutik proiektuaren kostu kontura mugitzen du. 
    - Proiektuaren bezeroari fakturatutako erosketak denbora eta materialen fakturazio metodoa erabiliz. Gainera, fakturatu gabeko salmenta transakzioak sortzen dira hemengo erosketetarako Dataverse-n. Produktuaren prezioen zerrenda Dataverse-n salmenta prezioetarako eta fakturatu gabeko salmenta eragiketetarako zenbatekoetarako erabiltzen da.
