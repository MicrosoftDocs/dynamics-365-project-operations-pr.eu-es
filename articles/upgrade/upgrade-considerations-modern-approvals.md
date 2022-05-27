---
title: Bertsio-gogoetak onarpen modernoetarako
description: Gaiak administratzaileek Modern Approvals funtzionaltasuna gaitzen dutenean kontuan hartu beharreko puntuak biltzen ditu.
author: stsporen
ms.date: 01/31/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: a3757f057a801318feccde9be3e49c7b40fa8fcb
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8578371"
---
# <a name="upgrade-considerations-for-modern-approvals"></a>Bertsio-gogoetak onarpen modernoetarako 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

2022ko apirileko Wave 1 bertsioaren barruan, Modern Approvals funtzioa lehenespenez gaituta egongo da. Funtzionalitate honek onarpen-logikaren fidagarritasuna hobetzen du eta onarpen-logikak huts egiten badu arrazoia zehaztu dezakezula ziurtatzen du.

Aldaketa honen baitan, proiektuen onarpenen egoera-aldaketak eguneratzen dira. Egoera orain zuzenean doa **Aurkeztua** to **Onartua**. **Zain** jada ez da onarpenetarako egoera. Onarpen bat egiteke dagoen zehazteko, egiaztatu onespena onarpen-multzo baten parte dela, eta berrikusi erantsitako onespen-multzoaren egoera.

## <a name="before-you-upgrade"></a>Berritu aurretik

Modern Approvals-era bertsio-berritu aurretik, ziurtatu ez duzula onarpen zain. Modern Approvals-ek ez du erabiltzen **Zain** egoera. Beraz, oraindik bezala markatuta dauden onarpen guztiak **Zain** bertsio berritu ondoren ez da prozesatuko.

## <a name="after-you-upgrade"></a>Berritu ondoren

Modern Approvals-era eguneratu ondoren, administratzaile batek onarpenak prozesatzen dituen hodeiko fluxua gaituta dagoela egiaztatu behar du.

1. Saioa hasi [flow.microsoft.com](https://flow.microsoft.com)
2. Orriaren goiko eskuinaldean, aldatu zure ingurunea eguneratu duzun ingurunera.
3. Hautatu **Irtenbideak** ingurunean instalatutako irtenbideak zerrendatzeko.
4. Irtenbideen zerrendan, hautatu **Proiektuaren Eragiketak** edo **Proiektu Zerbitzua**.
5. Aldatu iragazkia honetatik **Denak** to **Hodei Fluxuak**.
6. Egiaztatu **Proiektu-zerbitzua - Behin eta berriz programatu proiektuak onartzeko multzoak** aukeran ezarrita dago **On**. Hala ez bada, hautatu fluxua eta, ondoren, hautatu **Piztu**.
7. Egiaztatu prozesaketa bost minuturo gertatzen ari dela berrikusiz **Sistema-lanak** zerrendan **Ezarpenak** eremua.

## <a name="short-term-rollback"></a>Epe laburreko atzerapena

Ezin badituzu aldaketak hartu edo eginbide honekin arazo larri bat aurkitzen baduzu, aldi baterako jatorrizko onarpen-fluxura itzul dezakezu urrats hauek jarraituz:
1. Hasi saioa zure ingurunean eta egiaztatu zain ez dagoela onarpenik.
2. Joan **Ezarpenak** > **Proiektuaren Parametroak**.
3. Hautatu **Ezaugarrien Kontrola** eta gero hautatu **Onarpen modernoak** funtzioa desaktibatzeko.

## <a name="removing-the-feature-flag"></a>Ezaugarrien bandera kentzen

2022ko urriko Wave 2 eguneratzean, eginbide hau desaktibatzeko gaitasuna kenduko da.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
