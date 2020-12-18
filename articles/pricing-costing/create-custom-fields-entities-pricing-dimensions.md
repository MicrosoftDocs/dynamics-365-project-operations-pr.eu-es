---
title: Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa
description: Gai honek aukera multzo pertsonalizatuak edo entitateak nola sortu jakiteko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: fc5917856b8f28d36dc55593a68eba7823a00b36
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642798"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="14697-103">Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa</span><span class="sxs-lookup"><span data-stu-id="14697-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="14697-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="14697-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="14697-105">Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean prezio-dimentsio gisa erabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="14697-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="14697-106">Informazio gehiago lortzeko, ikusi [Prezio-dimentsioen informazio orokorra](pricing-dimensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="14697-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="14697-107">Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea.</span><span class="sxs-lookup"><span data-stu-id="14697-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="14697-108">Praktika on garrantzitsu honek malgutasuna eskaintzen du etorkizunean aldaketak beharren arabera eguneratu edo kentzeko.</span><span class="sxs-lookup"><span data-stu-id="14697-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="14697-109">Horrek zure lana berrerabiltzen lagunduko du eta aldaketa hauek beste instantzia batera eramatea erraztuko du Eskatutako aldaketa guztiak egin ondoren, esportatu irtenbide hau **Kudeatutako soluzioa** eta inportatu beste instantzia batzuetara zure prezioen konfigurazioa berrerabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="14697-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="14697-110">Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="14697-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="14697-111">Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="14697-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="14697-112">Biak prezio-soluzioan sortu behar dira.</span><span class="sxs-lookup"><span data-stu-id="14697-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="14697-113">Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.</span><span class="sxs-lookup"><span data-stu-id="14697-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="14697-114">Entitatean oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="14697-114">Entity-based dimensions</span></span>
<span data-ttu-id="14697-115">Entitateetan oinarritutako dimentsioak sortzeko, jarraitu urrats hauei:</span><span class="sxs-lookup"><span data-stu-id="14697-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="14697-116">Joan **Ezarpenak** > **Soluzioak** aukerara eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="14697-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="14697-117">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="14697-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="14697-118">Hautatu **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="14697-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="14697-119">Sartu geratzen den informazioa eta, ondoren, hautatu **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="14697-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![Titulu estandarraren entitatearen definizioa](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="14697-121">Aukera multzoetan oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="14697-121">Option set-based dimensions</span></span> 
<span data-ttu-id="14697-122">Aukera multzoan oinarritutako bi dimentsio sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="14697-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="14697-123">Erabili **Baliabideen lanaren kokapena** prezioaren jarraipena egiteko **Etxea** kokapen lana eta **Gunean** lana.</span><span class="sxs-lookup"><span data-stu-id="14697-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="14697-124">Erabili **Baliabideen lan orduak** balioekin **Erregularra** eta **Aparteko orduak** lana amaitutakoan marka bat aplikatzeko.</span><span class="sxs-lookup"><span data-stu-id="14697-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="14697-125">Ondorengo grafikoan **Baliabideen lanaren kokapena** dimentsioa.</span><span class="sxs-lookup"><span data-stu-id="14697-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![Baliabideen lanaren kokalekua izeneko aukera multzoan oinarritutako prezio-dimentsioa](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="14697-127">Ondorengo grafikoan **Baliabideen lan-orduak** dimentsioa.</span><span class="sxs-lookup"><span data-stu-id="14697-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![Baliabideen lanorduen izeneko aukera multzoan oinarritutako prezio-dimentsioa](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="14697-129">Joan **Ezarpenak** > **Soluzioak** aukerara eta sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="14697-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="14697-130">Soluzio arakatzailean, ezkerreko nabigazio-panelean, hautatu **Aukera multzoak**.</span><span class="sxs-lookup"><span data-stu-id="14697-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="14697-131">Hautatu **Berria** aukeran aukera multzo berri bat sortzeko, sartu falta den informazioa eta hautatu **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="14697-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="14697-132">Sortu datuak erakundeetan oinarritutako dimentsioetarako</span><span class="sxs-lookup"><span data-stu-id="14697-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="14697-133">Erakundeetan oinarritutako dimentsioetarako datuak sor ditzakezu eskuz edo Microsoft Excel inportazio edo zerbitzu deiak erabiliz.</span><span class="sxs-lookup"><span data-stu-id="14697-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="14697-134">Erabili prozedura honen urratsak bi titulu estandar sortzeko, adibidez, **Sistemen ingeniaria** eta **Sistemen ingeniari nagusia**, **Titulu estandarra** entitatean oinarritutako dimentsiotik.</span><span class="sxs-lookup"><span data-stu-id="14697-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="14697-135">Sortu nahi dituzun datuak txikiak badira, hurrengo adibidean bezala, inprimaki estandarra erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="14697-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="14697-136">Hautatu **Bilaketa aurreratua** atalera.</span><span class="sxs-lookup"><span data-stu-id="14697-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="14697-137">Hautatu entitatea eta, ondoren, **Titulu estandarra** atalean, hautatu **Emaitzak**.</span><span class="sxs-lookup"><span data-stu-id="14697-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="14697-138">**Titulu estandarra** entitateko errenkada guztiak erakutsiko dira.</span><span class="sxs-lookup"><span data-stu-id="14697-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="14697-139">Hautatu **Berria**, eta **Izena** atalean, idatzi "Sistemen ingeniaria" eta, ondoren, hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="14697-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="14697-140">Itxi orria.</span><span class="sxs-lookup"><span data-stu-id="14697-140">Close the page.</span></span> 
5. <span data-ttu-id="14697-141">Errepikatu 1-3 urratsak "Sistemen ingeniari nagusia" titulu estandarra sortzeko.</span><span class="sxs-lookup"><span data-stu-id="14697-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![Titulu estandarraren entitatearen laginak](media/ST-data.png)
