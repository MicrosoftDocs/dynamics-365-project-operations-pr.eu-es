---
title: Produktuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra - arina
description: Gai honek produktuan oinarritutako eskaintzaren lerroekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/30/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6aa428c486f149308ad078f9d7a80a0be0f0f04
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4178173"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="db89f-103">Produktuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra - arina</span><span class="sxs-lookup"><span data-stu-id="db89f-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="db89f-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="db89f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="db89f-105">Produktuetan oinarritutako aurrekontu lerroak sor ditzakezu Dynamics 365 Project Operations-en.</span><span class="sxs-lookup"><span data-stu-id="db89f-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="db89f-106">Produktuen araberako aurrekontu-ildoak eskuz gehi daitezke, edo produktuen katalogoko elementuak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="db89f-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="db89f-107">Produktuen katalogoa</span><span class="sxs-lookup"><span data-stu-id="db89f-107">Product catalog</span></span>

<span data-ttu-id="db89f-108">Produktuen katalogoko produktu bakoitzak unitate eta unitate multzo lehenetsiak ditu.</span><span class="sxs-lookup"><span data-stu-id="db89f-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="db89f-109">Hainbat produktuk atributu multzo bera partekatzen badute, ezaugarri horiek ere badituen produktuen familia sor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="db89f-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="db89f-110">Adibidez, enpresa batek harpidetzako lizentziak saltzen ditu software askotarako.</span><span class="sxs-lookup"><span data-stu-id="db89f-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="db89f-111">Harpidetza software guztiek bi atributu hauek dituzte:</span><span class="sxs-lookup"><span data-stu-id="db89f-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="db89f-112">Erabiltzaile kopurua</span><span class="sxs-lookup"><span data-stu-id="db89f-112">Number of users</span></span>
- <span data-ttu-id="db89f-113">Harpidetzaren iraupena hilabeteetan neurtuta</span><span class="sxs-lookup"><span data-stu-id="db89f-113">A subscription duration measured in months</span></span>

<span data-ttu-id="db89f-114">Katalogo mota hau mantentzeko izena duen produktu familia sortzea **Harpidetza softwarea**, eta horrek badu erabiltzaile kopurua eta harpidetzaren iraupena atributu gisa gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="db89f-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="db89f-115">Ondoren, produktu indibidualak gehi ditzakezu **Harpidetza softwarea** produktuen familia.</span><span class="sxs-lookup"><span data-stu-id="db89f-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="db89f-116">Gehitu produktuen katalogoko elementuak proiektuaren aurrekontuan</span><span class="sxs-lookup"><span data-stu-id="db89f-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="db89f-117">**Proiektuen eskaintza** eta **Proiektuaren kontratua** orriek atalak dituzte proiektuan oinarritutako ildoak eta produktuetan oinarritutako lineak.</span><span class="sxs-lookup"><span data-stu-id="db89f-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="db89f-118">Produktuetan oinarritutako lerroetarako, eskaintzen edo proiektuaren kontratuaren lerroko goitibeherako zerrendak prezio-zerrendako unitate eta unitate guztiak barne hartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="db89f-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="db89f-119">Produktu-zerrendako zati ez diren produktuak ere gehi ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="db89f-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="db89f-120">Gainera, produktuak beste prezio-zerrendetatik hauta ditzakezu edo zuzenean katalogotik hauta ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="db89f-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="db89f-121">Produktuak katalogo batetik zuzenean hautatzen dituzunean, produktu horren prezioen zerrenda lehenetsia erabiltzen da produktuaren salmenta prezioa lortzeko.</span><span class="sxs-lookup"><span data-stu-id="db89f-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="db89f-122">Lehenetsitako prezioen zerrenda zehazten ez bada, prezioa (0) izango da.</span><span class="sxs-lookup"><span data-stu-id="db89f-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="db89f-123">Aurrekontu-lerro bat produktuen katalogoan oinarrituta badago, salmenta-prezioa zuzenean alda dezakezu aurrekontuen lerroan.</span><span class="sxs-lookup"><span data-stu-id="db89f-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="db89f-124">Aurrekontuaren lerroa **Prezioak** bi balio erabilgarri dituen eremua:</span><span class="sxs-lookup"><span data-stu-id="db89f-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="db89f-125">**Gainidatzi prezioa**</span><span class="sxs-lookup"><span data-stu-id="db89f-125">**Override Pricing**</span></span>
- <span data-ttu-id="db89f-126">**Erabili lehenetsia**</span><span class="sxs-lookup"><span data-stu-id="db89f-126">**Use Default**</span></span>

<span data-ttu-id="db89f-127">Hautatzen baduzu **Gainidatzi prezioak**, lehenetsitako prezioa ez dago ezarrita.</span><span class="sxs-lookup"><span data-stu-id="db89f-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="db89f-128">Edo, produktuaren prezioa sartu behar duzu aurrekontuen lerroan.</span><span class="sxs-lookup"><span data-stu-id="db89f-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="db89f-129">Hautatzen baduzu **Erabili lehenetsia**, salmenta prezio lehenetsia erabiltzen da eta eremua blokeatuta dago editatzeko.</span><span class="sxs-lookup"><span data-stu-id="db89f-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="db89f-130">Salmenta prezio lehenetsiak produktuaren araberako lerroetan sartzen dira aurrekontu batean.</span><span class="sxs-lookup"><span data-stu-id="db89f-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="db89f-131">**Prezioa** eremua, eremuan ezarri behar da **Gainidatzi prezioak** eskaintzaren lerroetan prezio lehenetsia editatu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="db89f-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="db89f-132">Hau da, Dynamics 365 Sales-en produktuan oinarritutako lerroen portaeraren gaineko Project Operations-en berariazko gainidazketa.</span><span class="sxs-lookup"><span data-stu-id="db89f-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>
