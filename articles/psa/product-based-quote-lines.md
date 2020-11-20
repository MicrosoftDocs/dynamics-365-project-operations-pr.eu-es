---
title: Produktuetan oinarritutako eskaintzaren lerroak
description: Gai honek eskaintza eta produktuetan oinarritutako lerroei buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 9c3b2b35abe894e79d6f55a7ddd6e5c64d0f12f2
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4123183"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="68009-103">Produktuetan oinarritutako eskaintzaren lerroak</span><span class="sxs-lookup"><span data-stu-id="68009-103">Product-based quote lines</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="68009-104">Produktuetan oinarritutako aurrekontu lerroak sor ditzakezu Dynamics 365 Project Service Automation-en.</span><span class="sxs-lookup"><span data-stu-id="68009-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="68009-105">Produktuen araberako aurrekontu-ildoak "idazteko" lerroak izan daitezke, edo produktuen katalogoko elementuak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="68009-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="68009-106">Produktuen katalogoa</span><span class="sxs-lookup"><span data-stu-id="68009-106">Product catalog</span></span>

<span data-ttu-id="68009-107">Dynamics 365 produktuen katalogoko produktuek unitate eta unitate multzo lehenetsiak dituzte.</span><span class="sxs-lookup"><span data-stu-id="68009-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="68009-108">Hainbat produktuk atributu multzo bera partekatzen badute, ezaugarri horiek ere badituen produktuen familia sor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="68009-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="68009-109">Produktu familia bateko produktu guztiek ezaugarri berdinak heredatzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="68009-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="68009-110">Adibidez, enpresa batek harpidetzako lizentziak saltzen ditu software askotarako.</span><span class="sxs-lookup"><span data-stu-id="68009-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="68009-111">Harpidetza software guztiek bi atributu hauek dituzte:</span><span class="sxs-lookup"><span data-stu-id="68009-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="68009-112">Erabiltzaile kopurua</span><span class="sxs-lookup"><span data-stu-id="68009-112">Number of users</span></span> 
- <span data-ttu-id="68009-113">Harpidetzaren iraupena (hilabeteetan)</span><span class="sxs-lookup"><span data-stu-id="68009-113">Subscription duration (in months)</span></span>

<span data-ttu-id="68009-114">Katalogo mota hau mantentzeko modu ona da izena duen produktu familia sortzea **Harpidetza softwarea**, eta horrek badu **Erabiltzaile kopurua** eta **Harpidetzaren iraupena** atributu gisa.</span><span class="sxs-lookup"><span data-stu-id="68009-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software**, and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="68009-115">Ondoren, produktu indibidualak gehi ditzakezu, adibidez **Dynamics 365 Sales** edo **Dynamics 365 Field Service** aplikazioak **Harpidetza software** familia produktura.</span><span class="sxs-lookup"><span data-stu-id="68009-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="68009-116">Produktuen katalogoko elementuak proiektuaren aurrekontuan gehitzea</span><span class="sxs-lookup"><span data-stu-id="68009-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="68009-117">Proiektuen eskaintza eta proiektuaren kontratu orriek bi lerro mota dituzte ataletan: proiektuan oinarritutako ildoak eta produktuetan oinarritutako lineak.</span><span class="sxs-lookup"><span data-stu-id="68009-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="68009-118">Produktuetan oinarritutako ildoetarako, Dynamics 365 erabiltzen da produktuen katalogoko elementuak eskaintza batean gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="68009-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="68009-119">Eskaintzen edo proiektuaren kontratuaren lerroko goitibeherako zerrendak aurrekontuari edo proiektuaren kontratuei atxikitako produktuen prezio-zerrendako unitate eta unitate guztiak barne hartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="68009-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="68009-120">Eskaintzen produktu-zerrendako zati ez diren produktuak ere gehi ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="68009-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="68009-121">Gainera, produktuak beste prezio-zerrendetatik hauta ditzakezu edo produktuak zuzenean katalogotik hauta ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="68009-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="68009-122">Produktuak katalogo batetik zuzenean hautatzen dituzunean, produktu horren prezioen zerrenda lehenetsia erabiltzen da produktuaren salmenta prezioa lortzeko.</span><span class="sxs-lookup"><span data-stu-id="68009-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="68009-123">Lehenetsitako prezioen zerrenda zehazten ez bada, prezioa 0 (zero) izango da.</span><span class="sxs-lookup"><span data-stu-id="68009-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="68009-124">Aurrekontu-lerro bat produktuen katalogoan oinarrituta badago, salmenta-prezioa zuzenean alda dezakezu aurrekontuen lerroan.</span><span class="sxs-lookup"><span data-stu-id="68009-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="68009-125">Kontuan izan Dynamics 365-en aurrekontu-lerroak baduela **Prezioak** eremua.</span><span class="sxs-lookup"><span data-stu-id="68009-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="68009-126">Bi balio daude:</span><span class="sxs-lookup"><span data-stu-id="68009-126">Two values are available:</span></span>

- <span data-ttu-id="68009-127">Gainidatzi prezioa</span><span class="sxs-lookup"><span data-stu-id="68009-127">Override pricing</span></span>  
- <span data-ttu-id="68009-128">Erabili balio lehenetsiak</span><span class="sxs-lookup"><span data-stu-id="68009-128">Use default</span></span>

