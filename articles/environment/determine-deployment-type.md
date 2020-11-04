---
title: Zehaztu inplementazio mota
description: Gai honek zure enpresako Proiektuaren eragiketen inplementazio mota zuzena determinatzen laguntzeari buruzko informazioa eskaintzen du.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 564f2878553fe3904a7c47c7e80a3b57c763a3b2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071040"
---
# <a name="determine-your-deployment-type"></a><span data-ttu-id="0ff48-103">Zehaztu inplementazio mota</span><span class="sxs-lookup"><span data-stu-id="0ff48-103">Determine your deployment type</span></span>

<span data-ttu-id="0ff48-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="0ff48-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0ff48-105">Lizentzia erosi ondoren, hasi hemen Dynamics 365 Project Operations-en inplementazio eredu onena zehazteko [Instalazio gidatuko fluxua](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="0ff48-105">After you purchase the license, start here to determine the best deployment model of Dynamics 365 Project Operations using the [Guided installation flow](https://aka.ms/provisionprojectoperations).</span></span>
> <span data-ttu-id="0ff48-106">Gidatutako instalazio-fluxua finkatu ondoren, kudeaketa-atarira zuzenduko zara zure instalazioa osatzeko.</span><span class="sxs-lookup"><span data-stu-id="0ff48-106">After you have finshed the Guided installation flow, you will be directed to the correct management portal to complete your installation.</span></span> <span data-ttu-id="0ff48-107">Instalazioa osatzeko, ikusi inplementazioaren xehetasunak.</span><span class="sxs-lookup"><span data-stu-id="0ff48-107">See the deployment details to complete the installation.</span></span>


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a><span data-ttu-id="0ff48-108">Dynamics 365 Project Service Automation erabiltzen duten Dynamics-eko lehengo bezeroak</span><span class="sxs-lookup"><span data-stu-id="0ff48-108">Existing customers of Dynamics using Dynamics 365 Project Service Automation</span></span>
<span data-ttu-id="0ff48-109">Project Operations-ek Project Service Automation-ekin hornitutako gaitasunak biltzen ditu.</span><span class="sxs-lookup"><span data-stu-id="0ff48-109">Project Operations includes the capabilities that shipped with Project Service Automation.</span></span> <span data-ttu-id="0ff48-110">Aurrerantzean bezero horien bertsio berritzeko bidea argitaratuko da.</span><span class="sxs-lookup"><span data-stu-id="0ff48-110">An upgrade path will be released for these customers in the future.</span></span>

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a><span data-ttu-id="0ff48-111">Proiektu-kudeaketa eta kontabilitatea erabiltzen duten Dynamics 365 Finance-ren lehendik dauden bezeroak</span><span class="sxs-lookup"><span data-stu-id="0ff48-111">Existing customers of Dynamics 365 Finance using Project management and accounting</span></span> 

