---
title: Bertsio-berritu Onarpen modernoen hausnarketak
description: Artikuluak administratzaileek Modern Approvals funtzionaltasuna gaitzen dutenean kontuan hartu behar dituzten puntuak biltzen ditu.
author: stsporen
ms.date: 01/31/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 44a933c92d4ef8dff40f20200d74c4bbdf8caa76
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931729"
---
# <a name="upgrade-considerations-for-modern-approvals"></a>Bertsio-berritu Onarpen modernoen hausnarketak 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

2022ko apirileko kaleratzearen 1 bertsioaren barruan, Modern Approvals funtzioa lehenespenez gaituta egongo da. Funtzionalitate honek onarpen-logikaren fidagarritasuna hobetzen du eta onarpen-logikak huts egiten badu arrazoia zehaztu dezakezula ziurtatzen du.

Aldaketa horren barruan, proiektuen onarpenen egoera-aldaketak eguneratzen dira. Egoera orain zuzenean doa **Aurkeztua**-tik **Onartua**-ra. **Zain** jada ez da onarpenetarako egoera. Onarpen bat egiteke dagoen zehazteko, egiaztatu onespena onarpen-multzo baten parte dela, eta berrikusi erantsitako onarpen-multzoaren egoera.

## <a name="before-you-upgrade"></a>Bertsio-berritu aurretik

Modern Approvals-era bertsio-berritu aurretik, ziurtatu ez duzula onarpen pendienterik. Modern Approvals-ek ez du erabiltzen **Zain** egoera. Beraz, oraindik bezala markatuta dauden onarpen guztiak **Zain** bertsio berritu ondoren ez da prozesatuko.

## <a name="after-you-upgrade"></a>Bertsio-berritu ondoren

Modern Approvals-era eguneratu ondoren, administratzaile batek onarpenak prozesatzen dituen hodeiko fluxua gaituta dagoela egiaztatu behar du.

1. Hasi saioa [flow.microsoft.com](https://flow.microsoft.com)
2. Orriaren goiko eskuinaldean, aldatu zure ingurunea eguneratu duzun ingurunera.
3. Hautatu **Irtenbideak** ingurunean instalatutako irtenbideak zerrendatzeko.
4. Irtenbideen zerrendan, hautatu **Project Operations** edo **Project Service**.
5. Aldatu iragazkia honetatik **Denak** hona: **Hodei Fluxuak**.
6. Egiaztatu hori **Project Service - Behin eta berriz programatu proiektuak onartzeko multzoak** aukera ezarrita dago **Aktibatuta**. Ez badago, hautatu fluxua eta hautatu **Aktibatu**.
7. Egiaztatu prozesaketa bost minuturo gertatzen ari dela berrikusiz **Sistema-lanak** zerrendan **Ezarpenak** eremua.

## <a name="short-term-rollback"></a>Epe laburreko atzerapena

Ezin badituzu aldaketak hartu edo eginbide honekin arazo larri bat aurkitzen baduzu, aldi baterako jatorrizko onarpen-fluxura itzul dezakezu urrats hauek jarraituz:
1. Hasi saioa zure ingurunean eta egiaztatu ez dagoela onarpenik zain.
2. Joan **Ezarpenak** > **Proiektuaren parametroak** aukerara.
3. Hautatu **Ezaugarrien Kontrola** eta gero hautatu **Onarpen modernoak** funtzioa desaktibatzeko.

## <a name="removing-the-feature-flag"></a>Ezaugarrien bandera kentzen

2022ko urriko kaleratzeko 2 eguneratzean, eginbide hau desaktibatzeko gaitasuna kenduko da.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
