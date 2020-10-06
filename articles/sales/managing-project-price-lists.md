---
title: Proiektuaren prezio-zerrendak
description: Gai honek proiektuaren prezio-zerrendaren entitateari buruzko informazioa ematen du.
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
ms.openlocfilehash: d09a0dd8234641ca106c37a38d1d721dfb07236c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898651"
---
# <a name="project-price-lists"></a><span data-ttu-id="5b1d5-103">Proiektuaren prezio-zerrendak</span><span class="sxs-lookup"><span data-stu-id="5b1d5-103">Project price lists</span></span>

<span data-ttu-id="5b1d5-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="5b1d5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5b1d5-105">Dynamics 365 Project Operations-ek Prezioen zerrenda entitatea luzatzen du Dynamics 365 Sales-en.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-105">Dynamics 365 Project Operations extends the Price list entity in Dynamics 365 Sales.</span></span> 

## <a name="key-entities"></a><span data-ttu-id="5b1d5-106">Entitate gakoak</span><span class="sxs-lookup"><span data-stu-id="5b1d5-106">Key entities</span></span>

<span data-ttu-id="5b1d5-107">Prezio-zerrendan lau erakunde desberdinek eskaintzen duten informazioa biltzen da:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-107">A price list includes information that is provided by four different entities:</span></span>

- <span data-ttu-id="5b1d5-108">**Prezio-zerrenda**: entitate honek testuinguruari, monetari, daten eraginkortasunari eta denbora unitateari buruzko informazioa gordetzen du prezio-denborarako.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-108">**Price List**: This entity stores information about context, currency, date effectivity, and time unit for pricing time.</span></span> <span data-ttu-id="5b1d5-109">Testuinguruak erakusten du prezio-zerrendan kostu-tasak edo salmenta-tasak adierazten diren ala ez.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-109">Context shows whether the price list expresses cost rates or sales rates.</span></span> 
- <span data-ttu-id="5b1d5-110">**Moneta**: entitate honek prezioen moneta prezio-zerrendan gordetzen du.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-110">**Currency**:  This entity stores the currency of prices on the price list.</span></span> 
- <span data-ttu-id="5b1d5-111">**Data**: entitate hau sistemak transakzio bateko prezio lehenetsiak sartzen saiatzen denean erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-111">**Date**: This entity is used when the system tries to enter a default a price on a transaction.</span></span> <span data-ttu-id="5b1d5-112">Transakzioaren data biltzen duen data eraginkortasuna duen prezioen zerrenda hautatzen du.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-112">A price list that has date effectivity that includes the date of the transaction is selected.</span></span> <span data-ttu-id="5b1d5-113">Transakziorako data eraginkorra den prezio-zerrenda bat baino gehiago aurkitzen badu eta horri lotutako eskaintzari, kontratuei edo antolakuntza unitateari erantsita, orduan ez da preziorik lehenetsiko.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-113">If  more than one price list is found that is effective for the transaction date and is attached to the related quote, contract, or organizational unit, then no price is defaulted.</span></span> 
- <span data-ttu-id="5b1d5-114">**Ordua**: entitate honek prezioak adierazitako denbora-unitatea gordetzen du, hala nola eguneko- edo orduko-tasak.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-114">**Time**: This entity stores the unit of time that prices are expressed for, such as daily or hourly rates.</span></span> 

<span data-ttu-id="5b1d5-115">Prezio-zerrendako erakundeak erlazionatutako hiru taula ditu, prezioak gordetzen dituztenak:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-115">The Price list entity has three related tables that store prices:</span></span>

  - <span data-ttu-id="5b1d5-116">**Funtzio-prezioa**: taula honek funtzio- eta antolaketa-unitateen balioak konbinatzeko tasa gordetzen du eta giza baliabideen funtzioan oinarritutako prezioak ezartzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-116">**Role Price**: This table stores a rate for a combination of role and organizational unit values and is used to set up role-based prices for human resources.</span></span>
  - <span data-ttu-id="5b1d5-117">**Transakzioen kategoria prezioa**: taula honek prezioak transakzioen kategorien arabera gordetzen ditu eta gastu kategoriako prezioak ezartzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-117">**Transaction Category Price**: This table stores prices by transaction category and is used to set up expense category prices.</span></span>
  - <span data-ttu-id="5b1d5-118">**Prezio-zerrendako elementuak**: taula honek katalogoko produktuen prezioak gordetzen ditu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-118">**Price List Items**: This table stores prices for catalog products.</span></span>
 
