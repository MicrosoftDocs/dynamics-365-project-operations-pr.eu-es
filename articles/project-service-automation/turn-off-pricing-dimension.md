---
title: Desaktibatu prezio-dimentsioa
description: Gai honek prezio-dimentsioak Project Service soluzioan nola ezarri erakusten du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 689e5a8d-e39a-471d-a6c4-7e2fc3bb5590
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 5cf2cd86fb1eba50c8e08b2bd624669ab0b1deb3
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748903"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="14398-103">Desaktibatu prezio-dimentsioa</span><span class="sxs-lookup"><span data-stu-id="14398-103">Turn off a pricing dimension</span></span>

<span data-ttu-id="14398-104">Baliteke prezioen estrategia berrikusi eta eguneratu behar izatea zenbait urtean behin.</span><span class="sxs-lookup"><span data-stu-id="14398-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="14398-105">Egin ditzakezun eguneratzeek lehendik dagoen prezio-dimentsioa desaktibatzea eta berri bat sortzea eska dezakete.</span><span class="sxs-lookup"><span data-stu-id="14398-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="14398-106">Adibidez, baliteke aurrez prezioa **Funtzioa** aukerare arabera jarrita izatean, baina orain prezioa **Lan esperientzia** aukeraren arabera jartzea erabaki duzu.</span><span class="sxs-lookup"><span data-stu-id="14398-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="14398-107">Horrek **Funtzioa** prezio-dimentsio gisa desaktibatzea eta pezio-dimentsio berri gisa **Lanaren esperientzia** sortzea eska diezazuke.</span><span class="sxs-lookup"><span data-stu-id="14398-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="14398-108">Prezio-dimentsio bat desaktibatzeko, aurretiaz prestatutakoa edo pertsonalizatua den kontuan izan gabe, ezarri prezio-dimentsioaren **Kostuari aplikagarria** eta **Salmentei aplikagarria** eremuak **Ez** gisa.</span><span class="sxs-lookup"><span data-stu-id="14398-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="14398-109">Hala ere, hau egiten duzunean, errore-mezu hau jaso dezakezu.</span><span class="sxs-lookup"><span data-stu-id="14398-109">However, when you do this, you might receive the following error message.</span></span>

![Prezio-dimentsio bat desaktibatzean ager daitekeen negozio-prozesuaren errorea](media/Business-Process-Error.png)


<span data-ttu-id="14398-111">Errore-mezu horrek desaktibatu nahi den dimentsiorako aurrez konfiguratutako prezioen erregistroak daudela adierazten du.</span><span class="sxs-lookup"><span data-stu-id="14398-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="14398-112">Dimentsio bati erreferentzia egiten dioten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** erregistro guztiak ezabatu egin behar dira dimentsioaren aplikagarritasuna **Ez** gisa ezarri ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="14398-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="14398-113">Arau hori aurretiaz prestatutako prezio-dimentsioei eta sortu ditzakezun prezio-dimentsio pertsonalizatuei aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="14398-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="14398-114">Balidazio horren arrazoia Project Service-k **Funtzio-prezioa** erregistro bakoitzak dimentsioen konbinazio esklusiboa izan behar duela zehaztu duela da.</span><span class="sxs-lookup"><span data-stu-id="14398-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="14398-115">Adibidez, **2018ko AEBetako kostu-tasak** izeneko prezio-zerrendan, honako **Funtzio-prezio** errenkada hauek dituzu.</span><span class="sxs-lookup"><span data-stu-id="14398-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="14398-116">Titulu estandarra</span><span class="sxs-lookup"><span data-stu-id="14398-116">Standard Title</span></span>         | <span data-ttu-id="14398-117">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="14398-117">Org Unit</span></span>    |<span data-ttu-id="14398-118">Unitatea</span><span class="sxs-lookup"><span data-stu-id="14398-118">Unit</span></span>   |<span data-ttu-id="14398-119">Prezioa</span><span class="sxs-lookup"><span data-stu-id="14398-119">Price</span></span>  |<span data-ttu-id="14398-120">Moneta</span><span class="sxs-lookup"><span data-stu-id="14398-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="14398-121">Sistemen ingeniaria</span><span class="sxs-lookup"><span data-stu-id="14398-121">Systems Engineer</span></span>|<span data-ttu-id="14398-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="14398-122">Contoso US</span></span>|<span data-ttu-id="14398-123">Hour</span><span class="sxs-lookup"><span data-stu-id="14398-123">Hour</span></span>| <span data-ttu-id="14398-124">100</span><span class="sxs-lookup"><span data-stu-id="14398-124">100</span></span>|<span data-ttu-id="14398-125">USD</span><span class="sxs-lookup"><span data-stu-id="14398-125">USD</span></span>|
| <span data-ttu-id="14398-126">Sistemen ingeniari nagusia</span><span class="sxs-lookup"><span data-stu-id="14398-126">Senior Systems Engineer</span></span>|<span data-ttu-id="14398-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="14398-127">Contoso US</span></span>|<span data-ttu-id="14398-128">Hour</span><span class="sxs-lookup"><span data-stu-id="14398-128">Hour</span></span>| <span data-ttu-id="14398-129">150</span><span class="sxs-lookup"><span data-stu-id="14398-129">150</span></span>| <span data-ttu-id="14398-130">USD</span><span class="sxs-lookup"><span data-stu-id="14398-130">USD</span></span>|


<span data-ttu-id="14398-131">**Titulu estandarra** prezio-dimentsio gisa desaktibatzen duzunean eta Project Service-ren prezioen motorrak prezioa bilatzen duenean, sarrerako testuinguruko **Erakunde-unitatea** balioa soilik erabiliko du.</span><span class="sxs-lookup"><span data-stu-id="14398-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="14398-132">Sarrerako testuinguruaren **Erakunde-unitatea** "Contoso US" bada, emaitza ez-determinista izango da bi errenkadak bat etorriko direlako.</span><span class="sxs-lookup"><span data-stu-id="14398-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="14398-133">Egoera hori ekiditeko, **Funtzio-prezioa** erregistroak sortzen dituzunean, Project Service-k dimentsioen konbinazioa esklusiboa dela balioztatzen du.</span><span class="sxs-lookup"><span data-stu-id="14398-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="14398-134">Dimentsioa **Funtzio-prezioa** erregistroak sortu ondoren desaktibatzen bada, muga hori urratu daiteke.</span><span class="sxs-lookup"><span data-stu-id="14398-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="14398-135">Hori dela eta, beharrezkoa da dimentsioa desaktibatu aurretik dimentsio-balio hori beteta duten **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** errenkada guztiak ezabatzea.</span><span class="sxs-lookup"><span data-stu-id="14398-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>

