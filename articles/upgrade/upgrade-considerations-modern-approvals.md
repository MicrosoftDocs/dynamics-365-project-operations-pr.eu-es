---
title: Onarpen modernoetarako eguneratze-kontsiderazioak
description: Artikuluak administratzaileek kontuan hartu behar dituzten puntuak estaltzen ditu, onarpen modernoen funtzionaltasuna gaitzean.
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
# <a name="upgrade-considerations-for-modern-approvals"></a>Onarpen modernoetarako eguneratze-kontsiderazioak 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

2022ko apirilaren 1eko Wave 1 bertsioaren parte gisa, onarpen modernoen funtzionaltasuna aurrez zehaztuta egongo da. Funtzionaltasun horrek onarpen-logikaren fidagarritasuna hobetzen du, eta onarpen-logikak huts egiten badu, arrazoia zehaztu ahal izango duela bermatzen du.

Aldaketa horren parte gisa, proiektuak onartzeko estatu-aldaketak eguneratzen dira. Estatua orain zuzenean bidali **behar** da **·**. **Malda** ez da onarpenetarako estatu bat. Onarpen bat egiteke dagoen zehazteko, egiaztatu onarpena onarpen-multzo baten parte dela eta erantsitako onarpenen egoera berrikusten duela.

## <a name="before-you-upgrade"></a>Eguneratu aurretik

Onarpen modernoak eguneratu baino lehen, ziurtatu ez duela onarpenik. Onarpen modernoak ez ditu **Aldapako** estatua erabiltzen. Beraz, eguneraketaren ondoren oraindik malda gisa **markatuta dauden onarpenak** ez dira prozesatuko.

## <a name="after-you-upgrade"></a>Eguneratu ondoren

Onarpen modernoak eguneratu ondoren, administratzaile batek baliozkotu egin behar du onarpenak prozesatzen dituen hodeiaren fluxua gaitu dela.

1. Saioa [hasi flow.microsoft.com](https://flow.microsoft.com)
2. Orriaren goiko eskuinaldean, aldatu bere ingurua eguneratu duen ingurunera.
3. Ingurunean instalatutako soluzioak zerrendatzeko konponbideak **hautatu**.
4. Konponbideen zerrendan, aukeratu **proiektu-eragiketak** edo **proiektu-zerbitzua**.
5. Aldatu Guztien **iragazkia** **hodeian**.
6. Egiazta ezazu **proiektuak behin eta berriro onartzeko** programazio-zerbitzua – Programatu proiektu-zerbitzuaren aukera aktibatuta **dagoela**. Hala ez bada, fluxua hautatu eta, ondoren, **aktibatu**.
7. Egiazta ezazu prozesamendua bost minuturo gertatzen dela, konfigurazio-eremuko **sistemaren** lanen **zerrenda berrikusiz**.

## <a name="short-term-rollback"></a>Epe laburrerako itzulketa

Aldaketak onartu ezin baditu edo ezaugarri horrekin arazo larriren bat aurkitzen badu, aldi baterako itzuli daiteke jatorrizko onarpen-fluxura, honako urrats hauek eginez:
1. Bere ingurunean saioa hasi eta egiaztatu ez dagoela onarpenik.
2. Konfigurazio-proiektuaren **parametroetara.** > **·**
3. Funtzioa **desaktibatzeko, ezaugarrien kontrola** hautatu eta, ondoren, onarpen modernoak **hautatu**.

## <a name="removing-the-feature-flag"></a>Ezaugarrien adierazlea ezabatzea

2022ko urriaren 2ko Wave eguneratzean, funtzio hori desaktibatzeko gaitasuna ezabatuko da.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
