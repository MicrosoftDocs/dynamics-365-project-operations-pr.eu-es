---
title: Konfiguratu Gastuak kudeatzeko lan-fluxuak
description: Bidaia eta gastuen dokumentuak berrikusi eta onartzeko erabiltzen den lan-fluxuaren prozesua konfigura dezakezu.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: dfc5945f32bb8d4073fc31499979ba279fef66a4
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896536"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="a5b61-103">Konfiguratu Gastuak kudeatzeko lan-fluxuak</span><span class="sxs-lookup"><span data-stu-id="a5b61-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="a5b61-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="a5b61-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a5b61-105">Bidaia eta gastuen dokumentuak berrikusi eta onartzeko lan-fluxuaren prozesua konfigura dezakezu.</span><span class="sxs-lookup"><span data-stu-id="a5b61-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="a5b61-106">Gastuen txostenak, bidaia eskakizunak eta dirua aurreratzeko eskaeren fluxuak defini ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="a5b61-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="a5b61-107">Lan-fluxuak negozio-prozesua adierazten du eta dokumentu bat sisteman zehar nola igarotzen den definitzen du.</span><span class="sxs-lookup"><span data-stu-id="a5b61-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="a5b61-108">Lan-fluxuak ere adierazten du nork bete behar duen edo dokumentu bat onartu behar duen.</span><span class="sxs-lookup"><span data-stu-id="a5b61-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="a5b61-109">Zure erakundeko lan-fluxuaren sistema erabiltzearen abantaila ugari daude:</span><span class="sxs-lookup"><span data-stu-id="a5b61-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="a5b61-110">**Prozesu koherenteak**: Dokumentu zehatzen onarpen prozesua defini dezakezu, hala nola erosketa eskaerak eta gastuen txostenak.</span><span class="sxs-lookup"><span data-stu-id="a5b61-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="a5b61-111">Lan-fluxuaren sistema erabiliz dokumentuak modu koherentean eta eraginkorrean prozesatu eta onartzen direla ziurtatzen da.</span><span class="sxs-lookup"><span data-stu-id="a5b61-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="a5b61-112">**Prozesuaren ikusgaitasuna**: Lan-fluxu instantzia jakin baten egoera, historia eta errendimendu-metrikak jarrai ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="a5b61-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="a5b61-113">Horrek lan-fluxuan aldaketak egin behar diren ala ez zehazten lagunduko dizu eraginkortasuna hobetzeko.</span><span class="sxs-lookup"><span data-stu-id="a5b61-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="a5b61-114">**Lan zerrenda zentralizatua**: Erabiltzaileek lan zerrenda zentralizatua ikus dezakete esleitutako lan fluxuen zereginak eta onarpenak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="a5b61-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="a5b61-115">Lan-fluxua motak</span><span class="sxs-lookup"><span data-stu-id="a5b61-115">Workflow types</span></span>

<span data-ttu-id="a5b61-116">Ondorengo taulan sortu ditzakezun lan-fluxu motak zerrendatzen dira **Gastuen kudeaketa**.</span><span class="sxs-lookup"><span data-stu-id="a5b61-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="a5b61-117"><strong>Mota</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="a5b61-118"><strong>Erabili mota hau</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="a5b61-119"><strong>Gastuen txostenen onespen automatikoa</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="a5b61-120">Sortu onespen lan-fluxuak gastuen txostenetarako.</span><span class="sxs-lookup"><span data-stu-id="a5b61-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="a5b61-121"><strong>Gastuen txostenen argitaratze automatikoa</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="a5b61-122">Sortu argitalpen automatikoko lan-fluxuak gastuen txostenetarako.</span><span class="sxs-lookup"><span data-stu-id="a5b61-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="a5b61-123"><strong>Gastuen lerroko elementua</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="a5b61-124">Sortu onespen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.</span><span class="sxs-lookup"><span data-stu-id="a5b61-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="a5b61-125"><strong>Gastuen lineako elementuak automatikoki argitaratzea</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="a5b61-126">Sortu argitalpen automatikoen lan-fluxuak gastuen txosteneko lerroaren elementuetarako.</span><span class="sxs-lookup"><span data-stu-id="a5b61-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="a5b61-127"><strong>Bidaiatzeko eskakizuna</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="a5b61-128">Sortu onarpen-fluxuak bidaia-eskakizunetarako.</span><span class="sxs-lookup"><span data-stu-id="a5b61-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="a5b61-129"><strong>Diru-aurrerakinaren eskaera</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="a5b61-130">Sortu onarpen-fluxuak dirua aurreratzeko eskaeretarako.</span><span class="sxs-lookup"><span data-stu-id="a5b61-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="a5b61-131"><strong>BEZ zergaren berreskurapena</strong></span><span class="sxs-lookup"><span data-stu-id="a5b61-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="a5b61-132">Balio erantsiaren gaineko zerga (BEZ) berreskuratzeko onarpen-fluxuak sortu.</span><span class="sxs-lookup"><span data-stu-id="a5b61-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |