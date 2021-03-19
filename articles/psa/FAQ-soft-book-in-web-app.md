---
title: Nola egin dezaket "erreserba leuna" baliabideetan 2.x aplikazioaren bertsioan?
description: Artikulu honetan azaltzen nola soft liburua proiektua taldekideak Project Service batekin.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
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
ms.openlocfilehash: 18a1176c131e233f62f74dc0dd8a6aa3ee561da5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286008"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="1bda2-103">Nola egin dezaket "soft liburua" baliabideak aplikazioko web aplikazioa (Project Service aplikazioa v2.x)?</span><span class="sxs-lookup"><span data-stu-id="1bda2-103">How do I "soft book" resources in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="1bda2-104">Antolatu tentatively edo "soft liburua" baliabide taldeak proiektua erakusteko inprimatu nahi baliabidea proiektua bat esleitu.</span><span class="sxs-lookup"><span data-stu-id="1bda2-104">You can tentatively schedule or "soft book" a resource onto a project team to show you plan to assign the resource to a project.</span></span> <span data-ttu-id="1bda2-105">Soft bookings ez darabil baliabide baten ahalmena erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="1bda2-105">Soft bookings don’t consume a resource’s available capacity.</span></span> <span data-ttu-id="1bda2-106">Soft erreserbatuta taldeko kideak ezin zaizkie objektuak esleitu proiektua zereginak.</span><span class="sxs-lookup"><span data-stu-id="1bda2-106">Soft-booked team members can’t be assigned to project tasks.</span></span> <span data-ttu-id="1bda2-107">Egoera Disko Erreserbatuta eta Mota Committed Commit baliabideak soilik zereginak (assuming nahikoa disko erreserbatu ordu esleipena ahalegina estaltzen duten) bati eslei dakizkioke.</span><span class="sxs-lookup"><span data-stu-id="1bda2-107">Only resources with the Status Hard Booked and Commit Type Committed can be assigned to tasks (assuming they have enough hard booking hours to cover the assignment effort).</span></span>

<span data-ttu-id="1bda2-108">Soft erreserbatuta proiektua taldekideak erakutsi Taldeko Kide saretan lanorduekin beren soft erreserbatuta Soft Liburua zutabean agertzen dena.</span><span class="sxs-lookup"><span data-stu-id="1bda2-108">Soft-booked project team members show up in the Team Member grid with their soft-booked hours shown in the Soft Book column.</span></span> <span data-ttu-id="1bda2-109">Horiek ere adieraztea antolaketa board atalean.</span><span class="sxs-lookup"><span data-stu-id="1bda2-109">They also show up on the schedule board.</span></span> <span data-ttu-id="1bda2-110">Berriro, ez dute ahalmena consumption edozein adierazteko soft erreserbatu baliabide baten ahalmena darabil ez du.</span><span class="sxs-lookup"><span data-stu-id="1bda2-110">Again, they don’t indicate any consumption of capacity as soft-booking doesn’t consume capacity of a resource.</span></span>

<span data-ttu-id="1bda2-111">Hiru era daude soft liburua Project Service bertsio proiektua inprimatu taldearen kide 2.x.</span><span class="sxs-lookup"><span data-stu-id="1bda2-111">There are three ways to soft-book a team member onto a project with Project Service version 2.x.</span></span> <span data-ttu-id="1bda2-112">Soft liburua dezakezu antolaketa board, batekin baliatu Mantentzen Bookings edo lehenespenez sortu baliabide orokorra.</span><span class="sxs-lookup"><span data-stu-id="1bda2-112">You can soft-book with the schedule board, use the Maintain Bookings feature, or by creating a generic resource.</span></span> <span data-ttu-id="1bda2-113">Metodo horiek azpiko deskribatzen dira.</span><span class="sxs-lookup"><span data-stu-id="1bda2-113">These methods are described below.</span></span>

## <a name="soft-book-with-the-schedule-board"></a><span data-ttu-id="1bda2-114">Soft-honekin antolaketa board liburua</span><span class="sxs-lookup"><span data-stu-id="1bda2-114">Soft-book with the schedule board</span></span>

