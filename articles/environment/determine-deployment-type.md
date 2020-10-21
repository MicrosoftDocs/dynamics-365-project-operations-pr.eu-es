---
title: Inplementazio motak
description: Gai honek zure enpresako Proiektuaren eragiketen inplementazio mota zuzena determinatzen laguntzeari buruzko informazioa eskaintzen du.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: c3cf378caae4510482a8ee6771bf2e6decfe3b48
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948728"
---
# <a name="deployment-types"></a><span data-ttu-id="c57bb-103">Inplementazio motak</span><span class="sxs-lookup"><span data-stu-id="c57bb-103">Deployment types</span></span>

<span data-ttu-id="c57bb-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="c57bb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c57bb-105">Lizentzia erosi ondoren, hasi hemen Dynamics 365 Project Operations-en inplementazio eredu onena zehazteko [Instalazio gidatuko fluxua](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="c57bb-105">After you purchase the license, start here to determine the best deployment model of Dynamics 365 Project Operations using the [Guided installation flow](https://aka.ms/provisionprojectoperations).</span></span>
> <span data-ttu-id="c57bb-106">Gidatutako instalazio-fluxua finkatu ondoren, kudeaketa-atarira zuzenduko zara zure instalazioa osatzeko.</span><span class="sxs-lookup"><span data-stu-id="c57bb-106">After you have finshed the Guided installation flow, you will be directed to the correct management portal to complete your installation.</span></span> <span data-ttu-id="c57bb-107">Instalazioa osatzeko, ikusi beheko inplementazioaren xehetasunak.</span><span class="sxs-lookup"><span data-stu-id="c57bb-107">See the deployment details below to complete the installation.</span></span>


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a><span data-ttu-id="c57bb-108">Dynamics 365 Project Service Automation erabiltzen duten Dynamics-eko lehengo bezeroak</span><span class="sxs-lookup"><span data-stu-id="c57bb-108">Existing customers of Dynamics using Dynamics 365 Project Service Automation</span></span>
<span data-ttu-id="c57bb-109">Project Operations-ek Project Service Automation-ekin hornitutako gaitasunak biltzen ditu.</span><span class="sxs-lookup"><span data-stu-id="c57bb-109">Project Operations includes the capabilities that shipped with Project Service Automation.</span></span> <span data-ttu-id="c57bb-110">Aurrerantzean bezero horien bertsio berritzeko bidea argitaratuko da.</span><span class="sxs-lookup"><span data-stu-id="c57bb-110">An upgrade path will be released for these customers in the future.</span></span>

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a><span data-ttu-id="c57bb-111">Proiektu-kudeaketa eta kontabilitatea erabiltzen duten Dynamics 365 Finance-ren lehendik dauden bezeroak</span><span class="sxs-lookup"><span data-stu-id="c57bb-111">Existing customers of Dynamics 365 Finance using Project management and accounting</span></span> 

