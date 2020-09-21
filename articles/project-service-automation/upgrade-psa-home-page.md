---
title: Eguneratu orri nagusia
description: Gai honek Dynamics 365 Project Service Automation aplikazioko eginbide berri eta aldatuak bilatzeko tokiari eta azken bertsiora eguneratzeko prozesuari buruzko informazioa eskaintzen du.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 for Project Service 3.x
author: rumant
ms.assetid: c92d0849-e40c-4a56-9719-34030fbf5991
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 55f544636f39fc4faae06fdd512f859800bb7b44
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748900"
---
# <a name="upgrade-home-page"></a><span data-ttu-id="a1f03-103">Eguneratu orri nagusia</span><span class="sxs-lookup"><span data-stu-id="a1f03-103">Upgrade home page</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a><span data-ttu-id="a1f03-104">Eguneratu PSA-ren 2.x edo 1.x bertsiotik 3.x bertsiora</span><span class="sxs-lookup"><span data-stu-id="a1f03-104">Upgrade from PSA version 2.x or 1.x to version 3.x</span></span>

### <a name="new-instances"></a><span data-ttu-id="a1f03-105">Instantzia berriak</span><span class="sxs-lookup"><span data-stu-id="a1f03-105">New instances</span></span>

<span data-ttu-id="a1f03-106">2019ko maiatzaren 17tik aurrera, Project Service Automation beste instantzia batzuk hornitzeko prozesuan aukeratu zenean, 3.x bertsioa instalatu zen lehenespenez.</span><span class="sxs-lookup"><span data-stu-id="a1f03-106">As of May 17, 2019, when Project Service Automation is selected during the provisioning of a new instance, version 3.x is installed by default.</span></span>

### <a name="existing-instances"></a><span data-ttu-id="a1f03-107">Lehendik dauden instantziak</span><span class="sxs-lookup"><span data-stu-id="a1f03-107">Existing instances</span></span>

<span data-ttu-id="a1f03-108">Aurrez, PSA-ren 2.x bertsioko instantzia zuten bezeroek eta 3.x bertsiora eguneratu behar zuten, zeina PSA-ren bezeroaren interfaze bateratuan (UCI) oinarritutako bertsioa zen, Microsoft laguntza bilatu eta instantzien xehetasunak eskaini behar zituen laguntzak instantzia 3.x bertsiora eguneratzeko gaitu zitzan.</span><span class="sxs-lookup"><span data-stu-id="a1f03-108">Previously, customers who have an instance of PSA version 2.x and needed to upgrade to version 3.x, which is the Unified client interface-based (UCI) version of PSA , had to contact Microsoft Support and provide the details of thier instance so that support could enable the instance for upgrade to version 3.x.</span></span> <span data-ttu-id="a1f03-109">2020ko martxoaren 1etik aurrera, PSA 2.x bertsioaren instantzia bat duten eta 3.x bertsiora bertsio berritu behar duten bezeroek administrazioaren ataritik zuzenean eguneratu ahal izango dute Microsoft laguntzarekin harremanetan jarri beharrik izan gabe.</span><span class="sxs-lookup"><span data-stu-id="a1f03-109">As of March 1st, 2020, customers who have an instance of PSA version 2.x and need to upgrade to version 3.x, will able to upgrade their instances directly from the Admin portal without having to contact Microsoft Support.</span></span>  

