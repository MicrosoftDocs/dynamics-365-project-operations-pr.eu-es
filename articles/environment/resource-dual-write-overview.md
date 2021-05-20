---
title: Project Operations idazketa dualeko integrazioa
description: Gai honek Project Operations idazketa bikoitzeko integrazioaren ikuspegi orokorra eskaintzen du.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d9d6a7c367872219b4aca32aecb15d6837ebe296
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955643"
---
# <a name="project-operations-dual-write-integration-overview"></a>Project Operations idazketa dualeko integrazioaren ikuspegi orokorra

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Project Operations-en erabilerak [idazketa bikoitzeko gaitasunak](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) datuak zehar sinkronizatzeko Microsoft Dataverse eta Dynamics 365 Finance.

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak arteko integrazio horren zati gisa Dataverse eta Finance artean.

![Project Operations-en datu-fluxuen ikuspegi orokorra](./media/ProjectOperationsFlows.jpg)

Project Operations Dataverse-n Erabiltzaile interfaze modernoa (UI) eta koderik gabeko / kode baxuko hedapen erraza erabiltzen ditu Power Platform gaitasunak. Proiektuen kudeatzaileek, baliabideen kudeatzaileek, proiektuko taldekideek eta lehen lerroko beste pertsona batzuek Project Operations-en egiten dituzte jarduerak Dataverse-n.

Project Operations Finance-n proiektuen kontabilitatea eta diru-sarrerak ezagutzeko laguntza eskaintzen du. Project Operations Finance finantza esparruan sartzen dira salmenten gaineko zerga kalkulatzeko, moneta truke tasak, finantza dimentsioen berri emateko eta beste. Proiektuaren kontularien esperientziak gehienbat Finantzetan oinarritzen dira.

Project Operations-en integrazioa osagai hau osatzen dute:


- [Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa](resource-dual-write-setup-integration.md) 
- [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md)
- [Proiektuaren fakturak](resource-dual-write-project-invoice.md)
- [Gastuen kudeaketa](resource-dual-write-expense.md)
- [Saltzailearen faktura](resource-dual-write-vendor-invoice.md)
