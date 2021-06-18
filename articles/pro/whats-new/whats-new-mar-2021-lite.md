---
title: 2021eko martxoko berrikuntzak - Project Operations-en inplementazio arina
description: Gai honek informazioa eskaintzen du 2021eko martxoaren Project Operations inplementazio arinaren bertsioan eskuragarri dauden kalitate-eguneratzeei buruz.
author: sigitac
ms.date: 03/03/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: efddb96b2cb428b9dc0488c32eb5670d01322bcb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993851"
---
# <a name="whats-new-march-2021---project-operations-lite-deployment"></a><span data-ttu-id="ac83a-103">2021eko martxoko berrikuntzak - Project Operations-en inplementazio arina</span><span class="sxs-lookup"><span data-stu-id="ac83a-103">What's new March 2021 - Project Operations lite deployment</span></span>

<span data-ttu-id="ac83a-104">_Honi aplikatzen zaio: Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="ac83a-104">_Applies To: Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="ac83a-105">Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:</span><span class="sxs-lookup"><span data-stu-id="ac83a-105">This topic applies to the following Dynamics 365 Project Operations components and versions:</span></span>

- <span data-ttu-id="ac83a-106">Project Operations Dataverse ingurunearen 4.8.0.91 bertsioa</span><span class="sxs-lookup"><span data-stu-id="ac83a-106">Project Operations on Dataverse environment version 4.8.0.91</span></span> 

## <a name="quality-updates"></a><span data-ttu-id="ac83a-107">Kalitatearen eguneratzeak</span><span class="sxs-lookup"><span data-stu-id="ac83a-107">Quality updates</span></span>

