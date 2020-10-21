---
title: Kudeatu ordu-zonak
description: Proiektu bat sortzen denean, bere ordu-zona aplikatutako lan-ordu txantiloian definitutako ordu-eremuan oinarritzen da.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27f58f0dacc3404119a719547ad374629c740740
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961810"
---
# <a name="manage-time-zones"></a><span data-ttu-id="3b559-103">Kudeatu ordu-zonak</span><span class="sxs-lookup"><span data-stu-id="3b559-103">Manage time zones</span></span>

<span data-ttu-id="3b559-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="3b559-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="3b559-105">Proiektuak</span><span class="sxs-lookup"><span data-stu-id="3b559-105">Projects</span></span>

<span data-ttu-id="3b559-106">Proiektu bat sortzen denean, bere ordu-zona aplikatutako lan-ordu txantiloian definitutako ordu-eremuan oinarritzen da.</span><span class="sxs-lookup"><span data-stu-id="3b559-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="3b559-107">**Proiektua** izan ere, datak beti daude fitxa bakoitzean saioa hasita duen erabiltzailearen ordu-zonaren aldean, **Zeregina** fitxa. Lanaren banakako egitura ikusten duzunean, datak proiektuaren ordu-eremuan erakutsiko dira beti.</span><span class="sxs-lookup"><span data-stu-id="3b559-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="3b559-108">Zereginak</span><span class="sxs-lookup"><span data-stu-id="3b559-108">Tasks</span></span>

<span data-ttu-id="3b559-109">Zeregin bat sortzen denean, hasiera ordua, amaiera ordua eta eguneko orduak proiektuaren lan orduek kontrolatzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="3b559-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="3b559-110">Adibidez, zeregin bat ordu-zona -8 PST duen eta laneko ordutegia duen proiektu batekin sortzen bada: 9:00etatik 17:00etara astelehenetik ostiralera, esleipenik gabe sortutako edozein zereginek hasiera ordua errespetatuko dute eta proiektuaren egutegiaren amaiera ordua.</span><span class="sxs-lookup"><span data-stu-id="3b559-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="3b559-111">Kudeatu baliabideak ordu-zonekin</span><span class="sxs-lookup"><span data-stu-id="3b559-111">Manage resources with time zones</span></span>

