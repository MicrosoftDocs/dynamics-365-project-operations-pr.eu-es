---
title: Project Service Automation eguneratzearen 29, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 29. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 87f10d793f9edc055444a3cecea9ea709c1fd7ff7213d6cfaf6b3cbe83a6a5a6
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6985081"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a>Project Service Automation eguneratzearen 29, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 29. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.47.7 konpilazio-zenbakia du eta, oro har, 2021eko otsailean jarriko da erabilgarri automatikoki eguneratzeko moduan.

## <a name="update-release-29"></a>29. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira:

- Erabiltzaileek ezin dituzte lanorduak egun baliodunetan erregistratuta ikusi denbora sartzeko saretan.
- Onartutako gastuen sarrerak saretan editatu daitezke.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- Baliabideak esleitzeko esfortzuaren orduak ziurtatzeko balioztatzeko logika ezin da negatiboa izan.
- Pertsonalizatutako ekintza, **AssignResourcesForTask** eremu guztiak eguneratzen ditu aldatutako eremuen ordez.
- Fitxategian erregistratuta dauden plug-inekin edo lan-fluxuekin ingurune batean proiektu bat kopiatzean **CreateProject** gertaera, **msdyn_bulkgenerationstatus** atributua ez da eguneratu **CopyWBSToProject** huts egiten du.
- Proiektuaren egutegia zabaltzen duzunean, lanegunak ez dira ordenan gorantz ordenatzen proiektuaren zereginen eguneratze batzuek huts egin dezaten.
- Lehendik dagoen proiektu batean Proiektuen Kudeatzailea aldatzeak antolaketa-unitate lehenetsitako logika abiarazten du.

**Salmentak**

Arazo hauek konpondu dira:

- **Kontratua gauzatzea** fitxan **Kontratua** orrialdeak isilean huts egiten du hasierakoan, kontratu lerroak ez daudenean.