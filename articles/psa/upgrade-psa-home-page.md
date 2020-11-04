---
title: Eguneratu orri nagusia
description: Gai honek Dynamics 365 Project Service Automation aplikazioko eginbide berri eta aldatuak bilatzeko tokiari eta azken bertsiora eguneratzeko prozesuari buruzko informazioa eskaintzen du.
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 29e7b519b61e8709c025e9906d04aed0156f65eb
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071117"
---
# <a name="upgrade-home-page"></a>Eguneratu orri nagusia

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a>Eguneratu PSA-ren 2.x edo 1.x bertsiotik 3.x bertsiora

### <a name="new-instances"></a>Instantzia berriak

2019ko maiatzaren 17tik aurrera, Project Service Automation beste instantzia batzuk hornitzeko prozesuan aukeratu zenean, 3.x bertsioa instalatu zen lehenespenez.

### <a name="existing-instances"></a>Lehendik dauden instantziak

Aurrez, PSA-ren 2.x bertsioko instantzia zuten bezeroek eta 3.x bertsiora eguneratu behar zuten, zeina PSA-ren bezeroaren interfaze bateratuan (UCI) oinarritutako bertsioa zen, Microsoft laguntza bilatu eta instantzien xehetasunak eskaini behar zituen laguntzak instantzia 3.x bertsiora eguneratzeko gaitu zitzan. 2020ko martxoaren 1etik aurrera, PSA 2.x bertsioaren instantzia bat duten eta 3.x bertsiora bertsio berritu behar duten bezeroek administrazioaren ataritik zuzenean eguneratu ahal izango dute Microsoft laguntzarekin harremanetan jarri beharrik izan gabe.  

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

2020ko martxoaren 1etik aurrera, Dynamics PSAko bezeroek ezin izango dute ingurune berririk sortu PSA bertsio zaharragoekin, adibidez PSA 2.x bertsioa edo zaharragoa erabiliz. Edozein ingurune berrik PSA 3.x bertsioa soilik lortuko du.

> [!NOTE]
> Field Service eta PSA aplikazioen bertsio zaharrak erabiltzen dituzunean esperientzia onena izateko, joan **Sistemaren ezarpenak** orrira eta **Erabili Interfaze bateratu berria bakarrik (gomendagarria)** eremurako, hautatu **Ez** bertsio horiek ez baitaude UCI-n behar bezala kargatzeko diseinatuta. UCI desaktibatu ondoren, Field Service eta PSA-ren bertsio horiek ireki eta exekutatu ditzakezu web-bezero zaharra erabilita. 
