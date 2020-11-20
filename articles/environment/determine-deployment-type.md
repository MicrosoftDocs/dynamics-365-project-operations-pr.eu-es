---
title: Zehaztu inplementazio mota
description: Gai honek zure enpresako Proiektuaren eragiketen inplementazio mota zuzena determinatzen laguntzeari buruzko informazioa eskaintzen du.
author: stsporen
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e9d3a5d8e6e1daafac72a3b4c0380b679d1869bd
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401203"
---
# <a name="determine-your-deployment-type"></a><span data-ttu-id="11ae3-103">Zehaztu inplementazio mota</span><span class="sxs-lookup"><span data-stu-id="11ae3-103">Determine your deployment type</span></span>

<span data-ttu-id="11ae3-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="11ae3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="11ae3-105">Lizentzia erosi ondoren, hasi hemen Dynamics 365 Project Operations-en inplementazio eredu onena zehazteko [Instalazio gidatuko fluxua](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="11ae3-105">After you purchase the license, start here to determine the best deployment model of Dynamics 365 Project Operations using the [Guided installation flow](https://aka.ms/provisionprojectoperations).</span></span>
> <span data-ttu-id="11ae3-106">Gidatutako instalazio-fluxua finkatu ondoren, kudeaketa-atarira zuzenduko zara zure instalazioa osatzeko.</span><span class="sxs-lookup"><span data-stu-id="11ae3-106">After you have finshed the Guided installation flow, you will be directed to the correct management portal to complete your installation.</span></span> <span data-ttu-id="11ae3-107">Instalazioa osatzeko, ikusi inplementazioaren xehetasunak.</span><span class="sxs-lookup"><span data-stu-id="11ae3-107">See the deployment details to complete the installation.</span></span>


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a><span data-ttu-id="11ae3-108">Dynamics 365 Project Service Automation erabiltzen duten Dynamics-eko lehengo bezeroak</span><span class="sxs-lookup"><span data-stu-id="11ae3-108">Existing customers of Dynamics using Dynamics 365 Project Service Automation</span></span>
<span data-ttu-id="11ae3-109">Project Operations-ek Project Service Automation-ekin hornitutako gaitasunak biltzen ditu.</span><span class="sxs-lookup"><span data-stu-id="11ae3-109">Project Operations includes the capabilities that shipped with Project Service Automation.</span></span> <span data-ttu-id="11ae3-110">Bezero hauen bertsio berritzeko bide bat kaleratuko da 2021 bertsio 1 olatuan.</span><span class="sxs-lookup"><span data-stu-id="11ae3-110">An upgrade path will be released for these customers in the 2021 release wave 1.</span></span>

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a><span data-ttu-id="11ae3-111">Proiektu-kudeaketa eta kontabilitatea erabiltzen duten Dynamics 365 Finance-ren lehendik dauden bezeroak</span><span class="sxs-lookup"><span data-stu-id="11ae3-111">Existing customers of Dynamics 365 Finance using Project management and accounting</span></span> 

<span data-ttu-id="11ae3-112">Proiektuen kudeaketa eta kontabilitate funtzionalitatea erabiltzen duten Finantzetako lehendik dauden bezeroek bere horretan erabiltzen jarrai dezakete.</span><span class="sxs-lookup"><span data-stu-id="11ae3-112">Existing customers of Finance who use the Project management and accounting functionality can continue to use it as is.</span></span> <span data-ttu-id="11ae3-113">Ikusi [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma).</span><span class="sxs-lookup"><span data-stu-id="11ae3-113">See [Project Operations for stocked/production order scenarios](#pma).</span></span>


## <a name="deployment-types"></a><span data-ttu-id="11ae3-114">Inplementazio motak</span><span class="sxs-lookup"><span data-stu-id="11ae3-114">Deployment types</span></span>
<span data-ttu-id="11ae3-115">Project Operations-ek zure eskakizunekin bat etortzeko hainbat aukera onartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="11ae3-115">Project Operations supports multiple deployment options to match your requirements.</span></span> <span data-ttu-id="11ae3-116">Dynamics 365 bezero berria edo lehendik zaren, Project Operations-ek zure beharrak onar ditzake.</span><span class="sxs-lookup"><span data-stu-id="11ae3-116">Whether you're a new or existing Dynamics 365 customer, Project Operations can support your needs.</span></span>

<span data-ttu-id="11ae3-117">Gure [Inplementazio galdetegia](https://aka.ms/provisionprojectoperations) inplementazio egokia zehazten lagunduko dizu.</span><span class="sxs-lookup"><span data-stu-id="11ae3-117">Our [Deployment questionnaire](https://aka.ms/provisionprojectoperations) will help you determine the right deployment.</span></span> <span data-ttu-id="11ae3-118">Emaitzek inplementazio mota hauetakoren batera bideratuko zaituzte:</span><span class="sxs-lookup"><span data-stu-id="11ae3-118">The results will guide you toward one of the following deployment types:</span></span>

- [<span data-ttu-id="11ae3-119">Oinarrizko inplementazioa: kudeatu proformako fakturak</span><span class="sxs-lookup"><span data-stu-id="11ae3-119">Lite deployment – deal to proforma invoicing</span></span>](#lite)
- [<span data-ttu-id="11ae3-120">Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="11ae3-120">Project Operations for resource/non-stocked scenarios</span></span>](#integrated)
- [<span data-ttu-id="11ae3-121">Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="11ae3-121">Project Operations for stocked/production order scenarios</span></span>](#pma)

<span data-ttu-id="11ae3-122">Project Operations-ek ingurune berean biltegiratutako / ekoizteko eskaerak eta ez hornitutako / baliabideetan oinarritutako agertokiak onartzen dituzte entitate juridikoen mailako konfigurazioen bidez.</span><span class="sxs-lookup"><span data-stu-id="11ae3-122">Project Operations support stocked/production order scenarios and non-stocked/resource-based scenarios on the same environment through legal entity-level configurations.</span></span> <span data-ttu-id="11ae3-123">Adibidez, Contosok hornitutako / ekoizteko eskaeren gaitasunak erabil ditzake AEBetako fabrikazio instalazioetan (Entitate juridikoa = Contoso Manufacturing United States).</span><span class="sxs-lookup"><span data-stu-id="11ae3-123">For example, Contoso can use the stocked/production order capabilities in their US manufacturing facility (Legal entity = Contoso Manufacturing United States).</span></span> <span data-ttu-id="11ae3-124">Contosok hornituta ez dauden / baliabideetan oinarritutako gaitasunak erabil ditzake Erresuma Batuko Contoso Robotics Arms zerbitzuaren instalazioetan (Entitate juridikoa = Contoso Robotics United Kingdom).</span><span class="sxs-lookup"><span data-stu-id="11ae3-124">Contoso can use the non-stocked/resource-based capabilities in their Contoso Robotics Arms servicing facility in UK (Legal entity = Contoso Robotics United Kingdom).</span></span>

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a><span data-ttu-id="11ae3-125">Oinarrizko inplementazioa: kudeatu proformako fakturak</span><span class="sxs-lookup"><span data-stu-id="11ae3-125">Lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="11ae3-126">Lite inplementazioak gaitasun hauek ditu:</span><span class="sxs-lookup"><span data-stu-id="11ae3-126">The lite deployment includes the following capabilities:</span></span>

- <span data-ttu-id="11ae3-127">Dynamics 365 Sales aplikazioen esperientziak luzatzen dituzten proiektuen salmenta prozesua</span><span class="sxs-lookup"><span data-stu-id="11ae3-127">Sales process for projects that extends Dynamics 365 Sales application experiences</span></span>
- <span data-ttu-id="11ae3-128">Proiektuaren plangintza Microsoft Project weberako</span><span class="sxs-lookup"><span data-stu-id="11ae3-128">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="11ae3-129">Dimentsio anitzeko prezioak</span><span class="sxs-lookup"><span data-stu-id="11ae3-129">Multi-dimensional pricing</span></span>
- <span data-ttu-id="11ae3-130">Baliabide-kudeaketa bateratua</span><span class="sxs-lookup"><span data-stu-id="11ae3-130">Unified resource management</span></span>
- <span data-ttu-id="11ae3-131">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="11ae3-131">Time tracking</span></span>
- <span data-ttu-id="11ae3-132">Oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="11ae3-132">Basic expense</span></span>
- <span data-ttu-id="11ae3-133">Proforma eta bezeroari begira fakturazioa</span><span class="sxs-lookup"><span data-stu-id="11ae3-133">Proforma and customer-facing invoicing</span></span> 

#### <a name="deployment-steps"></a><span data-ttu-id="11ae3-134">Inplementazio-urratsak</span><span class="sxs-lookup"><span data-stu-id="11ae3-134">Deployment steps</span></span>
<span data-ttu-id="11ae3-135">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="11ae3-135">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="11ae3-136">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](lite-preview-subscription-sign-up.md) eta [Ingurune berria hornitzea](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="11ae3-136">For this deployment, see [Sign-up for preview subscriptions](lite-preview-subscription-sign-up.md) and [Provision new environment](lite-deployment.md).</span></span> 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a><span data-ttu-id="11ae3-137">Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="11ae3-137">Project Operations for resource/non-stocked scenarios</span></span>
<span data-ttu-id="11ae3-138">Baliabideen / hornitu gabeko eszenatokien Poject Operations-ek gaitasun hauek biltzen ditu:</span><span class="sxs-lookup"><span data-stu-id="11ae3-138">The Project Operations for resource/non-stocked scenarios includes the following capabilities:</span></span>
 
- <span data-ttu-id="11ae3-139">Dynamics 365 Sales aplikazioak luzatzen dituzten proiektuen salmenta prozesua</span><span class="sxs-lookup"><span data-stu-id="11ae3-139">Sales process for projects that extends the Dynamics 365 Sales application</span></span>
- <span data-ttu-id="11ae3-140">Proiektuaren plangintza Microsoft Project weberako</span><span class="sxs-lookup"><span data-stu-id="11ae3-140">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="11ae3-141">Dimentsio anitzeko prezioak</span><span class="sxs-lookup"><span data-stu-id="11ae3-141">Multi-dimensional pricing</span></span>
- <span data-ttu-id="11ae3-142">Baliabide-kudeaketa bateratua</span><span class="sxs-lookup"><span data-stu-id="11ae3-142">Unified resource management</span></span>
- <span data-ttu-id="11ae3-143">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="11ae3-143">Time tracking</span></span>
- <span data-ttu-id="11ae3-144">Oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="11ae3-144">Basic expense</span></span>
- <span data-ttu-id="11ae3-145">Gastu osoa</span><span class="sxs-lookup"><span data-stu-id="11ae3-145">Full expense</span></span>
- <span data-ttu-id="11ae3-146">OCR agiria</span><span class="sxs-lookup"><span data-stu-id="11ae3-146">Receipt OCR</span></span>
- <span data-ttu-id="11ae3-147">Proforma eta bezeroari begira fakturazioa</span><span class="sxs-lookup"><span data-stu-id="11ae3-147">Proforma and customer-facing invoicing</span></span> 
- <span data-ttu-id="11ae3-148">Proiektuen diru-sarreren aitorpena</span><span class="sxs-lookup"><span data-stu-id="11ae3-148">Revenue recognition for projects</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="11ae3-149">Inplementazio-urratsak</span><span class="sxs-lookup"><span data-stu-id="11ae3-149">Deployment steps</span></span>
<span data-ttu-id="11ae3-150">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="11ae3-150">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="11ae3-151">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](resource-sign-up-preview-subscription.md) eta [Ingurune berria hornitzea](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="11ae3-151">For this deployment, see [Sign-up for preview subscriptions](resource-sign-up-preview-subscription.md) and [Provision new environment](resource-provision-new-environment.md).</span></span> 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a><span data-ttu-id="11ae3-152">Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="11ae3-152">Project Operations for stocked/production order scenarios</span></span>

- <span data-ttu-id="11ae3-153">Proiektuaren antolaketa WBS erabiliz</span><span class="sxs-lookup"><span data-stu-id="11ae3-153">Project planning using WBS</span></span>
- <span data-ttu-id="11ae3-154">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="11ae3-154">Resource Management</span></span>
- <span data-ttu-id="11ae3-155">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="11ae3-155">Time Tracking</span></span>
- <span data-ttu-id="11ae3-156">Gastu osoa</span><span class="sxs-lookup"><span data-stu-id="11ae3-156">Full Expense</span></span>
- <span data-ttu-id="11ae3-157">OCR agiria</span><span class="sxs-lookup"><span data-stu-id="11ae3-157">Receipt OCR</span></span>
- <span data-ttu-id="11ae3-158">Fakturazio osoa</span><span class="sxs-lookup"><span data-stu-id="11ae3-158">Full Invoicing</span></span>
- <span data-ttu-id="11ae3-159">Diru-sarreren aitorpena</span><span class="sxs-lookup"><span data-stu-id="11ae3-159">Revenue Recognition</span></span>
- <span data-ttu-id="11ae3-160">Produkzio-eskaerak</span><span class="sxs-lookup"><span data-stu-id="11ae3-160">Production Orders</span></span>
- <span data-ttu-id="11ae3-161">Materialen inguruko laguntza</span><span class="sxs-lookup"><span data-stu-id="11ae3-161">Materials support</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="11ae3-162">Inplementazio-urratsak</span><span class="sxs-lookup"><span data-stu-id="11ae3-162">Deployment steps</span></span>
<span data-ttu-id="11ae3-163">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="11ae3-163">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="11ae3-164">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) eta [Ingurune berria hornitzea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span><span class="sxs-lookup"><span data-stu-id="11ae3-164">For this deployment, see [Sign-up for preview subscriptions](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) and [Provision new environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span></span> 

