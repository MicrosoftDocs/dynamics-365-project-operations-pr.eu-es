---
title: Ikusi baliabideen erabilera kargagarria
description: Gai honek baliabideen erabilerari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.prod: Applies to all versions of Project Service
ms.technology: Applies to all versions of Project Service
ms.assetid: 656511ac-6851-42d6-abd4-0c7e77ea5d9c
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8953015ced24ff10f0bec2570a840cf4e130b01a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748813"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="51d0c-103">Ikusi baliabideen erabilera kargagarria</span><span class="sxs-lookup"><span data-stu-id="51d0c-103">View chargeable utilization for resources</span></span>
 
<span data-ttu-id="51d0c-104">**Erabileraren ikuspegia** **Project Service-en baliabideen erabilera** orrialdean erreserbagarria den baliabidearen erabilera kargagarria erakusten da.</span><span class="sxs-lookup"><span data-stu-id="51d0c-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="51d0c-105">Ikuspegia antolaketan oinarrituta dagoenez aurkituko dituzu funtzio berdin asko.</span><span class="sxs-lookup"><span data-stu-id="51d0c-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![Ikuspegi Utilization Eginbideei](media/FAQ-utilization-1.png)
 

<span data-ttu-id="51d0c-107">Kalkuluak chargeable utilization funtzionatzen duela honela:</span><span class="sxs-lookup"><span data-stu-id="51d0c-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="51d0c-108">Chargeable utilization = (benetako ordu kargagarriak) / (baliabidearen ahalmena).</span><span class="sxs-lookup"><span data-stu-id="51d0c-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="51d0c-109">Gelaxkek kalkulatutako erabilera kargagarria adierazten dute hautatutako aldirako (egunak, asteak edo hilabeteak).</span><span class="sxs-lookup"><span data-stu-id="51d0c-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="51d0c-110">Erakutsi beren helburuko chargeable utilization as compared to baliabide chargeable utilization gelaxka bakoitzak koloreak.</span><span class="sxs-lookup"><span data-stu-id="51d0c-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="51d0c-111">Helburuko erabilera ezar daiteke edozer baliabideen funtzio lehenetsia edo baliabide taldeetan horri berari.</span><span class="sxs-lookup"><span data-stu-id="51d0c-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="51d0c-112">Kalkuluak begiratzen dio helburuko pertsonria lehenik eta behin, eta ondoren, baliabide-funtzio lehenetsiari.</span><span class="sxs-lookup"><span data-stu-id="51d0c-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="51d0c-113">Ezarri xedea baliabide batean</span><span class="sxs-lookup"><span data-stu-id="51d0c-113">Set target on a resource</span></span>

1. <span data-ttu-id="51d0c-114">Joan **Baliabideak** \> **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="51d0c-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="51d0c-115">Hautatu baliabide bat erregistroa irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="51d0c-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="51d0c-116">**Project Service** fitxan, helburuko erabilera ere ezar dezakezu baliabiderako.</span><span class="sxs-lookup"><span data-stu-id="51d0c-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![Eginbideei erabiltzearen arriskua helburuko utilization ezartzeko Project Service fitxan aurki daiteke](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="51d0c-118">Ezarri xedeen erabilera funtzio batean</span><span class="sxs-lookup"><span data-stu-id="51d0c-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="51d0c-119">Joan **Baliabideak** \> **Baliabidea funtzioak** atalera.</span><span class="sxs-lookup"><span data-stu-id="51d0c-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="51d0c-120">Hautatu funtzio bat erregistroa irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="51d0c-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="51d0c-121">Ezarri helburuko erabilera funtziorako.</span><span class="sxs-lookup"><span data-stu-id="51d0c-121">Set the target utilization for the role.</span></span>