<span data-ttu-id="1bda2-115">Soft-liburu antolaketa board honekin jarraitu prozedura honetan:</span><span class="sxs-lookup"><span data-stu-id="1bda2-115">To soft-book with the schedule board, follow this procedure:</span></span> 
1. <span data-ttu-id="1bda2-116">Ireki antolaketa-panela.</span><span class="sxs-lookup"><span data-stu-id="1bda2-116">Open the schedule board.</span></span>
2. <span data-ttu-id="1bda2-117">Hautatu Proiektua fitxa Erreserba-eskakizunak panelaren antolaketa-panelaren behealdean.</span><span class="sxs-lookup"><span data-stu-id="1bda2-117">Select the Project tab on the bottom Booking Requirements panel of the schedule board.</span></span>
3. <span data-ttu-id="1bda2-118">Aurkitu nahi duzun soft liburua baliabide atalean proiektua.</span><span class="sxs-lookup"><span data-stu-id="1bda2-118">Find the project you wish to soft-book a resource on.</span></span> <span data-ttu-id="1bda2-119">Hainbat projects baduzu, sakatu Proiektua zutabe-goiburuan eta ondoren erabili iragazkia proiektua zure bilatzeko.</span><span class="sxs-lookup"><span data-stu-id="1bda2-119">If you have many projects, click on the Project column header and then use the filter to find your project.</span></span>
4. <span data-ttu-id="1bda2-120">Proiektuan, sakatu ondoren, arrastatu eta ezabatu baliabideen ordua sareta atalean.</span><span class="sxs-lookup"><span data-stu-id="1bda2-120">Click on the project, then drag and drop it on the resource’s time grid.</span></span>
5. <span data-ttu-id="1bda2-121">Bertan irekitzen du Baliabide Booking Sortu eskuineko panela.</span><span class="sxs-lookup"><span data-stu-id="1bda2-121">This opens the Create Resource Booking panel on the right.</span></span> <span data-ttu-id="1bda2-122">Doitzeko hasiera- eta amaiera-data, hautatu Booking Egoera Soft gisa eta ezarri ordutan.</span><span class="sxs-lookup"><span data-stu-id="1bda2-122">Adjust the start and end date, select the Booking Status as Soft and set the hours.</span></span> 
6. <span data-ttu-id="1bda2-123">Sakatu Liburuan.</span><span class="sxs-lookup"><span data-stu-id="1bda2-123">Click Book.</span></span>
7. <span data-ttu-id="1bda2-124">Berriro, proiektuan lanean baliabidea orain erakutsiko Soft Liburua zutabean soft booked lanorduekin taldearen kide gisa.</span><span class="sxs-lookup"><span data-stu-id="1bda2-124">Back on the project, the resource will now show as a team member with the soft booked hours in the Soft Book column.</span></span>

<span data-ttu-id="1bda2-125">Kontuan izan ezin diozu ahal izateko, lan-diren kanpaina-xehatzea egitura (WBS) zereginak baliabide disko izan behar bezala esleitu nahi dizkiozun taldea atalean erreserbatuta.</span><span class="sxs-lookup"><span data-stu-id="1bda2-125">Note that you can’t assign them to tasks on the work breakdown structure (WBS) as resources must be hard booked on the team to be assigned.</span></span>

## <a name="soft-book-using-the-maintain-bookings-feature"></a><span data-ttu-id="1bda2-126">Soft-liburua Mantentzen Bookings eginbidea erabiliz</span><span class="sxs-lookup"><span data-stu-id="1bda2-126">Soft-book using the Maintain Bookings feature</span></span>

