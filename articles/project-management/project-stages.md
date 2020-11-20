---
title: Proiektuaren faseak
description: Gai honek eskuragarri dauden proiektuen etapei buruzko informazioa eskaintzen du Microsoft Dynamics Project Operations-en.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: aa3d692a46165b01eafbd7619578cead8dd912d6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127458"
---
# <a name="project-stages"></a><span data-ttu-id="d60ce-103">Proiektuaren faseak</span><span class="sxs-lookup"><span data-stu-id="d60ce-103">Project stages</span></span>

<span data-ttu-id="d60ce-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="d60ce-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d60ce-105">Proiektuaren faseak diseinatu egiten dira proiektuaren egoera aurrera doan heinean.</span><span class="sxs-lookup"><span data-stu-id="d60ce-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="d60ce-106">Pertsonalizazioak faseak automatikoki eguneratzeko erabil daitezke negozio prozesuen fluxuekin, Power Automate edo plug-in luzapenak.</span><span class="sxs-lookup"><span data-stu-id="d60ce-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="d60ce-107">Hurrengo fase hauek negozio-prozesuaren fluxu lehenetsian zehazten dira:</span><span class="sxs-lookup"><span data-stu-id="d60ce-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="d60ce-108">Berria</span><span class="sxs-lookup"><span data-stu-id="d60ce-108">New</span></span>
- <span data-ttu-id="d60ce-109">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="d60ce-109">Quote</span></span>
- <span data-ttu-id="d60ce-110">Plana</span><span class="sxs-lookup"><span data-stu-id="d60ce-110">Plan</span></span>
- <span data-ttu-id="d60ce-111">Entregatu</span><span class="sxs-lookup"><span data-stu-id="d60ce-111">Deliver</span></span>
- <span data-ttu-id="d60ce-112">Osoa</span><span class="sxs-lookup"><span data-stu-id="d60ce-112">Complete</span></span>
- <span data-ttu-id="d60ce-113">Itxi</span><span class="sxs-lookup"><span data-stu-id="d60ce-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="d60ce-114">Berria</span><span class="sxs-lookup"><span data-stu-id="d60ce-114">New</span></span>

<span data-ttu-id="d60ce-115">Proiektu bat sortzen duzunean, proiektu fasea **Berria** gisa ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="d60ce-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="d60ce-116">Proiektua txantiloi batetik sortu bada, baliteke antolaketa, estimazioa eta taldeko datuak izatea.</span><span class="sxs-lookup"><span data-stu-id="d60ce-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="d60ce-117">Bestela esanda, proiektuaren eskema besterik ez da, eta gainerako osagaiak sartu behar dira.</span><span class="sxs-lookup"><span data-stu-id="d60ce-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="d60ce-118">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="d60ce-118">Quote</span></span>

<span data-ttu-id="d60ce-119">Proiektu bat eskaintza bati esleitzean edo proiektua eskaintza batetik sortzean, proiektuaren fasea **Eskaintza** gisa ezartzen da, eta estimatutako hasiera- eta amaiera-datak eguneratzen dira.</span><span class="sxs-lookup"><span data-stu-id="d60ce-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="d60ce-120">Proiektua **Eskaintza** fasean dagoen bitartean, **Proiektuaren entitatea** orriko **Salmentak** fitxak eskaintzaren xehetasunak erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="d60ce-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="d60ce-121">Plana</span><span class="sxs-lookup"><span data-stu-id="d60ce-121">Plan</span></span>

<span data-ttu-id="d60ce-122">Proiektu bati erlazionatuta dagoen eskaintza bat irabaztean, eta proiektua **Kontratuta** fasera mugitu bada, proiektuaren fasea **Antolatu** fasera eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="d60ce-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="d60ce-123">Proiektua **Antolatu** fasean dagoen bitartean, **Proiektuaren entitatea** orriak kontratuaren xehetasunak erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="d60ce-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="d60ce-124">Entregatu</span><span class="sxs-lookup"><span data-stu-id="d60ce-124">Deliver</span></span>

<span data-ttu-id="d60ce-125">Proiektuaren plana amaitutakoan eta proiektua hasteko prest zaudenean, proiektu-kudeatzaileak proiektuaren fasea eguneratu beharko luke **Entregatu** fasera proiektua hasi dela erakusteko.</span><span class="sxs-lookup"><span data-stu-id="d60ce-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="d60ce-126">Osatu</span><span class="sxs-lookup"><span data-stu-id="d60ce-126">Complete</span></span> 

<span data-ttu-id="d60ce-127">Proiektuko lanak amaitutakoan, proiektu-kudeatzaileak fasea eguneratu dezake **Osatuta** fasera.</span><span class="sxs-lookup"><span data-stu-id="d60ce-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="d60ce-128">Proiektuaren fasea **Osatuta** fasera eguneratuz gero, proiektu-kudeatzaileak lana ehuneko 100ean amaitu dela adierazi du, baina proiektua irekita mantentzen dela, zain dauden denbora- edo gastu-sarrerak erregistratu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="d60ce-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="d60ce-129">Itxi</span><span class="sxs-lookup"><span data-stu-id="d60ce-129">Close</span></span>

<span data-ttu-id="d60ce-130">Proeikturako trantsakzio guztiak erregistratu direnean, proiektu-kudeatzaileak fasea eguneratu dezake **Itxi** fasera.</span><span class="sxs-lookup"><span data-stu-id="d60ce-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="d60ce-131">Puntu horretan, ezin da transakziorik erregistratu, eta proiektua irakurtzeko soilik egongo da.</span><span class="sxs-lookup"><span data-stu-id="d60ce-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>

