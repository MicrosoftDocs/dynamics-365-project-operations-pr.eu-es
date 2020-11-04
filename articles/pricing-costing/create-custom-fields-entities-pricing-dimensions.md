---
title: Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa
description: Gai honek aukera multzo pertsonalizatuak edo entitateak nola sortu jakiteko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 9dd43be79f8e906298578911b3bff03e66c2f1e5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071074"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="e8cf0-103">Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa</span><span class="sxs-lookup"><span data-stu-id="e8cf0-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="e8cf0-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="e8cf0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e8cf0-105">Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e8cf0-106">Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="e8cf0-107">Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="e8cf0-108">Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="e8cf0-109">Sortu prezio-dimentsioetarako soluzio pertsonalizatua</span><span class="sxs-lookup"><span data-stu-id="e8cf0-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="e8cf0-110">Joan **Ezarpenak** > **Soluzioak** aukerara eta, ondoren, hautatu **Berria** aukeran soluzio berri bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-110">Go to **Settings** > **Solutions** , and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="e8cf0-111">Soluzioari eman **\<your organization name> prezio-dimentsioak** izena, sartu gainerako beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-111">Name the solution, **\<your organization name> pricing dimensions** , enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="e8cf0-112">Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="e8cf0-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="e8cf0-113">Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="e8cf0-114">Biak prezio-soluzioan sortu behar dira.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="e8cf0-115">Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="e8cf0-116">Entitatean oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="e8cf0-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="e8cf0-117">Joan **Ezarpenak** > **Soluzioak** aukerara eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-117">Go to **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="e8cf0-118">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="e8cf0-119">Hautatu **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="e8cf0-120">Sartu geratzen den informazioa eta, ondoren, hautatu **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="e8cf0-121">Aukera multzoetan oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="e8cf0-121">Option set-based dimensions</span></span> 
<span data-ttu-id="e8cf0-122">Aukera multzoan oinarritutako bi dimentsio sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="e8cf0-123">**Baliabideen lanaren kokapena** entitatea **Hasiera** kokapen lanaren eta **Gunean** lanaren prezioaren jarraipena egiteko, eta erabili **Baliabideen lanorduak** entitatea **Ohiko** eta **Aparteko orduak** entitateetan lana amaitutakoan gainprezio bat aplikatzeko.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="e8cf0-124">Joan **Ezarpenak** > **Soluzioak** aukerara eta sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-124">Go to **Settings** > **Solutions** , and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="e8cf0-125">Soluzio arakatzailean, ezkerreko nabigazio-panelean, hautatu **Aukera multzoak**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="e8cf0-126">Hautatu **Berria** aukeran aukera multzo berri bat sortzeko, sartu falta den informazioa eta hautatu **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="e8cf0-127">Sortu datuak erakundeetan oinarritutako dimentsioetarako</span><span class="sxs-lookup"><span data-stu-id="e8cf0-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="e8cf0-128">Erakundeetan oinarritutako dimentsioetarako datuak sor ditzakezu eskuz edo Microsoft Excel inportazio edo zerbitzu deiak erabiliz.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="e8cf0-129">Erabili prozedura honen urratsak bi titulu estandar sortzeko, adibidez, **Sistemen ingeniaria** eta **Sistemen ingeniari nagusia** , **Titulu estandarra** entitatean oinarritutako dimentsiotik.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="e8cf0-130">Sortu nahi dituzun datuak txikiak badira, hurrengo adibidean bezala, inprimaki estandarra erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="e8cf0-131">Hautatu **Bilaketa aurreratua** , hautatu entitatea **Izenburu estandarra** eta, ondoren, hautatu **Emaitzak**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-131">Select **Advanced Find** , select the entity **Standard Title** , and then select **Results**.</span></span> <span data-ttu-id="e8cf0-132">**Titulu estandarra** entitateko errenkada guztiak erakutsiko dira.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="e8cf0-133">Hautatu **Berria** , eta **Izena** atalean, idatzi "Sistemen ingeniaria" eta, ondoren, hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-133">Select **New** , and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="e8cf0-134">Itxi inprimakia.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-134">Close the form.</span></span> 
4. <span data-ttu-id="e8cf0-135">Errepikatu 1-3 urratsak "Sistemen ingeniari nagusia" titulu estandarra sortzeko.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="e8cf0-136">Gehitu beharrezko entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="e8cf0-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="e8cf0-137">Entitate hauek gehitu beharko dituzu prezio-soluzioan.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="e8cf0-138">Erabili prozedura honen urratsak prezio-soluzioaren eskema garrantzitsu batzuk egiteko, entitateak prezio-dimentsio berriez jabetzeko.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="e8cf0-139">Hautatu **Ezarpenak** > **Soluzioak** eta sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-139">Select **Settings** > **Solutions** , and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="e8cf0-140">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Gehitu badaudenak** > **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="e8cf0-141">**Soluzio-osagaiak** elkarrizketa-koadroan, hautatu aukera hauetariko bat:</span><span class="sxs-lookup"><span data-stu-id="e8cf0-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="e8cf0-142">Benetakoa</span><span class="sxs-lookup"><span data-stu-id="e8cf0-142">Actual</span></span>
  - <span data-ttu-id="e8cf0-143">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="e8cf0-143">Bookable Resource</span></span>
  - <span data-ttu-id="e8cf0-144">Aurreikuspenaren lerroa</span><span class="sxs-lookup"><span data-stu-id="e8cf0-144">Estimate Line</span></span>
  - <span data-ttu-id="e8cf0-145">Fakturaren lerroaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="e8cf0-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="e8cf0-146">Kutxako liburuaren lerroa</span><span class="sxs-lookup"><span data-stu-id="e8cf0-146">Journal Line</span></span>
  - <span data-ttu-id="e8cf0-147">Proiektu-kontratuaren lerroko xehetasunak</span><span class="sxs-lookup"><span data-stu-id="e8cf0-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="e8cf0-148">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="e8cf0-148">Project Team Member</span></span>
  - <span data-ttu-id="e8cf0-149">Eskaintzaren lerroaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="e8cf0-149">Quote Line Detail</span></span>
  - <span data-ttu-id="e8cf0-150">Funtzio-prezioaren gainprezioa</span><span class="sxs-lookup"><span data-stu-id="e8cf0-150">Role Price Markup</span></span>
  - <span data-ttu-id="e8cf0-151">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="e8cf0-151">Role Price</span></span> 
  - <span data-ttu-id="e8cf0-152">Denbora-sarrera</span><span class="sxs-lookup"><span data-stu-id="e8cf0-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="e8cf0-153">Ziurtatu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak sartzea.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="e8cf0-154">Goiko hautatutako entitateen menpeko erakunderen bat eskatuko zaizunean, hautatu **Ez** aukeran.</span><span class="sxs-lookup"><span data-stu-id="e8cf0-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