<span data-ttu-id="68009-129">Eremu hau ezarrita baduzu **Gainidatzi prezioa**, Dynamics 365-ek ez du prezio lehenetsirik zehazten.</span><span class="sxs-lookup"><span data-stu-id="68009-129">If you set this field to **Override pricing**, Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="68009-130">Produktuaren prezioa sartu behar duzu aurrekontuen lerroan.</span><span class="sxs-lookup"><span data-stu-id="68009-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="68009-131">Eremu hau ezarrita baduzu **Erabili lehenetsia**, Dynamics 365-ek salmenta-prezio lehenetsia erabiltzen du eta eremua blokeatzen du edizioa ekiditeko.</span><span class="sxs-lookup"><span data-stu-id="68009-131">If you set this field to **Use default**, Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="68009-132">PSA instalatu ondoren, salmenta prezio lehenetsiak produktuaren araberako lerroetan sartzen dira aurrekontu batean.</span><span class="sxs-lookup"><span data-stu-id="68009-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="68009-133">**Prezioa** eremua, eremuan ezarri behar da **Gainidatzi prezioak** eskaintzaren lerroetan prezio lehenetsia editatu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="68009-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![Ezarri fakturaren prezioak](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="68009-135">Produktuen kantitate faktoreak</span><span class="sxs-lookup"><span data-stu-id="68009-135">Quantity factors for products</span></span>

<span data-ttu-id="68009-136">PSAk kantitate faktoreak erabiltzen ditu harpidedun oinarritutako produktuen salmenta sustatzeko.</span><span class="sxs-lookup"><span data-stu-id="68009-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="68009-137">Harpidetzetan oinarritutako produktuetarako, aurrekontuan edo proiektuaren kontratuaren lerroan erabiltzaile-hilabete kopurua adierazten da.</span><span class="sxs-lookup"><span data-stu-id="68009-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="68009-138">Normalean, harpidedun softwarearen prezioa katalogoan gordetzen da erabiltzaile bakoitzeko prezio gisa.</span><span class="sxs-lookup"><span data-stu-id="68009-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="68009-139">Hala ere, beste denbora deskribapen batzuk erabil ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="68009-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="68009-140">Salmenta prozesuan, aurrekontuen lerroko prezioa erabiltzaile bakoitzeko, salmentako IT agentearen bidez negoziatu eta deskontatu zen hileko prezioa izan ohi da.</span><span class="sxs-lookup"><span data-stu-id="68009-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="68009-141">Akordio bakoitzak erabiltzaile kopurua eta harpidetza hilabete desberdinak ditu.</span><span class="sxs-lookup"><span data-stu-id="68009-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="68009-142">Aurrekontuen lerroaren zenbatekoa kalkulatzeko erabiltzen den kantitatea erabiltzaile kopurua eta harpidetza hilabeteen produktua da.</span><span class="sxs-lookup"><span data-stu-id="68009-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="68009-143">Salmenta mota hori onartzeko, PSAk kantitate faktoreen kontzeptua sartu zuen.</span><span class="sxs-lookup"><span data-stu-id="68009-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="68009-144">Kopuru-faktoreek produktuaren atributuetan oinarritzen dira Dynamics 365-en.</span><span class="sxs-lookup"><span data-stu-id="68009-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="68009-145">Produktu baterako propietate espezifikoak konfiguratzen dituzunean, PSAk propietate horien edo propietate guztien azpimultzoa uzten dizu kantitate faktore gisa.</span><span class="sxs-lookup"><span data-stu-id="68009-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="68009-146">PSAk balioztatzen du zenbakizko datu mota bat duten zenbakizko propietateak edo produktuaren propietateak kantitate faktore gisa markatzen direla.</span><span class="sxs-lookup"><span data-stu-id="68009-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="68009-147">Kantitate-faktoreak konfiguratutako produktu bat aurrekontu-lerrora gehitzen denean, **Kopurua** aurrekontuen lerroan irakurtzeko soilik eremu bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="68009-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="68009-148">Kantitate faktoreak diren produktuaren propietateen balioak sartu ondoren, PSAk aurrekontuen lerroaren kantitatea kalkulatzen du.</span><span class="sxs-lookup"><span data-stu-id="68009-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="68009-149">Adibidez, Dynamics 365-ek propietate hauek izan ditzake:</span><span class="sxs-lookup"><span data-stu-id="68009-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="68009-150">**Erabiltzaile kop**: erabiltzaile kopurua</span><span class="sxs-lookup"><span data-stu-id="68009-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="68009-151">**Hilabete kop**: harpidetza-hilabete kopurua</span><span class="sxs-lookup"><span data-stu-id="68009-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="68009-152">**SKU produktua**</span><span class="sxs-lookup"><span data-stu-id="68009-152">**Product SKU**</span></span> 

<span data-ttu-id="68009-153">**Erabiltzaile kop** eta **Hilabete kop** propietateak kantitate faktore gisa markatu daitezke produktuaren lerroko propietateak editatzean.</span><span class="sxs-lookup"><span data-stu-id="68009-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![Erabiltzaileen kopurua eta hilabete kopurua ez izatea kalitate faktore gisa](media/basic-guide-11.png)
 
