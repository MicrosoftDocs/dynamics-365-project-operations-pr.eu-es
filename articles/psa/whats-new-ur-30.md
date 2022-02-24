---
title: Project Service Automation eguneratzearen 30, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 30. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 1169ee13c42e982cb30a40d92df660f8933786a9
ms.sourcegitcommit: b4a05c7d5512d60abdb0d05bedd390e288e8adc9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/02/2021
ms.locfileid: "5852825"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a>Project Service Automation eguneratzearen 30, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 30. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honen konpilazio-zenbakia V3.10.51.61 da eta, oro har, 2021eko apirileko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-30"></a>30. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira:

- Errorea gertatzen da denbora - sarrera sortu eta gordetzen duzunean **Sortu bizkor** orrialdea bada **Rola** eremua kendu da.
- Denbora sartzeko iragazkiak iragazki eragile okerra aplikatzen du.
- Kopiatutako denbora-orriak ez dira automatikoki bistaratzen hautatzen duzunean **Kopiatu Astea** denbora sartzeko kontrolean.

**Baliabideen kudeaketa**

Arazo hauek konpondu dira:

- Erreserba luzatzen duzunean, erreserba gogorrari esleitutako erreserba egoera ez da zuzena. Erreserba luzatzeak errespetatutako egoera errespetatzen du **Konprometituta** erreserba konfiguratzeko metadatuetan.
- Baliozko erreserba-egoera zehazten ez denean, errore-mezua ez dago behar bezala lokalizatuta.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- Proiektuak ezin dira moneta batean sortu eta erlazionatutako lanak beste moneta batean sartzen dituzte.

**Salmentak**

Arazo hauek konpondu dira:

- Prezio zerrenda kopiatzen denean, prezioak ez dira eguneratzen.
- Aurrekontua irabazi gisa ixteak huts egiten du kostuaren xehetasunak jatorrizko balioa duenean.
- **Proiektuaren zeregina** entitatean, **Aurreikusitako kostua** izena aldatu zaio **Aurreikusitako kostua (oinarria)**.
- Fakturak sortu edo ezabatzen direnean erreferentziazko salbuespen nulua sortzen da.
