---
title: Eguneratu orri nagusia
description: Gai honek Dynamics 365 Project Service Automation aplikazioko eginbide berri eta aldatuak bilatzeko tokiari eta azken bertsiora eguneratzeko prozesuari buruzko informazioa eskaintzen du.
ms.prod: ''
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
author: rumant
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a2e17fbdfb71eb62053236bf6c8a3d1aedf332df
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012346"
---
# <a name="upgrade-home-page"></a>Eguneratu orri nagusia

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a>Eguneratu PSA-ren 2.x edo 1.x bertsiotik 3.x bertsiora

### <a name="new-instances"></a>Instantzia berriak

2019ko maiatzaren 17tik aurrera, Project Service Automation beste instantzia batzuk hornitzeko prozesuan aukeratu zenean, 3.x bertsioa instalatu zen lehenespenez.

### <a name="existing-instances"></a>Lehendik dauden instantziak

Lehenago, PSA-ren 2.x bertsioko instantzia duten bezeroek eta 3.x bertsiora eguneratu behar zutenek, zeina PSA-ren bezeroaren interfaze bateratuan (UCI) oinarritutako bertsioa zen, laguntza bilatu eta instantzien xehetasunak eskaini behar zituen Microsoft Laguntza teknikoak instantzia 3.x bertsiora eguneratzeko gaitu zezan. 2020ko martxoaren 1etik aurrera, PSA 2.x bertsioaren instantzia duten eta 3.x bertsiora aldatu behar duten bezeroek beren instantziak zuzenean Administrazio ataritik eguneratu ahal izango dituzte, Microsoft Laguntza teknikoarekin harremanetan jarri beharrik izan gabe.  

> [!NOTE]
> PSA-ren 3.x bertsioak aldaketa garrantzitsuak ditu. Interfaze bateratuaren markoan sortu da erabiltzaileran esperientzia hobe bat eskaintzeko. Berriro diseinatutako aplikazioak erabiltzailearen iterfaze koherente eta uniformea bidaltzen du, eta diseinuaren printzipio dinamikoei jarraitzen dio edozein tamainako pantailako edo gailuko ikuspegi egokiena lortzeko. Beste aldaketa batzuk egon dira aplikazioan. Prezioak, erreserba eta esleipen baliabideak, denbora, gastuak eta onarpenak dira aldatu diren area batzuk.

Eguneratze prozesua hasi aurretik, honako zeregin hauek osatzea gomendatzen dizugu:

- Ziurtatu Dynamics 365 Field Service eta Project Service Automation identifikatutako instantzian instalatuta daudela. Bi soluzioak instalatuta badaude, biak eguneratzea planifikatu beharko zenuke instantziaren ohiko erabilera berrekin baino lehen.
- Ondo berrikusi jarraian dauden gaiak. Bertsioen arteko aldaketen kontzientziazioak eta ulermenak eguneratze prozesuan lagunduko dizu. Gai hauek PSA-n egindako aldaketa garrantzitsuei buruzko informazioa eskainiko dizu, baita 3.x bertsiora eguneratzeko kontuak hartu beharrekoak eta gomendioak ere.

    - [Project Service Automation-en 3. bertsioko berrikuntzak edo aldaketak](whats-new-changed-v3.md)
    - [Eguneratzean kontuan hartzekoak - Project Service Automation-en 2.x edo 1.x bertsiotik 3. bertsiora](upgrade-v3.md)

- Eguneratu sandbox instantzia inplementazioko aldaketak ebaluatzeko produkzio-instantzia eguneratu baino lehen.

Aipatutako gaiak berrikusi ondoren eta PSA-ren 3.x bertsiora edo Bezeroaren interfaze bateratuan oinarritutako bertsiora eguneratzeko prest daudenean, bidali eskaera bat Mricrosoft-en laguntzara eguneratzea erabilgarri egon dadin administrazio-zentroan. Eskaeran, eman instantziaren xehetasunak.

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a>PSA-ren aurreko bertsioak (PSA-ren 2.x bertsioa) sortu berri den instantzia batean

2019ko maiatzaren 17tik aurrera, instantzia berri guztiek UCIa izango dute lehenetsitako bezero gisa. Aldaketa honekin lerrokatzeko, PSA-ren 3.x bertsioa eta Field Service-ren 8.x bertsioa lehenespenez hornituko dira, bertsio horiek UCI bezeroarekin lan egiteko diseinatuta daudelako.

2020ko martxoaren 1etik aurrera, Dynamics PSA-ko bezeroek ezin izango dute ingurune berri bat sortu PSAren bertsio zaharrekin, adibidez PSA 2.x bertsioa edo txikiagoa. Edozein ingurune berrik PSA 3.x bertsioa soilik lortuko du.

> [!NOTE]
> Field Service eta PSA aplikazioen bertsio zaharrak erabiltzen dituzunean esperientzia onena izateko, joan **Sistemaren ezarpenak** orrira eta **Erabili Interfaze bateratu berria bakarrik (gomendagarria)** eremurako, hautatu **Ez** bertsio horiek ez baitaude UCI-n behar bezala kargatzeko diseinatuta. UCI desaktibatu ondoren, Field Service eta PSA-ren bertsio horiek ireki eta exekutatu ditzakezu web-bezero zaharra erabilita. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]