> [!NOTE]
> <span data-ttu-id="a1f03-110">PSA-ren 3.x bertsioak aldaketa garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="a1f03-110">PSA version 3.x includes significant changes.</span></span> <span data-ttu-id="a1f03-111">Interfaze bateratuaren markoan sortu da erabiltzaileran esperientzia hobe bat eskaintzeko.</span><span class="sxs-lookup"><span data-stu-id="a1f03-111">It has been built on the Unified Interface framework to help provide an improved user experience.</span></span> <span data-ttu-id="a1f03-112">Berriro diseinatutako aplikazioak erabiltzailearen iterfaze koherente eta uniformea bidaltzen du, eta diseinuaren printzipio dinamikoei jarraitzen dio edozein tamainako pantailako edo gailuko ikuspegi egokiena lortzeko.</span><span class="sxs-lookup"><span data-stu-id="a1f03-112">The redesigned app delivers a consistent, uniform user interface (UI), and it follows responsive design principles for optimal viewing on any screen size or device.</span></span> <span data-ttu-id="a1f03-113">Beste aldaketa batzuk egon dira aplikazioan.</span><span class="sxs-lookup"><span data-stu-id="a1f03-113">There have been other changes throughout the application.</span></span> <span data-ttu-id="a1f03-114">Prezioak, erreserba eta esleipen baliabideak, denbora, gastuak eta onarpenak dira aldatu diren area batzuk.</span><span class="sxs-lookup"><span data-stu-id="a1f03-114">Some of the areas that have been changed include pricing, booking and assigning resources, time, expenses, and approvals.</span></span>

<span data-ttu-id="a1f03-115">Eguneratze prozesua hasi aurretik, honako zeregin hauek osatzea gomendatzen dizugu:</span><span class="sxs-lookup"><span data-stu-id="a1f03-115">Before you begin the upgrade process, we recommend that you complete the following tasks:</span></span>

