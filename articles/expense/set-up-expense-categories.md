---
title: Konfiguratu gastu-kategoriak
description: Gai honek gastuen txostenak egiteko kategoria partekatuak eta kategoria partekatuak konfiguratzeko moduari buruzko informazioa eskaintzen du.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: f051d70f3dfe3b241dc0a206c0cdfda000f87c76
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896671"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="2afcd-103">Konfiguratu gastu-kategoriak</span><span class="sxs-lookup"><span data-stu-id="2afcd-103">Set up expense categories</span></span>

<span data-ttu-id="2afcd-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="2afcd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2afcd-105">Langileek gastuen txostenak sortzen dituztenean, erregistratzen duten gastu bakoitza gastu-kategoria batekin lotu behar da.</span><span class="sxs-lookup"><span data-stu-id="2afcd-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="2afcd-106">Gastuen kategoriak zure erakundeko pertsona juridikoetan parteka daitezkeen kategoria partekatuetatik eratortzen dira.</span><span class="sxs-lookup"><span data-stu-id="2afcd-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="2afcd-107">Zure erakundea nola definitzen den kontuan hartuta, gastu-kategoria hauek beste arlo batzuetan ere parteka daitezke.</span><span class="sxs-lookup"><span data-stu-id="2afcd-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="2afcd-108">Zure erakundearen definizioan eta ezarpen taldearen gidalerroetan oinarrituta, Gastuen kudeaketan erabiltzen diren kategoriak Gastuen kudeaketan soilik erabiliko diren edo beste arlo batzuetan partekatu behar diren zehaztu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="2afcd-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="2afcd-109">Kategoria horiek Proiektuen kudeaketa eta kontabilitate eta Gastuen kudeaketaren artean edo proiektuen kudeaketa eta kontabilitate eta Ekoizpenaren artean parteka daitezke.</span><span class="sxs-lookup"><span data-stu-id="2afcd-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="2afcd-110">Hala ere, ezin dira banatu Gastuen kudeaketaren eta produkzioaren artean.</span><span class="sxs-lookup"><span data-stu-id="2afcd-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="2afcd-111">Konfigurazio prozesua hasi aurretik, erabaki hauek hartu behar dira gastu kategoria bakoitzerako:</span><span class="sxs-lookup"><span data-stu-id="2afcd-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="2afcd-112">Zer da gastu-kategoria?</span><span class="sxs-lookup"><span data-stu-id="2afcd-112">What is the expense category?</span></span> <span data-ttu-id="2afcd-113">Adibide gisa, hegaldien, hotelaren edo kilometrajearen kategoriak daude.</span><span class="sxs-lookup"><span data-stu-id="2afcd-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="2afcd-114">Gastuen kategoria Proiektuen kudeaketan eta kontabilitatean ere erabil al daiteke?</span><span class="sxs-lookup"><span data-stu-id="2afcd-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="2afcd-115">Ahal bada, erabaki hauek ere hartu beharko dituzu:</span><span class="sxs-lookup"><span data-stu-id="2afcd-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="2afcd-116">Zein kostu kontu erabiliko dira ondorengo gastuetarako?</span><span class="sxs-lookup"><span data-stu-id="2afcd-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="2afcd-117">Kostua</span><span class="sxs-lookup"><span data-stu-id="2afcd-117">Cost</span></span>
        - <span data-ttu-id="2afcd-118">Nominen esleipena</span><span class="sxs-lookup"><span data-stu-id="2afcd-118">Payroll allocation</span></span>
        - <span data-ttu-id="2afcd-119">WIP - kostuaren balioa</span><span class="sxs-lookup"><span data-stu-id="2afcd-119">WIP-cost value</span></span>
        - <span data-ttu-id="2afcd-120">Kostua-elementua</span><span class="sxs-lookup"><span data-stu-id="2afcd-120">Cost-item</span></span>
        - <span data-ttu-id="2afcd-121">WIP-kostuaren balioa-elementua</span><span class="sxs-lookup"><span data-stu-id="2afcd-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="2afcd-122">Metatutako galera</span><span class="sxs-lookup"><span data-stu-id="2afcd-122">Accrued loss</span></span>
        - <span data-ttu-id="2afcd-123">WIP-metatutako galera</span><span class="sxs-lookup"><span data-stu-id="2afcd-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="2afcd-124">Zein diru-sarrera erabiliko dira diru-iturri hauek lortzeko?</span><span class="sxs-lookup"><span data-stu-id="2afcd-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="2afcd-125">Fakturatutako diru-sarrerak</span><span class="sxs-lookup"><span data-stu-id="2afcd-125">Invoiced revenue</span></span>
        - <span data-ttu-id="2afcd-126">Metatutako diru-sarrerak-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="2afcd-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="2afcd-127">WIP-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="2afcd-127">WIP-sales value</span></span>
        - <span data-ttu-id="2afcd-128">Metatutako diru-sarrerak-produkzioa</span><span class="sxs-lookup"><span data-stu-id="2afcd-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="2afcd-129">WIP-ekoizpena</span><span class="sxs-lookup"><span data-stu-id="2afcd-129">WIP-production</span></span>
        - <span data-ttu-id="2afcd-130">Metatutako diru-sarrerak-errentagarritasuna</span><span class="sxs-lookup"><span data-stu-id="2afcd-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="2afcd-131">WIP-irabaziak</span><span class="sxs-lookup"><span data-stu-id="2afcd-131">WIP-profit</span></span>
        - <span data-ttu-id="2afcd-132">Metatutako diru-sarrera-harpidetza</span><span class="sxs-lookup"><span data-stu-id="2afcd-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="2afcd-133">WIP-harpidetza</span><span class="sxs-lookup"><span data-stu-id="2afcd-133">WIP-subscription</span></span>

- <span data-ttu-id="2afcd-134">Zer da gastu mota?</span><span class="sxs-lookup"><span data-stu-id="2afcd-134">What is the expense type?</span></span>
- <span data-ttu-id="2afcd-135">Zein da gastu kategoriako ordainketa modu lehenetsia?</span><span class="sxs-lookup"><span data-stu-id="2afcd-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="2afcd-136">Gastu kategoriako gastuak banatu behar al dira?</span><span class="sxs-lookup"><span data-stu-id="2afcd-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="2afcd-137">Zein da gastu-kategoriako kontu lehenetsi nagusia?</span><span class="sxs-lookup"><span data-stu-id="2afcd-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="2afcd-138">Zein da gastuen kategorian lehenetsitako salmenten gaineko zerga taldea?</span><span class="sxs-lookup"><span data-stu-id="2afcd-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="2afcd-139">Ordainketa modu osagarriak onartzen al dira gastuen kategorian?</span><span class="sxs-lookup"><span data-stu-id="2afcd-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="2afcd-140">Hala bada, zer dira?</span><span class="sxs-lookup"><span data-stu-id="2afcd-140">If so, what are they?</span></span>
- <span data-ttu-id="2afcd-141">Ba al dago azpikategoririk gastu kategoria honetan?</span><span class="sxs-lookup"><span data-stu-id="2afcd-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="2afcd-142">Azpikategoriak badaude, erabaki hauek ere hartu beharko dituzu:</span><span class="sxs-lookup"><span data-stu-id="2afcd-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="2afcd-143">Zerga berreskuratzetik kanpo dago azpikategorietako bat?</span><span class="sxs-lookup"><span data-stu-id="2afcd-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="2afcd-144">Zein da azpikategorien salmenten gaineko zergaren taldea?</span><span class="sxs-lookup"><span data-stu-id="2afcd-144">What is the item sales tax group of the subcategories?</span></span>