<span data-ttu-id="c57bb-112">Proiektuen kudeaketa eta kontabilitate funtzionalitatea erabiltzen duten Finantzetako lehendik dauden bezeroek bere horretan jarrai dezakete.</span><span class="sxs-lookup"><span data-stu-id="c57bb-112">Existing customers of Finance who use the Project management and accounting functionality can continue use this as is.</span></span> <span data-ttu-id="c57bb-113">Ikusi [Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations](#pma).</span><span class="sxs-lookup"><span data-stu-id="c57bb-113">See [Project Operations for stocked/production order scenarios](#pma).</span></span>

<span data-ttu-id="c57bb-114">Project Operations-ek zure eskakizunekin bat etortzeko hainbat aukera onartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="c57bb-114">Project Operations supports multiple deployment options to match your requirements.</span></span> <span data-ttu-id="c57bb-115">Dynamics 365 bezero berria edo lehendik zaren, Project Operations-ek zure beharrak onar ditzake.</span><span class="sxs-lookup"><span data-stu-id="c57bb-115">Whether you are a new or existing Dynamics 365 customer, Project Operations can support your needs.</span></span>

<span data-ttu-id="c57bb-116">Gure [Inplementazio galdetegia](https://aka.ms/provisionprojectoperations) inplementazio egokia zehazten lagunduko dizu.</span><span class="sxs-lookup"><span data-stu-id="c57bb-116">Our [Deployment questionnaire](https://aka.ms/provisionprojectoperations) will help you determine the right deployment.</span></span> <span data-ttu-id="c57bb-117">Emaitzek inplementazio mota hauetakoren batera bideratuko zaituzte:</span><span class="sxs-lookup"><span data-stu-id="c57bb-117">The results will guide you toward one of the following deployment types:</span></span>

- [<span data-ttu-id="c57bb-118">Oinarrizko inplementazioa: kudeatu proformako fakturak</span><span class="sxs-lookup"><span data-stu-id="c57bb-118">Lite deployment – deal to proforma invoicing</span></span>](#lite)
- [<span data-ttu-id="c57bb-119">Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="c57bb-119">Project Operations for resource/non-stocked scenarios</span></span>](#integrated)
- [<span data-ttu-id="c57bb-120">Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="c57bb-120">Project Operations for stocked/production order scenarios</span></span>](#pma)

<span data-ttu-id="c57bb-121">Project Operations-ek ingurune berean biltegiratutako / ekoizteko eskaerak eta ez hornitutako / baliabideetan oinarritutako agertokiak onartzen dituzte entitate juridikoen mailako konfigurazioen bidez.</span><span class="sxs-lookup"><span data-stu-id="c57bb-121">Project Operations support stocked/production order scenarios and non-stocked/resource-based scenarios on the same environment through legal entity-level configurations.</span></span> <span data-ttu-id="c57bb-122">Adibidez, Contosok hornitutako / ekoizteko eskaeren gaitasunak balia ditzake AEBetako fabrikazio-instalazioetan (entitate juridikoa = Contoso Manufacturing United States) eta ez ditu hornitutako / baliabideetan oinarritutako gaitasunak Erresuma Batuko Contoso Robotics Arms zerbitzuaren instalazioetan (Entitate juridikoa = Contoso Robotics United Erresuma).</span><span class="sxs-lookup"><span data-stu-id="c57bb-122">For example, Contoso can leverage stocked/production order capabilities in their US manufacturing facility (Legal entity = Contoso Manufacturing United States) and non-stocked/resource-based capabilities in their Contoso Robotics Arms servicing facility in UK (Legal entity = Contoso Robotics United Kingdom).</span></span>

## <a name="a-namelitelite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="c57bb-123"><a name="lite"><a/>Oinarrizko inplementazioa: kudeatu proformako fakturak</span><span class="sxs-lookup"><span data-stu-id="c57bb-123"><a name="lite"><a/>Lite deployment - deal to proforma invoicing</span></span>
<span data-ttu-id="c57bb-124">Lite inplementazioak gaitasun hauek ditu:</span><span class="sxs-lookup"><span data-stu-id="c57bb-124">The lite deployment includes the following capabilities:</span></span>

- <span data-ttu-id="c57bb-125">Proiektuaren plangintza Microsoft Project weberako</span><span class="sxs-lookup"><span data-stu-id="c57bb-125">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="c57bb-126">Dimentsio anitzeko prezioak</span><span class="sxs-lookup"><span data-stu-id="c57bb-126">Multi-dimensional pricing</span></span>
- <span data-ttu-id="c57bb-127">Baliabide-kudeaketa bateratua</span><span class="sxs-lookup"><span data-stu-id="c57bb-127">Unified Resource Management</span></span>
- <span data-ttu-id="c57bb-128">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="c57bb-128">Time Tracking</span></span>
- <span data-ttu-id="c57bb-129">Oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="c57bb-129">Basic Expense</span></span>
- <span data-ttu-id="c57bb-130">Faktura-proposamena</span><span class="sxs-lookup"><span data-stu-id="c57bb-130">Invoice Proposal</span></span>

### <a name="deployment-steps"></a><span data-ttu-id="c57bb-131">Inplementazio-urratsak:</span><span class="sxs-lookup"><span data-stu-id="c57bb-131">Deployment steps:</span></span>
<span data-ttu-id="c57bb-132">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="c57bb-132">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="c57bb-133">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](lite-preview-subscription-sign-up.md) eta [Ingurune berria hornitzea](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="c57bb-133">For this deployment, see [Sign-up for preview subscriptions](lite-preview-subscription-sign-up.md) and [Provision new environment](lite-deployment.md).</span></span> 


## <a name="a-nameintegratedproject-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="c57bb-134"><a name="integrated"><a/>Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="c57bb-134"><a name="integrated"><a/>Project Operations for resource/non-stocked scenarios</span></span>
<span data-ttu-id="c57bb-135">Baliabideen / hornitu gabeko eszenatokien Poject Operations-ek gaitasun hauek biltzen ditu:</span><span class="sxs-lookup"><span data-stu-id="c57bb-135">The Project Operations for resource/non-stocked scenarios includes the following capabilities:</span></span>
  
- <span data-ttu-id="c57bb-136">Proiektuaren plangintza Microsoft Project weberako</span><span class="sxs-lookup"><span data-stu-id="c57bb-136">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="c57bb-137">Dimentsio anitzeko prezioak</span><span class="sxs-lookup"><span data-stu-id="c57bb-137">Multi-dimensional pricing</span></span>
- <span data-ttu-id="c57bb-138">Baliabide-kudeaketa bateratua</span><span class="sxs-lookup"><span data-stu-id="c57bb-138">Unified Resource Management</span></span>
- <span data-ttu-id="c57bb-139">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="c57bb-139">Time Tracking</span></span>
- <span data-ttu-id="c57bb-140">Oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="c57bb-140">Basic Expense</span></span>
- <span data-ttu-id="c57bb-141">Gastu osoa</span><span class="sxs-lookup"><span data-stu-id="c57bb-141">Full Expense</span></span>
- <span data-ttu-id="c57bb-142">OCR agiria</span><span class="sxs-lookup"><span data-stu-id="c57bb-142">Receipt OCR</span></span>
- <span data-ttu-id="c57bb-143">Fakturazio osoa</span><span class="sxs-lookup"><span data-stu-id="c57bb-143">Full Invoicing</span></span>
- <span data-ttu-id="c57bb-144">Diru-sarreren aitorpena</span><span class="sxs-lookup"><span data-stu-id="c57bb-144">Revenue Recognition</span></span>

### <a name="deployment-steps"></a><span data-ttu-id="c57bb-145">Inplementazio-urratsak:</span><span class="sxs-lookup"><span data-stu-id="c57bb-145">Deployment steps:</span></span>
<span data-ttu-id="c57bb-146">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="c57bb-146">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="c57bb-147">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](resource-sign-up-preview-subscription.md) eta [Ingurune berria hornitzea](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="c57bb-147">For this deployment, see [Sign-up for preview subscriptions](resource-sign-up-preview-subscription.md) and [Provision new environment](resource-provision-new-environment.md).</span></span> 


## <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a><span data-ttu-id="c57bb-148">Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations</span><span class="sxs-lookup"><span data-stu-id="c57bb-148">Project Operations for stocked/production order scenarios</span></span>

- <span data-ttu-id="c57bb-149">Proiektuaren antolaketa WBS erabiliz</span><span class="sxs-lookup"><span data-stu-id="c57bb-149">Project planning using WBS</span></span>
- <span data-ttu-id="c57bb-150">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="c57bb-150">Resource Management</span></span>
- <span data-ttu-id="c57bb-151">Denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="c57bb-151">Time Tracking</span></span>
- <span data-ttu-id="c57bb-152">Gastu osoa</span><span class="sxs-lookup"><span data-stu-id="c57bb-152">Full Expense</span></span>
- <span data-ttu-id="c57bb-153">OCR agiria</span><span class="sxs-lookup"><span data-stu-id="c57bb-153">Receipt OCR</span></span>
- <span data-ttu-id="c57bb-154">Fakturazio osoa</span><span class="sxs-lookup"><span data-stu-id="c57bb-154">Full Invoicing</span></span>
- <span data-ttu-id="c57bb-155">Diru-sarreren aitorpena</span><span class="sxs-lookup"><span data-stu-id="c57bb-155">Revenue Recognition</span></span>
- <span data-ttu-id="c57bb-156">Produkzio-eskaerak</span><span class="sxs-lookup"><span data-stu-id="c57bb-156">Production Orders</span></span>
- <span data-ttu-id="c57bb-157">Materialen inguruko laguntza</span><span class="sxs-lookup"><span data-stu-id="c57bb-157">Materials support</span></span>

### <a name="deployment-steps"></a><span data-ttu-id="c57bb-158">Inplementazio-urratsak:</span><span class="sxs-lookup"><span data-stu-id="c57bb-158">Deployment steps:</span></span>
<span data-ttu-id="c57bb-159">Erabili proiektuaren eragiketen hedapen eredu onena [Inplementazio-galdetegia](https://aka.ms/provisionprojectoperations).</span><span class="sxs-lookup"><span data-stu-id="c57bb-159">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="c57bb-160">Inplementazio honetarako, ikusi [Izena eman aurrebista harpidetzak lortzeko](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) eta [Ingurune berria hornitzea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span><span class="sxs-lookup"><span data-stu-id="c57bb-160">For this deployment, see [Sign-up for preview subscriptions](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) and [Provision new environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span></span> 



