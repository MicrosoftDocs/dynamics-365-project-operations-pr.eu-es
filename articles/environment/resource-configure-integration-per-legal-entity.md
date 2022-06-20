---
title: Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera
description: Artikulu honetan, erakunde juridiko bidezko integrazioa proiektu-eragiketetan nola konfiguratu behar den ematen da.
author: sigitac
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 3f33e641ee0932655282618c99a26e2603660059
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914617"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a>Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honetan erakunde juridikoz konfiguratzeko Dynamics 365 Project Operations beharrezkoak diren urratsak deskribatzen dira.

## <a name="enable-feature-keys-in-dynamics-365-finance"></a>Dynamics 365 Finance-n funtzio-teklak gaitu

Bete urrats hauek beharrezko eginbideak gaitzeko.

1. Dynamics 365 Finance atalean, joan hona **Ezaugarrien kudeaketa** lan-eremua.
2. **Ezaugarrien zerrenda**, aurkitu eta gaitu ezaugarri hauek:
  
    - **Gaitu proiektu baterako hainbat kontratu lerro**
    - **Dynamics 365 Customer Engagement-en proiektu-eragiketak gaitu**

> [!NOTE]
> **Ezaugarri teklak** zerrendatuta ikusten ez baduzu, egiaztatu zure Finantza bertsioak gutxieneko bertsioaren baldintza betetzen duela (10.0.13 bertsioaren aplikazioa kalitate eguneratze guztiekin aplikatuta edo berriagoa). Aukeratu **Egiaztatu eguneratzeak** funtzioen zerrenda freskatzeko.

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a>Definitu Project Operations-ek hedatzeko agertokia pertsona juridiko baterako

Dynamics 365 Customer Engagement-en proiektu-eragiketak gaitu ditzakezu, erakunde juridiko mailan. Dynamics 365 Customer Engagement-en proiektu-eragiketak erabiltzen dituen erakunde juridiko bat izan dezake, biltegiratutako baliabideetan oinarritutako agertokietarako. Ingurune berean, beste entitate juridiko bat izan dezakezu Proiektuaren eragiketak erabiliz, hornitutako / ekoizteko eskaeren agertokietarako.

1. Dynamics 365 Finance-n, joan proiektuen kudeaketara **eta kontabilitate-proiektu** > **eta-parametroen konfigurazio** > **globalera**.
2. Eskura dauden erakunde juridikoen zerrendan, aukeratu zein entitatetan jarriko diren Dynamics 365 Customer Engagement-en kontratu-lerroak eta proiektu-eragiketak. Utzi hautatutako proiektuen eragiketak erabiliko dituzten pertsona juridikoak biltegiratzeko / ekoizteko eskaera agertokietarako.

> [!NOTE]
> Pertsona juridikoa lehendik proiekturik ez badu soilik hauta daiteke.

## <a name="configure-project-management-and-accounting-parameters"></a>Konfiguratu Proiektuaren kudeaketa eta kontabilitatearen parametroak

Dynamics 365 Customer Engagement-en proiektu-eragiketak erabiltzen dituen erakunde juridiko bakoitzak aurrez zehaztutako parametroen multzo bat behar du. Parametro hauek **Proiektuaren eragiketak** fitxako **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean. Parametroak dira:

  - **Fakturazio mota lehenetsiak**: Project Operations-ek fakturazio mota lehenetsien multzo finko bat erabiltzen du, Finantza lineako propietateekin mapatu behar dena. Sortu erregistro bat fakturazio mota bakoitzerako: **Zehaztu gabea**, **Kargagarria**, **Ez da ordaindu behar**, **Osagarria** eta **Ez dago erabilgarri**.
  - **Proiektuaren kategoria lehenetsiak**: Hautatu transakzio mota bakoitzerako erabiliko diren lehenetsitako proiektuen kategoriak. Lehenetsi hauek fitxategian erabiliko dira **Project Operations Integration aldizkaria** eta proiektuaren benetako transakzio kategoriarik zehazten ez den estimazioetan.
  - **Iragarpenak**: Aukeratu iragarpen eredua denbora eta gastuen kalkuluak egiteko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]