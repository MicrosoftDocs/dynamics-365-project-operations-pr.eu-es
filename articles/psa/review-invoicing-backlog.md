---
title: Berrikusi proiektuen eta proiektuen kontratuen fakturazioaren lana
description: Artikulu honek denbora, gastu eta produktuen atzerapenak berrikusi eta fakturatzeko prest gisa markatzeko moduari buruzko informazioa eskaintzen du.
author: rumant
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 833ace7fd6285191f4b023a029286cd36b5de8f4
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928877"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a>Berrikusi proiektuen eta proiektuen kontratuen fakturazioaren lana

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Transakzioa faktura sortzeko eta prozesatzeko prest dagoenean, transakzioa **Fakturatzeko prest** gisa markatu beharko litzateke. Artikulu honek sor daitezkeen transakzio motak deskribatzen ditu.

## <a name="review-the-time-and-material-billing-backlog"></a>Berrikusi denbora eta materialen fakturazioaren lana

Proiektu baterako denbora edo gastu sarrera bat bidaltzen eta onartzen denean, PSA-k proiektu bat sortzen du. Proiektuaren eta transakzioen klasearen konbinazioa denbora eta materialen proiektu baterako kontratuaren lerro bati esleitzen bazaio, sarrera onartzean benetako bi datu sortzen dira:

- Benetako kostua 
- Fakturatu gabeko benetako salmentak

Fakturatu gabeko benetako salmentek fakturazioaren lana adierazten du eta fakturazio-egoera **Fakturatzeko prest** egon behar da. Proiektuaren faktura sortzen denean, **Fakturatzeko prest** gisa markatuta dauden fakturatu gabeko benetako salmentak fakturen lerroko xehetasun gisa kopiatzen dira.

Denbora eta materialei dagokien fakturazioaren lana ikusteko, joan **Salmentak** \> **Fakturazioa** \> **Denboraren eta materialaren fakturazioaren atala**. Hautatu fakturatzeko prest dauden fakturatu gabeko benetako salmenta guztiak eta, ondoren, hautatu **Fakturatzeko prest**. Datu erreal horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.

![Denbora eta materialen fakturazioaren lana.](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a>Berrikusi produktuaren fakturazioaren lana

PSA-n, proiektuko kontratuak produktuetan oinarritutako kontratuaren lerroak dituenean, lerro horiek fakturaziorako kontsideratzen dira proiektuaren kontratuaren faktura sortzen den bakoitzean. **Fakturatzeko prest** gisa markatuta dauden kontratuaren lerroak dituen edozein produktu proiektuaren fakturan kopiatzen da proiektuaren faktura-lerro gisa.

Produktuen fakturazio lana berrikusteko, joan **Salmentak** \> **Fakturazioa** \> **Produktuen fakturazioaren lana** aukerara. Hautatu fakturatzeko prest dauden produktuan oinarritutako kontratuaren lerro guztiak eta, ondoren, hautatu **Fakturatzeko prest**. Lerro horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.

![Produktuaren fakturazioaren lana.](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a>Berrikusi prezio finkoko kontratuen mugarriak

Prezio finkoko fakturazio-metodoa duen proiektuaren kontratuaren lerro bakoitzak zehaztu beharko ditu kontratuaren mugarriak. Kontratuaren mugarriak horiek **Fakturatzeko prest** gisa markatuta daudenean soilik fakturatu daitezke. 

Fakturazio-mugarriak berrikusteko, joan **Salmentak** \> **Fakturazioa** \> **Prezio finkoen mugarriak** atalera. Hautatu fakturatzeko prest dauden mugarriak eta, ondoren, hautatu **Fakturatzeko prest**. Mugarri horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.

![Prezio finkoaren mugarriak.](media/FPBacklog.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
