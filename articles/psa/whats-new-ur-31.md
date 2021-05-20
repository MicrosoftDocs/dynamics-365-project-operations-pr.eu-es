---
title: Project Service Automation eguneratzearen 31, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 31. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: a595c0a129ac35d3416984e57908e73e1eaef2fd
ms.sourcegitcommit: 6e1498502461e86cff722ccaf8795ff11c7c47ad
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5945520"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a>Project Service Automation eguneratzearen 31, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 31. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honen konpilazio-zenbakia V3.10.52.77 da eta, oro har, 2021eko maiatzeko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-31"></a>31. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira:

- Denboraren sarrera kontrolatzeko komando botoiak **Erreserbatzeko Baliabidea** orrialdea nahasgarria zen.
- Urtean erreferentziazko salbuespen nulua sortu zen **Project.SetTrackingFields** denbora sarrera onartzerakoan.

**Baliabideen kudeaketa**

Arazo hauek konpondu dira:

- **Sortu taldeko kidea** ez du behar bezala erakusten erreserbaren konfigurazioko metadatuen ezarpena **Erreserbaren lehenetsitako konpromiso egoera**.
- PSA 1.X-tik 3.X-ra eguneratzean, eguneratze prozesuak huts egiten du **UpgradeResourceRequirements**.


**Salmentak**

Arazo hauek konpondu dira:

- Benetako diru-sarrerek zenbatekoak proiektuaren monetara bihurtzen dituzte jarraipen-saretan.
- Moneta lehenetsia ez da argia egunkari-lerroak, aurrekontu-lerroak eta kontratu-lerroak sortzerakoan erakunde baten oinarrizko moneta proiektuaren moneta desberdina den agertokietan.
- **Aldizkariaren balioztapenaren zain** kontsultak ez du proiektuaren arabera iragazten.
- Gainerako salmentak proiektu batean gaizki kalkulatzen dira.
- Kontaktu batean oinarritutako aurrekontuek huts egiten dute prezio zerrendarik gabe sortzen direnean.
- Hautatzen duzunean ez da prozesatzeko birarik erakusten **Berretsi faktura**.
- Hautatzen duzunean ez da prozesatzeko birarik erakusten **Sortu faktura**.
- Aurrekontua galdu ahala itxiz gero, ez dira erreserbak bertan behera geratuko.







