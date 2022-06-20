---
title: Berretsi proiektuaren saltzailearen faktura
description: Artikulu honetan azaltzen da nola baieztatu proiektu-hornitzailearen faktura bat Microsoften Dynamics 365 Project Operations eta proiektuaren hornitzailearen faktura bat baieztatzeak duen finantza-inpaktua.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 092b3cd5981f7d9bb8767c7a2acb2f4952801d06
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8932419"
---
# <a name="confirm-a-project-vendor-invoice"></a>Berretsi proiektuaren saltzailearen faktura

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Microsoften Dynamics 365 Project Operations hornitzaile-faktura baten linea guztiak egiaztatu ondoren, Confirmar ekintza erabil dezakezu hornitzailearen faktura baieztatzeko.

**Hornitzaile-faktura batean baieztatzean**, honako portaera hau gertatzen da:

1. Hornitzailearen fakturaren egoera berretsi egiten **da**.
2. Baieztatutako hornitzailearen faktura eta horiekin lotutako erregistroak irakurketa bakarrekoak izango dira, eta ezin dira editatu, ezta ezabatu ere.
3. Kostu errealen batek hornitzailearen faktura-lerroari egiten badio erreferentzia, kointzidentzia-prozesuaren zati gisa, erreferentzia egiten zaion hornitzailearen faktura-lerroarekin lotutako kostuen datu erreal guztiak inbertitzen dira.
4. Kostuen datu erreal berriak hornitzailearen faktura-lerroaren informazioa erabiliz sortzen dira.
5. Hornitzailearen faktura berretsi ondoren, ezin du zuzenketa-egunkaririk sortu, denbora-sarreraren berreskurapenak prozesatu, ez eta inbertitutako material originalen denbora, gastua edo benetako datuak bertan behera utzi ere.

> [!NOTE]
> Hornitzaile-faktura baten linearen batek egiaztapen-egoera **osatua ez bada**, hornitzailearen faktura ezin da baieztatu.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
