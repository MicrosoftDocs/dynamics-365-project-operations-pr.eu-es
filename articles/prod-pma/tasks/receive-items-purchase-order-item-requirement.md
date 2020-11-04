---
title: Jaso erosketa eskaeran elementuak eskakizunetik
description: Gai honetan artikuluaren baldintza batetik erosketa-eskaera bateko artikuluak nola jaso azaltzen da.
author: Yowelle
manager: AnnBe
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: a5b3622458da957ed150311f6ea75d5f1444d5f1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071203"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="63402-103">Jaso erosketa eskaeran elementuak eskakizunetik</span><span class="sxs-lookup"><span data-stu-id="63402-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="63402-104">Gai honetan artikuluaren baldintza batetik erosketa-eskaera bateko artikuluak nola jaso azaltzen da.</span><span class="sxs-lookup"><span data-stu-id="63402-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="63402-105">Artikuluaren transakzioaren ordez elementuaren eskakizuna erabiliz gero, elementua benetan erabili aurretik entregatzeko asmoa dezakezu, erosketa-agindua sortu, artikulua merkataritza-akordioaren esparruan sartu eta produktuaren eskakizuna produkzioaren plangintzan sartu.</span><span class="sxs-lookup"><span data-stu-id="63402-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="63402-106">Zeregin honek USSI datu multzoa erabiltzen du.</span><span class="sxs-lookup"><span data-stu-id="63402-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="63402-107">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Proiektuak > Proiektu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="63402-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="63402-108">Zerrendan, hautatu desiratutako errenkadako estekan.</span><span class="sxs-lookup"><span data-stu-id="63402-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="63402-109">Ekintza panelean, hautatu **Plana**.</span><span class="sxs-lookup"><span data-stu-id="63402-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="63402-110">Aukeratu **Elementuen eskakizunak**.</span><span class="sxs-lookup"><span data-stu-id="63402-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="63402-111">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="63402-111">Select **New**.</span></span>
6. <span data-ttu-id="63402-112">Errenkada berrian, sartu edo hautatu balio bat **Elementuaren zenbakia** eremua.</span><span class="sxs-lookup"><span data-stu-id="63402-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="63402-113">**Kantitatea** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="63402-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="63402-114">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="63402-114">Select **Save**.</span></span>
9. <span data-ttu-id="63402-115">Ekintza panelean, hautatu **Kudeatu**.</span><span class="sxs-lookup"><span data-stu-id="63402-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="63402-116">Hautatu **Funtzioak**.</span><span class="sxs-lookup"><span data-stu-id="63402-116">Select **Functions**.</span></span>
11. <span data-ttu-id="63402-117">Hautatu **Sortu erosketa-eskaerak**.</span><span class="sxs-lookup"><span data-stu-id="63402-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="63402-118">Hautatu **Barne hatu guztia** kontrol-laukia.</span><span class="sxs-lookup"><span data-stu-id="63402-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="63402-119">**Salmentaren kontua** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="63402-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="63402-120">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="63402-120">Select **OK**.</span></span>
15. <span data-ttu-id="63402-121">Nabigazio panelean, joan hona: **Moduluak > Ordaindu beharreko kontuak > Erosi aginduak > Erosketa-agindu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="63402-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="63402-122">Zerrendan, hautatu desiratutako errenkadako estekan.</span><span class="sxs-lookup"><span data-stu-id="63402-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="63402-123">Ekintza panelean, hautatu **Erosi**.</span><span class="sxs-lookup"><span data-stu-id="63402-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="63402-124">Hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="63402-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="63402-125">Ekintza panelean, hautatu **Jaso**.</span><span class="sxs-lookup"><span data-stu-id="63402-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="63402-126">Hautatu **Produktuaren ordainagiria**.</span><span class="sxs-lookup"><span data-stu-id="63402-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="63402-127">**Produktuaren ordainagiria** eremua, idatzi balio bat.</span><span class="sxs-lookup"><span data-stu-id="63402-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="63402-128">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="63402-128">Select **OK**.</span></span>

