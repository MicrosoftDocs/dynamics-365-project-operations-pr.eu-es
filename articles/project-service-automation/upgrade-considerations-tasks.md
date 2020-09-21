---
title: Zereginen xehetasunen egiturari buruzko gogoeta eguneratuak
description: Gai honek zereginen xehetasunen egitura Project Service Automation-en 2.x-tik 3.x-ra bertsio-berritzeari buruzko informazioa ematen du.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 2.x
author: ruhercul
ms.assetid: 9e43d5b5-ca5d-41f5-9012-c48f8e3080f9
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 9aa35dd8784bfa55737b0836e653afd0442b80c2
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748901"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="f8744-103">Zereginen xehetasunen egiturari buruzko gogoeta eguneratuak</span><span class="sxs-lookup"><span data-stu-id="f8744-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="f8744-104">Gai honek zereginen xehetasunen egitura Project Service Automation-en 2.x-tik 3.x-ra bertsio-berritzeari buruzko informazioa ematen du.</span><span class="sxs-lookup"><span data-stu-id="f8744-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="f8744-105">Gai honek Project Service Automation-eko (PSA) proiektu baten egoera osasuntsua definitzen du, bertsio-berritzea ondo egin dadin beharrezkoa dena.</span><span class="sxs-lookup"><span data-stu-id="f8744-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="f8744-106">Bertsio-berritzeak huts egitea eragiten duten blokeo baldintza arruntei buruzko informazioa ere badago.</span><span class="sxs-lookup"><span data-stu-id="f8744-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="f8744-107">Proiektuen zereginak eta haien funtzioak proiektuaren antolaketan zehazteari buruzko informazio gehiago lortzeko, ikusi [Proiektuen antolaketa](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="f8744-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="f8744-108">Entitate gakoak</span><span class="sxs-lookup"><span data-stu-id="f8744-108">Key entities</span></span>
<span data-ttu-id="f8744-109">Jada baliabidez kargatutako zereginen xehetasunen egitura zehatza lortzeko, erakunde hauek behar dira:</span><span class="sxs-lookup"><span data-stu-id="f8744-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="f8744-110">Proiektua</span><span class="sxs-lookup"><span data-stu-id="f8744-110">Project</span></span>](../developer/entities/msdyn_project.md)
- [<span data-ttu-id="f8744-111">Proiektu-taldea</span><span class="sxs-lookup"><span data-stu-id="f8744-111">Project Team</span></span>](../developer/entities/msdyn_projectteam.md)
- [<span data-ttu-id="f8744-112">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="f8744-112">Project Task</span></span>](../developer/entities/msdyn_projecttask.md)
- [<span data-ttu-id="f8744-113">Baliabide-esleipenak</span><span class="sxs-lookup"><span data-stu-id="f8744-113">Resource Assignments</span></span>](../developer/entities/msdyn_resourceassignment.md)
- [<span data-ttu-id="f8744-114">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="f8744-114">Project Task Dependency</span></span>](../developer/entities/msdyn_projecttaskdependency.md)
- [<span data-ttu-id="f8744-115">Baliabide erreserbagarriak</span><span class="sxs-lookup"><span data-stu-id="f8744-115">Bookable Resources</span></span>](../developer/entities/bookableresource.md)

