---
title: Gastuen kudeaketaren lan-fluxua
description: Gai honek lan fluxuaren sistema nola erabil dezakezun azaltzen du Microsoft Dynamics 365 Finance, Gastuen kudeaketan gastuen txostenak berrikusteko prozesua ezartzeko.
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
ms.openlocfilehash: bbee90450749c89f643d96e4d41a387c45e9abc5
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960547"
---
# <a name="expense-management-workflow"></a><span data-ttu-id="451d1-103">Gastuen kudeaketaren lan-fluxua</span><span class="sxs-lookup"><span data-stu-id="451d1-103">Expense management workflow</span></span>

<span data-ttu-id="451d1-104">Fluxuaren sistema erabil dezakezu, Gastuen kudeaketan gastuen txostenak berrikusteko prozesua ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="451d1-104">You can use the workflow system to set up a review process for expense reports in Expense management.</span></span> <span data-ttu-id="451d1-105">Gastu txostenak nork onartzen dituen zehazteko irizpide hauek erabiltzen dituen lan fluxua konfigura dezakezu:</span><span class="sxs-lookup"><span data-stu-id="451d1-105">You can set up a workflow that uses the following criteria to determine who approves expense reports:</span></span>

- <span data-ttu-id="451d1-106">Langilearen berri emateko hierarkia eta aurrez definitutako onarpen mugak</span><span class="sxs-lookup"><span data-stu-id="451d1-106">The employee reporting hierarchy and predefined approval limits</span></span>
- <span data-ttu-id="451d1-107">Behin-behineko onartzaileak eta behin betiko onartzailea onartzen dituen maila anitzeko onespena</span><span class="sxs-lookup"><span data-stu-id="451d1-107">Multi-level approval that supports interim approvers and a final approver</span></span>
- <span data-ttu-id="451d1-108">Finantza dimentsioak eta proiektuaren erantzukizuna</span><span class="sxs-lookup"><span data-stu-id="451d1-108">Financial dimensions and project responsibility</span></span>
- <span data-ttu-id="451d1-109">Erabiltzaile edo erabiltzaile talde jakin batzuei esleitzea</span><span class="sxs-lookup"><span data-stu-id="451d1-109">Assignment to specific users or user groups</span></span>

<span data-ttu-id="451d1-110">Lan-fluxuen onarpenak sor daitezke gastuen txostenak, bidaia-eskaerak, dirua aurreratzeko eta balio erantsiaren gaineko zergaren (BEZ) berreskurapenetarako.</span><span class="sxs-lookup"><span data-stu-id="451d1-110">Workflow approvals can be created for expense reports, travel requisitions, cash advances, and value-added tax (VAT) recovery.</span></span>

<span data-ttu-id="451d1-111">**Adibidez**</span><span class="sxs-lookup"><span data-stu-id="451d1-111">**Example**</span></span>

<span data-ttu-id="451d1-112">Hurrengo prozesua gastu-txosten baten kudeaketa-fluxuaren adibidea da.</span><span class="sxs-lookup"><span data-stu-id="451d1-112">The following process is an example of the expense management workflow for an expense report.</span></span>