<span data-ttu-id="0ff48-112">Proiektuen kudeaketa eta kontabilitate funtzionalitatea erabiltzen duten Finantzetako lehendik dauden bezeroek bere horretan jarraitzeko.</span><span class="sxs-lookup"><span data-stu-id="0ff48-112">Existing customers of Finance who use the Project management and accounting functionality can continue to use this as is.</span></span> <span data-ttu-id="0ff48-113">Ikusi [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma).</span><span class="sxs-lookup"><span data-stu-id="0ff48-113">See [Project Operations for stocked/production order scenarios](#pma).</span></span>


## <a name="deployment-types"></a><span data-ttu-id="0ff48-114">Inplementazio motak</span><span class="sxs-lookup"><span data-stu-id="0ff48-114">Deployment types</span></span>
<span data-ttu-id="0ff48-115">Project Operations-ek zure eskakizunekin bat etortzeko hainbat aukera onartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="0ff48-115">Project Operations supports multiple deployment options to match your requirements.</span></span> <span data-ttu-id="0ff48-116">Dynamics 365 bezero berria edo lehendik zaren, Project Operations-ek zure beharrak onar ditzake.</span><span class="sxs-lookup"><span data-stu-id="0ff48-116">Whether you're a new or existing Dynamics 365 customer, Project Operations can support your needs.</span></span>

<span data-ttu-id="0ff48-117">Gure [Inplementazio galdetegia](https://aka.ms/provisionprojectoperations) inplementazio egokia zehazten lagunduko dizu.</span><span class="sxs-lookup"><span data-stu-id="0ff48-117">Our [Deployment questionnaire](https://aka.ms/provisionprojectoperations) will help you determine the right deployment.</span></span> <span data-ttu-id="0ff48-118">Emaitzek inplementazio mota hauetakoren batera bideratuko zaituzte:</span><span class="sxs-lookup"><span data-stu-id="0ff48-118">The results will guide you toward one of the following deployment types:</span></span>

- [<span data-ttu-id="0ff48-119">Oinarrizko inplementazioa: kudeatu proformako fakturak</span><span class="sxs-lookup"><span data-stu-id="0ff48-119">Lite deployment – deal to proforma invoicing</span></span>](#lite)
- [<span data-ttu-id="0ff48-120">Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="0ff48-120">Project Operations for resource/non-stocked scenarios</span></span>](#integrated)
- [<span data-ttu-id="0ff48-121">Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="0ff48-121">Project Operations for stocked/production order scenarios</span></span>](#pma)

<span data-ttu-id="0ff48-122">Project Operations-ek ingurune berean biltegiratutako / ekoizteko eskaerak eta ez hornitutako / baliabideetan oinarritutako agertokiak onartzen dituzte entitate juridikoen mailako konfigurazioen bidez.</span><span class="sxs-lookup"><span data-stu-id="0ff48-122">Project Operations support stocked/production order scenarios and non-stocked/resource-based scenarios on the same environment through legal entity-level configurations.</span></span> <span data-ttu-id="0ff48-123">Adibidez, Contosok hornitutako / ekoizteko eskaeren gaitasunak erabil ditzake AEBetako fabrikazio instalazioetan (Entitate juridikoa = Contoso Manufacturing United States).</span><span class="sxs-lookup"><span data-stu-id="0ff48-123">For example, Contoso can use the stocked/production order capabilities in their US manufacturing facility (Legal entity = Contoso Manufacturing United States).</span></span> <span data-ttu-id="0ff48-124">Contosok hornituta ez dauden / baliabideetan oinarritutako gaitasunak erabil ditzake Erresuma Batuko Contoso Robotics Arms zerbitzuaren instalazioetan (Entitate juridikoa = Contoso Robotics United Kingdom).</span><span class="sxs-lookup"><span data-stu-id="0ff48-124">Contoso can use the non-stocked/resource-based capabilities in their Contoso Robotics Arms servicing facility in UK (Legal entity = Contoso Robotics United Kingdom).</span></span>

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a><span data-ttu-id="0ff48-125">Oinarrizko inplementazioa: kudeatu proformako fakturak</span><span class="sxs-lookup"><span data-stu-id="0ff48-125">Lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="0ff48-126">Lite inplementazioak gaitasun hauek ditu:</span><span class="sxs-lookup"><span data-stu-id="0ff48-126">The lite deployment includes the following capabilities:</span></span>

- <span data-ttu-id="0ff48-127">Proiektuaren plangintza Microsoft Project weberako</span><span class="sxs-lookup"><span data-stu-id="0ff48-127">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="0ff48-128">Dimentsio anitzeko prezioak</span><span class="sxs-lookup"><span data-stu-id="0ff48-128">Multi-dimensional pricing</span></span>
- <span data-ttu-id="0ff48-129">Baliabide-kudeaketa bateratua</span><span class="sxs-lookup"><span data-stu-id="0ff48-129">Unified Resource Management</span></span>
- <span data-ttu-id="0ff48-130">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="0ff48-130">Time Tracking</span></span>
- <span data-ttu-id="0ff48-131">Oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="0ff48-131">Basic Expense</span></span>
- <span data-ttu-id="0ff48-132">Faktura-proposamena</span><span class="sxs-lookup"><span data-stu-id="0ff48-132">Invoice Proposal</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="0ff48-133">Inplementazio-urratsak</span><span class="sxs-lookup"><span data-stu-id="0ff48-133">Deployment steps</span></span>
<span data-ttu-id="0ff48-134">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="0ff48-134">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="0ff48-135">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](lite-preview-subscription-sign-up.md) eta [Ingurune berria hornitzea](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="0ff48-135">For this deployment, see [Sign-up for preview subscriptions](lite-preview-subscription-sign-up.md) and [Provision new environment](lite-deployment.md).</span></span> 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a><span data-ttu-id="0ff48-136">Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="0ff48-136">Project Operations for resource/non-stocked scenarios</span></span>
<span data-ttu-id="0ff48-137">Baliabideen / hornitu gabeko eszenatokien Poject Operations-ek gaitasun hauek biltzen ditu:</span><span class="sxs-lookup"><span data-stu-id="0ff48-137">The Project Operations for resource/non-stocked scenarios includes the following capabilities:</span></span>
  
- <span data-ttu-id="0ff48-138">Proiektuaren plangintza Microsoft Project weberako</span><span class="sxs-lookup"><span data-stu-id="0ff48-138">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="0ff48-139">Dimentsio anitzeko prezioak</span><span class="sxs-lookup"><span data-stu-id="0ff48-139">Multi-dimensional pricing</span></span>
- <span data-ttu-id="0ff48-140">Baliabide-kudeaketa bateratua</span><span class="sxs-lookup"><span data-stu-id="0ff48-140">Unified Resource Management</span></span>
- <span data-ttu-id="0ff48-141">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="0ff48-141">Time Tracking</span></span>
- <span data-ttu-id="0ff48-142">Oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="0ff48-142">Basic Expense</span></span>
- <span data-ttu-id="0ff48-143">Gastu osoa</span><span class="sxs-lookup"><span data-stu-id="0ff48-143">Full Expense</span></span>
- <span data-ttu-id="0ff48-144">OCR agiria</span><span class="sxs-lookup"><span data-stu-id="0ff48-144">Receipt OCR</span></span>
- <span data-ttu-id="0ff48-145">Fakturazio osoa</span><span class="sxs-lookup"><span data-stu-id="0ff48-145">Full Invoicing</span></span>
- <span data-ttu-id="0ff48-146">Diru-sarreren aitorpena</span><span class="sxs-lookup"><span data-stu-id="0ff48-146">Revenue Recognition</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="0ff48-147">Inplementazio-urratsak</span><span class="sxs-lookup"><span data-stu-id="0ff48-147">Deployment steps</span></span>
<span data-ttu-id="0ff48-148">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="0ff48-148">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="0ff48-149">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](resource-sign-up-preview-subscription.md) eta [Ingurune berria hornitzea](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="0ff48-149">For this deployment, see [Sign-up for preview subscriptions](resource-sign-up-preview-subscription.md) and [Provision new environment](resource-provision-new-environment.md).</span></span> 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a><span data-ttu-id="0ff48-150">Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="0ff48-150">Project Operations for stocked/production order scenarios</span></span>

- <span data-ttu-id="0ff48-151">Proiektuaren antolaketa WBS erabiliz</span><span class="sxs-lookup"><span data-stu-id="0ff48-151">Project planning using WBS</span></span>
- <span data-ttu-id="0ff48-152">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="0ff48-152">Resource Management</span></span>
- <span data-ttu-id="0ff48-153">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="0ff48-153">Time Tracking</span></span>
- <span data-ttu-id="0ff48-154">Gastu osoa</span><span class="sxs-lookup"><span data-stu-id="0ff48-154">Full Expense</span></span>
- <span data-ttu-id="0ff48-155">OCR agiria</span><span class="sxs-lookup"><span data-stu-id="0ff48-155">Receipt OCR</span></span>
- <span data-ttu-id="0ff48-156">Fakturazio osoa</span><span class="sxs-lookup"><span data-stu-id="0ff48-156">Full Invoicing</span></span>
- <span data-ttu-id="0ff48-157">Diru-sarreren aitorpena</span><span class="sxs-lookup"><span data-stu-id="0ff48-157">Revenue Recognition</span></span>
- <span data-ttu-id="0ff48-158">Produkzio-eskaerak</span><span class="sxs-lookup"><span data-stu-id="0ff48-158">Production Orders</span></span>
- <span data-ttu-id="0ff48-159">Materialen inguruko laguntza</span><span class="sxs-lookup"><span data-stu-id="0ff48-159">Materials support</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="0ff48-160">Inplementazio-urratsak</span><span class="sxs-lookup"><span data-stu-id="0ff48-160">Deployment steps</span></span>
<span data-ttu-id="0ff48-161">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="0ff48-161">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="0ff48-162">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) eta [Ingurune berria hornitzea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span><span class="sxs-lookup"><span data-stu-id="0ff48-162">For this deployment, see [Sign-up for preview subscriptions](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) and [Provision new environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span></span> 

