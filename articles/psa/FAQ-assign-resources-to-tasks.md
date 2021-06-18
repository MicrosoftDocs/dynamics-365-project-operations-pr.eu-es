---
title: Esleitu baliabide bat zeregin bati
description: Gai honek proiektuaren baliabideak zereginei esleitzeari buruzko informazioa ematen du.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
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
ms.openlocfilehash: a348130ee5760196b2f008ea811e7a81758dd73e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993221"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="abfc1-103">Esleitu baliabide bat zeregin bati</span><span class="sxs-lookup"><span data-stu-id="abfc1-103">Assign a resource to a task</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="abfc1-104">Baliabide bat hiru modutan eslei daiteke Microsoft Dynamics 365 Project Service Automation-en.</span><span class="sxs-lookup"><span data-stu-id="abfc1-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="abfc1-105">Erreserbatu baliabidea taldearen kide gisa eta esleitu baliabidea zereginari</span><span class="sxs-lookup"><span data-stu-id="abfc1-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="abfc1-106">Proiektu-taldeari baliabide bat gehi diezaiokezu eta baliabidea zereginetan eslei dezakezu proiektuaren antolaketan.</span><span class="sxs-lookup"><span data-stu-id="abfc1-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="abfc1-107">**Taldekidea** fitxan, gehitu taldekide berria hautatuta **Berria**.</span><span class="sxs-lookup"><span data-stu-id="abfc1-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="abfc1-108">**Taldekidea sorrera bizkorra** panela irekitzen da, hautatu baliabide erreserbagarriaren izena eta funtzio bat ezarri.</span><span class="sxs-lookup"><span data-stu-id="abfc1-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="abfc1-109">Hautatu baliabide erreserbagarrirako ondorengo esleipen metodo bat:</span><span class="sxs-lookup"><span data-stu-id="abfc1-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="abfc1-110">**Gaitasun osoa** aukerarekin baliabidearen ahalmena osoa zehaztutako liburu batetik eta data.</span><span class="sxs-lookup"><span data-stu-id="abfc1-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="abfc1-111">**Ehunekoaren gaitasuna** aukerak baliabidearen ahalmenaren ehuneko batean erreserbatzen du baliabidea zehaztutako daten artean.</span><span class="sxs-lookup"><span data-stu-id="abfc1-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="abfc1-112">**Orduak berdin banatu** aukerak epe jakin batean zehaztatutako orduak erreserbatzen ditu, zehaztatutako hasiera- eta amaiera-daten artean berdin banatuz, egunen arabera.</span><span class="sxs-lookup"><span data-stu-id="abfc1-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="abfc1-113">**Aurreikusitako orduaren arabera** ordu jakin baterako erreserbatzen du baliabidea, egunean ordu jakin batzuk zehaztutako datetan.</span><span class="sxs-lookup"><span data-stu-id="abfc1-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="abfc1-114">Ez hautatu **Bat ere ez** baliabidea taldean gehitzen duelako, baina ez du sortzen edozein bookings absorb baliabidearen ahalmena.</span><span class="sxs-lookup"><span data-stu-id="abfc1-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="abfc1-115">Zeregin baten **Antolaketa** saretan, hautatu, **Baliabidea** ikonoa baliabide gelaxkan **Taldekideak** aukeran, eta, ondoren, hautatu gehitu duzun taldekidea.</span><span class="sxs-lookup"><span data-stu-id="abfc1-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members**, select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="abfc1-116">**Taldekidea** eta **Kontziliazioa** fitxetan, baliabideak erakusten ditu erreserbatuta orduak zein esleitutako orduak.</span><span class="sxs-lookup"><span data-stu-id="abfc1-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="abfc1-117">Orduak berdinak izan behar dira, baina ez da behar beharrezkoa, erreserbak eta esleipenak ez daudelako estu batera.</span><span class="sxs-lookup"><span data-stu-id="abfc1-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="abfc1-118">**Kontziliazioa** fitxak xehetasunak ematen ditu ezberdinak direnean, adibidez, baliabide bati erreserbatu dituzunak baina ordu gehiago esleitzen dizkiozunean.</span><span class="sxs-lookup"><span data-stu-id="abfc1-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="abfc1-119">Behar izanez gero, informazioa zuzendu dezakezu baliabidearen erreserba luzatzeko edo esleipena aldatzeko.</span><span class="sxs-lookup"><span data-stu-id="abfc1-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="abfc1-120">Sortu zeregin-esleipenaren bidez taldeko kide orokor bat</span><span class="sxs-lookup"><span data-stu-id="abfc1-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="abfc1-121">Zereginen esleipenen bidez taldekide generikoa sortzean, leku-marka edo baliabide generikoa sortzen duzu, izena duen baliabidearen ezaugarriak azaltzen dituena, zereginetan lan egin nahi duzun horrenak.</span><span class="sxs-lookup"><span data-stu-id="abfc1-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="abfc1-122">Zuk ondoren, sortu eskakizuna (edo eskakizunaren bidez eskaera eskaera bidali) izena duen baliabidea bilatzeko eta erreserbatzeko balio duena.</span><span class="sxs-lookup"><span data-stu-id="abfc1-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="abfc1-123">**Antolaketa** saretan zeregin batean, hautatu **Baliabidea** ikonoa baliabide gelaxkan.</span><span class="sxs-lookup"><span data-stu-id="abfc1-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="abfc1-124">Idatzi leku-marka baliabide izena gisa erabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="abfc1-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="abfc1-125">Adibidez, programaren kudeatzailea.</span><span class="sxs-lookup"><span data-stu-id="abfc1-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="abfc1-126">Hautatu **Sortu**, eta **Sorrera bizkorra proiektuaren taldekidea** eremuan, ezarri baliabide generikoaren funtzioa.</span><span class="sxs-lookup"><span data-stu-id="abfc1-126">Select **Create**, and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="abfc1-127">Jarrai dezakezu esleitzen zereginak leku-marka baliabide honi baliabidea zereginaren **Baliabide hautatzailea** eremuan hautatuz</span><span class="sxs-lookup"><span data-stu-id="abfc1-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="abfc1-128">**Taldekideak** atalean zerrendatuta daude.</span><span class="sxs-lookup"><span data-stu-id="abfc1-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="abfc1-129">Noiz egin ari bertan orokorra baliabidea esleitu hautatu orokorra baliabide- **Taldearen** fitxan eta, gero, hautatu **Sortu Eskakizun** baliabide eskakizun baliabide orokorra sortzeko.</span><span class="sxs-lookup"><span data-stu-id="abfc1-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="abfc1-130">Hautatu **Liburua** baliabide orokorra.</span><span class="sxs-lookup"><span data-stu-id="abfc1-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="abfc1-131">Bilatu eta erreserbatutako baliabide benetako antolaketa board ondoren, erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="abfc1-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="abfc1-132">Baliabide kudeatzailea arabera betetze-eskakizun hautatuta bidali dezakezu ere.</span><span class="sxs-lookup"><span data-stu-id="abfc1-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="abfc1-133">Baliabidea orokorra baliabide named beteta dagoenean, orokorra baliabide-taldetik kendu eta orokorra baliabide esleitutako zeregina orokorra baliabide baliabide eskakizun beteta baliabidea named esleitzen zaizkio.</span><span class="sxs-lookup"><span data-stu-id="abfc1-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="abfc1-134">Esleitu izena duen baliabidea baliabide erreserbagarrien zerrendatik</span><span class="sxs-lookup"><span data-stu-id="abfc1-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="abfc1-135">Bilaketa-koadroa, **Baliabide hautatzailea** eremukoa, erabil dezakezu baliabide erreserbagarri guztiak bilatu eta zeregin bat esleitzeko.</span><span class="sxs-lookup"><span data-stu-id="abfc1-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="abfc1-136">Horrela esleitutako baliabideak erreserbatu gabe taldeari gehitzen zaizkio.</span><span class="sxs-lookup"><span data-stu-id="abfc1-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="abfc1-137">Hau da taldekide bat gehitzea eta Inor metodo gisa hautatzearen berdina da.</span><span class="sxs-lookup"><span data-stu-id="abfc1-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="abfc1-138">Baliabidea **Taldea** eta **Kontziliazioa** fitxetan agertzen da, esleipen eta erreserba defizita duten baliabide gisa.</span><span class="sxs-lookup"><span data-stu-id="abfc1-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="abfc1-139">Erreserbatutako horiek erabilgarritasuna beren erabili nahi izanez gero.</span><span class="sxs-lookup"><span data-stu-id="abfc1-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="abfc1-140">**Antolaketa** saretan zeregin batean, hautatu **Baliabidea** ikonoa baliabide gelaxkan.</span><span class="sxs-lookup"><span data-stu-id="abfc1-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="abfc1-141">Hasiera-izen bat idazten.</span><span class="sxs-lookup"><span data-stu-id="abfc1-141">Start typing a name.</span></span> <span data-ttu-id="abfc1-142">Bilaketaren emaitzak **Beste baliabideak** ataleko **Baliabide hautatzailea** eremuan bistaratzen dira.</span><span class="sxs-lookup"><span data-stu-id="abfc1-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="abfc1-143">Hautatu zereginari esleitu nahi diozun balabidea.</span><span class="sxs-lookup"><span data-stu-id="abfc1-143">Select the resource that you want to assign to the task.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]