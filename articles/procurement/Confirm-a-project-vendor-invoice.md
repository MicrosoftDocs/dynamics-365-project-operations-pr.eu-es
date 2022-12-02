---
title: Berretsi proiektuaren saltzailearen fakturak
description: Artikulu honek proiektuko saltzaileen faktura nola bertan berretsi azaltzen du Microsoft Dynamics 365 Project Operations eta proiektuaren hornitzaileen faktura berrestearen uztearen eragin ekonomikoa azaltzen du.
author: suvaidya
ms.date: 8/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: suvaidya
ms.openlocfilehash: 9739b15753aa34c51a0aa1e6dfeb7f590655ca7a
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475457"
---
# <a name="confirm-project-vendor-invoices"></a>Berretsi proiektuaren saltzailearen fakturak

**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations

**PM-ren eskuzko berrespena beharrezkoa da** parametroa gaituta dago, bertan sortzen diren saltzaileen fakturak Microsoft Dataverse izan **Zirriborroa** egoera. Horrela sortzen diren saltzaileen fakturak berrikusi eta eskuz berretsi behar dira. **PM-ren eskuzko berrespena beharrezkoa da** parametroa desgaituta dago, bertan sortzen diren saltzaileen fakturak Dataverse izan Zirriborroa egoera. Ez da ekintza gehiago behar. 

Dynamics 365 Project Operations-en hornitzaile-faktura bateko lerro guztiak egiaztatu ondoren , **Berretsi** ekintza erabil dezakezu saltzaileen faktura berresteko.

Hautatzen duzunean **berretsi** Saltzaileen fakturan, portaera hau gertatzen da:

1. Horra eguneratzen da hornitzailearen fakturaren egoera **berretsita**.
1. Berretsitako hornitzailearen faktura eta haiei lotutako erregistroak irakurtzeko soilik bihurtzen dira, eta ezin dira editatu edo ezabatu.
1. Kostu errealen batek hornitzaileen faktura-lerroari erreferentzia egiten badio bat-etortze-prozesuaren zati gisa, erreferentziatutako saltzaileen faktura-lerroarekin erlazionatutako kostu erreal guztiak alderantzikatu egiten dira.
1. Kostu erreal berriak hornitzaileen faktura lerroko informazioa erabiliz sortzen dira.
1. Berriro ere sor ditzakezu zuzenketa-aldizkariak, denbora-sarrerak gogorarazpenak prozesatu eta jatorrizko denboraren, gastuen edo material errealen onarpena bertan behera utzi.
1. Dynamics 365 Finance-n, **proiektuaren kostua** balioa Proiektuaren integrazio aldizkaria erabiliz eguneratzen da, eta Kontratazioen integrazio kontua *alderantziz* Proiektua integratzeko aldizkaria argitaratu ondoren.

> [!NOTE]
> Saltzaile-faktura bateko lerro guztiek **osatuta** ez den egiaztapen-egoera dutenean, saltzaile-faktura berretsi daiteke.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
