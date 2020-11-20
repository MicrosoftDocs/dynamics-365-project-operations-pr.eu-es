---
title: Sortu proiektu-erreserba bat antolaketa-paneletik
description: Gai honek proiektuaren erreserba egitasmoaren taulan sortzen den informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: ccbfedec82b2d9035b51cf1b283ae5c441f1cbcc
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122283"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="d531d-103">Sortu proiektu-erreserba bat antolaketa-paneletik</span><span class="sxs-lookup"><span data-stu-id="d531d-103">Create a project booking from the Schedule board</span></span>

<span data-ttu-id="d531d-104">Baliabide bat erreseba dezakezu zuzenean **Taldea** fitxan proiektua taldearen proiektuan edo baliabide eskakizun batetik orokorra taldearen kide zeregin bat sortzen eta, ondoren, osatu proiektua taldearen kide honekin sortutako eskakizun hauen artean.</span><span class="sxs-lookup"><span data-stu-id="d531d-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="d531d-105">Baliabidearen antolaketa-panelan zuzenean proiektua inprimatu ere erreserbatutako dezakezu.</span><span class="sxs-lookup"><span data-stu-id="d531d-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="d531d-106">Hiru era daude hau ebazteko:</span><span class="sxs-lookup"><span data-stu-id="d531d-106">There are three ways to do this:</span></span>

- <span data-ttu-id="d531d-107">**Sortutako baliabide eskakizuna erreserbatu:** baliabideen eskakizuna sor dezakezu baliabide generiko bat sortu eta proiektu baten barruan zereginak esleitu ondoren.</span><span class="sxs-lookup"><span data-stu-id="d531d-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="d531d-108">**Liburua bete beharrekoa:** eskakizun nagusienak Ordutegiaren taulan agertzen dira **Proiektua** fitxa.</span><span class="sxs-lookup"><span data-stu-id="d531d-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="d531d-109">**Erreserbatu baliabide eskakizun berri batetik:** baliabide eskakizuna hutsetik sor dezakezu eta proiektu batekin lotu.</span><span class="sxs-lookup"><span data-stu-id="d531d-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="d531d-110">Antolaketa-taulan, baliabide-eskakizunak **Ireki eskakizunak** fitxan agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="d531d-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="d531d-111">Erreserbatu sortutako baliabide eskakizun batetik</span><span class="sxs-lookup"><span data-stu-id="d531d-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="d531d-112">Baliabide orokorra sortzeko eta zeregin bat edo gehiago proiektua barruan esleitu.</span><span class="sxs-lookup"><span data-stu-id="d531d-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="d531d-113">Gero, sortu baliabide-eskakizun bat taldeko kide orokor batetik.</span><span class="sxs-lookup"><span data-stu-id="d531d-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="d531d-114">Tresna-barran antolaketa-panelan, baliabide hau erakutsiko tresna-barran, **Ireki Eskakizunak** fitxa. Baliteke erabili behar duzu zutabe iragazkiak saretan hainbat eskakizunak irekita baldin baduzu.</span><span class="sxs-lookup"><span data-stu-id="d531d-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="d531d-115">![Ireki Eskakizunak fitxa Antolaketa panelean](media/FAQ-Project-Booking-Schedule-Board-1.png "Taula bookings eta esleipenetan Eginbideei")</span><span class="sxs-lookup"><span data-stu-id="d531d-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="d531d-116">Hautatu eskakizuna.</span><span class="sxs-lookup"><span data-stu-id="d531d-116">Select the requirement.</span></span> <span data-ttu-id="d531d-117">**Bilaketa erabilgarritasuna** fitxa agertuko da hautatutako errenkada goialdean.</span><span class="sxs-lookup"><span data-stu-id="d531d-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="d531d-118">Fitxan hautatzean, hautatu antolaketa board Antolaketa-panela modua launches eta iragazkiak baliabide eskakizun betetzen dituzten erabilgarri dauden baliabideak.</span><span class="sxs-lookup"><span data-stu-id="d531d-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="d531d-119">Gero, bertatik baliabide erreserbatutako dezakezu.</span><span class="sxs-lookup"><span data-stu-id="d531d-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="d531d-120">Arrastatu ataleko eta dezakezu antolaketa board beheko batetik errenkada hautatutako goiko gelaxkan baliabide bat ezabatu.</span><span class="sxs-lookup"><span data-stu-id="d531d-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="d531d-121">Duenean jareginez da, bertan irekitzen du **Baliabide Booking Sortu** eskuineko panela.</span><span class="sxs-lookup"><span data-stu-id="d531d-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="d531d-122">Hautatu **Liburua** books baliabide talde proiektua inprimatu.</span><span class="sxs-lookup"><span data-stu-id="d531d-122">Selecting **Book** books the resource onto the project team.</span></span>

