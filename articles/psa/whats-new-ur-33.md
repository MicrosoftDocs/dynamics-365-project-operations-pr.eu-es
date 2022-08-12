---
title: Project Service Automation eguneratzearen 33, V3 bertsioko berrikuntzak edo aldaketak
description: Artikulu honetan Project Service Automation Update Release 33, V3-n eskuragarri dauden ezaugarriak eta zuzenketak zerrendatzen dira.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: d9c282e8b95b111ce71fb441e4dbb2d04f904e0f
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8915399"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a>Project Service Automation eguneratzearen 33, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Dynamics 365 9.x-rekin bateragarria da. Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Artikulu honetan, Project Service Automation V3, Update Release 33 eta beste hainbat ezaugarri eta zuzenketa berri edo aldatu diren ezaugarriak eta zuzenketak zerrendatzen dira. Bertsio honek V3.10.54.98 sorrera-zenbakia du eta orokorrean 2021eko uztailean auto-eguneratze baten bidez eskuragarri dago.

## <a name="update-release-33"></a>33. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira:

- Bi blokeatutako eremuak, **msdyn_description** eta **msdyn_externaldescription** bidali ondoren editatu daitezke.
- Errore-mezu bat gertatzen da proiektu batekin zerikusia ez duen gastua sortzen bada.
- Denbora sarrera bat sortzen denean, baliabide rolak rol inaktibo bihurtzen du lehenespenez.
- Gogoratutako eta ezabatutako gastuarekin lotutako egunkari lerroak ez dira ezabatzen.
- **Denbora sarreraren sorrera azkarreko inprimakian**, eguneratu **Proiektuaren ataza zerrenda** ikuspegia lehenespenez bistaratutako data ataza hasierako datara aldatzeko.
- Fitxategiaren denbora sarrera bat sortzen duzunean baliabide erreserbagarriaren **Erlazionatuta** fitxategik, denbora sarrera gaizki sortu da saioa hasita duen erabiltzailearen baliabide erreserbagarri nagusiaren ordez.
- Eremu berriak gehitzen dira **MDD homologazio masiboa** elkarrizketa-koadroan.

**Proiektuaren antolaketa**

Arazo hauek konpondu dira:
- Proiektuaren sorrera motela proiektuko lan orduen txantiloiak egutegi konplexuekin aplikatzen direnean.
- Hasiera-data amaiera-data baino handiagoa denean, errore bat agertzen da kopiatzeko proiektuaren txantiloian, eremu bakoitzeko denbora-osagaian desberdintasunak daudelako.

**Baliabide-kudeaketa**

Arazo hauek konpondu dira:
- Parametro oker bat erabiltzen da baliabideak erabiltzeko kontsultan eta XML-k iragazkiaren emaitza okerrak ekartzen ditu **Baliabideen erabilera** saretan.
- **Luzatu Erreserbak** baieztapenean erreserbak amaitzeko data okerra da.

**Salmentak**

Arazo hauek konpondu dira:
- Errore mezu bat gertatzen da kategoriako prezioa falta den balioekin sortzen bada.
- Errore mezu bat gertatzen da kontratu lerroaren mugarri bat eskaera lerro gabe sortzen bada.