> ![Eginbideei erabiltzearen arriskua helburuko utilization ezartzeko Project Service fitxan aurki daiteke](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="51d0c-123">Kalkulatu baliabideen erabilera kargagarria</span><span class="sxs-lookup"><span data-stu-id="51d0c-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="51d0c-124">Baliabide erabilera kargagarria kalkulatzeko aurrebaldintza batzuk bete beharko dituzu.</span><span class="sxs-lookup"><span data-stu-id="51d0c-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="51d0c-125">Ezarri funtzio lehenetsia baliabide indibidualetarako</span><span class="sxs-lookup"><span data-stu-id="51d0c-125">Set default role for individual resource</span></span>

<span data-ttu-id="51d0c-126">Lehenik, helburuko erabilera ezar daiteke banako baliabidean edo baliabide-funtzioetan.</span><span class="sxs-lookup"><span data-stu-id="51d0c-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="51d0c-127">Helburuak baliabide-funtzioak erabiltzen ari bazara, baliabide taldeetan izan behar du funtzio lehenetsia.</span><span class="sxs-lookup"><span data-stu-id="51d0c-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="51d0c-128">Hau ezartzeko, joan **Baliabideak** \> **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="51d0c-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="51d0c-129">Aukeratu baliabide bat, ireki erregistroa eta, ondoren, hautatu **Project Service** fitxa.</span><span class="sxs-lookup"><span data-stu-id="51d0c-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="51d0c-130">**Baliabideen funtzioa** saretan, ziurtatu funtzio bat dagoela baliabiderako eta **Lehenespenezkoa da** ezarrita dagoela **Bai** aukeran.</span><span class="sxs-lookup"><span data-stu-id="51d0c-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="51d0c-131">Aldatu baliabide-funtzio honen fakturazio mota.</span><span class="sxs-lookup"><span data-stu-id="51d0c-131">Change billing type for resource role</span></span>

<span data-ttu-id="51d0c-132">Baliabide-funtzioak izan fakturazio mota **Kargagarria** ezarri behar da.</span><span class="sxs-lookup"><span data-stu-id="51d0c-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="51d0c-133">Joan **Baliabideak** \> **Baliabidea funtzioak** atalera.</span><span class="sxs-lookup"><span data-stu-id="51d0c-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="51d0c-134">Ireki eguneratu nahi duzun erregistro bat irekitzeko eta, ondoren, ezarri **Kargagarria** mota lehenetsia fakturazio-funtzio bat.</span><span class="sxs-lookup"><span data-stu-id="51d0c-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="51d0c-135">Ezarri baliabide funtzioetarako lanorduak</span><span class="sxs-lookup"><span data-stu-id="51d0c-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="51d0c-136">Baliabidearen ahalmena kalkuluak lanorduak izan behar du.</span><span class="sxs-lookup"><span data-stu-id="51d0c-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="51d0c-137">Joan **Baliabideak** \> **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="51d0c-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="51d0c-138">Hautatu baliabidea erregistroa irekitzeko eta hautatu **Erakutsi lanorduak**.</span><span class="sxs-lookup"><span data-stu-id="51d0c-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="51d0c-139">Baliabideen zerrenda eguneratu dezakezu **Lanordu txantiloia** aplikatuz **Baliabide zerrenda** ikuspegitik.</span><span class="sxs-lookup"><span data-stu-id="51d0c-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="51d0c-140">Kargatzeko benetako orduak konpontzeko arazoak</span><span class="sxs-lookup"><span data-stu-id="51d0c-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="51d0c-141">Bertan, entitate kargagarria **Benetako datuak** entitatetik hartzen da.</span><span class="sxs-lookup"><span data-stu-id="51d0c-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="51d0c-142">Fakturazio-mota dute **Kargagarria** batekin kalkuluetan agertzen dena eta horregatik izan behar duzu projects non sartuko den benetako zenbatekoak kalkulatu direnak chargeable.</span><span class="sxs-lookup"><span data-stu-id="51d0c-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="51d0c-143">Ez chargeable utilization ikusten ari zara, baduzu hona hemen zenbait gauza dezakezu:</span><span class="sxs-lookup"><span data-stu-id="51d0c-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="51d0c-144">Baliabideak gaitasunerako lanorduak ditu definituta.</span><span class="sxs-lookup"><span data-stu-id="51d0c-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="51d0c-145">Baliabidea ditu edozer bat zehaztutako banaka utilization helburuko edo da funtzio lehenetsia esleitu bertan.</span><span class="sxs-lookup"><span data-stu-id="51d0c-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="51d0c-146">Funtzioa baliozkorik definituta horretarako utilization helburuko ditu.</span><span class="sxs-lookup"><span data-stu-id="51d0c-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="51d0c-147">Benetako zenbatekoak Kalkulatu fakturazio mota **Kargagarria** izan bat utilization kalkulatzeko expecting dira aldi baterako.</span><span class="sxs-lookup"><span data-stu-id="51d0c-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="51d0c-148">Egiaztatu ikusten ari zarela benetakoak baino beste benetako zenbatekoak kalkulatu fakturazio duen erregistro mota:</span><span class="sxs-lookup"><span data-stu-id="51d0c-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="51d0c-149">Erabilitako benetakoa funtzioa fakturazio-zerbait beste chargeable baino mota lehenetsia da.</span><span class="sxs-lookup"><span data-stu-id="51d0c-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="51d0c-150">Funtzioa proiektua kontratu-lineak proiektuan backing konfiguratu da. ez-chargeable.</span><span class="sxs-lookup"><span data-stu-id="51d0c-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="51d0c-151">Proiektuak ez du erlazionatutako kontratuaren lerrorik.</span><span class="sxs-lookup"><span data-stu-id="51d0c-151">The project does not have an associated contract line.</span></span>

