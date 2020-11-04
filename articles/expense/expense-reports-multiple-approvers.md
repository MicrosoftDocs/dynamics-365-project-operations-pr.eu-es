---
title: Gastuen txostenak eta hainbat onartzaile
description: Gai honetan pertsona batek baino gehiagok onartzea eskatzen duten gastuen txostenen inguruko informazioa ematen da.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 548673541cee5ce598721f94415c0444995c8325
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071039"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="ca8e0-103">Gastuen txostenak eta hainbat onartzaile</span><span class="sxs-lookup"><span data-stu-id="ca8e0-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="ca8e0-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="ca8e0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ca8e0-105">Zure erakundearen gastuak onartzeko gidalerroen arabera, agian batek baino gehiagok onartu beharko dute bidalitako gastuen txostena.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="ca8e0-106">Gastu-txostenak onartzeko lan-fluxuaren prozesua konfiguratzen duzunean, zereginak edo urratsak dituzten lan-fluxuko elementuak gehi ditzakezu gastu-txostenaren onartzaileentzako edo gehiagorentzat.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="ca8e0-107">Adibidez, baliteke gastu-txosten guztiak bi pertsonek, txostena aurkeztu duen langilearen zuzendariak eta ordaindu beharreko kontuetako koordinatzaileak, onartzea.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="ca8e0-108">Gastu-txostenen onarpen anitz behar izatea erabakitzen baduzu, lan-fluxuko elementuak modu hauetako batean gehi ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="ca8e0-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="ca8e0-109">Gehitu urrats bat duen onespen elementu bat.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-109">Add one approval element that has one step.</span></span> <span data-ttu-id="ca8e0-110">Adibidez, urratsak gastu-txostena erabiltzaile talde bati esleitzea eta erabiltzaile taldeko kideen ehuneko 50ak onartzea eska dezake.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="ca8e0-111">Gehitu hainbat urrats dituen onespen-elementu bat.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="ca8e0-112">Adibidez, onarpen-elementuak urrats hauek izan ditzake:</span><span class="sxs-lookup"><span data-stu-id="ca8e0-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="ca8e0-113">Gastu txostena aurkeztu duen langilearen zuzendariak onartzen du.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="ca8e0-114">Ordaindu beharreko kontuetako idazkariak egiaztagiriak eta gastuen txosteneko elementuak egiaztatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="ca8e0-115">Aurrekontuaren jabeak gastuen txostena onartzen du.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="ca8e0-116">Gehitu onarpen elementu ugari, eta horietako bakoitzak urrats bat du.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="ca8e0-117">Adibidez, urrats hauetako bakoitzerako beste onespen elementu bat gehi dezakezu:</span><span class="sxs-lookup"><span data-stu-id="ca8e0-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="ca8e0-118">Langilearen zuzendariak gastuen txostena onartzen du.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="ca8e0-119">Aurrekontuaren jabeak gastuen txostena onartzen du.</span><span class="sxs-lookup"><span data-stu-id="ca8e0-119">The budget owner approves the expense report.</span></span>