<span data-ttu-id="3b559-112">Erabiltzean emaitza zehatzak eta aurresatekoak lortzeko **Luzatu erreserba**, funtsezko bi baldintza bete behar dira:</span><span class="sxs-lookup"><span data-stu-id="3b559-112">For accurate and predictable results when using **Extend Booking**, there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="3b559-113">Erabiltzaileak bere gailuaren ordu-eremua sisteman zehaztutako ordu-zonarekin bat etor dadin konfiguratu behar du **Pertsonalizazio-ezarpenak**.</span><span class="sxs-lookup"><span data-stu-id="3b559-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![Ordu-eremuaren ezarpenak Windows 10-en](media/reconcile-assignments-03.png)

  ![Ordutegi-eremuaren ezarpenak pertsonalizazio-ezarpenetan](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="3b559-116">Baliabide erreserbagarriak eskatutako luzapena definitzeko erabilitako sarrerak gainjartzen den lanaldiko minutu bat izan behar du gutxienez.</span><span class="sxs-lookup"><span data-stu-id="3b559-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="3b559-117">Adibidez, goizeko 9:00etatik 19:00etara bitarteko lanorduekin honako baliabide hauek.</span><span class="sxs-lookup"><span data-stu-id="3b559-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![Baliabideen sarrerak alderatzea](media/reconcile-assignments-05.png)

<span data-ttu-id="3b559-119">Taula honek hau erakusten du:</span><span class="sxs-lookup"><span data-stu-id="3b559-119">The following table shows:</span></span>

- <span data-ttu-id="3b559-120">Proiektuaren egutegi-txantiloi bat</span><span class="sxs-lookup"><span data-stu-id="3b559-120">A project calendar template</span></span>
- <span data-ttu-id="3b559-121">A baliabidea: baliabide honek egutegi bera du eta proiektuaren ordu-eremu berean dago.</span><span class="sxs-lookup"><span data-stu-id="3b559-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="3b559-122">Erreserbaren hasiera-ordua goizeko 09:00etan izango da.</span><span class="sxs-lookup"><span data-stu-id="3b559-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="3b559-123">B Baliabidea: Baliabide hau proiektuarekiko beste ordu-zona batean dago eta goizeko 7:00etan hasten da haien ordu-gunean.</span><span class="sxs-lookup"><span data-stu-id="3b559-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="3b559-124">Hala ere, erreserbak goizeko 09:00etan hasiko dira, esleipen-sarreraren hasiera-ordu goiztiarrena delako.</span><span class="sxs-lookup"><span data-stu-id="3b559-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="3b559-125">C eta D baliabideak: baliabideak ordu-zona desberdinetan daude, bata bestearekin eta proiektuarekin desberdinak, eta erreserbak dagozkien hasiera-orduak baino lehenago hasten dira.</span><span class="sxs-lookup"><span data-stu-id="3b559-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="3b559-126">Entitatea</span><span class="sxs-lookup"><span data-stu-id="3b559-126">Entity</span></span>  |<span data-ttu-id="3b559-127">Egutegia</span><span class="sxs-lookup"><span data-stu-id="3b559-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="3b559-128">Proiektuaren egutegi-txantiloia</span><span class="sxs-lookup"><span data-stu-id="3b559-128">Project calendar template</span></span>   | ![proiektuaren egutegia](media/reconcile-assignments-06.png) |
|<span data-ttu-id="3b559-130">A baliabidea</span><span class="sxs-lookup"><span data-stu-id="3b559-130">Resource A</span></span>  | ![A baliabidearen egutegia](media/reconcile-assignments-06.png) |
|<span data-ttu-id="3b559-132">B baliabidea</span><span class="sxs-lookup"><span data-stu-id="3b559-132">Resource B</span></span>  |  ![B baliabidearen egutegia](media/reconcile-assignments-07.png) |
|<span data-ttu-id="3b559-134">C baliabidea</span><span class="sxs-lookup"><span data-stu-id="3b559-134">Resource C</span></span>  |  ![C baliabidearen egutegia](media/reconcile-assignments-08.png) |
|<span data-ttu-id="3b559-136">D baliabidea</span><span class="sxs-lookup"><span data-stu-id="3b559-136">Resource D</span></span>  | ![D baliabidearen egutegia](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="3b559-138">Helbidera nabigatzen duzunean **Adiskidetzea** ikuspegia, baliabideen esleipenak eta horrekin lotutako erreserba eskasia bistaratzen dira.</span><span class="sxs-lookup"><span data-stu-id="3b559-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![Bateratze-ikuspegia hedapenaren aurretik](media/reconcile-assignments-10.png)

<span data-ttu-id="3b559-140">Baliabide bakoitzerako hedapenaren erreserbaren funtzionalitatea erabili ondoren, erreserbak baliabide bakoitzerako behar bezala hedatzen dira, baliabide bakoitzaren lan orduak gabeziaren sestrarekin gainjartzen direlako.</span><span class="sxs-lookup"><span data-stu-id="3b559-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![Bateratze-ikuspegia erreserba luzatu ostean](media/reconcile-assignments-11.png) 

<span data-ttu-id="3b559-142">Kontuan izan erreserben xehetasunak aztertuz gero, erreserbak hasteko orduaren aldeak erakusten dituela.</span><span class="sxs-lookup"><span data-stu-id="3b559-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="3b559-143">Erreserbak esleipenaren sestra hasierako ordua baino lehenago hasten dira eta baliabidearen erabilgarri dagoen ordua baino lehenago hasten dira.</span><span class="sxs-lookup"><span data-stu-id="3b559-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![Antolaketa-taulako baliabideen erreserba berriak](media/reconcile-assignments-12.png)
