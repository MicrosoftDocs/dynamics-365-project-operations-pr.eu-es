---
title: Project Service Automation integrazio-parametroak
description: Gai honetan integratzen zarenean lehenetsitako datuak nola sartzen diren konfiguratzen da Microsoft Dynamics 365 for Project Service Automation Microsoftekin Dynamics 365 Finance.
author: ruhercul
ms.date: 03/03/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 9793b680fc2be3b300689c4aded8005470f30519
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006406"
---
# <a name="project-service-automation-integration-parameters"></a>Project Service Automation integrazio-parametroak

[!include[banner](../includes/banner.md)]

Gainean **Project Service Automation integrazio parametroak** orrialdean, integratzen zarenean lehenetsitako datuak nola sartzen diren konfigura dezakezu Dynamics 365 Project Service Automation hurrengoarekin Dynamics 365 Finance. Project Service Automation Finantzara proiektuak ongi sinkronizatzeko, honako eremuak konfiguratu behar dituzu.

Irekitzeko **Project Service Automation integrazio parametroak** orrialdea, joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Dynamics 365 for Project Service Automation integrazio parametroak**. 

> [!NOTE]
> - Proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa eskuragarri daude 8.0 bertsioan.
> - Datu bateratuen integrazioa eskuragarri dago 8.0.1 bertsioan edo hurrengoan.


| Fitxa                    | Eremua                | Deskribapenak |
|------------------------|----------------------|-------------|
| Orokorra                | Lehenetsitako proiektu mota | Aukeratu lehenetsitako proiektu mota. Proiektuak Project Service Automation-etik sinkronizatzen direnean, balio hori erabiltzen da integrazio txantiloian lehenetsitako balioa eman ez baduzu. Sinkronizazioan zehar **Proiektu mota** proiektu berrien eremua balio horri ezartzen zaio. Hala ere, baliteke eguneratu egin daiteke proiektuaren kontratu lerroak Project Service Automation-etik sinkronizatzen direnean. |
|                        | Denboraren kategoria        | Hautatu denboraren kategoria lehenetsia. Balio hori ordu-kalkuluak Project Service Automation-etik sinkronizatzen direnean erabiltzen da. Orduen kalkuluak eta orduko errealitateak Project Service Automation-etik sinkronizatzen direnean, **Kategoria** Finantza proiektuen ordu berrien aurreikuspenen eremua balio horretara ezarrita dago. |
|                        | Prezioaren kategoria         | Hautatu prezioaren kategoria lehenetsia. Balio hori prezioaren datu bateratuak Project Service Automation-etik sinkronizatzen direnean erabiltzen da. Prezioaren datu bateratuak Project Service Automation-etik sinkronizatzen direnean, **Kategoria** Finantza prezioaren transakzioen eremua balio horretara ezarrita dago. |
| Proiektu taldearen lehenespenak | Proiektu mota         | Egin klik **Berria** proiektu talde lehenetsia ezartzeko proiektu mota hautatzeko errenkada bat gehitzeko. Proiektu mota zehatz bat konfigurazioan behin bakarrik hauta daiteke. |
|                        | Proiektu taldea        | Aukeratu proiektu talde lehenetsia hautatutako proiektu motarako. Project Service Automation proiektu berriak sinkronizatzen direnean, **Proiektu taldea** eremua proiektu motarako balio lehenetsian ezarrita dago integrazio txantiloian balio lehenetsirik eman ez baduzu. |
| Fakturazio mota lehenetsiak  | Fakturazio mota         | Egin klik **Berria** jabetza-lerro lehenetsia ezartzeko fakturazio mota hautatzeko errenkada bat gehitzeko. Fakturazio mota zehatz bat konfigurazioan behin bakarrik hauta daiteke. |
|                        | Linearen jabetza        | Aukeratu lehenetsitako lerroaren jabetza hautatutako fakturazio-motarako. Ordu berrien kalkuluak, gastu berrien kalkuluak edo egiazko berriak sinkronizatzen direnean Project Service Automation-etik **Linearen jabetza** eremuak fakturazio motaren lehenetsitako balioa du. |
| Funtzionaltasuna blokeatzea  | Ez da aplikagarria       | Aukeratu Finantzan desgaitzeko funtzionalitatea Project Service Automation-etik sortutako proiektu eta kontratuetarako. Adibidez, kontratuak eta proiektuak editatzeko gaitasuna desaktiba dezakezu, lanen banakako egiturak sor ditzakezu eta Finantzetan denbora-orriak sartu. Kontabilitatearekin lotutako eremuak gaitzen jarraituko dute, parametroaren ezarpenak erabilgarri ez uzten baditu ere. Berez, funtzionalitate guztiak gaituta daude. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]