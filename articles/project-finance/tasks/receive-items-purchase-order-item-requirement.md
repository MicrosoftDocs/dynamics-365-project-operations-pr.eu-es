---
title: Jaso erosketa eskaeran elementuak eskakizunetik
description: Gai honetan artikuluaren baldintza batetik erosketa-eskaera bateko artikuluak nola jaso azaltzen da.
author: KimANelson
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
ms.assetid: c61e3a5e-da3d-4f4c-87fa-03dea19f6936
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c5ed287aa24aff647ef1dc625f9e9f5f086ee662
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748800"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="0d49d-103">Jaso erosketa eskaeran elementuak eskakizunetik</span><span class="sxs-lookup"><span data-stu-id="0d49d-103">Receive items on purchase order from item requirement</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="0d49d-104">Gai honetan artikuluaren baldintza batetik erosketa-eskaera bateko artikuluak nola jaso azaltzen da.</span><span class="sxs-lookup"><span data-stu-id="0d49d-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="0d49d-105">Artikuluaren transakzioaren ordez elementuaren eskakizuna erabiliz gero, elementua benetan erabili aurretik entregatzeko asmoa dezakezu, erosketa-agindua sortu, artikulua merkataritza-akordioaren esparruan sartu eta produktuaren eskakizuna produkzioaren plangintzan sartu.</span><span class="sxs-lookup"><span data-stu-id="0d49d-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="0d49d-106">Zeregin honek USSI datu multzoa erabiltzen du.</span><span class="sxs-lookup"><span data-stu-id="0d49d-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="0d49d-107">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Proiektuak > Proiektu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="0d49d-108">Zerrendan, hautatu desiratutako errenkadako estekan.</span><span class="sxs-lookup"><span data-stu-id="0d49d-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="0d49d-109">Ekintza panelean, hautatu **Plana**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="0d49d-110">Aukeratu **Elementuen eskakizunak**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="0d49d-111">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-111">Select **New**.</span></span>
6. <span data-ttu-id="0d49d-112">Errenkada berrian, sartu edo hautatu balio bat **Elementuaren zenbakia** eremua.</span><span class="sxs-lookup"><span data-stu-id="0d49d-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="0d49d-113">**Kantitatea** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="0d49d-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="0d49d-114">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-114">Select **Save**.</span></span>
9. <span data-ttu-id="0d49d-115">Ekintza panelean, hautatu **Kudeatu**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="0d49d-116">Hautatu **Funtzioak**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-116">Select **Functions**.</span></span>
11. <span data-ttu-id="0d49d-117">Hautatu **Sortu erosketa-eskaerak**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="0d49d-118">Hautatu **Barne hatu guztia** kontrol-laukia.</span><span class="sxs-lookup"><span data-stu-id="0d49d-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="0d49d-119">**Salmentaren kontua** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="0d49d-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="0d49d-120">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-120">Select **OK**.</span></span>
15. <span data-ttu-id="0d49d-121">Nabigazio panelean, joan hona: **Moduluak > Ordaindu beharreko kontuak > Erosi aginduak > Erosketa-agindu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="0d49d-122">Zerrendan, hautatu desiratutako errenkadako estekan.</span><span class="sxs-lookup"><span data-stu-id="0d49d-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="0d49d-123">Ekintza panelean, hautatu **Erosi**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="0d49d-124">Hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="0d49d-125">Ekintza panelean, hautatu **Jaso**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="0d49d-126">Hautatu **Produktuaren ordainagiria**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="0d49d-127">**Produktuaren ordainagiria** eremua, idatzi balio bat.</span><span class="sxs-lookup"><span data-stu-id="0d49d-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="0d49d-128">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="0d49d-128">Select **OK**.</span></span>

