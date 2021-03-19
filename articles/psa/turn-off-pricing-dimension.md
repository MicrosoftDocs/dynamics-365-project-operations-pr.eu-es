---
title: Desaktibatu prezio-dimentsioa
description: Gai honek prezio-dimentsioak Project Service soluzioan nola ezarri erakusten du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 6e4b80b9c4b1b0f57d04079c9d2f84051b451d29
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281823"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="90ca9-103">Desaktibatu prezio-dimentsioa</span><span class="sxs-lookup"><span data-stu-id="90ca9-103">Turn off a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="90ca9-104">Baliteke prezioen estrategia berrikusi eta eguneratu behar izatea zenbait urtean behin.</span><span class="sxs-lookup"><span data-stu-id="90ca9-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="90ca9-105">Egin ditzakezun eguneratzeek lehendik dagoen prezio-dimentsioa desaktibatzea eta berri bat sortzea eska dezakete.</span><span class="sxs-lookup"><span data-stu-id="90ca9-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="90ca9-106">Adibidez, baliteke aurrez prezioa **Funtzioa** aukerare arabera jarrita izatean, baina orain prezioa **Lan esperientzia** aukeraren arabera jartzea erabaki duzu.</span><span class="sxs-lookup"><span data-stu-id="90ca9-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="90ca9-107">Horrek **Funtzioa** prezio-dimentsio gisa desaktibatzea eta pezio-dimentsio berri gisa **Lanaren esperientzia** sortzea eska diezazuke.</span><span class="sxs-lookup"><span data-stu-id="90ca9-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="90ca9-108">Prezio-dimentsio bat desaktibatzeko, aurretiaz prestatutakoa edo pertsonalizatua den kontuan izan gabe, ezarri prezio-dimentsioaren **Kostuari aplikagarria** eta **Salmentei aplikagarria** eremuak **Ez** gisa.</span><span class="sxs-lookup"><span data-stu-id="90ca9-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="90ca9-109">Hala ere, hau egiten duzunean, errore-mezu hau jaso dezakezu.</span><span class="sxs-lookup"><span data-stu-id="90ca9-109">However, when you do this, you might receive the following error message.</span></span>

![Prezio-dimentsio bat desaktibatzean ager daitekeen negozio-prozesuaren errorea](media/Business-Process-Error.png)


<span data-ttu-id="90ca9-111">Errore-mezu horrek desaktibatu nahi den dimentsiorako aurrez konfiguratutako prezioen erregistroak daudela adierazten du.</span><span class="sxs-lookup"><span data-stu-id="90ca9-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="90ca9-112">Dimentsio bati erreferentzia egiten dioten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** erregistro guztiak ezabatu egin behar dira dimentsioaren aplikagarritasuna **Ez** gisa ezarri ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="90ca9-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="90ca9-113">Arau hori aurretiaz prestatutako prezio-dimentsioei eta sortu ditzakezun prezio-dimentsio pertsonalizatuei aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="90ca9-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="90ca9-114">Balidazio horren arrazoia Project Service-k **Funtzio-prezioa** erregistro bakoitzak dimentsioen konbinazio esklusiboa izan behar duela zehaztu duela da.</span><span class="sxs-lookup"><span data-stu-id="90ca9-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="90ca9-115">Adibidez, **2018ko AEBetako kostu-tasak** izeneko prezio-zerrendan, honako **Funtzio-prezio** errenkada hauek dituzu.</span><span class="sxs-lookup"><span data-stu-id="90ca9-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="90ca9-116">Titulu estandarra</span><span class="sxs-lookup"><span data-stu-id="90ca9-116">Standard Title</span></span>         | <span data-ttu-id="90ca9-117">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="90ca9-117">Org Unit</span></span>    |<span data-ttu-id="90ca9-118">Unitatea</span><span class="sxs-lookup"><span data-stu-id="90ca9-118">Unit</span></span>   |<span data-ttu-id="90ca9-119">Prezioa</span><span class="sxs-lookup"><span data-stu-id="90ca9-119">Price</span></span>  |<span data-ttu-id="90ca9-120">Moneta</span><span class="sxs-lookup"><span data-stu-id="90ca9-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="90ca9-121">Sistemen ingeniaria</span><span class="sxs-lookup"><span data-stu-id="90ca9-121">Systems Engineer</span></span>|<span data-ttu-id="90ca9-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="90ca9-122">Contoso US</span></span>|<span data-ttu-id="90ca9-123">Hour</span><span class="sxs-lookup"><span data-stu-id="90ca9-123">Hour</span></span>| <span data-ttu-id="90ca9-124">100</span><span class="sxs-lookup"><span data-stu-id="90ca9-124">100</span></span>|<span data-ttu-id="90ca9-125">USD</span><span class="sxs-lookup"><span data-stu-id="90ca9-125">USD</span></span>|
| <span data-ttu-id="90ca9-126">Sistemen ingeniari nagusia</span><span class="sxs-lookup"><span data-stu-id="90ca9-126">Senior Systems Engineer</span></span>|<span data-ttu-id="90ca9-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="90ca9-127">Contoso US</span></span>|<span data-ttu-id="90ca9-128">Hour</span><span class="sxs-lookup"><span data-stu-id="90ca9-128">Hour</span></span>| <span data-ttu-id="90ca9-129">150</span><span class="sxs-lookup"><span data-stu-id="90ca9-129">150</span></span>| <span data-ttu-id="90ca9-130">USD</span><span class="sxs-lookup"><span data-stu-id="90ca9-130">USD</span></span>|


<span data-ttu-id="90ca9-131">**Titulu estandarra** prezio-dimentsio gisa desaktibatzen duzunean eta Project Service-ren prezioen motorrak prezioa bilatzen duenean, sarrerako testuinguruko **Erakunde-unitatea** balioa soilik erabiliko du.</span><span class="sxs-lookup"><span data-stu-id="90ca9-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="90ca9-132">Sarrerako testuinguruaren **Erakunde-unitatea** "Contoso US" bada, emaitza ez-determinista izango da bi errenkadak bat etorriko direlako.</span><span class="sxs-lookup"><span data-stu-id="90ca9-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="90ca9-133">Egoera hori ekiditeko, **Funtzio-prezioa** erregistroak sortzen dituzunean, Project Service-k dimentsioen konbinazioa esklusiboa dela balioztatzen du.</span><span class="sxs-lookup"><span data-stu-id="90ca9-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="90ca9-134">Dimentsioa **Funtzio-prezioa** erregistroak sortu ondoren desaktibatzen bada, muga hori urratu daiteke.</span><span class="sxs-lookup"><span data-stu-id="90ca9-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="90ca9-135">Hori dela eta, beharrezkoa da dimentsioa desaktibatu aurretik dimentsio-balio hori beteta duten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** errenkada guztiak ezabatzea.</span><span class="sxs-lookup"><span data-stu-id="90ca9-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]