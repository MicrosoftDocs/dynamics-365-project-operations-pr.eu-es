---
title: Nola esleitzen da baliabide erreserbagarria zeregin bati web aplikazioan
description: Baliabide erreserbagarriak esleitzeko moduen ikuspegi orokorra.
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
ms.openlocfilehash: b4296837cabd4c6f7e2d2924079658e45ce8b87c
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286278"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="cede0-103">Nola eslei daiteke baliabide erreserbagarri bat zeregin bati web-aplikazioan (Project Service aplikazioa v2.x)?</span><span class="sxs-lookup"><span data-stu-id="cede0-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="cede0-104">Baliabide bat bi modutan eslei daiteke Project Service-n.</span><span class="sxs-lookup"><span data-stu-id="cede0-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="cede0-105">Baliabide taldearen kide gisa erreserbatutako eta ondoren, zeregin bat esleitu.</span><span class="sxs-lookup"><span data-stu-id="cede0-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="cede0-106">Bestela, duzu sor dezakezu funtzio-zeregin bidez orokorra taldearen kide zereginekin lan, talde bat sortu eta, ondoren, egin named baliabidearekin backing eskakizunak.</span><span class="sxs-lookup"><span data-stu-id="cede0-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="cede0-107">Kontutan izan dela nahi duzun baliabidea bookable zeregin bat esleitu, bookable baliabide taldeko kide izan behar bookings nahikoa erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="cede0-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="cede0-108">Egoera-erreserbatu Commit Mota Disko Liburua eta Committed Egoera izan behar du.</span><span class="sxs-lookup"><span data-stu-id="cede0-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="cede0-109">Baliabidearen erreserba nahikoa ez badaude, Project Service-k esleipena kendu eta errore-mezu hau bistaratzen du:</span><span class="sxs-lookup"><span data-stu-id="cede0-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="cede0-110">*Ezin da esleitu baliabidea zereginean - Baliabide hauek ez dute nahikoa ordu erreserbatuta proiektuan*</span><span class="sxs-lookup"><span data-stu-id="cede0-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="cede0-111">Erreserbatu baliabidea taldearen kide gisa eta esleitu baliabidea zereginari</span><span class="sxs-lookup"><span data-stu-id="cede0-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="cede0-112">Metodo honekin proiektua taldeari baliabide bat gehitu aurkitzea esleitu zereginak, baliabideak antolaketan proiektua.</span><span class="sxs-lookup"><span data-stu-id="cede0-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="cede0-113">Hemen da hori egiteko modua:</span><span class="sxs-lookup"><span data-stu-id="cede0-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="cede0-114">Saretan taldearen kide, gehitu taldeko kide berria hautatuta **Berria**.</span><span class="sxs-lookup"><span data-stu-id="cede0-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="cede0-115">Taldearen Kide Sortze Bizkorren pantailan, hautatu baliabide bookable izena eta funtzio bat ezarri.</span><span class="sxs-lookup"><span data-stu-id="cede0-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="cede0-116">Hautatu **Noiztik** eta **Noiz arte** datak.</span><span class="sxs-lookup"><span data-stu-id="cede0-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="cede0-117">![Taldekidea gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-1.png "Taldekidea gehitzeko pantaila-argazkia")</span><span class="sxs-lookup"><span data-stu-id="cede0-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="cede0-118">Hautatu booking baliabidea-kopuruan metodoak ondorengo aukeretako bat:</span><span class="sxs-lookup"><span data-stu-id="cede0-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="cede0-119">**Gaitasun osoa** aukerarekin baliabidearen ahalmena osoa zehaztutako liburu batetik eta data.</span><span class="sxs-lookup"><span data-stu-id="cede0-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="cede0-120">**Ehunekoaren gaitasuna** aukerak baliabidearen ahalmenaren ehuneko batean erreserbatzen du baliabidea zehaztutako daten artean.</span><span class="sxs-lookup"><span data-stu-id="cede0-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="cede0-121">**Orduak berdin banatuta** aukerak epe jakin batean ordu, zehaztutako, igaro uniformeki egunaren ordua banatzen baliabidea books batetik eta data.</span><span class="sxs-lookup"><span data-stu-id="cede0-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="cede0-122">**Aurreikusitako orduaren arabera** ordu jakin baterako erreserbatzen du baliabidea, egunean ordu jakin batzuk zehaztutako datetan.</span><span class="sxs-lookup"><span data-stu-id="cede0-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="cede0-123">Ez hautatu **Bat ere ez** baliabidea taldean gehitzen duelako, baina ez du sortzen edozein bookings absorb baliabidearen ahalmena.</span><span class="sxs-lookup"><span data-stu-id="cede0-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="cede0-124">Hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="cede0-124">Select **Save**.</span></span>

    <span data-ttu-id="cede0-125">Kontuan hartu erreserbatu-orduak azal-ahalegina ordu eta baliabide hau esleitu zeregin data-barruti nahikoa izan behar.</span><span class="sxs-lookup"><span data-stu-id="cede0-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="cede0-126">Horiek ez lerrokatzea aplikazioan, ezin diozu baliabidea zeregina.</span><span class="sxs-lookup"><span data-stu-id="cede0-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="cede0-127">Lan egin diren kanpaina-xehatzea egitura (WBS) zereginaren, sakatu baliabidea gelaxka goitibeherako.</span><span class="sxs-lookup"><span data-stu-id="cede0-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="cede0-128">Orduan:</span><span class="sxs-lookup"><span data-stu-id="cede0-128">Then:</span></span> 

    1. <span data-ttu-id="cede0-129">Hautatu **Gehitu**.</span><span class="sxs-lookup"><span data-stu-id="cede0-129">Select **Add**.</span></span>
    2. <span data-ttu-id="cede0-130">Hautatu ataleko goitibeherako **Baliabideak** eta gaineko gehitu taldeko kide hautatzeko.</span><span class="sxs-lookup"><span data-stu-id="cede0-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="cede0-131">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="cede0-131">Select **OK**.</span></span> <span data-ttu-id="cede0-132">Taldeko kide orain den esleitutako zeregina.</span><span class="sxs-lookup"><span data-stu-id="cede0-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="cede0-133">![WBSekin baliabideak gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-2.png "WBSekin baliabideak gehitzeko pantaila-argazkia")</span><span class="sxs-lookup"><span data-stu-id="cede0-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="cede0-134">Taldearen kide saretan, ikusiko duzu baliabideen agregatuen esleitutako Esleitutako Ordu atalean ordu.</span><span class="sxs-lookup"><span data-stu-id="cede0-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="cede0-135">Izango da, baliabide-booked ordu berdina edo txikiagoa.</span><span class="sxs-lookup"><span data-stu-id="cede0-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="cede0-136">![Baliabide bati esleitutako orduen pantaila-argazkia](media/FAQ-Resources-to-Tasks2-3.png "Baliabide bati esleitutako orduen pantaila-argazkia")</span><span class="sxs-lookup"><span data-stu-id="cede0-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="cede0-137">Baliabidea esleitzen saiatzen ari zara zeregina abiarazten baliabideak bookings amaiera-data ondoren, baliabidea ez agertuko-barrako goitibeheran.</span><span class="sxs-lookup"><span data-stu-id="cede0-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="cede0-138">Kontutan izan ditzakezu esleitzea baliabide beren booked ordu baino gehiago ordu baliabidea esleitu gabeko ahalmena gelditzen diren zenbait badu.</span><span class="sxs-lookup"><span data-stu-id="cede0-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="cede0-139">Kasu honetan, baliabide soilik partzialki esleituko bookings beren gehienez.</span><span class="sxs-lookup"><span data-stu-id="cede0-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="cede0-140">Esleitu gabeko zeregin ordu gainerako horiek lan diren kanpaina-xehatzea egitura Unstaffed Ordu zutabe gehituz ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="cede0-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="cede0-141">Baliabideak ordu booked beren esleitzen baduzu (beren booked ordu berdina da ordu esleitutako beren), eslei diezazkiekezu are gehiago zereginak saiatzean hurrengo errore-mezua ikusiko duzu:</span><span class="sxs-lookup"><span data-stu-id="cede0-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="cede0-142">*Ezin da esleitu baliabidea zereginean - Baliabide hauek ez dute nahikoa ordu erreserbatuta proiektuan.*</span><span class="sxs-lookup"><span data-stu-id="cede0-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="cede0-143">Gainera, lehenetsia proiektua kudeatzailea taldearen kide proiektuan sortzean taldeari gehitutako bookings edozein gabe gehituko da eta ezin zaizkie objektuak esleitu zeregin guztiak.</span><span class="sxs-lookup"><span data-stu-id="cede0-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="cede0-144">Horiek ez erakutsi, baliabide-barrako goitibeheran zereginetarako.</span><span class="sxs-lookup"><span data-stu-id="cede0-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="cede0-145">Baliabide hau esleitu nahi badituzu, talde batetik ezaba eta, ondoren, berriro gehitzeko bat Ere ez guztirako baldintza kopuruak metodo bat beharko duzu.</span><span class="sxs-lookup"><span data-stu-id="cede0-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="cede0-146">Xede proiektuaren lehenespenez proiektua approver gutxienez da daitezen da duten ari taldera gehitu, proiektuan sortzen denean arrazoia.</span><span class="sxs-lookup"><span data-stu-id="cede0-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="cede0-147">Funtzio-zeregin bidez orokorra taldearen kide zereginekin lan sortu</span><span class="sxs-lookup"><span data-stu-id="cede0-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="cede0-148">Metodo hori assures baliabide-dituzte zereginak bookings nahikoa.</span><span class="sxs-lookup"><span data-stu-id="cede0-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="cede0-149">Lehenik eta behin, sortu leku-marka edo ultimately zereginak lantzeko zereginak funtzio esleituz ondoren talde bat sortzen du nahi duzun baliabidea named ezaugarri deskribatzen duen baliabide orokorra.</span><span class="sxs-lookup"><span data-stu-id="cede0-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="cede0-150">Hemen da hori egiteko modua:</span><span class="sxs-lookup"><span data-stu-id="cede0-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="cede0-151">Lan egin diren kanpaina-xehatzea egitura, hautatu zeregin bat.</span><span class="sxs-lookup"><span data-stu-id="cede0-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="cede0-152">Hautatu **Esleitu Funtzioa** baliabide gelaxka goitibeherako ikonoa.</span><span class="sxs-lookup"><span data-stu-id="cede0-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="cede0-153">Hautatu **Funtzioa** goitibeherako eta orokorra baliabide funtzioa hautatzeko.</span><span class="sxs-lookup"><span data-stu-id="cede0-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="cede0-154">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="cede0-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="cede0-155">![WBS erabiliz baliabidea gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-4.png "WBS erabiliz baliabidea gehitzeko pantaila-argazkia")</span><span class="sxs-lookup"><span data-stu-id="cede0-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="cede0-156">Administrazio-funtzioak, WBS zereginak osatu dituzunean, hautatu **Sortu proiektu-taldea**.</span><span class="sxs-lookup"><span data-stu-id="cede0-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="cede0-157">Project Service-k orokorra taldekideak oinarrituta-funtzioak, resourcing erakundearen unitateak eta proiektua egutegi zeregina esleipenetan aggregating arabera kopurua gutxieneko sortzen du.</span><span class="sxs-lookup"><span data-stu-id="cede0-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="cede0-158">![Proiektuaren taldea sortzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-5.png "Proiektuaren taldea sortzeko pantaila-argazkia")</span><span class="sxs-lookup"><span data-stu-id="cede0-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="cede0-159">Taldeko Kide saretan, ikusiko duzu baliabide-funtzioak eta posizio izen Orokorra Baliabide mota.</span><span class="sxs-lookup"><span data-stu-id="cede0-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="cede0-160">Baliabideak bi ditu-funtzio bat behar diren, Sortu Taldearen eginbidea bi taldekideak sortzen du eta apart ezarri posizioaren izena erabiltzen.</span><span class="sxs-lookup"><span data-stu-id="cede0-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="cede0-161">![Bi baliabide generiko gehitzeko pantaila-argazkia](media/FAQ-Resources-to-Tasks2-6.png "Bi baliabide generiko gehitzeko pantaila-argazkia")</span><span class="sxs-lookup"><span data-stu-id="cede0-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="cede0-162">Baliabide Eskakizun atalean esteka hautatuta backing baliabide eskakizun orokorra taldearen kide ireki dezakezu.</span><span class="sxs-lookup"><span data-stu-id="cede0-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="cede0-163">![Ordezko baliabide-eskakizunak irekitzearen pantaila-argazkia](media/FAQ-Resources-to-Tasks2-7.png "Ordezko baliabide-eskakizunak irekitzearen pantaila-argazkia")</span><span class="sxs-lookup"><span data-stu-id="cede0-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="cede0-164">Hautatu **Erreserbatu** orokorra baliabidea, eta, ondoren, erabil dezakezu antolaketa board bilaketa eta erreserbatutako benetako baliabide.</span><span class="sxs-lookup"><span data-stu-id="cede0-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="cede0-165">Baliabide kudeatzailea arabera betetze-eskakizun hautatuta bidali dezakezu ere **Eskatzeko Bidali**.</span><span class="sxs-lookup"><span data-stu-id="cede0-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="cede0-166">Baliabidea orokorra baliabide named beteta dagoenean, orokorra baliabide-taldetik kendu eta orokorra baliabide esleitutako zeregina orokorra baliabide baliabide eskakizun beteta baliabidea named esleitzen zaizkio.</span><span class="sxs-lookup"><span data-stu-id="cede0-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 



[!INCLUDE[footer-include](../includes/footer-banner.md)]