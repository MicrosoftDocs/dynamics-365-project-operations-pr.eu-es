---
title: Zereginen xehetasunen egiturari buruzko gogoeta eguneratuak
description: Gai honek zereginen xehetasunen egitura Project Service Automation-en 2.x-tik 3.x-ra bertsio-berritzeari buruzko informazioa ematen du.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: 0b75fd372732f42a3557aaa5eccec1f24a644941
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121788"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="2ea35-103">Zereginen xehetasunen egiturari buruzko gogoeta eguneratuak</span><span class="sxs-lookup"><span data-stu-id="2ea35-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="2ea35-104">Gai honek zereginen xehetasunen egitura Project Service Automation-en 2.x-tik 3.x-ra bertsio-berritzeari buruzko informazioa ematen du.</span><span class="sxs-lookup"><span data-stu-id="2ea35-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="2ea35-105">Gai honek Project Service Automation-eko (PSA) proiektu baten egoera osasuntsua definitzen du, bertsio-berritzea ondo egin dadin beharrezkoa dena.</span><span class="sxs-lookup"><span data-stu-id="2ea35-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="2ea35-106">Bertsio-berritzeak huts egitea eragiten duten blokeo baldintza arruntei buruzko informazioa ere badago.</span><span class="sxs-lookup"><span data-stu-id="2ea35-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="2ea35-107">Proiektuen zereginak eta haien funtzioak proiektuaren antolaketan zehazteari buruzko informazio gehiago lortzeko, ikusi [Proiektuen antolaketa](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="2ea35-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="2ea35-108">Entitate gakoak</span><span class="sxs-lookup"><span data-stu-id="2ea35-108">Key entities</span></span>
<span data-ttu-id="2ea35-109">Jada baliabidez kargatutako zereginen xehetasunen egitura zehatza lortzeko, erakunde hauek behar dira:</span><span class="sxs-lookup"><span data-stu-id="2ea35-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="2ea35-110">Proiektua</span><span class="sxs-lookup"><span data-stu-id="2ea35-110">Project</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="2ea35-111">Proiektu-taldea</span><span class="sxs-lookup"><span data-stu-id="2ea35-111">Project Team</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="2ea35-112">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="2ea35-112">Project Task</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="2ea35-113">Baliabide-esleipenak</span><span class="sxs-lookup"><span data-stu-id="2ea35-113">Resource Assignments</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="2ea35-114">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="2ea35-114">Project Task Dependency</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="2ea35-115">Baliabide erreserbagarriak</span><span class="sxs-lookup"><span data-stu-id="2ea35-115">Bookable Resources</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="2ea35-116">Baliabideek kargatutako zereginen xehetasunen egitura zehazteko, urrats hauei jarraitu behar diezu:</span><span class="sxs-lookup"><span data-stu-id="2ea35-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="2ea35-117">Sortu proiektu berria.</span><span class="sxs-lookup"><span data-stu-id="2ea35-117">Create a new project.</span></span> <span data-ttu-id="2ea35-118">Proiektu berria sortzeari buruzko informazio gehiago lortzeko, ikusi [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span><span class="sxs-lookup"><span data-stu-id="2ea35-118">For more information about how to create a new project, see [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="2ea35-119">Sortu zeregin bat edo gehiago.</span><span class="sxs-lookup"><span data-stu-id="2ea35-119">Create one or more tasks.</span></span> <span data-ttu-id="2ea35-120">Zeregin bat sortzeari buruzko informazio gehiago lortzeko, ikusi [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span><span class="sxs-lookup"><span data-stu-id="2ea35-120">For more information about how to create a task, see [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="2ea35-121">Zehaztu zereginaren mendekotasunak.</span><span class="sxs-lookup"><span data-stu-id="2ea35-121">Define the task dependencies.</span></span> <span data-ttu-id="2ea35-122">Informazio gehiago lortzeko, ikusi [Proiektuaren zereginen mendekotasuna](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span><span class="sxs-lookup"><span data-stu-id="2ea35-122">For more information, see [Project Task Dependency](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="2ea35-123">Esleitu proiektuko taldekideak proiektuari.</span><span class="sxs-lookup"><span data-stu-id="2ea35-123">Assign project team members to the project.</span></span> <span data-ttu-id="2ea35-124">Informazio gehiago lortzeko, ikus [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span><span class="sxs-lookup"><span data-stu-id="2ea35-124">For more information, see [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="2ea35-125">Esleitu proiektuko taldekideak zereginei.</span><span class="sxs-lookup"><span data-stu-id="2ea35-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="2ea35-126">Informazio gehiago lortzeko, ikus [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span><span class="sxs-lookup"><span data-stu-id="2ea35-126">For more information, see [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="2ea35-127">Proiektu-taldeko erlazioak</span><span class="sxs-lookup"><span data-stu-id="2ea35-127">Project team relationships</span></span>

<span data-ttu-id="2ea35-128">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="2ea35-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="2ea35-129">Proiektuko taldekide guztiek baliabide erreserbagarri bati esleituta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="2ea35-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="2ea35-130">Proiektuko taldekide guztiek proiektu berari esleituta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="2ea35-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="2ea35-131">Proiektuaren zereginen erlazioak</span><span class="sxs-lookup"><span data-stu-id="2ea35-131">Project task relationships</span></span>
<span data-ttu-id="2ea35-132">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="2ea35-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="2ea35-133">Proiektu berarekin erlazionatutako edozein zeregin esleituta egon behar dira.</span><span class="sxs-lookup"><span data-stu-id="2ea35-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="2ea35-134">Lerroko zeregin guztiek zeregin nagusia izan behar dute.</span><span class="sxs-lookup"><span data-stu-id="2ea35-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="2ea35-135">Lerroko zeregin guztiek proiektu nagusi bat izan behar dute.</span><span class="sxs-lookup"><span data-stu-id="2ea35-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="2ea35-136">Baliozko baldintzak</span><span class="sxs-lookup"><span data-stu-id="2ea35-136">Valid conditions</span></span>

- <span data-ttu-id="2ea35-137">Zereginen iraupen guztiak ordu bat baino handiagoa edo berdina (> =) eta 1.800.000 minutu baino gutxiagokoa (1.250 egun) izan behar du. \*</span><span class="sxs-lookup"><span data-stu-id="2ea35-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="2ea35-138">Zeregin guztien hasierako data hau baino lehenagokoa izan behar da: 2000/01/01.\*</span><span class="sxs-lookup"><span data-stu-id="2ea35-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="2ea35-139">Zeregin guztien hasierako data ezin da izan gaur egun baino 17 urte baino lehenagokoa.\*</span><span class="sxs-lookup"><span data-stu-id="2ea35-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="2ea35-140">Zeregin guztiek hasierako data amaierako dataren berdina edo lehenagokoa izan behar da.</span><span class="sxs-lookup"><span data-stu-id="2ea35-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="2ea35-141">Sailkapenen transakzio mota guztiek (gastua, materiala, zerga eta denbora) balioak izan behar dituzte **Lehenespeneko unitatea** eta **Salmenta-unitatea** aukeretarako.</span><span class="sxs-lookup"><span data-stu-id="2ea35-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="2ea35-142">Letrak dituzten data formatuak ekidin behar dira.</span><span class="sxs-lookup"><span data-stu-id="2ea35-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="2ea35-143">Balizko urrats aringarriak</span><span class="sxs-lookup"><span data-stu-id="2ea35-143">Potential mitigation steps</span></span>
- <span data-ttu-id="2ea35-144">Erabili Bilatu aurreratua Proiektuaren IDrik ez duten Proiektuen zereginak identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="2ea35-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="2ea35-145">Erabili Bilaketa aurreratua Proiektuaren zereginak identifikatzeko iraupena > 1.800.000 baino handiagoa denean.</span><span class="sxs-lookup"><span data-stu-id="2ea35-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="2ea35-146">Datu-aldaketak egin aurretik, datuak egoera txarrean izatera eraman dituen entitatearekin lotutako pertsonalizazio guztiak aztertu beharko zenituzke.</span><span class="sxs-lookup"><span data-stu-id="2ea35-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="2ea35-147">Pertsonalizazio horiek datuekin lotutako eguneratzeekin jarraitu aurretik zuzendu beharko lirateke.</span><span class="sxs-lookup"><span data-stu-id="2ea35-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="2ea35-148">Umezurtz geratu diren identifikatutako zereginetarako, pentsatu zeregin horiek ezabatzea beharrezkoak ez badira edo proiektu nagusi egokiarekin lotu behar badira.</span><span class="sxs-lookup"><span data-stu-id="2ea35-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="2ea35-149">Iraupena 1.250 egun baino handiagoa den edozein zereginetarako, iraupen totala adieraziko duten zeregin ugari gehitzea gomendatzen da, bideragarria bada.</span><span class="sxs-lookup"><span data-stu-id="2ea35-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="2ea35-150">Izartxo batekin (\*) aipatutako elementuek mugak dituzte bezero-erlazioen kudeaketak (CRM) 7.320 errepikapen-hedapen bakarrik onartzen dituelako.</span><span class="sxs-lookup"><span data-stu-id="2ea35-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="2ea35-151">Muga horren azpitik egon behar duzu.</span><span class="sxs-lookup"><span data-stu-id="2ea35-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="2ea35-152">Baliabide-esleipenaren erlazioak</span><span class="sxs-lookup"><span data-stu-id="2ea35-152">Resource Assignment relationships</span></span>
<span data-ttu-id="2ea35-153">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="2ea35-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="2ea35-154">Zereginen xehetasunen egiturako baliabideen esleipen guztiek proiektu berari lotuta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="2ea35-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="2ea35-155">Zereginen xehetasunen egiturako baliabideen esleipen guztiek proiektu bereko proiektu-taldekide berari esleituta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="2ea35-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="2ea35-156">Balizko urrats aringarriak</span><span class="sxs-lookup"><span data-stu-id="2ea35-156">Potential mitigation steps</span></span>
- <span data-ttu-id="2ea35-157">Identifikatu goian azaldutako baldintzetatik kanpo dauden zeregin guztiak.</span><span class="sxs-lookup"><span data-stu-id="2ea35-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="2ea35-158">Dagoeneko balio ez duten baliabide-esleipenak ezabatu egin beharko lirateke.</span><span class="sxs-lookup"><span data-stu-id="2ea35-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="2ea35-159">Proiektuaren zereginaren mendekotasunaren erlazioak</span><span class="sxs-lookup"><span data-stu-id="2ea35-159">Project task dependency relationships</span></span>
<span data-ttu-id="2ea35-160">Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:</span><span class="sxs-lookup"><span data-stu-id="2ea35-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="2ea35-161">Proiektuaren zereginen mendekotasun guztiak proiektu berarekin lotuta egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="2ea35-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="2ea35-162">Zeregin batek ezin dio erreferentzia egin mendekotasun berari behin baino gehiagotan.</span><span class="sxs-lookup"><span data-stu-id="2ea35-162">A task can't have the same dependency referenced more than once.</span></span>
