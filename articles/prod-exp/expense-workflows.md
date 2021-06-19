---
title: Konfiguratu gastuak kudeatzeko lan-fluxuak
description: Bidaia eta gastuen dokumentuak berrikusi eta onartzeko lan-fluxuaren prozesua konfigura dezakezu.
author: ShylaThompson
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 4070b4fb5109464abdabbce971688fb881dfcf2c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005101"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="3495d-103">Konfiguratu gastuak kudeatzeko lan-fluxuak</span><span class="sxs-lookup"><span data-stu-id="3495d-103">Set up Expense management workflows</span></span>

<span data-ttu-id="3495d-104">Bidaia eta gastuen dokumentuak berrikusi eta onartzeko erabiltzen den lan-fluxuaren prozesua konfigura dezakezu.</span><span class="sxs-lookup"><span data-stu-id="3495d-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="3495d-105">Lan-fluxuak definitzeko dokumentuek gastuen txostenak, bidaia eskakizunak eta dirua aurreratzeko eskaerak defini ditzakete.</span><span class="sxs-lookup"><span data-stu-id="3495d-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="3495d-106">Lan-fluxuak negozio-prozesua adierazten du.</span><span class="sxs-lookup"><span data-stu-id="3495d-106">A workflow represents a business process.</span></span> <span data-ttu-id="3495d-107">Dokumentu bat sisteman zehar nola igarotzen den zehazten du eta zeregin bat nork bete edo dokumentu bat onartu behar duen adierazten du.</span><span class="sxs-lookup"><span data-stu-id="3495d-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="3495d-108">Zure erakundeko lan-fluxuaren sistema erabiltzearen abantaila ugari daude:</span><span class="sxs-lookup"><span data-stu-id="3495d-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="3495d-109">**Prozesu koherenteak**: Dokumentu zehatzen onarpen prozesua defini dezakezu, hala nola erosketa eskaerak eta gastuen txostenak.</span><span class="sxs-lookup"><span data-stu-id="3495d-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="3495d-110">Lan-fluxuaren sistema erabiliz dokumentuak modu koherentean eta eraginkorrean prozesatu eta onartzen direla ziurtatzen da.</span><span class="sxs-lookup"><span data-stu-id="3495d-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="3495d-111">Prozesuaren ikusgaitasuna: Lan-fluxu instantzia jakin baten egoera, historia eta errendimendu-metrikak jarrai ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="3495d-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="3495d-112">Horrek lan-fluxuan aldaketak egin behar diren ala ez zehazten lagunduko dizu eraginkortasuna hobetzeko.</span><span class="sxs-lookup"><span data-stu-id="3495d-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="3495d-113">Lan zerrenda zentralizatua: Erabiltzaileek lan zerrenda zentralizatua ikus dezakete esleitutako lan fluxuen zereginak eta onarpenak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="3495d-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="3495d-114">**Sor ditzakezun la-fluxuen motak**</span><span class="sxs-lookup"><span data-stu-id="3495d-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="3495d-115">Ondorengo taulan sortu ditzakezun lan-fluxu motak zerrendatzen dira **Gastuak**.</span><span class="sxs-lookup"><span data-stu-id="3495d-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="3495d-116"><strong>Mota</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="3495d-117"><strong>Erabili mota hau</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="3495d-118"><strong>Gastuen txostena</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="3495d-119">Sortu onespen lan-fluxuak gastuen txostenetarako.</span><span class="sxs-lookup"><span data-stu-id="3495d-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="3495d-120"><strong>Gastuen txostenen argitaratze automatikoa</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="3495d-121">Sortu argitalpen automatikoko lan-fluxuak gastuen txostenetarako.</span><span class="sxs-lookup"><span data-stu-id="3495d-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="3495d-122"><strong>Gastuen lerroko elementua</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="3495d-123">Sortu onespen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.</span><span class="sxs-lookup"><span data-stu-id="3495d-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="3495d-124"><strong>Gastuen lineako elementuak automatikoki argitaratzea</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="3495d-125">Sortu argitalpen automatikoen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.</span><span class="sxs-lookup"><span data-stu-id="3495d-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="3495d-126"><strong>Bidaiatzeko eskakizuna</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="3495d-127">Sortu onarpen-fluxuak bidaia-eskakizunetarako.</span><span class="sxs-lookup"><span data-stu-id="3495d-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="3495d-128"><strong>Diru-aurrerakinaren eskaera</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="3495d-129">Sortu onarpen-fluxuak dirua aurreratzeko eskaeretarako.</span><span class="sxs-lookup"><span data-stu-id="3495d-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="3495d-130"><strong>BEZ zergaren berreskurapena</strong></span><span class="sxs-lookup"><span data-stu-id="3495d-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="3495d-131">Balio erantsiaren gaineko zerga (BEZ) berreskuratzeko onarpen-fluxuak sortu.</span><span class="sxs-lookup"><span data-stu-id="3495d-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |



[!INCLUDE[footer-include](../includes/footer-banner.md)]