---
title: Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera
description: Gai honek Project Operations-eko legezko entitatearen integrazioa konfiguratzeari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 64606a20a49fd8e9602b6ac3c1ab1880796eb128
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8585823"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a>Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek konfiguratzeko beharrezko pausoak ematen dizkizu Dynamics 365 Project Operations pertsona juridiko bakoitzeko.

## <a name="enable-feature-keys-in-dynamics-365-finance"></a>Gaitu eginbide-gakoak Dynamics 365 Finance-en

Bete urrats hauek beharrezko eginbideak gaitzeko.

1. Dynamics 365 Finance atalean, joan **Ezaugarrien kudeaketa** lan-eremua.
2. **Ezaugarrien zerrenda**, aurkitu eta gaitu ezaugarri hauek:
  
    - **Gaitu proiektu baterako hainbat kontratu lerro**
    - **Gaitu Proiektuaren Eragiketak Dynamics 365 Customer Engagement-en**

> [!NOTE]
> **Ezaugarri teklak** zerrendatuta ikusten ez baduzu, egiaztatu zure Finantza bertsioak gutxieneko bertsioaren baldintza betetzen duela (10.0.13 bertsioaren aplikazioa kalitate eguneratze guztiekin aplikatuta edo berriagoa). Aukeratu **Egiaztatu eguneratzeak** funtzioen zerrenda freskatzeko.

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a>Definitu Project Operations-ek hedatzeko agertokia pertsona juridiko baterako

Proiektuen Eragiketak gaitu ditzakezu Dynamics 365 Customer Engagement-en pertsona juridiko mailan. Pertsona juridiko bat izan dezakezu Project Operations erabiliz Dynamics 365 Customer Engagement-en baliabideetan edo hornituta ez dauden agertokietarako. Ingurune berean, beste entitate juridiko bat izan dezakezu Proiektuaren eragiketak erabiliz, hornitutako / ekoizteko eskaeren agertokietarako.

1. Dynamics 365 Finance atalean, joan hona **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametro globalak**.
2. Eskuragarri dauden entitate juridikoen zerrendan, hautatu Dynamics 365 Customer Engagement funtzioak kontratu-lerro anitz eta Proiektu Eragiketak gaituta dauden entitateak. Utzi hautatutako proiektuen eragiketak erabiliko dituzten pertsona juridikoak biltegiratzeko / ekoizteko eskaera agertokietarako.

> [!NOTE]
> Pertsona juridikoa lehendik proiekturik ez badu soilik hauta daiteke.

## <a name="configure-project-management-and-accounting-parameters"></a>Konfiguratu Proiektuaren kudeaketa eta kontabilitatearen parametroak

Dynamics 365 Customer Engagement-en Project Operations erabiltzen duen pertsona juridiko bakoitzak parametro lehenetsi bat behar du. Parametro hauek **Proiektuaren eragiketak** fitxako **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean. Parametroak dira:

  - **Fakturazio mota lehenetsiak**: Project Operations-ek fakturazio mota lehenetsien multzo finko bat erabiltzen du, Finantza lineako propietateekin mapatu behar dena. Sortu erregistro bat fakturazio mota bakoitzerako: **Zehaztu gabea**, **Kargagarria**, **Ez da ordaindu behar**, **Osagarria** eta **Ez dago erabilgarri**.
  - **Proiektuaren kategoria lehenetsiak**: Hautatu transakzio mota bakoitzerako erabiliko diren lehenetsitako proiektuen kategoriak. Lehenetsi hauek fitxategian erabiliko dira **Project Operations Integration aldizkaria** eta proiektuaren benetako transakzio kategoriarik zehazten ez den estimazioetan.
  - **Iragarpenak**: Aukeratu iragarpen eredua denbora eta gastuen kalkuluak egiteko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]