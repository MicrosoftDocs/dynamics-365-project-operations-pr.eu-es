---
title: Proiekturako erosketa eskaerak
description: Artikulu honetan proiektu baterako erosketa aginduak sortzeko erabil ditzakezun metodoak deskribatzen dira. Erabiltzen duzun metodoa erosketa-aginduaren helburuaren arabera, eta erositako elementuak kontsumitu eta kargatu egiten dira proiektua.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071024"
---
# <a name="purchase-orders-for-a-project"></a><span data-ttu-id="f5d90-104">Proiekturako erosketa eskaerak</span><span class="sxs-lookup"><span data-stu-id="f5d90-104">Purchase orders for a project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f5d90-105">Artikulu honetan proiektu baterako erosketa aginduak sortzeko erabil ditzakezun metodoak deskribatzen dira.</span><span class="sxs-lookup"><span data-stu-id="f5d90-105">This article describes the various methods that you can use to create purchase orders for a project.</span></span> <span data-ttu-id="f5d90-106">Erabiltzen duzun metodoa erosketa-aginduaren helburuaren arabera, eta erositako elementuak kontsumitu eta kargatu egiten dira proiektua.</span><span class="sxs-lookup"><span data-stu-id="f5d90-106">The method that you use depends on the purpose of the purchase order, and when the purchased items are consumed and charged to a project.</span></span>

### <a name="methods-for-creating-a-purchase-order"></a><span data-ttu-id="f5d90-107">Erosketa eskaera sortzeko metodoak</span><span class="sxs-lookup"><span data-stu-id="f5d90-107">Methods for creating a purchase order</span></span>

<span data-ttu-id="f5d90-108">Proiektuen kudeaketan eta kontabilitatean erosketa eskaera bat sortzeko metodo hauetako bat erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="f5d90-108">You can use one of the following methods to create a purchase order in Project management and accounting.</span></span> <span data-ttu-id="f5d90-109">Erosketa eskaeraren xedeak zehazten du noiz kontsumitzen den eta, beraz, noiz kobratzen diren proiektu batean proiektuak.</span><span class="sxs-lookup"><span data-stu-id="f5d90-109">The purpose of the purchase order determines when the purchase order is consumed and, therefore, when items are charged to a project.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f5d90-110">Metodoa</span><span class="sxs-lookup"><span data-stu-id="f5d90-110">Method</span></span></th>
<th><span data-ttu-id="f5d90-111">Helburua</span><span class="sxs-lookup"><span data-stu-id="f5d90-111">Purpose</span></span></th>
<th><span data-ttu-id="f5d90-112">Elementuen kontsumoa</span><span class="sxs-lookup"><span data-stu-id="f5d90-112">Consumption of items</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f5d90-113">Sortu erosketa-eskaerak zuzenean proiektutik.</span><span class="sxs-lookup"><span data-stu-id="f5d90-113">Create a purchase order directly from a project.</span></span></td>
<td><span data-ttu-id="f5d90-114">Erabili metodo hori erosteko elementuak kanpoko saltzaile bati proiektu batean kontsumitzeko.</span><span class="sxs-lookup"><span data-stu-id="f5d90-114">Use this method to purchase items from an external vendor for consumption on a project.</span></span> <span data-ttu-id="f5d90-115">Erosketa aginduaren sor dezakezu bi modutan:</span><span class="sxs-lookup"><span data-stu-id="f5d90-115">You can create the purchase order in two ways:</span></span>
<ul>
<li><span data-ttu-id="f5d90-116">Proiektutik bertatik.</span><span class="sxs-lookup"><span data-stu-id="f5d90-116">From the project itself.</span></span> <span data-ttu-id="f5d90-117">Kasu honetan, proiektua dagoeneko zehaztuta dago erosketa eskaerarako.</span><span class="sxs-lookup"><span data-stu-id="f5d90-117">In this case, the project is already defined for the purchase order.</span></span></li>
<li><span data-ttu-id="f5d90-118">Proiektuaren erosketa eskaerara nabigatuz.</span><span class="sxs-lookup"><span data-stu-id="f5d90-118">By navigating to the project purchase order.</span></span> <span data-ttu-id="f5d90-119">Erosketa eskaera sortzeko saltzailea eta proiektua hautatu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="f5d90-119">You must select both the vendor and the project to create the purchase order for.</span></span></li>
</ul></td>
<td><span data-ttu-id="f5d90-120">Elementuak saltzailearen faktura eguneratzen denean kontsumitzen dira.</span><span class="sxs-lookup"><span data-stu-id="f5d90-120">Items are consumed when the vendor invoice is updated.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f5d90-121">Sortu erosketa agindua erosketa agindutik.</span><span class="sxs-lookup"><span data-stu-id="f5d90-121">Create a purchase order from a sales order.</span></span></td>
<td><span data-ttu-id="f5d90-122">Erabili erosketa-elementuen metodo hori salmenta-agindua sortzerakoan proiektutik.</span><span class="sxs-lookup"><span data-stu-id="f5d90-122">Use this method to purchase items when you create a sales order from a project.</span></span></td>
<td><span data-ttu-id="f5d90-123">Artikuluak bezeroari salmenta eskaera fakturatzen zaionean kontsumitzen dira.</span><span class="sxs-lookup"><span data-stu-id="f5d90-123">Items are consumed when the sales order is invoiced to the customer.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f5d90-124">Sortu erosketa eskaera elementu baten eskakizunetik abiatuta.</span><span class="sxs-lookup"><span data-stu-id="f5d90-124">Create a purchase order from an item requirement.</span></span></td>
<td><span data-ttu-id="f5d90-125">Erabili erosketa-elementuen metodo hori elementu-eskakizun bat sortzerakoan proiektutik.</span><span class="sxs-lookup"><span data-stu-id="f5d90-125">Use this method to purchase items when you create an item requirement from a project.</span></span></td>
<td><span data-ttu-id="f5d90-126">Elementuak kontsumitzen dira elementuaren eskakizunaren pakete irristagarria eguneratuta dago.</span><span class="sxs-lookup"><span data-stu-id="f5d90-126">Items are consumed when the item requirement packing slip is updated.</span></span></td>
</tr>
</tbody>
</table>

> [!NOTE] 
> <span data-ttu-id="f5d90-127">Saltzailearen faktura edo ontziratze agiria eguneratzen duzunean, elementuaren eskakizunean ontziratze agiria eguneratzeko eskatuko zaizu.</span><span class="sxs-lookup"><span data-stu-id="f5d90-127">When you update the vendor invoice or packing slip, you're prompted to update the packing slip on the item requirement.</span></span>

<span data-ttu-id="f5d90-128">Informazio gehiagorako, ikus [Jaso erosketa eskaeran elementuak eskakizunetik](tasks/receive-items-purchase-order-item-requirement.md).</span><span class="sxs-lookup"><span data-stu-id="f5d90-128">For more information, see [Receive items on purchase order from item requirement](tasks/receive-items-purchase-order-item-requirement.md).</span></span>

