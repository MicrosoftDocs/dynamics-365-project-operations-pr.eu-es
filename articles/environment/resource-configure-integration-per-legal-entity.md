---
title: Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera
description: Gai honek Project Operations-eko legezko entitatearen integrazioa konfiguratzeari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: fc3f5be1318d482ece9a6e9e4fadc3cf628ff79577776e679f32cef7c0b2fc8f
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6999391"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a>Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek konfiguratzeko beharrezko pausoak ematen dizkizu Dynamics 365 Project Operations pertsona juridiko bakoitzeko.

## <a name="enable-feature-keys-in-dynamics-365-finance"></a>Gaitu gako nagusiak Dynamics 365 Finance-n

Bete urrats hauek beharrezko eginbideak gaitzeko.

1. Dynamics 365 Finance-n, joan **Eginbideen kudeaketa** lan-eremura.
2. **Ezaugarrien zerrenda**, aurkitu eta gaitu ezaugarri hauek:
  
    - **Gaitu proiektu baterako hainbat kontratu lerro**
    - **Gaitu Project Operations Dynamics 365 Customer Engagement**

> [!NOTE]
> **Ezaugarri teklak** zerrendatuta ikusten ez baduzu, egiaztatu zure Finantza bertsioak gutxieneko bertsioaren baldintza betetzen duela (10.0.13 bertsioaren aplikazioa kalitate eguneratze guztiekin aplikatuta edo berriagoa). Aukeratu **Egiaztatu eguneratzeak** funtzioen zerrenda freskatzeko.

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a>Definitu Project Operations-ek hedatzeko agertokia pertsona juridiko baterako

Project Operations-en gaitu ditzakezu Dynamics 365 Customer Engagement entitate juridiko mailan. Project Operations-eko Dynamics 365 Customer Engagement baliabideetan / stockean oinarritutako eszenatokietarako. Ingurune berean, beste entitate juridiko bat izan dezakezu Proiektuaren eragiketak erabiliz, hornitutako / ekoizteko eskaeren agertokietarako.

1. Dynamics 365 Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa orokorra eta kontabilitate parametroak**.
2. Eskuragarri dauden pertsona juridikoen zerrendan, hautatu kontratu-lerro ugari eta proiektuaren eragiketak dauden entitateak Dynamics 365 Customer Engagement funtzioak gaituta egongo dira. Utzi hautatutako proiektuen eragiketak erabiliko dituzten pertsona juridikoak biltegiratzeko / ekoizteko eskaera agertokietarako.

> [!NOTE]
> Pertsona juridikoa lehendik proiekturik ez badu soilik hauta daiteke.

## <a name="configure-project-management-and-accounting-parameters"></a>Konfiguratu Proiektuaren kudeaketa eta kontabilitatearen parametroak

Proiektuaren eragiketak erabiltzen dituen pertsona juridiko bakoitza Dynamics 365 Customer Engagement parametro lehenetsien multzo bat behar du. Parametro hauek **Proiektuaren eragiketak** fitxako **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean. Parametroak dira:

  - **Fakturazio mota lehenetsiak**: Project Operations-ek fakturazio mota lehenetsien multzo finko bat erabiltzen du, Finantza lineako propietateekin mapatu behar dena. Sortu erregistro bat fakturazio mota bakoitzerako: **Zehaztu gabea**, **Kargagarria**, **Ez da ordaindu behar**, **Osagarria** eta **Ez dago erabilgarri**.
  - **Proiektuaren kategoria lehenetsiak**: Hautatu transakzio mota bakoitzerako erabiliko diren lehenetsitako proiektuen kategoriak. Lehenetsi hauek fitxategian erabiliko dira **Project Operations Integration aldizkaria** eta proiektuaren benetako transakzio kategoriarik zehazten ez den estimazioetan.
  - **Iragarpenak**: Aukeratu iragarpen eredua denbora eta gastuen kalkuluak egiteko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]