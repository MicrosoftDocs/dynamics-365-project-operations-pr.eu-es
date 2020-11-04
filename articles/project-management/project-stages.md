---
title: Proiektuaren faseak
description: Gai honek eskuragarri dauden proiektuen etapei buruzko informazioa eskaintzen du Microsoft Dynamics Project Operations-en.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 554ad63bc44cbe5a1fe91eb47fedbb74bbedd4b6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071163"
---
# <a name="project-stages"></a><span data-ttu-id="a8ed6-103">Proiektuaren faseak</span><span class="sxs-lookup"><span data-stu-id="a8ed6-103">Project stages</span></span>

<span data-ttu-id="a8ed6-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="a8ed6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a8ed6-105">Proiektuaren faseak diseinatu egiten dira proiektuaren egoera aurrera doan heinean.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="a8ed6-106">Pertsonalizazioak faseak automatikoki eguneratzeko erabil daitezke negozio prozesuen fluxuekin, Power Automate edo plug-in luzapenak.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="a8ed6-107">Hurrengo fase hauek negozio-prozesuaren fluxu lehenetsian zehazten dira:</span><span class="sxs-lookup"><span data-stu-id="a8ed6-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="a8ed6-108">Berria</span><span class="sxs-lookup"><span data-stu-id="a8ed6-108">New</span></span>
- <span data-ttu-id="a8ed6-109">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="a8ed6-109">Quote</span></span>
- <span data-ttu-id="a8ed6-110">Plana</span><span class="sxs-lookup"><span data-stu-id="a8ed6-110">Plan</span></span>
- <span data-ttu-id="a8ed6-111">Entregatu</span><span class="sxs-lookup"><span data-stu-id="a8ed6-111">Deliver</span></span>
- <span data-ttu-id="a8ed6-112">Osoa</span><span class="sxs-lookup"><span data-stu-id="a8ed6-112">Complete</span></span>
- <span data-ttu-id="a8ed6-113">Itxi</span><span class="sxs-lookup"><span data-stu-id="a8ed6-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="a8ed6-114">Berria</span><span class="sxs-lookup"><span data-stu-id="a8ed6-114">New</span></span>

<span data-ttu-id="a8ed6-115">Proiektu bat sortzen duzunean, proiektu fasea **Berria** gisa ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="a8ed6-116">Proiektua txantiloi batetik sortu bada, baliteke antolaketa, estimazioa eta taldeko datuak izatea.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="a8ed6-117">Bestela esanda, proiektuaren eskema besterik ez da, eta gainerako osagaiak sartu behar dira.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="a8ed6-118">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="a8ed6-118">Quote</span></span>

<span data-ttu-id="a8ed6-119">Proiektu bat eskaintza bati esleitzean edo proiektua eskaintza batetik sortzean, proiektuaren fasea **Eskaintza** gisa ezartzen da, eta estimatutako hasiera- eta amaiera-datak eguneratzen dira.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote** , and the estimated start and end dates are updated.</span></span> <span data-ttu-id="a8ed6-120">Proiektua **Eskaintza** fasean dagoen bitartean, **Proiektuaren entitatea** orriko **Salmentak** fitxak eskaintzaren xehetasunak erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="a8ed6-121">Plana</span><span class="sxs-lookup"><span data-stu-id="a8ed6-121">Plan</span></span>

<span data-ttu-id="a8ed6-122">Proiektu bati erlazionatuta dagoen eskaintza bat irabaztean, eta proiektua **Kontratuta** fasera mugitu bada, proiektuaren fasea **Antolatu** fasera eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="a8ed6-123">Proiektua **Antolatu** fasean dagoen bitartean, **Proiektuaren entitatea** orriak kontratuaren xehetasunak erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="a8ed6-124">Entregatu</span><span class="sxs-lookup"><span data-stu-id="a8ed6-124">Deliver</span></span>

<span data-ttu-id="a8ed6-125">Proiektuaren plana amaitutakoan eta proiektua hasteko prest zaudenean, proiektu-kudeatzaileak proiektuaren fasea eguneratu beharko luke **Entregatu** fasera proiektua hasi dela erakusteko.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="a8ed6-126">Osatu</span><span class="sxs-lookup"><span data-stu-id="a8ed6-126">Complete</span></span> 

<span data-ttu-id="a8ed6-127">Proiektuko lanak amaitutakoan, proiektu-kudeatzaileak fasea eguneratu dezake **Osatuta** fasera.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="a8ed6-128">Proiektuaren fasea **Osatuta** fasera eguneratuz gero, proiektu-kudeatzaileak lana ehuneko 100ean amaitu dela adierazi du, baina proiektua irekita mantentzen dela, zain dauden denbora- edo gastu-sarrerak erregistratu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-128">By updating the project stage to **Complete** , the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="a8ed6-129">Itxi</span><span class="sxs-lookup"><span data-stu-id="a8ed6-129">Close</span></span>

<span data-ttu-id="a8ed6-130">Proeikturako trantsakzio guztiak erregistratu direnean, proiektu-kudeatzaileak fasea eguneratu dezake **Itxi** fasera.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="a8ed6-131">Puntu horretan, ezin da transakziorik erregistratu, eta proiektua irakurtzeko soilik egongo da.</span><span class="sxs-lookup"><span data-stu-id="a8ed6-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>