<span data-ttu-id="5b1d5-119">Prezio-zerrenda tasa-txartela da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-119">The price list is a rate card.</span></span> <span data-ttu-id="5b1d5-120">Tasa-txartela prezio-zerrendako entitatearen eta erlazionatutako errenkaden funtzio-prezioaren konbinaketa da, transakzioen kategoriako prezioa eta prezio zerrendako elementuen tauletan daude.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-120">A rate card is a combination of the Price List entity and related rows in the Role Price, Transaction Category Price, and Price List Items tables.</span></span>

## <a name="resource-roles"></a><span data-ttu-id="5b1d5-121">Baliabide-funtzioak</span><span class="sxs-lookup"><span data-stu-id="5b1d5-121">Resource roles</span></span>

<span data-ttu-id="5b1d5-122">*Baliabide-funtzioa* terminoak pertsona batek proiektu batean zeregin multzo zehatz bat egiteko izan behar dituen gaitasun, konpetentzia eta ziurtagirien multzoari egiten dio erreferentzia.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-122">The term *resource role* refers to a set of skills, competencies, and certifications that a person must have to perform a specific set of tasks on a project.</span></span>

<span data-ttu-id="5b1d5-123">Giza baliabideen denbora normalean proiektu jakin batean betetzen duen eginkizunaren arabera kotizatzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-123">Human resources time is quoted based on the role that a resource fills on a specific project.</span></span> <span data-ttu-id="5b1d5-124">Giza baliabideen denborarako, baliabideen funtzioan oinarritutako kostuak eta fakturazioa onartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-124">For human resource time, costing and billing is based on resource role.</span></span> <span data-ttu-id="5b1d5-125">Denbora **Ordua** salmenta-unitateko edozein unitatean preziatu daiteke.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-125">Time can be priced in any unit in the **Time** unit group.</span></span>

<span data-ttu-id="5b1d5-126">**Denbora** unitate-taldea Project Operations instalatzean sortzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-126">The **Time** unit group is created when you install Project Operations.</span></span> <span data-ttu-id="5b1d5-127">Lehenetsitako unitate bat du: **Ordua**.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-127">It has a default unit of **Hour**.</span></span> <span data-ttu-id="5b1d5-128">Ezin dituzu atributuak ezabatu, berrizendatu edo editatu **Ordua** salmenta-unitaterako edo **Ordua** unitaterako.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-128">You can't delete, rename, or edit the attributes fo the **Time** unit group or the **Hour** unit.</span></span> <span data-ttu-id="5b1d5-129">Hala ere, beste unitate batzuk gehitu ditzakezu **Ordua** salmenta-unitatean.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-129">However, you can add other units to the **Time** unit group.</span></span> <span data-ttu-id="5b1d5-130">Ezabatzen saiatzen bazara **Denbora** salmenta-unitatea edo **Ordua** unitatea, negozioaren logikan porrotak sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-130">If you try to delete either the **Time** unit group or the **Hour** unit, you might cause failures in the business logic.</span></span>
 
## <a name="transaction-categories-and-expense-categories"></a><span data-ttu-id="5b1d5-131">Transakzio kategoriak eta gastu kategoriak</span><span class="sxs-lookup"><span data-stu-id="5b1d5-131">Transaction categories and expense categories</span></span>

<span data-ttu-id="5b1d5-132">Proiektuen aholkulariek sortzen dituzten bidaiak eta gainerako gastuak normalean bezeroari fakturatzen zaizkio.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-132">Travel and other expenses that project consultants incur are billed to the customer.</span></span> <span data-ttu-id="5b1d5-133">Gastu kategorien prezioak prezio-zerrendaren arabera eginda daude.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-133">Pricing of expense categories is completed by using price lists.</span></span> <span data-ttu-id="5b1d5-134">Aireportua, hotela eta autoen alokairua gastu kategorien adibide dira.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-134">Airfare, hotel, and car rental are examples fo expense categories.</span></span> <span data-ttu-id="5b1d5-135">Gastuen prezio-zerrendaren lerro bakoitzak gastu-kategoria jakin baterako prezioak zehazten ditu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-135">Each price list line for expenses specifies pricing for a specific expense category.</span></span> <span data-ttu-id="5b1d5-136">Hiru metodo hauek erabiltzen dira gastuen kategoriak preziatzeko:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-136">The following three methods are used to price expense categories:</span></span>

