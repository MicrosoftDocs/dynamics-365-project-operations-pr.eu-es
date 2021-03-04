---
title: Onartzaile ugari gastuen txosten batean
description: Gai honetan hainbat pertsonak onartzea eskatzen duten gastuen txostenen inguruko informazioa ematen da.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9b6d07f00fd6c1ba2d860787665d95f95f7b1a89
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960592"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="52e56-103">Onartzaile ugari gastuen txosten batean</span><span class="sxs-lookup"><span data-stu-id="52e56-103">Multiple approvers on an expense report</span></span>

<span data-ttu-id="52e56-104">Zure erakundearen gastuak onartzeko gidalerroen arabera, agian batek baino gehiagok onartu beharko dute langile batek bidalitako gastuen txostena.</span><span class="sxs-lookup"><span data-stu-id="52e56-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="52e56-105">Gastu-txostenak onartzeko lan-fluxuaren prozesua konfiguratzen duzunean, zereginak edo urratsak dituzten lan-fluxuko elementuak gehi ditzakezu gastu-txostenaren onartzaileentzako edo gehiagorentzat.</span><span class="sxs-lookup"><span data-stu-id="52e56-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="52e56-106">Adibidez, baliteke gastu-txosten guztiak lehenik txostena aurkeztu duen langilearen zuzendariak eta, ondoren, ordaindu beharreko kontuetako koordinatzaileak, onartzea.</span><span class="sxs-lookup"><span data-stu-id="52e56-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="52e56-107">Gastu-txostenen onarpen anitz behar izatea erabakitzen baduzu, lan-fluxuko elementuak modu hauetako batean gehi ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="52e56-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="52e56-108">Gehitu urrats bat duen onespen elementu bat.</span><span class="sxs-lookup"><span data-stu-id="52e56-108">Add one approval element that has one step.</span></span> <span data-ttu-id="52e56-109">Adibidez, urratsak gastu-txostena erabiltzaile talde bati esleitzea eta erabiltzaile taldeko kideen ehuneko 50ak onartzea eska dezake.</span><span class="sxs-lookup"><span data-stu-id="52e56-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="52e56-110">Gehitu hainbat urrats dituen onespen-elementu bat.</span><span class="sxs-lookup"><span data-stu-id="52e56-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="52e56-111">Adibidez, onarpen-elementuak urrats hauek izan ditzake:</span><span class="sxs-lookup"><span data-stu-id="52e56-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="52e56-112">Gastu txostena aurkeztu duen langilearen zuzendariak onartzen du.</span><span class="sxs-lookup"><span data-stu-id="52e56-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="52e56-113">Ordaindu beharreko kontuetako idazkariak egiaztagiriak eta gastuen txosteneko elementuak egiaztatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="52e56-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="52e56-114">Aurrekontuaren jabeak gastuen txostena onartzen du.</span><span class="sxs-lookup"><span data-stu-id="52e56-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="52e56-115">Gehitu onarpen elementu ugari, eta horietako bakoitzak urrats bat du.</span><span class="sxs-lookup"><span data-stu-id="52e56-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="52e56-116">Adibidez, urrats hauetako bakoitzerako beste onespen elementu bat gehi dezakezu:</span><span class="sxs-lookup"><span data-stu-id="52e56-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="52e56-117">Langilearen zuzendariak gastuen txostena onartzen du.</span><span class="sxs-lookup"><span data-stu-id="52e56-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="52e56-118">Aurrekontuaren jabeak gastuen txostena onartzen du.</span><span class="sxs-lookup"><span data-stu-id="52e56-118">The budget owner approves the expense report.</span></span>
