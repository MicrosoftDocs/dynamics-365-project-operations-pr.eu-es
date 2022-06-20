---
title: Project Operations idazketa dualeko integrazioa
description: Artikulu honetan Project Operations-en eskritura dualaren integrazioari buruzko informazio orokorra ematen da.
author: sigitac
ms.date: 04/28/2021
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d365a036f96ff4f7b14107b43e8c6b70df0b5362
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8927957"
---
# <a name="project-operations-dual-write-integration-overview"></a>Project Operations idazketa dualeko integrazioaren ikuspegi orokorra

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Project Operations-ek idazkera dualerako gaitasunak [erabiltzen](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) ditu Dynamics 365 Finance-ren artean Microsoft Dataverse datuak sinkronizatzeko.

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak arteko integrazio horren zati gisa Dataverse eta Finance artean.

![Project Operations-en datu-fluxuen ikuspegi orokorra.](./media/ProjectOperationsFlows.jpg)

Project Operations Dataverse-n Erabiltzaile interfaze modernoa (UI) eta koderik gabeko / kode baxuko hedapen erraza erabiltzen ditu Power Platform gaitasunak. Proiektuen kudeatzaileek, baliabideen kudeatzaileek, proiektuko taldekideek eta lehen lerroko beste pertsona batzuek Project Operations-en egiten dituzte jarduerak Dataverse-n.

Project Operations Finance-n proiektuen kontabilitatea eta diru-sarrerak ezagutzeko laguntza eskaintzen du. Project Operations Finance finantza esparruan sartzen dira salmenten gaineko zerga kalkulatzeko, moneta truke tasak, finantza dimentsioen berri emateko eta beste. Proiektuaren kontularien esperientziak gehienbat Finantzetan oinarritzen dira.

Project Operations-en integrazioa osagai hau osatzen dute:


- [Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa](resource-dual-write-setup-integration.md) 
- [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md)
- [Proiektuaren fakturak](resource-dual-write-project-invoice.md)
- [Gastuen kudeaketa](resource-dual-write-expense.md)
- [Saltzailearen faktura](resource-dual-write-vendor-invoice.md)
