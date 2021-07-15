---
title: Diru sarreren ezagutzaren ikuspegi orokorra
description: Gai honek diru-sarreren ezagutzari buruzko informazioa eskaintzen du Project Operations-en.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: ab9b36b71223b1bcfe48de5f9b68b6fb6a98f388
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368011"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="69f58-103">Diru sarreren ezagutzaren ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="69f58-103">Revenue recognition overview</span></span>

<span data-ttu-id="69f58-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="69f58-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="69f58-105">Dynamics 365 Project Operations-en, diru-sarrerak ezagutzeko printzipioak aldatu egiten dira proiektu bat edo proiektuaren zati bat hautatutako fakturazio metodoaren arabera.</span><span class="sxs-lookup"><span data-stu-id="69f58-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="69f58-106">Gai honek diru-sarreren ezagutzari buruzko informazioa eskaintzen du Project Operations-en.</span><span class="sxs-lookup"><span data-stu-id="69f58-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="69f58-107">Denboraren eta materialen fakturazio-metodoa erabiliz kontabilizatutako transakzioak</span><span class="sxs-lookup"><span data-stu-id="69f58-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="69f58-108">Kostuen eta diru-sarreren aitorpena lotuta daude.</span><span class="sxs-lookup"><span data-stu-id="69f58-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="69f58-109">Transakzio kostua eta fakturatu gabeko salmentak [Project Operations Integration aldizkaria](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="69f58-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="69f58-110">Proiektuaren kostua eta diru-sarreren profilak fakturatu gabeko salmenten transakzioak liburu nagusian kontabilizatzen diren zehazten du.</span><span class="sxs-lookup"><span data-stu-id="69f58-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="69f58-111">**Diru sarrerak lortu** hautatuta badago, sistemak **WIP salmenten balioa** eta **Sarreren irabazien salmenten balioa** kontuak argitaratzean.</span><span class="sxs-lookup"><span data-stu-id="69f58-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="69f58-112">Hau metodo honen adibidea da.</span><span class="sxs-lookup"><span data-stu-id="69f58-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="69f58-113">Transakzio mota</span><span class="sxs-lookup"><span data-stu-id="69f58-113">Transaction type</span></span> | <span data-ttu-id="69f58-114">Zordunketa / Kreditua</span><span class="sxs-lookup"><span data-stu-id="69f58-114">Debit/Credit</span></span> | <span data-ttu-id="69f58-115">Kopurua</span><span class="sxs-lookup"><span data-stu-id="69f58-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="69f58-116">WIP-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="69f58-116">WIP Sales value</span></span> | <span data-ttu-id="69f58-117">Zordunketa</span><span class="sxs-lookup"><span data-stu-id="69f58-117">Debit</span></span> | <span data-ttu-id="69f58-118">100</span><span class="sxs-lookup"><span data-stu-id="69f58-118">100</span></span> |
  | <span data-ttu-id="69f58-119">Metatutako diru-sarrerak-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="69f58-119">Accrued revenue sales value</span></span> | <span data-ttu-id="69f58-120">Kreditua</span><span class="sxs-lookup"><span data-stu-id="69f58-120">Credit</span></span> | <span data-ttu-id="69f58-121">100</span><span class="sxs-lookup"><span data-stu-id="69f58-121">100</span></span> |

- <span data-ttu-id="69f58-122">Diru-sarrera ez da ezagutu fakturazioan.</span><span class="sxs-lookup"><span data-stu-id="69f58-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="69f58-123">Sistemak **Fakturatutako diru-sarrerak** kontua argitaratzean.</span><span class="sxs-lookup"><span data-stu-id="69f58-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="69f58-124">Hau metodo honen adibidea da.</span><span class="sxs-lookup"><span data-stu-id="69f58-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="69f58-125">Transakzio mota</span><span class="sxs-lookup"><span data-stu-id="69f58-125">Transaction type</span></span> | <span data-ttu-id="69f58-126">Zordunketa / Kreditua</span><span class="sxs-lookup"><span data-stu-id="69f58-126">Debit/Credit</span></span> | <span data-ttu-id="69f58-127">Kopurua</span><span class="sxs-lookup"><span data-stu-id="69f58-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="69f58-128">Bezeroen saldoa</span><span class="sxs-lookup"><span data-stu-id="69f58-128">Customer balance</span></span> | <span data-ttu-id="69f58-129">Zordunketa</span><span class="sxs-lookup"><span data-stu-id="69f58-129">Debit</span></span> | <span data-ttu-id="69f58-130">120</span><span class="sxs-lookup"><span data-stu-id="69f58-130">120</span></span> |
  | <span data-ttu-id="69f58-131">Salmenten zerga-ordaingarria</span><span class="sxs-lookup"><span data-stu-id="69f58-131">Sales tax payable</span></span> | <span data-ttu-id="69f58-132">Kreditua</span><span class="sxs-lookup"><span data-stu-id="69f58-132">Credit</span></span> | <span data-ttu-id="69f58-133">20</span><span class="sxs-lookup"><span data-stu-id="69f58-133">20</span></span> |
  | <span data-ttu-id="69f58-134">Fakturatutako diru-sarrerak</span><span class="sxs-lookup"><span data-stu-id="69f58-134">Invoiced Revenue</span></span> | <span data-ttu-id="69f58-135">Kreditua</span><span class="sxs-lookup"><span data-stu-id="69f58-135">Credit</span></span> | <span data-ttu-id="69f58-136">100</span><span class="sxs-lookup"><span data-stu-id="69f58-136">100</span></span> |

- <span data-ttu-id="69f58-137">Sarrerak fakturatu gabeko salmentak argitaratzen direnean metatzen badira, sistemak fakturatutakoan itzuliko ditu sortutako diru sarrerak.</span><span class="sxs-lookup"><span data-stu-id="69f58-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="69f58-138">Transakzio mota</span><span class="sxs-lookup"><span data-stu-id="69f58-138">Transaction type</span></span> | <span data-ttu-id="69f58-139">Zordunketa / Kreditua</span><span class="sxs-lookup"><span data-stu-id="69f58-139">Debit/Credit</span></span> | <span data-ttu-id="69f58-140">Kopurua</span><span class="sxs-lookup"><span data-stu-id="69f58-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="69f58-141">WIP-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="69f58-141">WIP Sales value</span></span> | <span data-ttu-id="69f58-142">Kreditua</span><span class="sxs-lookup"><span data-stu-id="69f58-142">Credit</span></span> | <span data-ttu-id="69f58-143">100</span><span class="sxs-lookup"><span data-stu-id="69f58-143">100</span></span> |
  | <span data-ttu-id="69f58-144">Metatutako diru-sarrerak-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="69f58-144">Accrued revenue sales value</span></span> | <span data-ttu-id="69f58-145">Zordunketa</span><span class="sxs-lookup"><span data-stu-id="69f58-145">Debit</span></span> | <span data-ttu-id="69f58-146">100</span><span class="sxs-lookup"><span data-stu-id="69f58-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="69f58-147">Prezio finkoko fakturazio-metodoa erabiliz kontabilizatutako transakzioak</span><span class="sxs-lookup"><span data-stu-id="69f58-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="69f58-148">Kostuen eta diru-sarreren aitorpena bereizita daude.</span><span class="sxs-lookup"><span data-stu-id="69f58-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="69f58-149">Transakzio kostua [Project Operations Integration aldizkaria](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="69f58-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="69f58-150">Fakturatu gabeko salmenta transakzioak ez dira sortzen.</span><span class="sxs-lookup"><span data-stu-id="69f58-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="69f58-151">Diru-sarrerak fakturatzerakoan antzeman daitezke proiektuaren kostua eta diru-sarreren profila badituzte **Proiektua amaitzeko kalkuluetarako erabilitako printzipioa** ezarri **WIP ez**.</span><span class="sxs-lookup"><span data-stu-id="69f58-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="69f58-152">Erabili metodo hau epe laburreko proiektu sinpleetarako.</span><span class="sxs-lookup"><span data-stu-id="69f58-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="69f58-153">Diru-sarrerak prezio finkoko diru-sarreren kalkuluen bidez aitortu daitezke **Bukatutako kontratua** edo **Osatutako ehunekoen sarreren aitorpena** metodoa.</span><span class="sxs-lookup"><span data-stu-id="69f58-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="69f58-154">Baliabide gehigarriak</span><span class="sxs-lookup"><span data-stu-id="69f58-154">Additional resources</span></span>
[<span data-ttu-id="69f58-155">Konfiguratu proiektu fakturagarrien kontabilitatearen artikulua</span><span class="sxs-lookup"><span data-stu-id="69f58-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="69f58-156">Prezio finkoko diru-sarrerak kalkulatzeko proiektuak</span><span class="sxs-lookup"><span data-stu-id="69f58-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="69f58-157">Kudeatu diru-sarreren kalkuluak</span><span class="sxs-lookup"><span data-stu-id="69f58-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="69f58-158">Metodoak osatzeko kostua</span><span class="sxs-lookup"><span data-stu-id="69f58-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]