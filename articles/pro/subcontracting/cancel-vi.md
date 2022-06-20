---
title: Utzi proiektuaren saltzailearen faktura
description: Artikulu honetan azaltzen da nola kitatu proiektu-hornitzailearen faktura bat Microsoften Dynamics 365 Project Operations eta proiektuaren hornitzailearen faktura bat kitatzeak duen finantza-inpaktua.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 7ddaadc0f6e336a8ba67bb4ad8000f7e894f3eb0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911535"
---
# <a name="cancel-a-project-vendor-invoice"></a>Utzi proiektuaren saltzailearen faktura

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Behin hornitzailearen faktura bat berretsita, ezin da editatu, ezta ezabatu ere. Hornitzailearen faktura batean akats bat baieztatu bada, Cancelar ekintza erabil dezakezu hornitzailearen fakturaren eragina iraultzeko eta hornitzailearen faktura berri bat sortzeko.

Hornitzaile-faktura batean Cancelar **hautatzean**, honako portaera hau gertatzen da:

1. Hornitzailearen fakturaren egoera Canceladora **eguneratzen da**.
2. Ezeztatutako hornitzailearen faktura eta horiekin lotutako erregistroak irakurketa bakarrekoak izango dira, eta ezin dira editatu, ezta ezabatu ere.
3. Hornitzailearen faktura-lerroen arabera sortu zen kostu erreal oro inbertitzen da.
4. Kostu errealak hornitzailearen faktura-lerroekin lotzen baziren bat-etortze-prozesuaren zati gisa, hornitzailearen fakturaren jatorrizko berrespenak itzuli egin zituen. Hornitzailearen faktura ezerezten den bitartean, benetako kostu horiek berriro sortzen dira. Jatorriaren arabera, denbora, gastua edo materialen erabilera izango dira.
5. Hornitzailearen faktura bertan behera utzi ondoren, zuzenketa-egunkariak sortu, denbora-sarreraren berreskurapenak prozesatu eta jatorrizko materialaren denboraren, gastuaren edo benetako datuen onarpena kikla dezake.

> [!NOTE]
> Proiektuaren hornitzailearen fakturak soilik kita daitezke. Beste estatu batzuetako hornitzaileen fakturak ezin dira ezeztatu.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
