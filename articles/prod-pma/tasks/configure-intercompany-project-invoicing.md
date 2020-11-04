---
title: Konfiguratu enpresen arteko proiektuen fakturazioa
description: Gai honek proiektuaren fakturazioa zure erakundeko bi enpresen artean nola konfiguratu erakusten du.
author: Yowelle
manager: AnnBe
ms.date: 07/29/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendTable, InterCompanyTradingRelationSetupVendor, SysDataAreaSelectLookup, ProjParameters, ProjPosting, ProjTransferPrice
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 1cb53cb63ee11082146455ec9f13790501dc3d1d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071095"
---
# <a name="configure-intercompany-project-invoicing"></a><span data-ttu-id="57918-103">Konfiguratu enpresen arteko proiektuen fakturazioa</span><span class="sxs-lookup"><span data-stu-id="57918-103">Configure intercompany project invoicing</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="57918-104">Gai honek proiektuaren fakturazioa zure erakundeko bi enpresen artean nola konfiguratu erakusten du.</span><span class="sxs-lookup"><span data-stu-id="57918-104">This topic shows how to set up project invoicing between two companies in your organization.</span></span> <span data-ttu-id="57918-105">Zeregin honek USSI datu multzoa erabiltzen du.</span><span class="sxs-lookup"><span data-stu-id="57918-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="57918-106">Nabigazio panelean, joan hona: **Moduluak > Ordaindu beharreko kontuak > Saltzaileak > Saltzaile guztiak**.</span><span class="sxs-lookup"><span data-stu-id="57918-106">In the navigation pane, go to **Modules > Accounts payable > Vendors > All vendors**.</span></span>
2. <span data-ttu-id="57918-107">**Saltzaile guztiak** zerrendan, eta hautatu nahi duzun erregistroa.</span><span class="sxs-lookup"><span data-stu-id="57918-107">In the **All vendors** list, find and select the desired record.</span></span>
3. <span data-ttu-id="57918-108">Ekintza panelean, hautatu **Orokorra**.</span><span class="sxs-lookup"><span data-stu-id="57918-108">On the Action Pane, select **General**.</span></span>
4. <span data-ttu-id="57918-109">Aukeratu **Enpresa artekoa**.</span><span class="sxs-lookup"><span data-stu-id="57918-109">Select **Intercompany**.</span></span>
5. <span data-ttu-id="57918-110">Ezarri **Aktiboa** hurrengora **Bai** enpresen arteko merkataritza ahalbidetzeko.</span><span class="sxs-lookup"><span data-stu-id="57918-110">Set **Active** to **Yes** to enable intercompany trading.</span></span>
6. <span data-ttu-id="57918-111">**Bezeroaren konpainia** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="57918-111">In the **Customer company** field, enter or select a value.</span></span>
7. <span data-ttu-id="57918-112">**Nire kontua** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="57918-112">In the **My account** field, enter or select a value.</span></span>
8. <span data-ttu-id="57918-113">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="57918-113">Select **Save**.</span></span>
9. <span data-ttu-id="57918-114">Itxi orrialdeak hasierako orrialdera itzultzeko.</span><span class="sxs-lookup"><span data-stu-id="57918-114">Close the pages to return to the home page.</span></span>
10. <span data-ttu-id="57918-115">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Konfigurazioa > Proiektuaren kudeaketa eta kontuaren parametroak**.</span><span class="sxs-lookup"><span data-stu-id="57918-115">In the navigation pane, go to **Modules > Project management and accounting > Setup > Project management and accounting parameters**.</span></span>
11. <span data-ttu-id="57918-116">Hautatu **Enpresa artekoa** fitxa.</span><span class="sxs-lookup"><span data-stu-id="57918-116">Select the **Intercompany** tab.</span></span>
12. <span data-ttu-id="57918-117">Mugitu graduatzailea hona **Bai** enpresen arteko baliabideen programazioa eta denbora-orriak gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="57918-117">Move the slider to **Yes** to enable intercompany resource scheduling and timesheets.</span></span>
13. <span data-ttu-id="57918-118">Zerrendan, markatu hautatutako errenkada.</span><span class="sxs-lookup"><span data-stu-id="57918-118">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="57918-119">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="57918-119">Select **New**.</span></span>
15. <span data-ttu-id="57918-120">**Utzitako legezko entitatea** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="57918-120">In the **Borrowing legal entity** field, enter or select a value.</span></span>
16. <span data-ttu-id="57918-121">Hautatu **Ospearen irabazia** kontrol-laukia.</span><span class="sxs-lookup"><span data-stu-id="57918-121">Select the **Accrue revenue** check box.</span></span>
17. <span data-ttu-id="57918-122">**Lehenetsitako denbora-orriaren kategoria** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="57918-122">In the **Default timesheet category** field, enter or select a value.</span></span>
18. <span data-ttu-id="57918-123">**Lehenetsitako gastuaren kategoria** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="57918-123">In the **Default expense category** field, enter or select a value.</span></span>
19. <span data-ttu-id="57918-124">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="57918-124">Select **Save**.</span></span>
20. <span data-ttu-id="57918-125">Itxi orria.</span><span class="sxs-lookup"><span data-stu-id="57918-125">Close the page.</span></span>
21. <span data-ttu-id="57918-126">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Konfigurazioa > Argitaratzea > Liburu nagusia argitaratzeko konfigurazioa**.</span><span class="sxs-lookup"><span data-stu-id="57918-126">In the navigation pane, go to **Modules > Project management and accounting > Setup > Posting > Ledger posting setup**.</span></span>
22. <span data-ttu-id="57918-127">**Liburu kontuen motak** eremuan, hautatu aukera bat.</span><span class="sxs-lookup"><span data-stu-id="57918-127">In the **Ledger account types** field, select an option.</span></span>
23. <span data-ttu-id="57918-128">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="57918-128">Select **New**.</span></span>
24. <span data-ttu-id="57918-129">**Kontu nagusia** errenkada berriaren eremuan, zehaztu nahi dituzun balioak.</span><span class="sxs-lookup"><span data-stu-id="57918-129">In the **Main account** field of the new row, specify the desired values.</span></span>
25. <span data-ttu-id="57918-130">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="57918-130">Select **Save**.</span></span>
26. <span data-ttu-id="57918-131">Itxi orria.</span><span class="sxs-lookup"><span data-stu-id="57918-131">Close the page.</span></span>
27. <span data-ttu-id="57918-132">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Konfigurazioa > Prezioak > Transferentziaren prezioa**.</span><span class="sxs-lookup"><span data-stu-id="57918-132">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Transfer price**.</span></span>
28. <span data-ttu-id="57918-133">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="57918-133">Select **New**.</span></span>
29. <span data-ttu-id="57918-134">**Data eraginkorra** eremua, idatzi data.</span><span class="sxs-lookup"><span data-stu-id="57918-134">In the **Effective date** field, enter a date.</span></span>
30. <span data-ttu-id="57918-135">**Utzitako legezko entitatea** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="57918-135">In the **Borrowing legal entity** field, enter or select a value.</span></span>
31. <span data-ttu-id="57918-136">**Transferentziaren prezioaren eredua** eremuan, hautatu aukera bat.</span><span class="sxs-lookup"><span data-stu-id="57918-136">In the **Transfer price model** field, select an option.</span></span>
32. <span data-ttu-id="57918-137">**Prezioa** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="57918-137">In the **Pricing** field, enter a number.</span></span>
33. <span data-ttu-id="57918-138">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="57918-138">Select **Save**.</span></span>

