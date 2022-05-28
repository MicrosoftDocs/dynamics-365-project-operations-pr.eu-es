---
title: Utzi proiektuko hornitzaileen faktura
description: Gai honek Microsoft-en proiektuko hornitzaileen faktura nola bertan behera utzi azaltzen du Dynamics 365 Project Operations eta proiektuaren hornitzaileen faktura bertan behera uztearen eragin ekonomikoa.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 87f6bdca30c5779e3d70922e75609ff4cdfca167
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580625"
---
# <a name="cancel-a-project-vendor-invoice"></a>Utzi proiektuko hornitzaileen faktura

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Saltzaileen faktura bat baieztatu ondoren, ezin da editatu edo ezabatu. Berretsitako saltzaile-faktura batean erroreren bat egon bazen, Utzi ekintza erabil dezakezu saltzaile-fakturaren eragina alderantzikatzeko eta hornitzaile-faktura berri bat sortzeko.

Hautatzen duzunean **Utzi** Saltzaileen fakturan, portaera hau gertatzen da:

1. Horra eguneratzen da hornitzailearen fakturaren egoera **Bertan behera utzita**.
2. Bertan behera utzitako hornitzailearen faktura eta haiei lotutako erregistroak irakurtzeko soilik bihurtzen dira, eta ezin dira editatu edo ezabatu.
3. Hornitzaileen fakturaren lerroetan oinarrituta sortu ziren kostu errealak saltzaileen fakturaren berrespenaren parte gisa alderantzikatu egiten dira.
4. Bat-etortze-prozesuaren zati gisa, kostu errealen bat hornitzaileen faktura-lerroekin lotzen bazen, jatorrizko hornitzailearen fakturaren berrespenak alderantzikatu zuen. Saltzaileen fakturak bertan behera uzten diren bitartean, kostu erreal horiek berriro sortzen dira. Jatorriek denbora, gastu edo material erabilerako sarrerak adierazten dituzte.
5. Saltzaileen faktura bertan behera utzi ondoren, berriro ere zuzenketa-aldizkariak sor ditzakezu, denbora-sarrerak gogorarazpenak prozesatu eta jatorrizko denboraren, gastuen edo material errealen onarpena bertan behera utzi.

> [!NOTE]
> Proiektuaren hornitzaileen fakturak soilik baliogabetu daitezke. Beste estatuetako saltzaileen fakturak ezin dira bertan behera utzi.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
