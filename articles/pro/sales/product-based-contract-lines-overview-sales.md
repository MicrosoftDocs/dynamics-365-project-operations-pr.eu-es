---
title: Produktuetan oinarritutako kontratuaren lerroen ikuspegi orokorra - arina
description: Gai honek kontratu eta produktuetan oinarritutako lerroei buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6e9ef33cc9c79f828e85733f4f5a199bce842700
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272643"
---
# <a name="product-based-contract-lines-overview---lite"></a><span data-ttu-id="d35a4-103">Produktuetan oinarritutako kontratuaren lerroen ikuspegi orokorra - arina</span><span class="sxs-lookup"><span data-stu-id="d35a4-103">Product-based contract lines overview - lite</span></span>

<span data-ttu-id="d35a4-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="d35a4-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d35a4-105">Produktuetan oinarritutako kontratuaren lerroak sor ditzakezu Dynamics 365 Project Operations-en.</span><span class="sxs-lookup"><span data-stu-id="d35a4-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="d35a4-106">Produktuen araberako kontratuaren lerroak eskuz sortutako lerroak izan daitezke, edo produktuen katalogoko elementuak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="d35a4-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="d35a4-107">Produktuen katalogoa</span><span class="sxs-lookup"><span data-stu-id="d35a4-107">Product catalog</span></span>

<span data-ttu-id="d35a4-108">Produktuen katalogoko produktuek unitate eta unitate multzo lehenetsiak dituzte.</span><span class="sxs-lookup"><span data-stu-id="d35a4-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="d35a4-109">Hainbat produktuk atributu multzo bera partekatzen badute, ezaugarri horiek ere badituen produktuen familia sor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="d35a4-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="d35a4-110">Produktu familia bateko produktu guztiek ezaugarri berdinak heredatzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="d35a4-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="d35a4-111">Adibidez, enpresa batek harpidetzako lizentziak saltzen ditu software askotarako.</span><span class="sxs-lookup"><span data-stu-id="d35a4-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="d35a4-112">Harpidetza software guztiek bi atributu hauek dituzte:</span><span class="sxs-lookup"><span data-stu-id="d35a4-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="d35a4-113">Erabiltzaile kopurua</span><span class="sxs-lookup"><span data-stu-id="d35a4-113">Number of users</span></span>
- <span data-ttu-id="d35a4-114">Harpidetzaren iraupena (hilabeteetan)</span><span class="sxs-lookup"><span data-stu-id="d35a4-114">Subscription duration (in months)</span></span>

<span data-ttu-id="d35a4-115">Katalogo mota hau mantentzeko, sortu izena duen produktu familia **Harpidetza softwarea**.</span><span class="sxs-lookup"><span data-stu-id="d35a4-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="d35a4-116">Gehitu atributuak, **Erabiltzaile kopurua** eta **Harpidetzaren iraupena** produktuen familiari.</span><span class="sxs-lookup"><span data-stu-id="d35a4-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="d35a4-117">Ondoren, gehitu produktu indibidualak **Harpidetza softwarea** produktuen familia.</span><span class="sxs-lookup"><span data-stu-id="d35a4-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="d35a4-118">Gehitu produktuen katalogoko elementuak proiektuaren kontratuan</span><span class="sxs-lookup"><span data-stu-id="d35a4-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="d35a4-119">Proiektuen kontratuek bi lerro mota dituzte ataletan: proiektuan oinarritutakoak eta produktuetan oinarritutakoak.</span><span class="sxs-lookup"><span data-stu-id="d35a4-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="d35a4-120">Produktuan oinarritutako lerroek produktu eta unitate guztiak biltzen dituzte kontratuko produktuen prezioen zerrendan.</span><span class="sxs-lookup"><span data-stu-id="d35a4-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="d35a4-121">Kontratuaren produktu-zerrendako zati ez diren produktuak gehi ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="d35a4-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="d35a4-122">Produktuak beste prezio zerrendetatik edo zuzenean produktuen katalogotik hauta ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="d35a4-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="d35a4-123">Produktuak katalogo batetik zuzenean hautatzen dituzunean, produktu horren prezioen zerrenda lehenetsia erabiltzen da produktuaren salmenta prezioa lortzeko.</span><span class="sxs-lookup"><span data-stu-id="d35a4-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="d35a4-124">Lehenetsitako prezioen zerrenda zehazten ez bada, prezioa 0 (zero) izango da.</span><span class="sxs-lookup"><span data-stu-id="d35a4-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="d35a4-125">Kontratuaren lerro bat produktuen katalogoan oinarrituta badago, salmenta-prezioa zuzenean alda dezakezu lerroan.</span><span class="sxs-lookup"><span data-stu-id="d35a4-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="d35a4-126">Kontratu linea batek du **Prezioak** bi balioekin eremua:</span><span class="sxs-lookup"><span data-stu-id="d35a4-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="d35a4-127">**Gainidatzi prezioa**</span><span class="sxs-lookup"><span data-stu-id="d35a4-127">**Override pricing**</span></span>
- <span data-ttu-id="d35a4-128">**Erabili balio lehenetsiak**</span><span class="sxs-lookup"><span data-stu-id="d35a4-128">**Use default**</span></span>

<span data-ttu-id="d35a4-129">**Prezioak** eremua **Gainidatzi prezioa** gisa ezartzen baduzu, ez da prezio lehenetsirik zehazten.</span><span class="sxs-lookup"><span data-stu-id="d35a4-129">If you set the **Pricing** field to **Override pricing**, the default price isn't set.</span></span> <span data-ttu-id="d35a4-130">Idatzi kontratuaren lerroko produktuaren prezioa.</span><span class="sxs-lookup"><span data-stu-id="d35a4-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="d35a4-131">Eremua ezartzen baduzu **Erabili lehenetsia**, salmenta prezio lehenetsia erabiltzen da eta eremua ezin da editatu.</span><span class="sxs-lookup"><span data-stu-id="d35a4-131">If you set the field to **Use default**, the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="d35a4-132">Project Operations instalatu ondoren, salmenta prezio lehenetsiak produktuaren araberako lerroetan sartzen dira kontratu batean.</span><span class="sxs-lookup"><span data-stu-id="d35a4-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="d35a4-133">**Prezioa** eremua, eremuan ezarri behar da **Gainidatzi prezioak** kontratuaren lerroetan prezio lehenetsia editatu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="d35a4-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="d35a4-134">Project Operations-ek produktuan oinarritutako lerroen portaera berraztertzen dute Dynamics 365 Sales-en.</span><span class="sxs-lookup"><span data-stu-id="d35a4-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]