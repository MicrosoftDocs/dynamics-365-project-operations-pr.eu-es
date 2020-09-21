---
title: Erreserbatu baliabide erreserbagarriak proiektuko talde bati eta esleitu zereginak
description: Gai honek proiektu taldeetara izena duten baliabideak erreserbatzeko eta hauek zereginetara esleitzeko informazioa eskaintzen du .
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 11/28/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: e947986a-e83a-42f4-813e-c82bdfbec33c
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 079ba299f912c75f9ed739d4b6aa3c63189d11d0
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748817"
---
# <a name="book-named-bookable-resources-to-a-project-team-and-assign-tasks"></a><span data-ttu-id="77c93-103">Erreserbatu baliabide erreserbagarriak proiektuko talde bati eta esleitu zereginak</span><span class="sxs-lookup"><span data-stu-id="77c93-103">Book named bookable resources to a project team and assign tasks</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="77c93-104">Proiektuko taldeari izendatutako baliabide bat gehi diezaiokezu zuzenean taldean erreserbatuz.</span><span class="sxs-lookup"><span data-stu-id="77c93-104">You can  add a named resource to your project team by booking them directly onto the team.</span></span> <span data-ttu-id="77c93-105">Hori egiteko, bete pauso hauek.</span><span class="sxs-lookup"><span data-stu-id="77c93-105">To do this, complete the following steps.</span></span>

1. <span data-ttu-id="77c93-106">Project Service Automation-en, joan **Proiektuak** atalera eta ireki erreserba egiten ari zaren proiektua.</span><span class="sxs-lookup"><span data-stu-id="77c93-106">In  Project Service Automation, go to **Projects**, and select the open the project that you are booking for.</span></span>
2. <span data-ttu-id="77c93-107">**Proiektua** orrialdean **Taldea** fitxan, egin klik **Berria** aukeran.</span><span class="sxs-lookup"><span data-stu-id="77c93-107">On the **Project** page, on the **Team** tab, click **New**.</span></span> 

![Taldekide bat taldeko fitxatik gehitzea](media/RM-how-to-1.png)

3. <span data-ttu-id="77c93-109">**Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroan, hautatu erreserbatzeko baliabidea.</span><span class="sxs-lookup"><span data-stu-id="77c93-109">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="77c93-110">**Funtzioa** eremua baliabidearen lehenetsitako funtzioarekin beteko da esleituta badago.</span><span class="sxs-lookup"><span data-stu-id="77c93-110">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="77c93-111">Funtzioa alda dezakezu behar izanez gero.</span><span class="sxs-lookup"><span data-stu-id="77c93-111">You can change the role if needed.</span></span> 
4. <span data-ttu-id="77c93-112">Aukeratu baliabidea beharko den hasiera eta amaiera datak eta hautatu baliabidearen ahalmena esleitzeko metodoa.</span><span class="sxs-lookup"><span data-stu-id="77c93-112">Select the from and to dates that the resource will be needed and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="77c93-113">Taldekidea proiektuaren onartzailea izan dadin nahi baduzu, hautatu **Bai** eremua **Proiektuaren onartzailea** atalean.</span><span class="sxs-lookup"><span data-stu-id="77c93-113">If you want the team member to be a project approver, select **Yes** in the **Project Approver** field.</span></span> <span data-ttu-id="77c93-114">Horrek esan nahi du taldekideak proiektu honetarako gastuak eta sarrerak onartzea onar dezakeela.</span><span class="sxs-lookup"><span data-stu-id="77c93-114">This will mean that the team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="77c93-115">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="77c93-115">Click **Save**.</span></span>

![Taldekide bat gehitu sorrera bizkorra inprimakian](media/RM-how-to-2.png)


<span data-ttu-id="77c93-117">Erreserbatutako baliabidea proiektuan zereginetara eslei dezakezu.</span><span class="sxs-lookup"><span data-stu-id="77c93-117">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="77c93-118">**Proiektua** orrialdean, egin klik **Antolaketa** fitxan baliabide berriari zereginak esleitzeko.</span><span class="sxs-lookup"><span data-stu-id="77c93-118">On the **Project** page, click the **Schedule** tab to assign tasks to the new resource.</span></span> <span data-ttu-id="77c93-119">Zereginen sareko **Baliabideak** eremutik abian jarri den baliabide hautatzaileak hautatu ditzakezu taldekideak erakutsiko ditu.</span><span class="sxs-lookup"><span data-stu-id="77c93-119">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>

![Taldekide bat esleitzea egutegiko fitxako zeregin bati](media/RM-how-to-3.png)

<span data-ttu-id="77c93-121">Project Service Automation-en (PSA) 3. bertsioan, baliabideen erreserbak eta zereginen esleipenak ez daude oso lotuta.</span><span class="sxs-lookup"><span data-stu-id="77c93-121">In version 3 for Project Service Automation (PSA), resource bookings and task assignments are not tightly coupled.</span></span> <span data-ttu-id="77c93-122">Horrek esan nahi du baliabideen hautagailua antolaketan erabiltzen duzunean, taldekideei zereginak eslei diezazkiekeela proiektuan egindako erreserbek estaltzen dutena baino ordu gehiago.</span><span class="sxs-lookup"><span data-stu-id="77c93-122">This means that when you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>
<span data-ttu-id="77c93-123">Taldekideen erreserbak eta zereginen arteko desberdintasunak ikus ditzakezu **Taldea** fitxan edo **Baliabideen berdinkatzea** fitxa. Baliabideen erreserba eta esleipenen arteko desberdintasunak bateratu ditzakezu maila zehatzago batean.</span><span class="sxs-lookup"><span data-stu-id="77c93-123">You can see the differences between team member bookings and assignments on the **Team** tab or on the **Resource Reconciliation** tab. You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

![Baliabideen berdinkatzea fitxa](media/RM-how-to-4.png)

<span data-ttu-id="77c93-125">Baliabide hautagailua ere erabil dezakezu **Antolaketa** fitxan, proiektuko parte ez diren baliabideak bilatu eta hautatzeko.</span><span class="sxs-lookup"><span data-stu-id="77c93-125">You can also use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="77c93-126">Baliabide-hautatzailean agertzen dira **Bestelako baliabideak** moduan.</span><span class="sxs-lookup"><span data-stu-id="77c93-126">These are shown in the resource picker as **Other Resources**.</span></span>

![Taldeko kide ez den baliabidea zeregin bati esleitzea](media/RM-how-to-5.png)

<span data-ttu-id="77c93-128">Hau egiten duzunean, baliabidea proiektuko taldeari gehitu eta zereginari esleitzen zaio, baina ez da erreserbarik sortzen.</span><span class="sxs-lookup"><span data-stu-id="77c93-128">When you do this, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

![Zereginak bai baina erreserbarik ez duen taldekidea](media/RM-how-to-6.png)

<span data-ttu-id="77c93-130">**Berdinkatzea** fitxaren luzatzeko erreserba gaitasuna erabil dezakezu edo **Antolaketa-panela** aukera baliabidearen gaitasuna proiektua erreserbatzeko.</span><span class="sxs-lookup"><span data-stu-id="77c93-130">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

![Taldekide bati erreserbak luzatzea baliabide berdinkatzea fitxan](media/RM-how-to-7.png)

<span data-ttu-id="77c93-132">Taldekide bat zure proiektuan erreserbatu ondoren, erreserbak mantendu edo antolaketa-panela erabil dezakezu erreserbak kudeatzeko.</span><span class="sxs-lookup"><span data-stu-id="77c93-132">After a team member is booked on your project, you can use maintain bookings or use the Schedule Board directly to manage their bookings.</span></span>