<span data-ttu-id="1bda2-127">Erreserba leuna Mantendu erreserbarekin prozedura honi jarraitzen dio:</span><span class="sxs-lookup"><span data-stu-id="1bda2-127">To soft-book with Maintain Bookings follow this procedure:</span></span>
1. <span data-ttu-id="1bda2-128">Taldearen kide saretan, Sakatu Berria.</span><span class="sxs-lookup"><span data-stu-id="1bda2-128">From the team member grid, Click New.</span></span>
2. <span data-ttu-id="1bda2-129">Hautatu batetik /, bookable baliabide-funtzioak.</span><span class="sxs-lookup"><span data-stu-id="1bda2-129">Select the bookable resource, role, from/to.</span></span>
3. <span data-ttu-id="1bda2-130">Hautatu esleipen bat metodoa bat Ere ez:</span><span class="sxs-lookup"><span data-stu-id="1bda2-130">Select an allocation method other than None:</span></span>
- <span data-ttu-id="1bda2-131">Ahalmen osoa</span><span class="sxs-lookup"><span data-stu-id="1bda2-131">Full Capacity</span></span>
- <span data-ttu-id="1bda2-132">Ehuneko ahalmena</span><span class="sxs-lookup"><span data-stu-id="1bda2-132">Percentage Capacity</span></span>
- <span data-ttu-id="1bda2-133">Orduka, banatu modu uniformean</span><span class="sxs-lookup"><span data-stu-id="1bda2-133">By Hours Distribute Evenly</span></span>
- <span data-ttu-id="1bda2-134">Orduka, ordainketa goiztiarra</span><span class="sxs-lookup"><span data-stu-id="1bda2-134">By Hours Front Load</span></span>
4. <span data-ttu-id="1bda2-135">Sakatu Gorde.</span><span class="sxs-lookup"><span data-stu-id="1bda2-135">Click Save.</span></span> <span data-ttu-id="1bda2-136">Ikusiko duzu, baliabide taldeak sareta eta orduak haien Disko gisa adierazita.</span><span class="sxs-lookup"><span data-stu-id="1bda2-136">You’ll see the resource on the team grid and their hours indicated as Hard.</span></span>
5. <span data-ttu-id="1bda2-137">Mantendu baliabideen bookings Mantentzen Bookings sakatuz.</span><span class="sxs-lookup"><span data-stu-id="1bda2-137">Maintain the resource’s bookings by clicking Maintain Bookings.</span></span>
6. <span data-ttu-id="1bda2-138">Antolaketa board irekitzen duenean, zabaldu baliabide bookings beren erakusteko.</span><span class="sxs-lookup"><span data-stu-id="1bda2-138">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="1bda2-139">Ikusiko duzu, erreserbatu Disko gisa adierazita.</span><span class="sxs-lookup"><span data-stu-id="1bda2-139">You will see the booking indicated as Hard.</span></span>
7. <span data-ttu-id="1bda2-140">Aldatu Egoera atalean erreserbatu, egin klik eskuineko botoiarekin, hautatu Liburua Soft eta Soft ondoren.</span><span class="sxs-lookup"><span data-stu-id="1bda2-140">Right-click the booking, under Change Status, select Soft Book and then Soft.</span></span> <span data-ttu-id="1bda2-141">Erreserba-egoera Leuna da.</span><span class="sxs-lookup"><span data-stu-id="1bda2-141">The booking status is now Soft.</span></span>
8. <span data-ttu-id="1bda2-142">Itxi ostean antolaketa board, ikusiko duzu duzun baliabide-orduak aldatu Disko batetik Soft taldearen kide saretan.</span><span class="sxs-lookup"><span data-stu-id="1bda2-142">After closing the schedule board, you’ll see that the hours for the resource have changed from Hard to Soft on the team member grid.</span></span>
<span data-ttu-id="1bda2-143">Duzun disko baliabide taldearen inprimatu erreserbatutako eta, ondoren, esleitu ahal izateko, WBS, erabiltzean zereginak mantentzen bookings aldatu Disko egoera Soft oharra, bertan esleipenetan, ataletik ezabatuko baliabidearen, zereginak erreserbatuta baliabideak disko soilik eslei t gisa galdetuko.</span><span class="sxs-lookup"><span data-stu-id="1bda2-143">Note that if you hard book a resource onto the team and then assign them tasks in the WBS, when you use maintain bookings to change the status of Hard to Soft, it will remove the assignments from the tasks for that resource, as only hard booked resources can be assigned to tasks.</span></span>

## <a name="soft-book-by-creating-a-generic-resource"></a><span data-ttu-id="1bda2-144">Soft-orokorra baliabide sortuz liburua</span><span class="sxs-lookup"><span data-stu-id="1bda2-144">Soft-book by creating a generic resource</span></span>

<span data-ttu-id="1bda2-145">Orokorra baliabide taldearen kide sortzeko, antolaketa board edo Baliabide-Eskaera osatu eta mota aldatuz gero, erreserbatu zehar soft erreserbatu bat sor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="1bda2-145">You can create a soft-booking by generating a generic resource team member, fulfilling with schedule board or Resource Request and changing the type during the booking.</span></span>
<span data-ttu-id="1bda2-146">Hori egiteko, erabili prozedura hau:</span><span class="sxs-lookup"><span data-stu-id="1bda2-146">To do this, use the following procedure:</span></span>

