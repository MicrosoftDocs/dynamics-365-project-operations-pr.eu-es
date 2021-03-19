---
title: Konfiguratu eskulanaren eta gastuen kostu estandarrak
description: Gai honetan eskulanaren kostu estandarrak eta proiektu bateko gastuak nola ezarri azaltzen da.
author: Yowelle
manager: AnnBe
ms.date: 08/02/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjCostPriceHour, ProjSalesPriceHour, ProjCostPriceExpense, ProjSalesPriceCost
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b16ed50584b2b4535d1c61fe7069708182a4820e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288319"
---
# <a name="configure-standard-costs-for-labor-and-expenses"></a><span data-ttu-id="3de01-103">Konfiguratu eskulanaren eta gastuen kostu estandarrak</span><span class="sxs-lookup"><span data-stu-id="3de01-103">Configure standard costs for labor and expenses</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="3de01-104">Gai honetan eskulanaren kostu estandarrak eta proiektu bateko gastuak nola ezarri azaltzen da.</span><span class="sxs-lookup"><span data-stu-id="3de01-104">This topic explains how to set up standard costs for labor and expenses for a project.</span></span> <span data-ttu-id="3de01-105">Zeregin honek USSI datu multzoa erabiltzen du.</span><span class="sxs-lookup"><span data-stu-id="3de01-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="3de01-106">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Konfigurazioa > Prezioak > Kostuaren prezioa (ordua)**.</span><span class="sxs-lookup"><span data-stu-id="3de01-106">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (hour)**.</span></span>
2. <span data-ttu-id="3de01-107">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="3de01-107">Select **New**.</span></span>
3. <span data-ttu-id="3de01-108">**Data eraginkorra** eremua, idatzi data.</span><span class="sxs-lookup"><span data-stu-id="3de01-108">In the **Effective date** field, enter a date.</span></span>
4. <span data-ttu-id="3de01-109">**Kostuaren prezioa** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="3de01-109">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="3de01-110">Proiektuaren kategoriarentzako kostu prezio estandarra ezar dezakezu edo kostu prezioa langile kopuruaren, proiektuaren zenbakiaren, kategoriaren, dataren edo horien edozein konbinazioen arabera ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="3de01-110">You can set up a standard cost price for the project category, or you can set up a cost price by worker number, project number, category, date, or any combination of these.</span></span> <span data-ttu-id="3de01-111">Aplikatzen den kostu prezioa xehetasun maila altuena duen kostua da.</span><span class="sxs-lookup"><span data-stu-id="3de01-111">The cost price that is applied is the cost price with the highest level of detail.</span></span>  
5. <span data-ttu-id="3de01-112">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="3de01-112">Select **Save**.</span></span>
6. <span data-ttu-id="3de01-113">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Konfigurazioa > Prezioak > Salmentaren prezioa (ordua)**.</span><span class="sxs-lookup"><span data-stu-id="3de01-113">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (hour)**.</span></span>
7. <span data-ttu-id="3de01-114">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="3de01-114">Select **New**.</span></span>
8. <span data-ttu-id="3de01-115">**Data eraginkorra** eremua, idatzi data.</span><span class="sxs-lookup"><span data-stu-id="3de01-115">In the **Effective date** field, enter a date.</span></span>
9. <span data-ttu-id="3de01-116">**Baliozkoa hurrengorako** eremuan, hautatu aukera bat.</span><span class="sxs-lookup"><span data-stu-id="3de01-116">In the **Valid for** field, select an option.</span></span>
10. <span data-ttu-id="3de01-117">**Prezioa** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="3de01-117">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="3de01-118">Salmenta prezio estandarra ezar dezakezu orduko transakzioetarako edo proiektu kategoria baterako.</span><span class="sxs-lookup"><span data-stu-id="3de01-118">You can set up a standard sales price for hour transactions or for a project category.</span></span> <span data-ttu-id="3de01-119">Salmenta prezioak ere ezar ditzakezu langile kopuruaren, proiektuaren zenbakiaren, kategoriaren, transakzio dataren edo horien edozein konbinazioen arabera.</span><span class="sxs-lookup"><span data-stu-id="3de01-119">You can also set up sales prices by worker number, project number, category, transaction date, or any combination of these.</span></span> <span data-ttu-id="3de01-120">Benetako salmenta prezioa, langileak Hour aldizkarian transakzio bat egiten duenean aplikatzen dena, xehetasun maila altueneko salmenta prezioa da.</span><span class="sxs-lookup"><span data-stu-id="3de01-120">The actual sales price, which is applied when a worker enters a transaction in the Hour journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="3de01-121">Adibidez, salmenta prezio orokorra eta langilearen berariazko salmenta prezioa ezartzen badira, langilearen berariazko salmenta prezioa erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="3de01-121">For example, if both a general sales price and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
11. <span data-ttu-id="3de01-122">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="3de01-122">Select **Save**.</span></span>
12. <span data-ttu-id="3de01-123">Itxi orria.</span><span class="sxs-lookup"><span data-stu-id="3de01-123">Close the page.</span></span>
13. <span data-ttu-id="3de01-124">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Konfigurazioa > Prezioak > Kostuaren prezioa (gastua)**.</span><span class="sxs-lookup"><span data-stu-id="3de01-124">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (expense)**.</span></span>
14. <span data-ttu-id="3de01-125">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="3de01-125">Select **New**.</span></span>
15. <span data-ttu-id="3de01-126">**Data eraginkorra** eremua, idatzi data.</span><span class="sxs-lookup"><span data-stu-id="3de01-126">In the **Effective date** field, enter a date.</span></span>
16. <span data-ttu-id="3de01-127">**Kostuaren prezioa** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="3de01-127">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="3de01-128">Eremu anitz bete daitezke, baina erregistroa gordetzeko behar den gutxienekoa da.</span><span class="sxs-lookup"><span data-stu-id="3de01-128">Multiple fields can be filled in, but this is the minimum needed to save the record.</span></span>  
17. <span data-ttu-id="3de01-129">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="3de01-129">Select **Save**.</span></span>
18. <span data-ttu-id="3de01-130">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Konfigurazioa > Prezioak > Salmentaren prezioa (gastua)**.</span><span class="sxs-lookup"><span data-stu-id="3de01-130">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (expense)**.</span></span>
19. <span data-ttu-id="3de01-131">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="3de01-131">Select **New**.</span></span>
20. <span data-ttu-id="3de01-132">**Data eraginkorra** eremua, idatzi data.</span><span class="sxs-lookup"><span data-stu-id="3de01-132">In the **Effective date** field, enter a date.</span></span>
21. <span data-ttu-id="3de01-133">**Baliozkoa hurrengorako** eremuan, hautatu aukera bat.</span><span class="sxs-lookup"><span data-stu-id="3de01-133">In the **Valid for** field, select an option.</span></span>
22. <span data-ttu-id="3de01-134">**Prezioa** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="3de01-134">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="3de01-135">Benetako salmenta prezioa, langileak gastuaren aldizkarian transakzioak egiten duenean aplikatzen dena, xehetasun maila altueneko salmenta prezioa da.</span><span class="sxs-lookup"><span data-stu-id="3de01-135">The actual sales price, which is applied when a worker enters transactions in an expense journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="3de01-136">Adibidez, orokorra eta langilearen berariazko salmenta prezioa ezartzen badira, langilearen berariazko salmenta prezioa erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="3de01-136">For example, if both a general and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
23. <span data-ttu-id="3de01-137">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="3de01-137">Select **Save**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]