- <span data-ttu-id="5b1d5-137">**Kostuan**: gastuaren kostua bezeroari fakturatzen zaio eta ez da gainpreziorik aplikatuko.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-137">**At cost**: The expense cost is billed to the customer, and no markup is applied.</span></span>
- <span data-ttu-id="5b1d5-138">**Gainprezio portzentajea**: benetako kostuaren gaineko portzentajea bezeroari fakturatzen zaio.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-138">**Markup percentage**: The percentage over the actual cost is billed to the customer.</span></span> 
- <span data-ttu-id="5b1d5-139">**Prezioa unitateko**: gastu-kategoriako unitate bakoitzeko fakturazio-prezioa ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-139">**Price per unit**: A billing price is set for each unit of the expense category.</span></span> <span data-ttu-id="5b1d5-140">Bezeroari fakturatzen zaion zenbatekoa kontsultariak jakinarazten duen gastu unitateen arabera kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-140">The amount that is billed ot the customer is calculated based on the number of expense units that the consultant reports.</span></span> <span data-ttu-id="5b1d5-141">Kilometrajeak prezio bakoitzeko prezioaren metodoa erabiltzen du.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-141">Mileage uses the price-per-unit pricing method.</span></span> <span data-ttu-id="5b1d5-142">Adibidez, kilometro-gastuen kategoria 30 dolar (USD) eguneko edo 2 USD kilometroko izateko konfiguratu daiteke.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-142">For example, the mileage expense category can be configured for 30 US dollars (USD) per day or 2 USD per mile.</span></span> <span data-ttu-id="5b1d5-143">Aholkulari batek proiektu baten kilometrajea jakinarazten duenean, fakturatu beharreko zenbatekoa aholkulariak jakinarazi duen kilometro kopuruaren arabera kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-143">When a consultant reports mileage on a project, the amount to bill is calculated based on the number of miles that the consultant reported.</span></span>
 
## <a name="project-sales-pricing-and-overrides"></a><span data-ttu-id="5b1d5-144">Proiektuen salmentako prezioak eta baliogabetzeak</span><span class="sxs-lookup"><span data-stu-id="5b1d5-144">Project sales pricing and overrides</span></span>

<span data-ttu-id="5b1d5-145">Proiektuen eskaintzen eta kontratuen kasuan, proiektuen prezio-zerrendak produktuen prezio-zerrenda baino beste prezio eredu bat du.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-145">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="5b1d5-146">Produktuen katalogoan oinarritutako eskaintzaren lerroan, prezioa zuzendu eta funtzioetara zuzendu daiteke eskaintzaren lerroan. Eskaintzaren lerro bakoitzak katalogoko elementu bat besterik ez duelako.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-146">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="5b1d5-147">Dena den, proiektuan oinarritutako eskaintzaren lerroan, ezin duzu prezioa zuzendu eskaintzaren lerroan eta kategorietan zuzenean.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-147">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="5b1d5-148">Erabili proiektuaren prezioen zerrenda bi gainidazketa eredu desberdinak onartzeko.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-148">Use the project price list to support the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="5b1d5-149">Zure proiektuaren baliabideen eta katalogoko elementuen prezio-zerrenda berezi bat izatea gomendatzen dugu, prezioak baliogabetzen dituzunean bien arteko portaera desberdintasunak direla eta.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-149">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="5b1d5-150">Erakunde hauetako bakoitzak salerosketako prezioe-zerrenda bat edo gehiago izan ditzake proiektuaren prezioetarako:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-150">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="5b1d5-151">Bezeroa (kontua)</span><span class="sxs-lookup"><span data-stu-id="5b1d5-151">Customer (account)</span></span> 
- <span data-ttu-id="5b1d5-152">Abagunea</span><span class="sxs-lookup"><span data-stu-id="5b1d5-152">Opportunity</span></span> 
- <span data-ttu-id="5b1d5-153">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="5b1d5-153">Quote</span></span> 
- <span data-ttu-id="5b1d5-154">Proiektu-kontratua</span><span class="sxs-lookup"><span data-stu-id="5b1d5-154">Project Contract</span></span>

<span data-ttu-id="5b1d5-155">Prezio-zerrenda duten entitate horien elkartea proiektuaren prezio-zerrendek adierazten dute.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-155">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="5b1d5-156">Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-156">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="5b1d5-157">Lehenetsitako proiektuen prezio-zerrenda ez da automatikoki sartu bezeroaren erregistroan.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-157">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="5b1d5-158">Hala ere, proiektuaren prezio-zerrenda eskuz erantsi dezakezu bezeroaren erregistroan.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-158">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="5b1d5-159">Nolanahi ere, proiektuaren prezio-zerrenda eskuz erantsi behar zenuke bezeroarekin prezioen akordio pertsonalizatua denean.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-159">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="5b1d5-160">Proiektuen prezioen zerrenda salmenta erakunde bati atxikitakoan, informazio hau balioztatzen du:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-160">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="5b1d5-161">Prezio-zerrenda testuinguru bat da **Salmentak**.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-161">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="5b1d5-162">Monetak prezio-zerrendaren monetarekin bat dator.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-162">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="5b1d5-163">Proiektu baten kontratuan, lehentasun hurrenkera hau proiektuaren inguruko prezioen zerrendak automatikoki ezartzeko:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-163">On a project contract, the following order of precedence to automatically set related project price lists:</span></span>