| <span data-ttu-id="ac83a-108">**Ezaugarrien eremua**</span><span class="sxs-lookup"><span data-stu-id="ac83a-108">**Feature area**</span></span> | <span data-ttu-id="ac83a-109">**Erreferentzia-zenbakia**</span><span class="sxs-lookup"><span data-stu-id="ac83a-109">**Reference number**</span></span> | <span data-ttu-id="ac83a-110">**Kalitatearen eguneratzea**</span><span class="sxs-lookup"><span data-stu-id="ac83a-110">**Quality update**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ac83a-111">Fakturazioa eta prezioak</span><span class="sxs-lookup"><span data-stu-id="ac83a-111">Billing and pricing</span></span> | <span data-ttu-id="ac83a-112">2133873</span><span class="sxs-lookup"><span data-stu-id="ac83a-112">2133873</span></span> | <span data-ttu-id="ac83a-113">**Unitatearen salmenta-prezioa** moneta-ikurraren bistaratzea konpondu da **Gastuen aurreikuspenak** saretan.</span><span class="sxs-lookup"><span data-stu-id="ac83a-113">Fixed the display of **Unit Sales Price** currency symbol in the **Expense Estimates** grid.</span></span> |
| <span data-ttu-id="ac83a-114">Fakturazioa eta prezioak</span><span class="sxs-lookup"><span data-stu-id="ac83a-114">Billing and pricing</span></span> | <span data-ttu-id="ac83a-115">2174616</span><span class="sxs-lookup"><span data-stu-id="ac83a-115">2174616</span></span> | <span data-ttu-id="ac83a-116">Aurrekontua irabazten denean, kontratuaren prezioen zerrenda pertsonalizatua aipatzen da aurrekontutik kopiatutako kontratu-lerroaren xehetasunetan.</span><span class="sxs-lookup"><span data-stu-id="ac83a-116">When a quote is won, the contract custom pricelist is referenced on contract line details that are copied from the quote.</span></span> |
| <span data-ttu-id="ac83a-117">Abaguneen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="ac83a-117">Opportunity Management</span></span> | <span data-ttu-id="ac83a-118">2167475</span><span class="sxs-lookup"><span data-stu-id="ac83a-118">2167475</span></span> | <span data-ttu-id="ac83a-119">Zergaren zenbateko finkoa fakturatu gabeko sarrera erreala sortu duen fakturan.</span><span class="sxs-lookup"><span data-stu-id="ac83a-119">Fixed tax amount in the correction invoice that originated an unbilled actual entry.</span></span> |
| <span data-ttu-id="ac83a-120">Abaguneen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="ac83a-120">Opportunity Management</span></span> | <span data-ttu-id="ac83a-121">2176285</span><span class="sxs-lookup"><span data-stu-id="ac83a-121">2176285</span></span> | <span data-ttu-id="ac83a-122">Zergaren zenbatekoa ez da salmenta kontratuaren / aurrekontuaren lerroaren xehetasunetatik kopiatzea kontratuaren / aurrekontuaren lerroaren xehetasunetara kopiatzeko.</span><span class="sxs-lookup"><span data-stu-id="ac83a-122">Tax amount must not be copied from sales contract/quote line details to cost contract/quote line details.</span></span> |
| <span data-ttu-id="ac83a-123">Abaguneen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="ac83a-123">Opportunity Management</span></span> | <span data-ttu-id="ac83a-124">2188079</span><span class="sxs-lookup"><span data-stu-id="ac83a-124">2188079</span></span> | <span data-ttu-id="ac83a-125">Ez da fakturazio arau zatirik sortu behar lanekoak ez diren kontratuetarako.</span><span class="sxs-lookup"><span data-stu-id="ac83a-125">Split billing rule must not be created for contracts that are not work-based.</span></span> |
| <span data-ttu-id="ac83a-126">Antolaketa eta jarraipena</span><span class="sxs-lookup"><span data-stu-id="ac83a-126">Planning and Tracking</span></span> | <span data-ttu-id="ac83a-127">2138853</span><span class="sxs-lookup"><span data-stu-id="ac83a-127">2138853</span></span> | <span data-ttu-id="ac83a-128">Proiektuaren kopia funtzioa eguneratu da, erreferentziazko zereginak helmugako proiektuan kopiatuko direla kalkulatzeko lerroak ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="ac83a-128">Project copy function updated to ensure expense estimate lines that reference tasks are copied to the destination project.</span></span> |
| <span data-ttu-id="ac83a-129">Antolaketa eta jarraipena</span><span class="sxs-lookup"><span data-stu-id="ac83a-129">Planning and Tracking</span></span> | <span data-ttu-id="ac83a-130">2173259</span><span class="sxs-lookup"><span data-stu-id="ac83a-130">2173259</span></span> | <span data-ttu-id="ac83a-131">Proiektuaren kopia funtzioa eguneratu da, bistaratzen ez duela ziurtatzeko **WBS kopiatzea** errore-mezua zenbait agertokitan.</span><span class="sxs-lookup"><span data-stu-id="ac83a-131">Project copy function updated to ensure it doesn't display the **Copying WBS** error message in certain scenarios.</span></span> |
| <span data-ttu-id="ac83a-132">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="ac83a-132">Time and Expense</span></span> | <span data-ttu-id="ac83a-133">2148910</span><span class="sxs-lookup"><span data-stu-id="ac83a-133">2148910</span></span> | <span data-ttu-id="ac83a-134">**Editatu sarrera** orriko bistaratze-arazoa konpondu da **Denbora-sarrera** saretan.</span><span class="sxs-lookup"><span data-stu-id="ac83a-134">Fixed display issue with the **Edit Entry** page in the **Time Entry** grid.</span></span> |
| <span data-ttu-id="ac83a-135">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="ac83a-135">Time and Expense</span></span> | <span data-ttu-id="ac83a-136">2159798</span><span class="sxs-lookup"><span data-stu-id="ac83a-136">2159798</span></span> | <span data-ttu-id="ac83a-137">Kontrol estuak onartutako gastuen sarrerak ezin direla editatu ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="ac83a-137">Tightened controls to ensure approved expense entries can't be edited.</span></span> |


