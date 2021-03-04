---
title: Konfiguratu gastuak kudeatzeko lan-fluxuak
description: Bidaia eta gastuen dokumentuak berrikusi eta onartzeko lan-fluxuaren prozesua konfigura dezakezu.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8f3235d12499c68a52f9d1c7e118e7bc91dc3a0a
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960502"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="00c5e-103">Konfiguratu gastuak kudeatzeko lan-fluxuak</span><span class="sxs-lookup"><span data-stu-id="00c5e-103">Set up Expense management workflows</span></span>

<span data-ttu-id="00c5e-104">Bidaia eta gastuen dokumentuak berrikusi eta onartzeko erabiltzen den lan-fluxuaren prozesua konfigura dezakezu.</span><span class="sxs-lookup"><span data-stu-id="00c5e-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="00c5e-105">Lan-fluxuak definitzeko dokumentuek gastuen txostenak, bidaia eskakizunak eta dirua aurreratzeko eskaerak defini ditzakete.</span><span class="sxs-lookup"><span data-stu-id="00c5e-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="00c5e-106">Lan-fluxuak negozio-prozesua adierazten du.</span><span class="sxs-lookup"><span data-stu-id="00c5e-106">A workflow represents a business process.</span></span> <span data-ttu-id="00c5e-107">Dokumentu bat sisteman zehar nola igarotzen den zehazten du eta zeregin bat nork bete edo dokumentu bat onartu behar duen adierazten du.</span><span class="sxs-lookup"><span data-stu-id="00c5e-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="00c5e-108">Zure erakundeko lan-fluxuaren sistema erabiltzearen abantaila ugari daude:</span><span class="sxs-lookup"><span data-stu-id="00c5e-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="00c5e-109">**Prozesu koherenteak**: Dokumentu zehatzen onarpen prozesua defini dezakezu, hala nola erosketa eskaerak eta gastuen txostenak.</span><span class="sxs-lookup"><span data-stu-id="00c5e-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="00c5e-110">Lan-fluxuaren sistema erabiliz dokumentuak modu koherentean eta eraginkorrean prozesatu eta onartzen direla ziurtatzen da.</span><span class="sxs-lookup"><span data-stu-id="00c5e-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="00c5e-111">Prozesuaren ikusgaitasuna: Lan-fluxu instantzia jakin baten egoera, historia eta errendimendu-metrikak jarrai ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="00c5e-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="00c5e-112">Horrek lan-fluxuan aldaketak egin behar diren ala ez zehazten lagunduko dizu eraginkortasuna hobetzeko.</span><span class="sxs-lookup"><span data-stu-id="00c5e-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="00c5e-113">Lan zerrenda zentralizatua: Erabiltzaileek lan zerrenda zentralizatua ikus dezakete esleitutako lan fluxuen zereginak eta onarpenak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="00c5e-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="00c5e-114">**Sor ditzakezun la-fluxuen motak**</span><span class="sxs-lookup"><span data-stu-id="00c5e-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="00c5e-115">Ondorengo taulan sortu ditzakezun lan-fluxu motak zerrendatzen dira **Gastuak**.</span><span class="sxs-lookup"><span data-stu-id="00c5e-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="00c5e-116"><strong>Mota</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="00c5e-117"><strong>Erabili mota hau</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="00c5e-118"><strong>Gastuen txostena</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="00c5e-119">Sortu onespen lan-fluxuak gastuen txostenetarako.</span><span class="sxs-lookup"><span data-stu-id="00c5e-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="00c5e-120"><strong>Gastuen txostenen argitaratze automatikoa</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="00c5e-121">Sortu argitalpen automatikoko lan-fluxuak gastuen txostenetarako.</span><span class="sxs-lookup"><span data-stu-id="00c5e-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="00c5e-122"><strong>Gastuen lerroko elementua</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="00c5e-123">Sortu onespen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.</span><span class="sxs-lookup"><span data-stu-id="00c5e-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="00c5e-124"><strong>Gastuen lineako elementuak automatikoki argitaratzea</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="00c5e-125">Sortu argitalpen automatikoen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.</span><span class="sxs-lookup"><span data-stu-id="00c5e-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="00c5e-126"><strong>Bidaiatzeko eskakizuna</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="00c5e-127">Sortu onarpen-fluxuak bidaia-eskakizunetarako.</span><span class="sxs-lookup"><span data-stu-id="00c5e-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="00c5e-128"><strong>Diru-aurrerakinaren eskaera</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="00c5e-129">Sortu onarpen-fluxuak dirua aurreratzeko eskaeretarako.</span><span class="sxs-lookup"><span data-stu-id="00c5e-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="00c5e-130"><strong>BEZ zergaren berreskurapena</strong></span><span class="sxs-lookup"><span data-stu-id="00c5e-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="00c5e-131">Balio erantsiaren gaineko zerga (BEZ) berreskuratzeko onarpen-fluxuak sortu.</span><span class="sxs-lookup"><span data-stu-id="00c5e-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |

