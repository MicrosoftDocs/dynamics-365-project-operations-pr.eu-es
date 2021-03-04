---
title: Baliabide-kudeaketa gida (Project Service Automation 3.x)
description: Gai honek baliabideak kudeatzeko eremuan izandako aldaketen inguruko informazioa ematen du.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 94f9adc67163254486387a1ce59d5d3e8e93c335
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148628"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="b1f32-103">Baliabide-kudeaketa gida (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="b1f32-103">Resource management changes (Project Service Automation 3.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

<span data-ttu-id="b1f32-104">Gai honen atalek Dynamics 365 Project Service Automation aplikazioaren 3.x bertsioako baliabideak kudeatzeko eremuan egin diren aldaketen inguruko informazioa ematen dute.</span><span class="sxs-lookup"><span data-stu-id="b1f32-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="b1f32-105">Proiektuaren aurreikuspenak</span><span class="sxs-lookup"><span data-stu-id="b1f32-105">Project estimates</span></span>

<span data-ttu-id="b1f32-106">**msdyn \_projecttask** entitatean (**Proiektuaren zeregina**) oinarrituta egon beharrean, proiektuaren aurreikuspenak **msdyn \_resourceassignment** entitatean (**Baliabide-esleipena**) oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="b1f32-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="b1f32-107">Baliabide-esleipenak zereginen planifikazioa eta prezioak egiteko "egia iturri" bihurtu dira.</span><span class="sxs-lookup"><span data-stu-id="b1f32-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="b1f32-108">Lerro-zereginak</span><span class="sxs-lookup"><span data-stu-id="b1f32-108">Line tasks</span></span>

<span data-ttu-id="b1f32-109">PSA aplikazioaren 3.x bertsioan, lerro-zereginak zaharkituta daude.</span><span class="sxs-lookup"><span data-stu-id="b1f32-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="b1f32-110">Esleipenek zeregin osoa adierazten dute lerro-zereginen ordez.</span><span class="sxs-lookup"><span data-stu-id="b1f32-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="b1f32-111">Hurrengo adibidean, "Probako zeregina" izeneko zeregina A eta B taldeko kideei nola esleitu zaien ikusten da PSA-ren aurreko bertsioetan eta PSA-ren 3.x bertsioan.</span><span class="sxs-lookup"><span data-stu-id="b1f32-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="b1f32-112">**PSA-ren 3.x bertsioaren aurretik:**</span><span class="sxs-lookup"><span data-stu-id="b1f32-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="b1f32-113">Probako zeregina</span><span class="sxs-lookup"><span data-stu-id="b1f32-113">Test task</span></span>

        - <span data-ttu-id="b1f32-114">Probako zeregina - 1. lerro-zeregina</span><span class="sxs-lookup"><span data-stu-id="b1f32-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="b1f32-115">Esleipena Ari</span><span class="sxs-lookup"><span data-stu-id="b1f32-115">Assignment to A</span></span>

        - <span data-ttu-id="b1f32-116">Probako zeregina - 2. lerro-zeregina</span><span class="sxs-lookup"><span data-stu-id="b1f32-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="b1f32-117">Esleipena Bri</span><span class="sxs-lookup"><span data-stu-id="b1f32-117">Assignment to B</span></span>

- <span data-ttu-id="b1f32-118">**PSA-ren 3.x bertsioa:**</span><span class="sxs-lookup"><span data-stu-id="b1f32-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="b1f32-119">Probako zeregina</span><span class="sxs-lookup"><span data-stu-id="b1f32-119">Test task</span></span>

        - <span data-ttu-id="b1f32-120">Esleipena Ari</span><span class="sxs-lookup"><span data-stu-id="b1f32-120">Assignment to A</span></span>
        - <span data-ttu-id="b1f32-121">Esleipena Bri</span><span class="sxs-lookup"><span data-stu-id="b1f32-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="b1f32-122">Esleitu gabeko esleipena</span><span class="sxs-lookup"><span data-stu-id="b1f32-122">Unassigned assignment</span></span>

<span data-ttu-id="b1f32-123">PSA-ren 3.x bertsion, esleitu gabeko esleipena **NULUA** taldekidea eta **NULUA** baliabideari esleitutako esleipena da.</span><span class="sxs-lookup"><span data-stu-id="b1f32-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="b1f32-124">Esleipen gabeko esleipenak bi egoeratan gerta daitezke:</span><span class="sxs-lookup"><span data-stu-id="b1f32-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="b1f32-125">Zeregin bat sortu bada, baina oraindik taldekideren bati esleitu ez bazaio, esleitu gabeko esleipena sortzen da beti.</span><span class="sxs-lookup"><span data-stu-id="b1f32-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="b1f32-126">Zeregin bateko esleipendun guztiak kentzen badira, zeregin horretarako esleitu gabeko esleipena sortzen da berriro.</span><span class="sxs-lookup"><span data-stu-id="b1f32-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="b1f32-127">Proiektuaren zereginen entitateko eremuak antolatzea</span><span class="sxs-lookup"><span data-stu-id="b1f32-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="b1f32-128">**msdyn \_projecttask** entitateko eremuak zaharkituta geratu dira, **msdyn \_resourceassignment** entitatera mugitu dira edo orain **msdyn \_projectteam** entitatean (**Proiektu-taldeko kidea**) aipatzen dira.</span><span class="sxs-lookup"><span data-stu-id="b1f32-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="b1f32-129">Zaharkitutako eremua on msdyn\_projecttask atalean (Proiektuaren zeregina)</span><span class="sxs-lookup"><span data-stu-id="b1f32-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="b1f32-130">Eremu berria msdyn\_resourceassignment atalean (Baliabideen esleipena)</span><span class="sxs-lookup"><span data-stu-id="b1f32-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="b1f32-131">Iruzkina</span><span class="sxs-lookup"><span data-stu-id="b1f32-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="b1f32-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="b1f32-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="b1f32-133">Bat ere ez</span><span class="sxs-lookup"><span data-stu-id="b1f32-133">None</span></span> | |
| <span data-ttu-id="b1f32-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="b1f32-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="b1f32-135">Bat ere ez</span><span class="sxs-lookup"><span data-stu-id="b1f32-135">None</span></span> | |
| <span data-ttu-id="b1f32-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="b1f32-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="b1f32-137">Bat ere ez</span><span class="sxs-lookup"><span data-stu-id="b1f32-137">None</span></span> | |
| <span data-ttu-id="b1f32-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="b1f32-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="b1f32-139">Bat ere ez</span><span class="sxs-lookup"><span data-stu-id="b1f32-139">None</span></span> | |
| <span data-ttu-id="b1f32-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="b1f32-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="b1f32-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="b1f32-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="b1f32-142">Eremuan gordetako JavaScript Object Notation (JSON) datuen egituraren formatua aldatu da.</span><span class="sxs-lookup"><span data-stu-id="b1f32-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="b1f32-143">Antolaketaren ingerada</span><span class="sxs-lookup"><span data-stu-id="b1f32-143">Schedule contour</span></span>

<span data-ttu-id="b1f32-144">Antolaketaren ingerada **Aurreikusitako lana** eremuan gordetzen da (**msdyn \_plannedwork**) **Baliabide-esleipena** entitate bakoitzean (**msdyn \_resourceassignment**).</span><span class="sxs-lookup"><span data-stu-id="b1f32-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="b1f32-145">Egitura</span><span class="sxs-lookup"><span data-stu-id="b1f32-145">Structure</span></span>

<span data-ttu-id="b1f32-146">Antolaketaren ingeradaren egitura berria antolatutako egun bakoitzerako definitzen diren denbora-tarte malguek osatzen dute.</span><span class="sxs-lookup"><span data-stu-id="b1f32-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="b1f32-147">Denbora-tarte bakoitzean propietate hauek daude:</span><span class="sxs-lookup"><span data-stu-id="b1f32-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="b1f32-148">**Hasi** – Eguneko lanaldiaren hasiera, proiektuaren egutegiaren arabera.</span><span class="sxs-lookup"><span data-stu-id="b1f32-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="b1f32-149">**Amaitu** – Eguneko lanaldiaren amaiera, proiektuaren egutegiaren arabera.</span><span class="sxs-lookup"><span data-stu-id="b1f32-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="b1f32-150">**Orduak** – Egunean esleitzen zaion ordu kopurua.</span><span class="sxs-lookup"><span data-stu-id="b1f32-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="b1f32-151">**Adibidea**</span><span class="sxs-lookup"><span data-stu-id="b1f32-151">**Example**</span></span>

<span data-ttu-id="b1f32-152">Adibide honek proiektuaren egutegia erabiltzen du, non laneguna goizeko 9etatik arratsaldeko 5etara den UTC-8 ordu-zonan.</span><span class="sxs-lookup"><span data-stu-id="b1f32-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="b1f32-153">Programazio automatikoa eta eskuzko programazioa</span><span class="sxs-lookup"><span data-stu-id="b1f32-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="b1f32-154">Zeregin bat automatikoki programatuta badago, orduak aurrez kargatzen dira eta zereginen iraupena murriztu liteke.</span><span class="sxs-lookup"><span data-stu-id="b1f32-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="b1f32-155">**Adibidea**</span><span class="sxs-lookup"><span data-stu-id="b1f32-155">**Example**</span></span>

<span data-ttu-id="b1f32-156">Honako zeregin hau automatikoki programatuta dago 3 egunetan 18 ordu egiteko (2018ko abenduaren 3tik 2018ko abenduaren 5era).</span><span class="sxs-lookup"><span data-stu-id="b1f32-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="b1f32-157">Zeregin bat eskuz programatuta badago, orduak uniformeki banatzen dira data guztietan.</span><span class="sxs-lookup"><span data-stu-id="b1f32-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="b1f32-158">**Adibidea**</span><span class="sxs-lookup"><span data-stu-id="b1f32-158">**Example**</span></span>