1. <span data-ttu-id="5b1d5-164">Eskaintza</span><span class="sxs-lookup"><span data-stu-id="5b1d5-164">Quote</span></span>
2. <span data-ttu-id="5b1d5-165">Abagunea</span><span class="sxs-lookup"><span data-stu-id="5b1d5-165">Opportunity</span></span>
3. <span data-ttu-id="5b1d5-166">Bezeroa</span><span class="sxs-lookup"><span data-stu-id="5b1d5-166">Customer</span></span> 
4. <span data-ttu-id="5b1d5-167">Ezarpen orokorrak</span><span class="sxs-lookup"><span data-stu-id="5b1d5-167">Global settings</span></span> 

<span data-ttu-id="5b1d5-168">Proiektuen prezio-zerrenda lehenespenez sartzen denean, sistemak balioztatzen du moneta bezeroaren monetarekin bat datorrela eta sartu diren prezio-zerrenden lehenetsiak testuinguruan **salmentak**.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-168">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="5b1d5-169">Prezio-zerrenda bat edo gehiago bezeroak, abagunean, eskaintzak eta proiektu-kontratuaren salmentako entitateekin lotu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-169">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="5b1d5-170">Gaitasun honek iraupen luzeko proiektu kontratuetarako zehaztutako prezioak onartzen ditu, non prezio-zerrenda bat baino gehiago eska dezakezun inflazioaren ondorioz gertatzen diren prezioen eguneratzeak kontatzeko.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-170">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="5b1d5-171">Hala ere, bezeroa, abagunea, eskaintza edo proiektu-kontratuaren entitatearekin lotzen dituzun prezioen zerrendek data eraginkortasun bat badute, baliteke prezio lehenetsiak okerrak izatea.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-171">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="5b1d5-172">Hori dela eta, ziurtatu behar duzu data eraginkortasuna bata bestearen gainjartzen duten proiektuen prezio-zerrendak ez daudela entitate horiekin lotuta.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-172">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>

### <a name="deal-specific-price-overrides"></a><span data-ttu-id="5b1d5-173">Eskaintzari buruzko prezioen baliogabetzea</span><span class="sxs-lookup"><span data-stu-id="5b1d5-173">Deal-specific price overrides</span></span>

<span data-ttu-id="5b1d5-174">Eskaintzaren berariazko berrientzat sor ditzakezu eskaintzaren edo proiektu-kontratuan lehenetsitako proiektuen prezio-zerrendetan.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-174">You can create deal-specific overrides for selected prices on project price lists that are entered by default on a quote or project contract.</span></span>

<span data-ttu-id="5b1d5-175">Berez, proiektu-kontratuak salmenta prezio-zerrenda nagusiaren kopia bat lortzen du beti harekin lotura zuzena izan beharrean.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-175">By default, a project contract always gets a copy of the master sales price list instead of a direct link to it.</span></span> <span data-ttu-id="5b1d5-176">Jokabide horrek bezeroari lanaren aitorpenerako (SOW) bezeroari egiten dizkion prezioen hitzarmenak bermatzen laguntzen du prezio-zerrenda nagusia aldatzen bada.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-176">This behavior helps guarantee that price agreements that are made with a customer for a statement of work (SOW) don't change if the master price list is changed.</span></span>

<span data-ttu-id="5b1d5-177">Hala ere, eskaintzan, prezio-zerrenda maisua erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-177">However, on a quote, you can use a master price list.</span></span> <span data-ttu-id="5b1d5-178">Bestela, prezioe-zerrenda nagusia kopiatu eta editatu dezakezu eskaintza horietara soilik aplikatzen den prezio-zerrenda pertsonalizatua sortzeko.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-178">Alternatively, you can copy a master price list and edit it to create a custom price list that applies only to that quote.</span></span> <span data-ttu-id="5b1d5-179">Eskaintzen inguruko prezio-zerrenda berria sortzeko, **Eskaintza** orrian, hautatu **Sortu prezio pertsonalizatuak**.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-179">To create a new price list that is specific to a quote, on the **Quote** page, select **Create custom pricing**.</span></span> <span data-ttu-id="5b1d5-180">Eskaintzen proiektuaren berariazko prezio-zerrendara sar dezakezu eskaintzetan soilik.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-180">You can access the deal-specific project price list only from the quote.</span></span> 