<span data-ttu-id="f8744-116">Baliabideek kargatutako zereginen xehetasunen egitura zehazteko, urrats hauei jarraitu behar diezu:</span><span class="sxs-lookup"><span data-stu-id="f8744-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="f8744-117">Sortu proiektu berria.</span><span class="sxs-lookup"><span data-stu-id="f8744-117">Create a new project.</span></span> <span data-ttu-id="f8744-118">Proiektu berria sortzeari buruzko informazio gehiago lortzeko, ikusi [msdyn_project](../developer/entities/msdyn_project.md).</span><span class="sxs-lookup"><span data-stu-id="f8744-118">For more information about how to create a new project, see [msdyn_project](../developer/entities/msdyn_project.md).</span></span>
2. <span data-ttu-id="f8744-119">Sortu zeregin bat edo gehiago.</span><span class="sxs-lookup"><span data-stu-id="f8744-119">Create one or more tasks.</span></span> <span data-ttu-id="f8744-120">Zeregin bat sortzeari buruzko informazio gehiago lortzeko, ikusi [msdyn_projecttask](../developer/entities/msdyn_projecttask.md).</span><span class="sxs-lookup"><span data-stu-id="f8744-120">For more information about how to create a task, see [msdyn_projecttask](../developer/entities/msdyn_projecttask.md).</span></span>
3. <span data-ttu-id="f8744-121">Zehaztu zereginaren mendekotasunak.</span><span class="sxs-lookup"><span data-stu-id="f8744-121">Define the task dependencies.</span></span> <span data-ttu-id="f8744-122">Informazio gehiago lortzeko, ikusi [Proiektuaren zereginen mendekotasuna](../developer/entities/msdyn_projecttaskdependency.md).</span><span class="sxs-lookup"><span data-stu-id="f8744-122">For more information, see [Project Task Dependency](../developer/entities/msdyn_projecttaskdependency.md).</span></span>
4. <span data-ttu-id="f8744-123">Esleitu proiektuko taldekideak proiektuari.</span><span class="sxs-lookup"><span data-stu-id="f8744-123">Assign project team members to the project.</span></span> <span data-ttu-id="f8744-124">Informazio gehiago lortzeko, ikus [msdyn_projectteam](../developer/entities/msdyn_projectteam.md).</span><span class="sxs-lookup"><span data-stu-id="f8744-124">For more information, see [msdyn_projectteam](../developer/entities/msdyn_projectteam.md).</span></span>
5. <span data-ttu-id="f8744-125">Esleitu proiektuko taldekideak zereginei.</span><span class="sxs-lookup"><span data-stu-id="f8744-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="f8744-126">Informazio gehiago lortzeko, ikus [msdyn_resourceassignment](../developer/entities/msdyn_resourceassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f8744-126">For more information, see [msdyn_resourceassignment](../developer/entities/msdyn_resourceassignment.md).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="f8744-127">Proiektu-taldeko erlazioak</span><span class="sxs-lookup"><span data-stu-id="f8744-127">Project team relationships</span></span>

<span data-ttu-id="f8744-128">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="f8744-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="f8744-129">Proiektuko taldekide guztiek baliabide erreserbagarri bati esleituta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="f8744-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="f8744-130">Proiektuko taldekide guztiek proiektu berari esleituta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="f8744-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="f8744-131">Proiektuaren zereginen erlazioak</span><span class="sxs-lookup"><span data-stu-id="f8744-131">Project task relationships</span></span>
<span data-ttu-id="f8744-132">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="f8744-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="f8744-133">Proiektu berarekin erlazionatutako edozein zeregin esleituta egon behar dira.</span><span class="sxs-lookup"><span data-stu-id="f8744-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="f8744-134">Lerroko zeregin guztiek zeregin nagusia izan behar dute.</span><span class="sxs-lookup"><span data-stu-id="f8744-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="f8744-135">Lerroko zeregin guztiek proiektu nagusi bat izan behar dute.</span><span class="sxs-lookup"><span data-stu-id="f8744-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="f8744-136">Baliozko baldintzak</span><span class="sxs-lookup"><span data-stu-id="f8744-136">Valid conditions</span></span>

