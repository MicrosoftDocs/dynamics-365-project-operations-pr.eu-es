---
title: Sortu eremu eta entitate pertsonalizatuak
description: Gai honetan Power Apps plataformako soluzioan aukera multzoak eta entitateak nola sortu azaltzen da.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: c58745a46e84a40b90fbb3cbf89b10e293588fc3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290509"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="09471-103">Sortu eremu eta entitate pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="09471-103">Create custom fields and entities</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="09471-104">Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean Power Apps plataforman.</span><span class="sxs-lookup"><span data-stu-id="09471-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="09471-105">Gai honetako prozedurak Project Service Automation-en (PSA) web interfazea erabiliz osatu behar dira.</span><span class="sxs-lookup"><span data-stu-id="09471-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="09471-106">Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea.</span><span class="sxs-lookup"><span data-stu-id="09471-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="09471-107">Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du.</span><span class="sxs-lookup"><span data-stu-id="09471-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="09471-108">Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="09471-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="09471-109">Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="09471-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="09471-110">Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="09471-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="09471-111">Biak prezio-soluzioan sortu behar dira.</span><span class="sxs-lookup"><span data-stu-id="09471-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="09471-112">Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.</span><span class="sxs-lookup"><span data-stu-id="09471-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="09471-113">Entitatean oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="09471-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="09471-114">PSAn, sakatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="09471-114">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="09471-115">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="09471-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="09471-116">Egin klik **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="09471-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="09471-117">Sartu geratzen den informazioa eta, ondoren, egin klik **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="09471-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![Titulu estandarraren entitatearen definizioa](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="09471-119">Aukera multzoetan oinarritutako dimentsioak</span><span class="sxs-lookup"><span data-stu-id="09471-119">Option set-based dimensions</span></span> 
<span data-ttu-id="09471-120">Aukera multzoan oinarritutako bi dimentsio sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="09471-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="09471-121">**Baliabideen lanaren kokapena** entitatea **Hasiera** kokapen lanaren eta **Gunean** lanaren prezioaren jarraipena egiteko, eta erabili **Baliabideen lanorduak** entitatea **Ohiko** eta **Aparteko orduak** entitateetan lana amaitutakoan gainprezio bat aplikatzeko.</span><span class="sxs-lookup"><span data-stu-id="09471-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="09471-122">PSAn, sakatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="09471-122">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="09471-123">Soluzio arakatzailean, ezkerreko nabigazio-panelean, hautatu **Aukera multzoak**.</span><span class="sxs-lookup"><span data-stu-id="09471-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="09471-124">Egin klik **Berria** aukeran aukera multzo berri bat sortzeko, sartu falta den informazioa eta egin klik **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="09471-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="09471-125">Baliabideen lanaren kokalekua izeneko aukera multzoan oinarritutako prezio-dimentsioa</span><span class="sxs-lookup"><span data-stu-id="09471-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="09471-126">Baliabideen lanorduen izeneko aukera multzoan oinarritutako prezio-dimentsioa</span><span class="sxs-lookup"><span data-stu-id="09471-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="09471-127">Sortu datuak erakundeetan oinarritutako dimentsioetarako</span><span class="sxs-lookup"><span data-stu-id="09471-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="09471-128">Erakundeetan oinarritutako dimentsioetarako datuak sor ditzakezu eskuz edo Microsoft Excel inportazio edo zerbitzu deiak erabiliz.</span><span class="sxs-lookup"><span data-stu-id="09471-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="09471-129">Erabili prozedura honen urratsak bi titulu estandar sortzeko, adibidez, **Sistemen ingeniaria** eta **Sistemen ingeniari nagusia**, **Titulu estandarra** entitatean oinarritutako dimentsiotik.</span><span class="sxs-lookup"><span data-stu-id="09471-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="09471-130">Sortu nahi dituzun datuak txikiak badira, hurrengo adibidean bezala, inprimaki estandarra erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="09471-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="09471-131">PSAn, sakatu **Bilaketa aurreratua**.</span><span class="sxs-lookup"><span data-stu-id="09471-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="09471-132">Hautatu entitatea eta, ondoren, **Titulu estandarra** atalean, sakatu **Emaitzak**.</span><span class="sxs-lookup"><span data-stu-id="09471-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="09471-133">**Titulu estandarra** entitateko errenkada guztiak erakutsiko dira.</span><span class="sxs-lookup"><span data-stu-id="09471-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="09471-134">Sakatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="09471-134">Click **New**.</span></span> <span data-ttu-id="09471-135">**Izena** atalean, idatzi "Sistemen ingeniaria" eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="09471-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="09471-136">Itxi inprimakia.</span><span class="sxs-lookup"><span data-stu-id="09471-136">Close the form.</span></span> 
4. <span data-ttu-id="09471-137">Errepikatu 1-3 urratsak "Sistemen ingeniari nagusia" titulu estandarra sortzeko.</span><span class="sxs-lookup"><span data-stu-id="09471-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="09471-138">Titulu estandarraren entitatearen laginak</span><span class="sxs-lookup"><span data-stu-id="09471-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]