<span data-ttu-id="5b1d5-181">Proiektuen prezio-zerrenda pertsonalizatua sortzen duzunean, prezio-zerrendako proiektuaren osagaiak soilik kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-181">When you create a custom project price list, only the project components of the price list are copied.</span></span> <span data-ttu-id="5b1d5-182">Bestela esanda, eskaintzan erantsitako proiektuaren prezio-zerrendaren kopia gisa sortu da prezio-zerrenda berria, eta prezio-zerrenda berri honek funtzio prezioak eta transakzioen kategorien prezioak soilik ditu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-182">In other words, a new price list created as a copy of the existing project price list that is attached on the quote, and this new price list has only related role prices and transaction category prices.</span></span>
  
## <a name="tracking-costs"></a><span data-ttu-id="5b1d5-183">Kostuen segimendua</span><span class="sxs-lookup"><span data-stu-id="5b1d5-183">Tracking costs</span></span>

<span data-ttu-id="5b1d5-184">Project Operations-en proiektuen giza baliabideen denboraren kostuak kontrolatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-184">Project Operations tracks costs for the use of human resource time on projects.</span></span> <span data-ttu-id="5b1d5-185">Proiektuan zehar sortzen diren beste gastu batzuen kostuak ere kontrolatzen ditu, hala nola bidaien gastuak.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-185">It also tracks costs for other expenses that are incurred during the project, such as travel expenses.</span></span>

<span data-ttu-id="5b1d5-186">Fakturen tasak bezala, giza baliabideen kostu tasak ere ezartzen dira prezio-zerrendak erabiliz.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-186">Like bill rates, cost rates for human resources are also set up using price lists.</span></span> <span data-ttu-id="5b1d5-187">Hona hemen kostuen prezio-zerrendaren eta salmenten prezio-zerrendaren portaeraren desberdintasun nagusiak:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-187">Here are the main differences in the behavior of the cost price list and sales price list:</span></span>

- <span data-ttu-id="5b1d5-188">Baliabide baten kostu-tasa ezin da proiektu, kontratu edo eskaintza jakin batean gainidatzi.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-188">The cost rate of a resource can’t be overridden on a specific project, contract, or quote.</span></span> <span data-ttu-id="5b1d5-189">Hala eta guztiz ere, fakturen tasak salbuetsi daitezke salerosketa bakoitzaren arabera, tratuaren izaeraren araberako aldaketak egiten badira.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-189">However, bill rates can be overridden on a per-deal basis if changes are made that are specific to the nature of the deal.</span></span> 

- <span data-ttu-id="5b1d5-190">Hurrengo eskaera kostuen prezio-zerrenda ebazteko erabiltzen da:</span><span class="sxs-lookup"><span data-stu-id="5b1d5-190">The following order is used to resolve a cost price list:</span></span>

    1. <span data-ttu-id="5b1d5-191">Unitate antolatzaileari atxikitako kostuen prezio-zerrenda.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-191">The cost price list that is attached to the organizational unit.</span></span>
    2. <span data-ttu-id="5b1d5-192">Project Operations-eko parametroei atxikitako kostuen prezio-zerrenda.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-192">The cost price list that is attached to the Project Operations parameters.</span></span> <span data-ttu-id="5b1d5-193">Parametroetara kostuen prezio-zerrendak erantsi daitezkeenez, moneta bat egiten du proiektuaren, kontratuaren edo eskaintzaren unitate antolatzailearen kontratuaren moneta eta kostuen prezio-zerrendaren monetaren artean.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-193">Because cost price lists in many different currencies can be attached to the parameters, a currency match is completed between the currency of the contracting organizational unit of the project, contract, or quote, and the currency of the cost price list.</span></span>
    3. <span data-ttu-id="5b1d5-194">Gastuei dagokienez, kostu prezioen eta gainprezioaren gaineko prezioen metodoak ez dira kostuen prezio-zerrendetan aplikatzen.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-194">For expenses, the at-cost and markup-over-cost pricing methods don’t apply to cost price lists.</span></span> <span data-ttu-id="5b1d5-195">Nahiz eta prezio metodo horiek kostu prezio-zerrendako lerroetan erabili, transakzioen kategorien kostuak konfiguratzeko, sistemak ez ditu jaramonik egiten eta ez da kostu prezio lehenetsirik sartuko.</span><span class="sxs-lookup"><span data-stu-id="5b1d5-195">Even if these pricing methods are used on cost price list lines to set up transaction category costs, the system ignores them, and no default cost price is entered.</span></span>