- <span data-ttu-id="f8744-137">Zereginen iraupen guztiak ordu bat baino handiagoa edo berdina (> =) eta 1.800.000 minutu baino gutxiagokoa (1.250 egun) izan behar du. \*</span><span class="sxs-lookup"><span data-stu-id="f8744-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="f8744-138">Zeregin guztien hasierako data hau baino lehenagokoa izan behar da: 2000/01/01.\*</span><span class="sxs-lookup"><span data-stu-id="f8744-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="f8744-139">Zeregin guztien hasierako data ezin da izan gaur egun baino 17 urte baino lehenagokoa.\*</span><span class="sxs-lookup"><span data-stu-id="f8744-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="f8744-140">Zeregin guztiek hasierako data amaierako dataren berdina edo lehenagokoa izan behar da.</span><span class="sxs-lookup"><span data-stu-id="f8744-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="f8744-141">Sailkapenen transakzio mota guztiek (gastua, materiala, zerga eta denbora) balioak izan behar dituzte **Lehenespeneko unitatea** eta **Salmenta-unitatea** aukeretarako.</span><span class="sxs-lookup"><span data-stu-id="f8744-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="f8744-142">Letrak dituzten data formatuak ekidin behar dira.</span><span class="sxs-lookup"><span data-stu-id="f8744-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="f8744-143">Balizko urrats aringarriak</span><span class="sxs-lookup"><span data-stu-id="f8744-143">Potential mitigation steps</span></span>
- <span data-ttu-id="f8744-144">Erabili Bilatu aurreratua Proiektuaren IDrik ez duten Proiektuen zereginak identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="f8744-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="f8744-145">Erabili Bilaketa aurreratua Proiektuaren zereginak identifikatzeko iraupena > 1.800.000 baino handiagoa denean.</span><span class="sxs-lookup"><span data-stu-id="f8744-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="f8744-146">Datu-aldaketak egin aurretik, datuak egoera txarrean izatera eraman dituen entitatearekin lotutako pertsonalizazio guztiak aztertu beharko zenituzke.</span><span class="sxs-lookup"><span data-stu-id="f8744-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="f8744-147">Pertsonalizazio horiek datuekin lotutako eguneratzeekin jarraitu aurretik zuzendu beharko lirateke.</span><span class="sxs-lookup"><span data-stu-id="f8744-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="f8744-148">Umezurtz geratu diren identifikatutako zereginetarako, pentsatu zeregin horiek ezabatzea beharrezkoak ez badira edo proiektu nagusi egokiarekin lotu behar badira.</span><span class="sxs-lookup"><span data-stu-id="f8744-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="f8744-149">Iraupena 1.250 egun baino handiagoa den edozein zereginetarako, iraupen totala adieraziko duten zeregin ugari gehitzea gomendatzen da, bideragarria bada.</span><span class="sxs-lookup"><span data-stu-id="f8744-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="f8744-150">Izartxo batekin (\*) aipatutako elementuek mugak dituzte bezero-erlazioen kudeaketak (CRM) 7.320 errepikapen-hedapen bakarrik onartzen dituelako.</span><span class="sxs-lookup"><span data-stu-id="f8744-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="f8744-151">Muga horren azpitik egon behar duzu.</span><span class="sxs-lookup"><span data-stu-id="f8744-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="f8744-152">Baliabide-esleipenaren erlazioak</span><span class="sxs-lookup"><span data-stu-id="f8744-152">Resource Assignment relationships</span></span>
<span data-ttu-id="f8744-153">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="f8744-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="f8744-154">Zereginen xehetasunen egiturako baliabideen esleipen guztiek proiektu berari lotuta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="f8744-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="f8744-155">Zereginen xehetasunen egiturako baliabideen esleipen guztiek proiektu bereko proiektu-taldekide berari esleituta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="f8744-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="f8744-156">Balizko urrats aringarriak</span><span class="sxs-lookup"><span data-stu-id="f8744-156">Potential mitigation steps</span></span>
- <span data-ttu-id="f8744-157">Identifikatu goian azaldutako baldintzetatik kanpo dauden zeregin guztiak.</span><span class="sxs-lookup"><span data-stu-id="f8744-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="f8744-158">Dagoeneko balio ez duten baliabide-esleipenak ezabatu egin beharko lirateke.</span><span class="sxs-lookup"><span data-stu-id="f8744-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="f8744-159">Proiektuaren zereginaren mendekotasunaren erlazioak</span><span class="sxs-lookup"><span data-stu-id="f8744-159">Project task dependency relationships</span></span>
<span data-ttu-id="f8744-160">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="f8744-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="f8744-161">Proiektuaren zereginen mendekotasun guztiak proiektu berarekin lotuta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="f8744-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="f8744-162">Zeregin batek ezin dio erreferentzia egin mendekotasun berari behin baino gehiagotan.</span><span class="sxs-lookup"><span data-stu-id="f8744-162">A task can't have the same dependency referenced more than once.</span></span>