- <span data-ttu-id="a1f03-116">Ziurtatu Dynamics 365 Field Service eta Project Service Automation identifikatutako instantzian instalatuta daudela.</span><span class="sxs-lookup"><span data-stu-id="a1f03-116">Verify whether both Dynamics 365 Field Service and Project Service Automation are installed on the identified instance.</span></span> <span data-ttu-id="a1f03-117">Bi soluzioak instalatuta badaude, biak eguneratzea planifikatu beharko zenuke instantziaren ohiko erabilera berrekin baino lehen.</span><span class="sxs-lookup"><span data-stu-id="a1f03-117">If both solutions are installed, you should plan to upgrade both before you resume regular use of the instance.</span></span>
- <span data-ttu-id="a1f03-118">Ondo berrikusi jarraian dauden gaiak.</span><span class="sxs-lookup"><span data-stu-id="a1f03-118">Carefully review the following topics.</span></span> <span data-ttu-id="a1f03-119">Bertsioen arteko aldaketen kontzientziazioak eta ulermenak eguneratze prozesuan lagunduko dizu.</span><span class="sxs-lookup"><span data-stu-id="a1f03-119">Awareness and understanding of the changes between versions will help you with the upgrade process.</span></span> <span data-ttu-id="a1f03-120">Gai hauek PSA-n egindako aldaketa garrantzitsuei buruzko informazioa eskainiko dizu, baita 3.x bertsiora eguneratzeko kontuak hartu beharrekoak eta gomendioak ere.</span><span class="sxs-lookup"><span data-stu-id="a1f03-120">These topics provide information about the major changes in PSA, together with considerations and recommendations for planning your upgrade to version 3.x.</span></span>

    - [<span data-ttu-id="a1f03-121">Project Service Automation-en 3. bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="a1f03-121">What's new or changed in Project Service Automation version 3</span></span>](whats-new-changed-v3.md)
    - [<span data-ttu-id="a1f03-122">Eguneratzean kontuan hartzekoak - Project Service Automation-en 2.x edo 1.x bertsiotik 3. bertsiora</span><span class="sxs-lookup"><span data-stu-id="a1f03-122">Upgrade considerations - Project Service Automation version 2.x or 1.x to version 3</span></span>](upgrade-v3.md)

- <span data-ttu-id="a1f03-123">Eguneratu sandbox instantzia inplementazioko aldaketak ebaluatzeko produkzio-instantzia eguneratu baino lehen.</span><span class="sxs-lookup"><span data-stu-id="a1f03-123">Upgrade your sandbox instance to evaluate the changes in your implementation before you upgrade your production instance.</span></span>

<span data-ttu-id="a1f03-124">Aipatutako gaiak berrikusi ondoren eta PSA-ren 3.x bertsiora edo Bezeroaren interfaze bateratuan oinarritutako bertsiora eguneratzeko prest daudenean, bidali eskaera bat Mricrosoft-en laguntzara eguneratzea erabilgarri egon dadin administrazio-zentroan.</span><span class="sxs-lookup"><span data-stu-id="a1f03-124">After you've reviewed the topics that were mentioned earlier and are ready to upgrade to PSA version 3.x or the UCI-based version, submit a request to Microsoft support to make the upgrade available from Admin center.</span></span> <span data-ttu-id="a1f03-125">Eskaeran, eman instantziaren xehetasunak.</span><span class="sxs-lookup"><span data-stu-id="a1f03-125">In your request, provide the details of your instance.</span></span>

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a><span data-ttu-id="a1f03-126">PSA-ren aurreko bertsioak (PSA-ren 2.x bertsioa) sortu berri den instantzia batean</span><span class="sxs-lookup"><span data-stu-id="a1f03-126">Older versions of PSA (PSA version 2.x) in a newly created instance</span></span>

<span data-ttu-id="a1f03-127">2019ko maiatzaren 17tik aurrera, instantzia berri guztiek UCIa izango dute lehenetsitako bezero gisa.</span><span class="sxs-lookup"><span data-stu-id="a1f03-127">As of May 17, 2019, all new instances will have UCI as the default client.</span></span> <span data-ttu-id="a1f03-128">Aldaketa honekin lerrokatzeko, PSA-ren 3.x bertsioa eta Field Service-ren 8.x bertsioa lehenespenez hornituko dira, bertsio horiek UCI bezeroarekin lan egiteko diseinatuta daudelako.</span><span class="sxs-lookup"><span data-stu-id="a1f03-128">For alignment with this change, PSA version 3.x and Field Service version 8.x will be provisioned by default, because these versions are designed to work with the UCI client.</span></span>

<span data-ttu-id="a1f03-129">2020ko martxoaren 1etik aurrera, Dynamics PSAko bezeroek ezin izango dute ingurune berririk sortu PSA bertsio zaharragoekin, adibidez PSA 2.x bertsioa edo zaharragoa erabiliz.</span><span class="sxs-lookup"><span data-stu-id="a1f03-129">Starting March 1st 2020, customers of Dynamics PSA will no longer be able to create a new environments with older versions of PSA, for example PSA version 2.x or lower.</span></span> <span data-ttu-id="a1f03-130">Edozein ingurune berrik PSA 3.x bertsioa soilik lortuko du.</span><span class="sxs-lookup"><span data-stu-id="a1f03-130">Any new environment will be to get only version 3.x of PSA.</span></span>

> [!NOTE]
> <span data-ttu-id="a1f03-131">Field Service eta PSA aplikazioen bertsio zaharrak erabiltzen dituzunean esperientzia onena izateko, joan **Sistemaren ezarpenak** orrira eta **Erabili Interfaze bateratu berria bakarrik (gomendagarria)** eremurako, hautatu **Ez** bertsio horiek ez baitaude UCI-n behar bezala kargatzeko diseinatuta.</span><span class="sxs-lookup"><span data-stu-id="a1f03-131">For the best experience when you use older versions of the Field Service and PSA applications, go to the **System settings** page and for the field, **Use the new Unified Interface only (recommended)** field, select **No** as these versions aren't designed to be correctly loaded in UCI.</span></span> <span data-ttu-id="a1f03-132">UCI desaktibatu ondoren, Field Service eta PSA-ren bertsio horiek ireki eta exekutatu ditzakezu web-bezero zaharra erabilita.</span><span class="sxs-lookup"><span data-stu-id="a1f03-132">After you have turned off UCI, you can open and run these versions of Field Service and PSA by using the old web client.</span></span> <span data-ttu-id="a1f03-133">UCI bezeroa desaktibatzeari buruzko argibideak lortzeko, ikusi [Gaitu Interfaze bateratua bakarrik](../admin/enable-unified-interface-only.md).</span><span class="sxs-lookup"><span data-stu-id="a1f03-133">For instructions about how to turn off the UCI client, see [Enable unified interface only](../admin/enable-unified-interface-only.md).</span></span>
