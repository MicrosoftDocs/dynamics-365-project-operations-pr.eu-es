---
title: Project Service Automation eguneratzearen 33, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 33. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334497"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a>Project Service Automation eguneratzearen 33, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Dynamics 365 9.x-rekin bateragarria da. Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 33. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.54.98 sorrera-zenbakia du eta orokorrean 2021eko uztailean auto-eguneratze baten bidez eskuragarri dago.

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
