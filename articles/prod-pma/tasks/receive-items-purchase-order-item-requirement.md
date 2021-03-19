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
ms.openlocfilehash: c2083516ff929113fd6db377acfe5aeb104666dd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288213"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="9ecca-103">Jaso erosketa eskaeran elementuak eskakizunetik</span><span class="sxs-lookup"><span data-stu-id="9ecca-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="9ecca-104">Gai honetan artikuluaren baldintza batetik erosketa-eskaera bateko artikuluak nola jaso azaltzen da.</span><span class="sxs-lookup"><span data-stu-id="9ecca-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="9ecca-105">Artikuluaren transakzioaren ordez elementuaren eskakizuna erabiliz gero, elementua benetan erabili aurretik entregatzeko asmoa dezakezu, erosketa-agindua sortu, artikulua merkataritza-akordioaren esparruan sartu eta produktuaren eskakizuna produkzioaren plangintzan sartu.</span><span class="sxs-lookup"><span data-stu-id="9ecca-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="9ecca-106">Zeregin honek USSI datu multzoa erabiltzen du.</span><span class="sxs-lookup"><span data-stu-id="9ecca-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="9ecca-107">Nabigazio-panelean, joan **Moduluak > Proiektuaren kudeaketa eta kontua > Proiektuak > Proiektu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="9ecca-108">Zerrendan, hautatu desiratutako errenkadako estekan.</span><span class="sxs-lookup"><span data-stu-id="9ecca-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="9ecca-109">Ekintza panelean, hautatu **Plana**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="9ecca-110">Aukeratu **Elementuen eskakizunak**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="9ecca-111">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-111">Select **New**.</span></span>
6. <span data-ttu-id="9ecca-112">Errenkada berrian, sartu edo hautatu balio bat **Elementuaren zenbakia** eremua.</span><span class="sxs-lookup"><span data-stu-id="9ecca-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="9ecca-113">**Kantitatea** eremuan, idatzi zenbakia.</span><span class="sxs-lookup"><span data-stu-id="9ecca-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="9ecca-114">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-114">Select **Save**.</span></span>
9. <span data-ttu-id="9ecca-115">Ekintza panelean, hautatu **Kudeatu**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="9ecca-116">Hautatu **Funtzioak**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-116">Select **Functions**.</span></span>
11. <span data-ttu-id="9ecca-117">Hautatu **Sortu erosketa-eskaerak**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="9ecca-118">Hautatu **Barne hatu guztia** kontrol-laukia.</span><span class="sxs-lookup"><span data-stu-id="9ecca-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="9ecca-119">**Salmentaren kontua** eremua, idatzi edo hautatu balioa.</span><span class="sxs-lookup"><span data-stu-id="9ecca-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="9ecca-120">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-120">Select **OK**.</span></span>
15. <span data-ttu-id="9ecca-121">Nabigazio panelean, joan hona: **Moduluak > Ordaindu beharreko kontuak > Erosi aginduak > Erosketa-agindu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="9ecca-122">Zerrendan, hautatu desiratutako errenkadako estekan.</span><span class="sxs-lookup"><span data-stu-id="9ecca-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="9ecca-123">Ekintza panelean, hautatu **Erosi**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="9ecca-124">Hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="9ecca-125">Ekintza panelean, hautatu **Jaso**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="9ecca-126">Hautatu **Produktuaren ordainagiria**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="9ecca-127">**Produktuaren ordainagiria** eremua, idatzi balio bat.</span><span class="sxs-lookup"><span data-stu-id="9ecca-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="9ecca-128">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="9ecca-128">Select **OK**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]