1. <span data-ttu-id="451d1-113">Langile batek gastuen txostena sortu eta gordetzen du.</span><span class="sxs-lookup"><span data-stu-id="451d1-113">An employee creates and saves an expense report.</span></span>
2. <span data-ttu-id="451d1-114">Langilearen gastuen txostena bidaltzen du onartzeko.</span><span class="sxs-lookup"><span data-stu-id="451d1-114">The employee submits the expense report for approval.</span></span> <span data-ttu-id="451d1-115">Onartzailea lan-fluxua konfiguratu zenean definitutako arauetan oinarrituta identifikatzen da.</span><span class="sxs-lookup"><span data-stu-id="451d1-115">The approver is identified based on the rules that were defined when the workflow was set up.</span></span>
3. <span data-ttu-id="451d1-116">Onartzaileak gastuen txostena onartzeko prest dagoela jakinarazten dio.</span><span class="sxs-lookup"><span data-stu-id="451d1-116">The approver receives a notification that an expense report is ready for approval.</span></span> <span data-ttu-id="451d1-117">Onartzaileak gastuen txostena aztertzen du eta baldintza hauek betetzen direla egiaztatzen du:</span><span class="sxs-lookup"><span data-stu-id="451d1-117">The approver reviews the expense report and verifies that the following conditions are met:</span></span>

    - <span data-ttu-id="451d1-118">Gastuek ez dute inolako gastu politikarik urratzen.</span><span class="sxs-lookup"><span data-stu-id="451d1-118">The expenses don't violate any expense policies.</span></span> <span data-ttu-id="451d1-119">Gastu batek politika bat urratzen badu, onartzaileak egiaztatzen du gastuen txostenak baliozko negozio justifikazioa duela.</span><span class="sxs-lookup"><span data-stu-id="451d1-119">If an expense violates a policy, the approver verifies that the expense report includes a valid business justification.</span></span>
    - <span data-ttu-id="451d1-120">Ordainagiri elektronikoak gastuen txostenari eransten zaizkio.</span><span class="sxs-lookup"><span data-stu-id="451d1-120">Electronic receipts are attached to the expense report.</span></span>

4. <span data-ttu-id="451d1-121">Onesleak gastuen txostena onartzen du.</span><span class="sxs-lookup"><span data-stu-id="451d1-121">The approver approves the expense report.</span></span>
5. <span data-ttu-id="451d1-122">Gastuen txostena Kobratu beharreko kontuen koordinatzaileari esleitzen zaio argitaratzeagatik.</span><span class="sxs-lookup"><span data-stu-id="451d1-122">The expense report is assigned to the Accounts payable coordinator for posting.</span></span>
6. <span data-ttu-id="451d1-123">Urrats hauetako bat gertatzen da, argitaratze automatikoa konfiguratuta dagoen ala ez kontuan hartuta:</span><span class="sxs-lookup"><span data-stu-id="451d1-123">One of the following steps occurs, depending on whether automatic posting is configured:</span></span>

    - <span data-ttu-id="451d1-124">Bidalketa automatikoa konfiguratzen bada, gastuen txostena ordaintzeko prozesatuko da eta gastuen txostenaren egoera eguneratuko da.</span><span class="sxs-lookup"><span data-stu-id="451d1-124">If automatic posting is configured, the expense report is processed for payment, and the status of the expense report is updated.</span></span>
    - <span data-ttu-id="451d1-125">Bidalketa automatikoa konfiguratuta ez badago, ordaindu beharreko Kontuen koordinatzaileak egiaztatzen du jatorrizko ordainagiri guztiak aurkeztu direla eta ordainagiriak gastuen txosteneko gastuekin bat datozela.</span><span class="sxs-lookup"><span data-stu-id="451d1-125">If automatic posting isn't configured, the Accounts payable coordinator verifies that all original receipts have been submitted, and that the receipts are aligned with the expenses on the expense report.</span></span> <span data-ttu-id="451d1-126">Gastu txostenean sartutako zerga kode guztiak zuzenak direla ere egiaztatu behar da.</span><span class="sxs-lookup"><span data-stu-id="451d1-126">All tax codes that are entered on the expense report must also be verified as correct.</span></span>

<span data-ttu-id="451d1-127">Baldintza horiek egiaztatu ondoren, gastuen txostena argitaratuko da.</span><span class="sxs-lookup"><span data-stu-id="451d1-127">After these requirements are verified, the expense report is posted.</span></span>

<span data-ttu-id="451d1-128">Gastuen txostena argitaratu ondoren, gastuen txostena ordaintzeko baimena ematen da eta langileari itzulketa egiten zaio.</span><span class="sxs-lookup"><span data-stu-id="451d1-128">After the expense report is posted, payment is authorized for the expense report, and the employee is reimbursed.</span></span>