1. <span data-ttu-id="1bda2-147">Proiektuan WBS, lanean esleitu funtzioak zereginak orokorra taldekideak-sortu nahi duzun.</span><span class="sxs-lookup"><span data-stu-id="1bda2-147">On the project WBS, assign roles to the tasks you wish to generate generic team members for.</span></span>
2. <span data-ttu-id="1bda2-148">Sakatu Sortu proiektu-taldea.</span><span class="sxs-lookup"><span data-stu-id="1bda2-148">Click Generate Project Team.</span></span>
3. <span data-ttu-id="1bda2-149">Proiektua taldearen kide saretan, hautatu baliabidea orokorra eta sakatu Liburua.</span><span class="sxs-lookup"><span data-stu-id="1bda2-149">On the project team member grid, select the generic resource and click Book.</span></span>
4. <span data-ttu-id="1bda2-150">Antolaketa-board, hautatu nahi duzun erreserbatutako baliabidea.</span><span class="sxs-lookup"><span data-stu-id="1bda2-150">On the schedule board, select the resource that you wish to book.</span></span>
5. <span data-ttu-id="1bda2-151">Sortu Baliabideen Booking antolaketa board panelean, atalean aldatu Booking Egoera Soft.</span><span class="sxs-lookup"><span data-stu-id="1bda2-151">On the schedule board’s Create Resource Booking panel, change the Booking Status to Soft.</span></span>
6. <span data-ttu-id="1bda2-152">Sakatu Liburua edo Liburua eta Irten.</span><span class="sxs-lookup"><span data-stu-id="1bda2-152">Click Book or Book and Exit.</span></span>

<span data-ttu-id="1bda2-153">Itxi ostean antolaketa board, ikusiko duzu, hautatutako baliabideen lanorduekin Soft erreserbatuta taldera gehitu, lehendabizi esleitutako ordu.</span><span class="sxs-lookup"><span data-stu-id="1bda2-153">After closing the schedule board, you’ll see the selected resource added to the team with Soft booked hours as well as assigned hours.</span></span> <span data-ttu-id="1bda2-154">Ere ikusiko duzu den baliabide orokorra egoerarik taldearen atalean soft erreserbatuta taldearen kide zereginak esleituta dauden adierazle gisa.</span><span class="sxs-lookup"><span data-stu-id="1bda2-154">You’ll also see that the generic resource remains on the team as an indicator that the tasks are assigned to a soft-booked team member.</span></span>

<span data-ttu-id="1bda2-155">Erreserbatuta disko taldearen kide soft erreserbatuta taldearen kide baliabide aldatzeko zereginak esleitu ahal izateko prest zaudenean, ondokoa egin:</span><span class="sxs-lookup"><span data-stu-id="1bda2-155">When you’re ready to change a soft-booked team member resource to a hard-booked team member so that you can assign them to tasks, do the following:</span></span>

1. <span data-ttu-id="1bda2-156">Baliabidearen hautatu eta sakatu Bookings Mantentzeko.</span><span class="sxs-lookup"><span data-stu-id="1bda2-156">Select that resource and click Maintain Bookings.</span></span>
2. <span data-ttu-id="1bda2-157">Antolaketa board irekitzen duenean, zabaldu baliabide bookings beren erakusteko.</span><span class="sxs-lookup"><span data-stu-id="1bda2-157">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="1bda2-158">Ikusiko duzu, erreserbatu Soft gisa ezarrita.</span><span class="sxs-lookup"><span data-stu-id="1bda2-158">You’ll see the booking marked as Soft.</span></span>
3. <span data-ttu-id="1bda2-159">Aldatu Egoera atalean erreserbatu, egin klik eskuineko botoiarekin, hautatu Liburua Gogorra eta Gogorra ondoren.</span><span class="sxs-lookup"><span data-stu-id="1bda2-159">Right-click the booking, under Change Status, select Hard Book and then Hard.</span></span> <span data-ttu-id="1bda2-160">Erreserba-egoera Gogorra da.</span><span class="sxs-lookup"><span data-stu-id="1bda2-160">The booking status is now Hard.</span></span>
4. <span data-ttu-id="1bda2-161">Itxi ostean antolaketa board, ikusiko duzu duzun baliabide-orduak aldatu Disko batetik Gogorra taldearen kide saretan.</span><span class="sxs-lookup"><span data-stu-id="1bda2-161">After closing the schedule board, you’ll see that the hours for the resource have changed from Soft to Hard on the team member grid.</span></span> <span data-ttu-id="1bda2-162">Baliteke orain esleitzen baliabidea zereginak (emandako erreserbatuta disko ordu eta esleipena zereginaren ahalegina ordu arteko lerrokatzea da).</span><span class="sxs-lookup"><span data-stu-id="1bda2-162">You may now assign the resource to tasks (provided there is alignment between the hard-booked hours and the effort hours of the task for assignment).</span></span> <span data-ttu-id="1bda2-163">Oharra duzun duzu ondoren elementu #3. urratsak, baliabide orokorra fulfilment urratsak disko, soft erreserbatuta bookable baliabidea egoera aldatzen duzunean, orokorra taldeko kide da kendu taldetik.</span><span class="sxs-lookup"><span data-stu-id="1bda2-163">Note that if you followed the generic resource fulfilment steps in item #3 above, when you change the status of the soft-booked bookable resource to hard, the generic team member is removed from the team.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]