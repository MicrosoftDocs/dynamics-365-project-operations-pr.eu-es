---
title: Project Service Automation eguneratzearen 40, V3 bertsioko berrikuntzak edo aldaketak
description: Artikulu honetan Update Release 40, V3-n Microsoft Dynamics 365 Project Service Automation eskuragarri dauden ezaugarriak eta zuzenketak zerrendatzen dira.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/31/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: dca7f340b8d544b183aa0390ac3c11a38f536ed0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912777"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>Project Service Automation eguneratzearen 40, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Dynamics 365 9.x-rekin bateragarria da. Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Artikulu honetan, Project Service Automation Update Release 40, V3-rako berriak diren edo aldatu diren ezaugarriak eta zuzenketak zerrendatzen dira. Bertsio honek V3.10.61.61 bilduma-zenbakia du, eta 2022ko otsailean eguneratuta.

## <a name="update-release-40"></a>40. eguneratze-bertsioa

### <a name="features"></a>Eginbideak
Project Service Automation a Project Operations - Lite eguneratzeko 1 fasea 2022ko otsailean jarriko dute martxan bezero guztientzat. Hautagarritasuna egiaztatzeko, ikus Project Service Automation-en Eguneratzea [Project Operations-era](upgrade-project-operations-non-stocked.md). Aplikazioa administrazio-zentroan agertzen ez bada, jar zaitez harremanetan euskarri teknikoarekin Power Platform eta eska ezazu hegaldia bere inguruneetarako gaituta egon dadila. Eskaeran, hegaldia gaitu behar den inguruneko identifikatzaileen zerrenda bat jaso behar da.

### <a name="bug-fixes"></a>Akatsen zuzenketa

Arazo hauek konpondu dira.

**Denbora eta gastua**
- Sarrera bat falta da ordu sarrera bat atzera botatzen edo bertan behera geratzen denean. 

**Salmentak**

- Erabiltzeko prest dauden osagarrien bidez kostuen edo salmenten zenbatespenak eguneratzen direnean, erabiltzailearen interfazetik kanpo baliozkoak ez diren JSON karga erabilgarriak behar ez bezala bidaltzeko aukera ematen zaio.
- Kotizazio-lerroak bista azkarraren bidez eguneratzen dituenean, kotizazioak aktibatzeko aukera ematen zaio.