<span data-ttu-id="b1f32-159">Honako zeregin hau eskuz programatuta dago 3 egunetan 18 ordu egiteko (2018ko abenduaren 3tik 2018ko abenduaren 5era).</span><span class="sxs-lookup"><span data-stu-id="b1f32-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="b1f32-160">Esleipen-unitatea</span><span class="sxs-lookup"><span data-stu-id="b1f32-160">Assignment unit</span></span>

<span data-ttu-id="b1f32-161">Esleipen-unitatea zaharkituta gelditu da PSA aplikazioaren 3.x bertsioan.</span><span class="sxs-lookup"><span data-stu-id="b1f32-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="b1f32-162">Zereginaren ahalegin orduak berdin banatzen dira eguneko, esleitutako baliabide guztien artean.</span><span class="sxs-lookup"><span data-stu-id="b1f32-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="b1f32-163">**Adibidea**</span><span class="sxs-lookup"><span data-stu-id="b1f32-163">**Example**</span></span>

<span data-ttu-id="b1f32-164">Adibide honetan, zeregina bi baliabideri esleitzen zaie eta automatikoki antolatuta dago 3 egunez 36 ordu egiteko (2018ko abenduaren 3tik 2018ko abenduaren 5era).</span><span class="sxs-lookup"><span data-stu-id="b1f32-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="b1f32-165">1. esleipena:</span><span class="sxs-lookup"><span data-stu-id="b1f32-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="b1f32-166">2. esleipena:</span><span class="sxs-lookup"><span data-stu-id="b1f32-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="b1f32-167">Prezio-dimentsioak</span><span class="sxs-lookup"><span data-stu-id="b1f32-167">Pricing dimensions</span></span>

<span data-ttu-id="b1f32-168">PSA-ren 3.x bertsioan, baliabide zehatzei buruzko prezioen dimentsioaren eremuak (adibidez, **Funtzioa** eta **Antolaketa-unitatea**) kendu dira **msdyn \_projecttask** erakundetik.</span><span class="sxs-lookup"><span data-stu-id="b1f32-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="b1f32-169">Eremu horiek dagoeneko proiektu-taldeko kidetik (**msdyn\_projectteam**), baliabide-esleipenekoa (**msdyn\_resourceassignment**), eskura daitezke proiektuaren aurreikuspenak sortzen direnean.</span><span class="sxs-lookup"><span data-stu-id="b1f32-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="b1f32-170">Beste eremu bat, **msdyn\_organizationaluni**, gehitu da **msdyn\_projectteam** entitatean.</span><span class="sxs-lookup"><span data-stu-id="b1f32-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="b1f32-171">Zaharkitutako eremua on msdyn\_projecttask atalean (Proiektuaren zeregina)</span><span class="sxs-lookup"><span data-stu-id="b1f32-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="b1f32-172">Horren ordez erabiltzen den msdyn\_projectteam (proiektu-taldeko kidea) ataleko eremua</span><span class="sxs-lookup"><span data-stu-id="b1f32-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="b1f32-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="b1f32-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="b1f32-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="b1f32-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="b1f32-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="b1f32-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="b1f32-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="b1f32-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="b1f32-177">Ingeradak</span><span class="sxs-lookup"><span data-stu-id="b1f32-177">Contours</span></span>

<span data-ttu-id="b1f32-178">Prezioen eta aurreikuspenen ingarada eremuak zeharkitu egin dira **msdyn\_projecttask** entitatean.</span><span class="sxs-lookup"><span data-stu-id="b1f32-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="b1f32-179">**msdyn\_resourceassignment** entitatera mugitu dira.</span><span class="sxs-lookup"><span data-stu-id="b1f32-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="b1f32-180">Zaharkitutako eremua on msdyn\_projecttask atalean (Proiektuaren zeregina)</span><span class="sxs-lookup"><span data-stu-id="b1f32-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="b1f32-181">Eremu berria msdyn\_resourceassignment atalean (Baliabideen esleipena)</span><span class="sxs-lookup"><span data-stu-id="b1f32-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="b1f32-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="b1f32-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="b1f32-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="b1f32-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="b1f32-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="b1f32-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="b1f32-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="b1f32-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="b1f32-186">Hurrengo eremuak **msdyn\_resourceassignment** entitatera gehitu dira:</span><span class="sxs-lookup"><span data-stu-id="b1f32-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="b1f32-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="b1f32-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="b1f32-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="b1f32-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="b1f32-189">Aurreikusitako, benetako eta gainerako kostuen eta salmenten eremuak aldatu gabe daude **msdyn\_projecttask** entitatean:</span><span class="sxs-lookup"><span data-stu-id="b1f32-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="b1f32-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="b1f32-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="b1f32-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="b1f32-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="b1f32-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="b1f32-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="b1f32-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="b1f32-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="b1f32-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="b1f32-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="b1f32-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="b1f32-195">msdyn\_remainingsales</span></span>
