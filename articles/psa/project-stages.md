---
title: Proiektuaren fase motak
description: Gai honek proiektuaren faseei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: 3503b17e54fc0b321582c30ce534e4cb3f497a5f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283668"
---
# <a name="project-stage-types"></a><span data-ttu-id="af84f-103">Proiektuaren fase motak</span><span class="sxs-lookup"><span data-stu-id="af84f-103">Project stage types</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="af84f-104">Proiektuaren faseak diseinatu egiten dira proiektuaren egoera aurrera doan heinean.</span><span class="sxs-lookup"><span data-stu-id="af84f-104">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="af84f-105">Pertsonalizazioak faseak automatikoki eguneratzeko erabil daitezke negozio prozesuen fluxuekin, Power Automate edo plug-in luzapenak.</span><span class="sxs-lookup"><span data-stu-id="af84f-105">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="af84f-106">Hurrengo fase hauek BPF lehenetsian zehazten dira:</span><span class="sxs-lookup"><span data-stu-id="af84f-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="af84f-107">Berria</span><span class="sxs-lookup"><span data-stu-id="af84f-107">New</span></span>
- <span data-ttu-id="af84f-108">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="af84f-108">Quote</span></span>
- <span data-ttu-id="af84f-109">Plana</span><span class="sxs-lookup"><span data-stu-id="af84f-109">Plan</span></span>
- <span data-ttu-id="af84f-110">Entregatu</span><span class="sxs-lookup"><span data-stu-id="af84f-110">Deliver</span></span>
- <span data-ttu-id="af84f-111">Osatu</span><span class="sxs-lookup"><span data-stu-id="af84f-111">Complete</span></span>
- <span data-ttu-id="af84f-112">Itxi</span><span class="sxs-lookup"><span data-stu-id="af84f-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="af84f-113">Berria</span><span class="sxs-lookup"><span data-stu-id="af84f-113">New</span></span>

<span data-ttu-id="af84f-114">Proiektu bat sortzen duzunean, proiektu fasea **Berria** gisa ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="af84f-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="af84f-115">Proiektua txantiloi batetik sortu bada, baliteke antolaketa, estimazioa eta taldeko datuak izatea.</span><span class="sxs-lookup"><span data-stu-id="af84f-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="af84f-116">Bestela esanda, proiektuaren eskema besterik ez da, eta gainerako osagaiak sartu behar dira.</span><span class="sxs-lookup"><span data-stu-id="af84f-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="af84f-117">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="af84f-117">Quote</span></span>

<span data-ttu-id="af84f-118">Proiektu bat eskaintza bati esleitzean edo proiektua eskaintza batetik sortzean, proiektuaren fasea **Eskaintza** gisa ezartzen da, eta estimatutako hasiera- eta amaiera-datak eguneratzen dira.</span><span class="sxs-lookup"><span data-stu-id="af84f-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="af84f-119">Proiektua **Eskaintza** fasean dagoen bitartean, **Proiektuaren entitatea** orriko **Salmentak** fitxak eskaintzaren xehetasunak erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="af84f-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="af84f-120">Plana</span><span class="sxs-lookup"><span data-stu-id="af84f-120">Plan</span></span>

<span data-ttu-id="af84f-121">Proiektu bati erlazionatuta dagoen eskaintza bat irabaztean, eta proiektua **Kontratuta** fasera mugitu bada, proiektuaren fasea **Antolatu** fasera eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="af84f-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="af84f-122">Proiektua **Antolatu** fasean dagoen bitartean, **Proiektuaren entitatea** orriak kontratuaren xehetasunak erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="af84f-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="af84f-123">Entregatu</span><span class="sxs-lookup"><span data-stu-id="af84f-123">Deliver</span></span>

<span data-ttu-id="af84f-124">Proiektuaren plana amaitutakoan eta proiektua hasteko prest zaudenean, proiektu-kudeatzaileak proiektuaren fasea eguneratu beharko luke **Entregatu** fasera proiektua hasi dela erakusteko.</span><span class="sxs-lookup"><span data-stu-id="af84f-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="af84f-125">Osatu</span><span class="sxs-lookup"><span data-stu-id="af84f-125">Complete</span></span> 

<span data-ttu-id="af84f-126">Proiektuko lanak amaitutakoan, proiektu-kudeatzaileak fasea eguneratu dezake **Osatuta** fasera.</span><span class="sxs-lookup"><span data-stu-id="af84f-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="af84f-127">Proiektuaren fasea **Osatuta** fasera eguneratuz gero, proiektu-kudeatzaileak lana ehuneko 100ean amaitu dela adierazi du, baina proiektua irekita mantentzen dela, zain dauden denbora- edo gastu-sarrerak erregistratu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="af84f-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="af84f-128">Itxi</span><span class="sxs-lookup"><span data-stu-id="af84f-128">Close</span></span>

<span data-ttu-id="af84f-129">Proeikturako trantsakzio guztiak erregistratu direnean, proiektu-kudeatzaileak fasea eguneratu dezake **Itxi** fasera.</span><span class="sxs-lookup"><span data-stu-id="af84f-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="af84f-130">Puntu horretan, ezin da transakziorik erregistratu, eta proiektua irakurtzeko soilik egongo da.</span><span class="sxs-lookup"><span data-stu-id="af84f-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]