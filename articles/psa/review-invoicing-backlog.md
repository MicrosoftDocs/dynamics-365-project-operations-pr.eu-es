---
title: Berrikusi proiektuen eta proiektuen kontratuen fakturazioaren lana
description: Gai honek denbora, gastua eta produktuen atzerapenak nola berrikusi eta fakturaziorako prest daudela markatzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom: ''
ms.author: rumant
ms.date: 03/11/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 092455a131f556e4f943f6bb89d7e38358f0a697
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150473"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a>Berrikusi proiektuen eta proiektuen kontratuen fakturazioaren lana

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Transakzioa faktura sortzeko eta prozesatzeko prest dagoenean, transakzioa **Fakturatzeko prest** gisa markatu beharko litzateke. Gai honetan sortu daitezkeen transakzio motak deskribatzen dira.

## <a name="review-the-time-and-material-billing-backlog"></a>Berrikusi denbora eta materialen fakturazioaren lana

Proiektu baterako denbora edo gastu sarrera bat bidaltzen eta onartzen denean, PSA-k proiektu bat sortzen du. Proiektuaren eta transakzioen klasearen konbinazioa denbora eta materialen proiektu baterako kontratuaren lerro bati esleitzen bazaio, sarrera onartzean benetako bi datu sortzen dira:

- Benetako kostua 
- Fakturatu gabeko benetako salmentak

Fakturatu gabeko benetako salmentek fakturazioaren lana adierazten du eta fakturazio-egoera **Fakturatzeko prest** egon behar da. Proiektuaren faktura sortzen denean, **Fakturatzeko prest** gisa markatuta dauden fakturatu gabeko benetako salmentak fakturen lerroko xehetasun gisa kopiatzen dira.

Denbora eta materialei dagokien fakturazioaren lana ikusteko, joan **Salmentak** \> **Fakturazioa** \> **Denboraren eta materialaren fakturazioaren atala**. Hautatu fakturatzeko prest dauden fakturatu gabeko benetako salmenta guztiak eta, ondoren, hautatu **Fakturatzeko prest**. Datu erreal horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.

![Denbora eta materialen fakturazioaren lana](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a>Berrikusi produktuaren fakturazioaren lana

PSA-n, proiektuko kontratuak produktuetan oinarritutako kontratuaren lerroak dituenean, lerro horiek fakturaziorako kontsideratzen dira proiektuaren kontratuaren faktura sortzen den bakoitzean. **Fakturatzeko prest** gisa markatuta dauden kontratuaren lerroak dituen edozein produktu proiektuaren fakturan kopiatzen da proiektuaren faktura-lerro gisa.

Produktuen fakturazio lana berrikusteko, joan **Salmentak** \> **Fakturazioa** \> **Produktuen fakturazioaren lana** aukerara. Hautatu fakturatzeko prest dauden produktuan oinarritutako kontratuaren lerro guztiak eta, ondoren, hautatu **Fakturatzeko prest**. Lerro horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.

![Produktuaren fakturazioaren lana](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a>Berrikusi prezio finkoko kontratuen mugarriak

Prezio finkoko fakturazio-metodoa duen proiektuaren kontratuaren lerro bakoitzak zehaztu beharko ditu kontratuaren mugarriak. Kontratuaren mugarriak horiek **Fakturatzeko prest** gisa markatuta daudenean soilik fakturatu daitezke. 

Fakturazio-mugarriak berrikusteko, joan **Salmentak** \> **Fakturazioa** \> **Prezio finkoen mugarriak** atalera. Hautatu fakturatzeko prest dauden mugarriak eta, ondoren, hautatu **Fakturatzeko prest**. Mugarri horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.

![Prezio finkoaren mugarriak](media/FPBacklog.png)
