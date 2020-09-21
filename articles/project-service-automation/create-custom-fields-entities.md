---
title: Sortu eremu eta entitate pertsonalizatuak
description: Gai honetan Power Apps plataformako soluzioan aukera multzoak eta entitateak nola sortu azaltzen da.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748930"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="81548-103">Sortu eremu eta entitate pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="81548-103">Create custom fields and entities</span></span> 

<span data-ttu-id="81548-104">Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean Power Apps plataforman.</span><span class="sxs-lookup"><span data-stu-id="81548-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="81548-105">Gai honetako prozedurak Project Service Automation-en (PSA) web interfazea erabiliz osatu behar dira.</span><span class="sxs-lookup"><span data-stu-id="81548-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="81548-106">Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea.</span><span class="sxs-lookup"><span data-stu-id="81548-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="81548-107">Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du.</span><span class="sxs-lookup"><span data-stu-id="81548-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="81548-108">Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="81548-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="81548-109">Sortu prezio-dimentsioetarako soluzio pertsonalizatua</span><span class="sxs-lookup"><span data-stu-id="81548-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="81548-110">PSAn, egin klik **Ezarpenak** > **Soluzioak** aukeran eta, ondoren, egin klik **Berria** aukeran soluzio berri bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="81548-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="81548-111">Soluzioari eman **\<zure erakundearen izena> prezio-dimentsioak** izena, sartu gainerako beharrezko informazioa eta ondoren egin klik **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="81548-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![Sortu prezio-dimentsioetarako soluzio pertsonalizatua](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="81548-113">Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="81548-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="81548-114">Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="81548-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="81548-115">Biak prezio-soluzioan sortu behar dira.</span><span class="sxs-lookup"><span data-stu-id="81548-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="81548-116">Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.</span><span class="sxs-lookup"><span data-stu-id="81548-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="81548-117">Entitatean oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="81548-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="81548-118">PSAn egin klik **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **\<zure erakundearen izena> prezioen dimentsioak** atalean.</span><span class="sxs-lookup"><span data-stu-id="81548-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="81548-119">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="81548-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="81548-120">Egin klik **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="81548-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="81548-121">Sartu geratzen den informazioa eta, ondoren, egin klik **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="81548-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![Titulu estandarraren entitatearen definizioa](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="81548-123">Aukera multzoetan oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="81548-123">Option set-based dimensions</span></span> 
<span data-ttu-id="81548-124">Aukera multzoan oinarritutako bi dimentsio sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="81548-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="81548-125">**Baliabideen lanaren kokapena** entitatea **Hasiera** kokapen lanaren eta **Gunean** lanaren prezioaren jarraipena egiteko, eta erabili **Baliabideen lanorduak** entitatea **Ohiko** eta **Aparteko orduak** entitateetan lana amaitutakoan gainprezio bat aplikatzeko.</span><span class="sxs-lookup"><span data-stu-id="81548-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="81548-126">PSAn egin klik **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **\<zure erakundearen izena> prezioen dimentsioak** atalean.</span><span class="sxs-lookup"><span data-stu-id="81548-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="81548-127">Soluzio arakatzailean, ezkerreko nabigazio-panelean, hautatu **Aukera multzoak**.</span><span class="sxs-lookup"><span data-stu-id="81548-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="81548-128">Egin klik **Berria** aukeran aukera multzo berri bat sortzeko, sartu falta den informazioa eta egin klik **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="81548-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="81548-129">Baliabideen lanaren kokalekua izeneko aukera multzoan oinarritutako prezio-dimentsioa</span><span class="sxs-lookup"><span data-stu-id="81548-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="81548-130">Baliabideen lanorduen izeneko aukera multzoan oinarritutako prezio-dimentsioa</span><span class="sxs-lookup"><span data-stu-id="81548-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="81548-131">Sortu datuak erakundeetan oinarritutako dimentsioetarako</span><span class="sxs-lookup"><span data-stu-id="81548-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="81548-132">Erakundeetan oinarritutako dimentsioetarako datuak sor ditzakezu eskuz edo Microsoft Excel inportazio edo zerbitzu deiak erabiliz.</span><span class="sxs-lookup"><span data-stu-id="81548-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="81548-133">Erabili prozedura honen urratsak bi titulu estandar sortzeko, adibidez, **Sistemen ingeniaria** eta **Sistemen ingeniari nagusia**, **Titulu estandarra** entitatean oinarritutako dimentsiotik.</span><span class="sxs-lookup"><span data-stu-id="81548-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="81548-134">Sortu nahi dituzun datuak txikiak badira, hurrengo adibidean bezala, inprimaki estandarra erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="81548-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="81548-135">PSAn, sakatu **Bilaketa aurreratua**.</span><span class="sxs-lookup"><span data-stu-id="81548-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="81548-136">Hautatu entitatea eta, ondoren, **Titulu estandarra** atalean, sakatu **Emaitzak**.</span><span class="sxs-lookup"><span data-stu-id="81548-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="81548-137">**Titulu estandarra** entitateko errenkada guztiak erakutsiko dira.</span><span class="sxs-lookup"><span data-stu-id="81548-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="81548-138">Sakatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="81548-138">Click **New**.</span></span> <span data-ttu-id="81548-139">**Izena** atalean, idatzi "Sistemen ingeniaria" eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="81548-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="81548-140">Itxi inprimakia.</span><span class="sxs-lookup"><span data-stu-id="81548-140">Close the form.</span></span> 
4. <span data-ttu-id="81548-141">Errepikatu 1-3 urratsak "Sistemen ingeniari nagusia" titulu estandarra sortzeko.</span><span class="sxs-lookup"><span data-stu-id="81548-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="81548-142">Titulu estandarraren entitatearen laginak</span><span class="sxs-lookup"><span data-stu-id="81548-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="81548-143">Gehitu beharrezko PSA entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="81548-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="81548-144">Project Service-eko entitate hauek gehitu beharko dituzu prezio-soluzioan.</span><span class="sxs-lookup"><span data-stu-id="81548-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="81548-145">Erabili prozedura honen urratsak prezio-soluzioaren eskema garrantzitsu batzuk egiteko, entitateak prezio-dimentsio berriez jabetzeko.</span><span class="sxs-lookup"><span data-stu-id="81548-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="81548-146">PSAn egin klik **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **\<zure erakundearen izena> prezioen dimentsioak** atalean.</span><span class="sxs-lookup"><span data-stu-id="81548-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="81548-147">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Gehitu badaudenak** > **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="81548-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="81548-148">**Soluzio-osagaiak** elkarrizketa-koadroan, hautatu aukera hauetariko bat:</span><span class="sxs-lookup"><span data-stu-id="81548-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="81548-149">Benetakoa</span><span class="sxs-lookup"><span data-stu-id="81548-149">Actual</span></span>
- <span data-ttu-id="81548-150">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="81548-150">Bookable Resource</span></span>
- <span data-ttu-id="81548-151">Aurreikuspenaren lerroa</span><span class="sxs-lookup"><span data-stu-id="81548-151">Estimate Line</span></span>
- <span data-ttu-id="81548-152">Fakturaren lerroaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="81548-152">Invoice Line Detail</span></span>
- <span data-ttu-id="81548-153">Kutxako liburuaren lerroa</span><span class="sxs-lookup"><span data-stu-id="81548-153">Journal Line</span></span>
- <span data-ttu-id="81548-154">Proiektu-kontratuaren lerroko xehetasunak</span><span class="sxs-lookup"><span data-stu-id="81548-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="81548-155">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="81548-155">Project Team Member</span></span>
- <span data-ttu-id="81548-156">Eskaintzaren lerroaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="81548-156">Quote Line Detail</span></span>
- <span data-ttu-id="81548-157">Funtzio-prezioaren gainprezioa</span><span class="sxs-lookup"><span data-stu-id="81548-157">Role Price Markup</span></span>
- <span data-ttu-id="81548-158">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="81548-158">Role Price</span></span> 
- <span data-ttu-id="81548-159">Denbora-sarrera</span><span class="sxs-lookup"><span data-stu-id="81548-159">Time Entry</span></span> 

> ![Gehitu lehendik dauden entitateak prezio-dimentsioen soluzioari](media/Existing-entities-to-PD-solution.png)

> ![Hautatu soluzioaren osagaiak](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="81548-162">Ziurtatu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak sartzea.</span><span class="sxs-lookup"><span data-stu-id="81548-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="81548-163">Goiko hautatutako entitateen menpeko erakunderen bat eskatuko zaizunean, egin klik **Ez** aukeran.</span><span class="sxs-lookup"><span data-stu-id="81548-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![Ez sartu erlazionatutako osagaiak](media/Do-not-include-required.png)