![Sortu baliabide-erreserba panela](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="d531d-124">Eskakizun Nagusia liburua</span><span class="sxs-lookup"><span data-stu-id="d531d-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="d531d-125">Xede proiektuaren Project Service automatikoki sortu Eskakizun Nagusia izeneko baliabide eskakizun sortzen da.</span><span class="sxs-lookup"><span data-stu-id="d531d-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="d531d-126">Bizkor erreserbatutako baliabide bat antolaketa board gabe eskakizun bat sortzeko erabiltzen den eskakizun hutsik bat da.</span><span class="sxs-lookup"><span data-stu-id="d531d-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="d531d-127">Eskakizun-hutsik dagoelako datak lehendabizi, guztirako baldintza kopuruak metodoa eta orduak ahal bada zehaztu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="d531d-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="d531d-128">Lehen eskakizunarekin baliabide bat erreserbatzeko, antolaketa-taulan, hautatu **Proiektua** fitxa. Baliteke zutabeko irizpidea erabiltzea **Proiektua** zutabean, hainbat proiektu badituzu.</span><span class="sxs-lookup"><span data-stu-id="d531d-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="d531d-129">![Zutabe-iragazkiak Antolaketa panelean](media/FAQ-Project-Booking-Schedule-Board-2.png "Taula bookings eta esleipenetan Eginbideei")</span><span class="sxs-lookup"><span data-stu-id="d531d-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="d531d-130">Hautatu eskakizun batek bere izena proiektua izena eta 0-iraupena da.</span><span class="sxs-lookup"><span data-stu-id="d531d-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="d531d-131">Hautatu **Bilaketa erabilgarritasuna** fitxa, errenkadan agertzen dena.</span><span class="sxs-lookup"><span data-stu-id="d531d-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="d531d-132">Hori puts antolaketa-panela Antolaketa Laguntzailearen moduan, eta erabilgarri dauden baliabideak proiektuan inprimatu booked daitezke erakusten du.</span><span class="sxs-lookup"><span data-stu-id="d531d-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="d531d-133">**Eskakizun Nagusia** 0 iraupena batekin eskakizun hutsik bat denez, behar duzu iraupena ezartzen, **Sortu Baliabide Erreserbatu** panela booking baliabide bat eta hautatu.</span><span class="sxs-lookup"><span data-stu-id="d531d-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="d531d-134">Hautatu antolaketa board behealdean **Proiektua Nagusia Eskakizun** eta arrastatu eta dezakezu, baliabide bat erreserbatutako da ezabatu.</span><span class="sxs-lookup"><span data-stu-id="d531d-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="d531d-135">**Eskakizun Nagusia** 0 iraupena batekin eskakizun hutsik bat denez, behar duzu iraupena ezartzen, **Sortu Baliabide Erreserbatu** panela booking baliabide bat eta hautatzen duzunean eta baliabidea erreserbatzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="d531d-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="d531d-136">Tresna-barran antolaketa board **Nagusia Eskakizun** bidez baliabide erreserbatutako duzunean gehitzen proiektua taldeari esleitutako edozein gabe.</span><span class="sxs-lookup"><span data-stu-id="d531d-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="d531d-137">Erreserbatu baliabide eskakizun berri batetik</span><span class="sxs-lookup"><span data-stu-id="d531d-137">Book from a new resource requirement</span></span>
<span data-ttu-id="d531d-138">Jarraitu hurrengo pausoak baliabide bat antolaketa paneletik liburu bat biguntzeko.</span><span class="sxs-lookup"><span data-stu-id="d531d-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="d531d-139">Joan **Baliabideen Eskakizunak** eta gero hautatu **Berria** baliabide eskakizun berri bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="d531d-139">Go to **Resource Requirements**, and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="d531d-140">**Proiektua** fitxan, hautatu proiektu bat eskakizuna proiektuarekin lotzeko.</span><span class="sxs-lookup"><span data-stu-id="d531d-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="d531d-141">Antolaketa-panelan, hori azkenaldian sortutako eskakizun gisa azalduko **Ireki Eskakizuna** bat egin dezakezu duen board antolaketa atalean.</span><span class="sxs-lookup"><span data-stu-id="d531d-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="d531d-142">Erreserbatu baliabidea proiektuko taldera gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="d531d-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="d531d-143">Baliabideari booked, dela orain zereginak eskuz esleitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="d531d-143">Now that the resource is booked, you must assign tasks manually.</span></span>

