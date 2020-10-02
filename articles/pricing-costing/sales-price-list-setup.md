---
title: Salmenten prezio-zerrendaren konfigurazioa
description: Gai honek proiektu-prezioaren salmenten prezio-zerrendak buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2a66802adfcadab7b4d34149b146ca3cb27c903e
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896446"
---
# <a name="sales-price-list-setup"></a><span data-ttu-id="e9704-103">Salmenten prezio-zerrendaren konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="e9704-103">Sales price list setup</span></span>

<span data-ttu-id="e9704-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="e9704-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e9704-105">Proiektuen eskaintzen eta kontratuen kasuan, proiektuen prezio-zerrendak produktuen prezio-zerrenda baino beste prezio eredu bat du.</span><span class="sxs-lookup"><span data-stu-id="e9704-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="e9704-106">Produktuen katalogoan oinarritutako eskaintzaren lerroan, prezioa zuzendu eta funtzioetara zuzendu daiteke eskaintzaren lerroan. Eskaintzaren lerro bakoitzak katalogoko elementu bat besterik ez duelako.</span><span class="sxs-lookup"><span data-stu-id="e9704-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="e9704-107">Dena den, proiektuan oinarritutako eskaintzaren lerroan, ezin duzu prezioa zuzendu eskaintzaren lerroan eta kategorietan zuzenean.</span><span class="sxs-lookup"><span data-stu-id="e9704-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="e9704-108">Proiektuaren prezioen zerrenda bi gainidazketa eredu desberdinekin funtzionatzeko erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="e9704-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="e9704-109">Zure proiektuaren baliabideen eta katalogoko elementuen prezio-zerrenda berezi bat izatea gomendatzen dugu, prezioak baliogabetzen dituzunean bien arteko portaera desberdintasunak direla eta.</span><span class="sxs-lookup"><span data-stu-id="e9704-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="e9704-110">Erakunde hauetako bakoitzak salerosketako prezioe-zerrenda bat edo gehiago izan ditzake proiektuaren prezioetarako:</span><span class="sxs-lookup"><span data-stu-id="e9704-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="e9704-111">Bezeroa (kontua)</span><span class="sxs-lookup"><span data-stu-id="e9704-111">Customer (account)</span></span> 
- <span data-ttu-id="e9704-112">Abagunea</span><span class="sxs-lookup"><span data-stu-id="e9704-112">Opportunity</span></span> 
- <span data-ttu-id="e9704-113">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="e9704-113">Quote</span></span> 
- <span data-ttu-id="e9704-114">Proiektu-kontratua</span><span class="sxs-lookup"><span data-stu-id="e9704-114">Project Contract</span></span>

<span data-ttu-id="e9704-115">Prezio-zerrenda duten entitate horien elkartea proiektuaren prezio-zerrendek adierazten dute.</span><span class="sxs-lookup"><span data-stu-id="e9704-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="e9704-116">Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="e9704-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="e9704-117">Lehenetsitako proiektuen prezio-zerrenda ez da automatikoki sartu bezeroaren erregistroan.</span><span class="sxs-lookup"><span data-stu-id="e9704-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="e9704-118">Hala ere, proiektuaren prezio-zerrenda eskuz erantsi dezakezu bezeroaren erregistroan.</span><span class="sxs-lookup"><span data-stu-id="e9704-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="e9704-119">Nolanahi ere, proiektuaren prezio-zerrenda eskuz erantsi behar zenuke bezeroarekin prezioen akordio pertsonalizatua denean.</span><span class="sxs-lookup"><span data-stu-id="e9704-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="e9704-120">Proiektuen prezioen zerrenda salmenta erakunde bati atxikitakoan, informazio hau balioztatzen du:</span><span class="sxs-lookup"><span data-stu-id="e9704-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="e9704-121">Prezio-zerrenda testuinguru bat da **Salmentak**.</span><span class="sxs-lookup"><span data-stu-id="e9704-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="e9704-122">Monetak prezio-zerrendaren monetarekin bat dator.</span><span class="sxs-lookup"><span data-stu-id="e9704-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="e9704-123">Proiektu baten kontratuan, lehentasun hurrenkera hau proiektuaren inguruko prezioen zerrendak automatikoki ezartzeko:</span><span class="sxs-lookup"><span data-stu-id="e9704-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="e9704-124">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="e9704-124">Quote</span></span>
2. <span data-ttu-id="e9704-125">Abagunea</span><span class="sxs-lookup"><span data-stu-id="e9704-125">Opportunity</span></span>
3. <span data-ttu-id="e9704-126">Bezeroa</span><span class="sxs-lookup"><span data-stu-id="e9704-126">Customer</span></span> 
4. <span data-ttu-id="e9704-127">Ezarpen orokorrak</span><span class="sxs-lookup"><span data-stu-id="e9704-127">Global settings</span></span> 

<span data-ttu-id="e9704-128">Proiektuen prezio-zerrenda lehenespenez sartzen denean, sistemak balioztatzen du moneta bezeroaren monetarekin bat datorrela eta sartu diren prezio-zerrenden lehenetsiak testuinguruan **salmentak**.</span><span class="sxs-lookup"><span data-stu-id="e9704-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="e9704-129">Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="e9704-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="e9704-130">Gaitasun honek iraupen luzeko proiektu kontratuetarako zehaztutako prezioak onartzen ditu, non prezio-zerrenda bat baino gehiago eska dezakezun inflazioaren ondorioz gertatzen diren prezioen eguneratzeak kontatzeko.</span><span class="sxs-lookup"><span data-stu-id="e9704-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="e9704-131">Hala ere, bezeroa, abagunea, eskaintza edo proiektu-kontratuaren entitatearekin lotzen dituzun prezioen zerrendek data eraginkortasun bat badute, baliteke prezio lehenetsiak okerrak izatea.</span><span class="sxs-lookup"><span data-stu-id="e9704-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="e9704-132">Hori dela eta, ziurtatu behar duzu data eraginkortasuna bata bestearen gainjartzen duten proiektuen prezio-zerrendak ez daudela entitate horiekin lotuta.</span><span class="sxs-lookup"><span data-stu-id="e9704-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
