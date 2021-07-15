---
title: Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko
description: Gai honek informazioa eta laginak eskaintzen ditu proiektuen programazio APIak erabiltzeko.
author: sigitac
ms.date: 06/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4915261c08a3271a919e04084e92a14b297c1b35
ms.sourcegitcommit: 2f16c2bc7c8350676a6a380c61fffa9958db6a0b
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/22/2021
ms.locfileid: "6293212"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="44ead-103">Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko</span><span class="sxs-lookup"><span data-stu-id="44ead-103">Use Project schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="44ead-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="44ead-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="44ead-105">Gai honetan zehaztutako funtzionaltasun batzuk edo guztiak erabilgarri dago aurrebista-bertsioaren zati gisa.</span><span class="sxs-lookup"><span data-stu-id="44ead-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="44ead-106">Edukia eta funtzionalitatea aldatu egin daitezke.</span><span class="sxs-lookup"><span data-stu-id="44ead-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="44ead-107">Antolaketa-entitateak</span><span class="sxs-lookup"><span data-stu-id="44ead-107">Scheduling entities</span></span>

<span data-ttu-id="44ead-108">Proiektuen programazio APIek eragiketak sortzeko, eguneratzeko eta ezabatzeko gaitasuna eskaintzen dute **Programazio entitateekin**.</span><span class="sxs-lookup"><span data-stu-id="44ead-108">Project schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="44ead-109">Entitate hauek Project for the Web-en antolaketa-motorearen bidez kudeatzen dira.</span><span class="sxs-lookup"><span data-stu-id="44ead-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="44ead-110">Sortu, eguneratu eta ezabatu eragiketak honekin **Programazio entitateak** lehenago mugatu ziren Dynamics 365 Project Operations oharrak.</span><span class="sxs-lookup"><span data-stu-id="44ead-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="44ead-111">Hurrengo taulan Proiektuaren programazio entitateen zerrenda osoa ematen da.</span><span class="sxs-lookup"><span data-stu-id="44ead-111">The following table provides a full list of the Project schedule entities.</span></span>

| <span data-ttu-id="44ead-112">Entitatearen izena</span><span class="sxs-lookup"><span data-stu-id="44ead-112">Entity name</span></span>  | <span data-ttu-id="44ead-113">Entitatearen izen logikoa</span><span class="sxs-lookup"><span data-stu-id="44ead-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="44ead-114">Project</span><span class="sxs-lookup"><span data-stu-id="44ead-114">Project</span></span> | <span data-ttu-id="44ead-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="44ead-115">msdyn_project</span></span> |
| <span data-ttu-id="44ead-116">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="44ead-116">Project Task</span></span>  | <span data-ttu-id="44ead-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="44ead-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="44ead-118">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="44ead-118">Project Task Dependency</span></span>  | <span data-ttu-id="44ead-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="44ead-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="44ead-120">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="44ead-120">Resource Assignment</span></span> | <span data-ttu-id="44ead-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="44ead-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="44ead-122">Proiektuaren ontzia</span><span class="sxs-lookup"><span data-stu-id="44ead-122">Project Bucket</span></span>  | <span data-ttu-id="44ead-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="44ead-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="44ead-124">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="44ead-124">Project Team Member</span></span> | <span data-ttu-id="44ead-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="44ead-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="44ead-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="44ead-126">OperationSet</span></span>

<span data-ttu-id="44ead-127">OperationSet lan-unitate eredua da, eragiketen eskaerak eragiketen hainbat transakzio baten barruan prozesatu behar direnean erabil daitekeena.</span><span class="sxs-lookup"><span data-stu-id="44ead-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="project-schedule-apis"></a><span data-ttu-id="44ead-128">Proiektuen antolaketa APIak</span><span class="sxs-lookup"><span data-stu-id="44ead-128">Project schedule APIs</span></span>

<span data-ttu-id="44ead-129">Jarraian, proiektuaren antolaketaren APIen zerrenda dago.</span><span class="sxs-lookup"><span data-stu-id="44ead-129">The following is a list of current Project schedule APIs.</span></span>

- <span data-ttu-id="44ead-130">**msdyn_CreateProjectV1**: API hau proiektu bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="44ead-131">Proiektua eta lehenetsitako proiektua berehala sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="44ead-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="44ead-132">**msdyn_CreateTeamMemberV1**: API hau proiektuko taldekide bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="44ead-133">Taldekideen erregistroa berehala sortzen da.</span><span class="sxs-lookup"><span data-stu-id="44ead-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="44ead-134">**msdyn_CreateOperationSetV1**: API hau transakzio baten barruan egin behar diren hainbat eskaera antolatzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="44ead-135">**msdyn_PSSCreateV1**: API hau entitate bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="44ead-136">Erakundea sortzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-136">The entity can be any of the Project scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="44ead-137">**msdyn_PSSUpdateV1**: API hau entitate bat eguneratzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="44ead-138">Erakundea eguneratzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-138">The entity can be any of the Project scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="44ead-139">**msdyn_PSSDeleteV1**: API hau entitate bat ezabatzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="44ead-140">Erakundea ezabatzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-140">The entity can be any of the Project scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="44ead-141">**msdyn_ExecuteOperationSetV1** : API hau emandako eragiketa multzoaren barneko eragiketa guztiak exekutatzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="44ead-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-project-schedule-apis-with-operationset"></a><span data-ttu-id="44ead-142">ProjectSet programarekin APIak erabiltzea OperationSet-ekin</span><span class="sxs-lookup"><span data-stu-id="44ead-142">Using Project schedule APIs with OperationSet</span></span>

<span data-ttu-id="44ead-143">Biekin grabatzen delako **CreateProjectV1** eta **CreateTeamMemberV1** berehala sortzen dira, API horiek ezin dira **OperationSet** zuzenean.</span><span class="sxs-lookup"><span data-stu-id="44ead-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="44ead-144">Hala ere, APIa erabil dezakezu beharrezko erregistroak sortzeko **OperationSet**, eta ondoren erabili aurrez sortutako erregistro hauek **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="44ead-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="44ead-145">Onartutako eragiketak</span><span class="sxs-lookup"><span data-stu-id="44ead-145">Supported operations</span></span>

| <span data-ttu-id="44ead-146">Antolaketa-entitatea</span><span class="sxs-lookup"><span data-stu-id="44ead-146">Scheduling entity</span></span> | <span data-ttu-id="44ead-147">Sortu</span><span class="sxs-lookup"><span data-stu-id="44ead-147">Create</span></span> | <span data-ttu-id="44ead-148">Eguneratzea</span><span class="sxs-lookup"><span data-stu-id="44ead-148">Update</span></span> | <span data-ttu-id="44ead-149">Ezabatu</span><span class="sxs-lookup"><span data-stu-id="44ead-149">Delete</span></span> | <span data-ttu-id="44ead-150">Gogoeta garrantzitsuak</span><span class="sxs-lookup"><span data-stu-id="44ead-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="44ead-151">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="44ead-151">Project task</span></span> | <span data-ttu-id="44ead-152">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-152">Yes</span></span> | <span data-ttu-id="44ead-153">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-153">Yes</span></span> | <span data-ttu-id="44ead-154">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-154">Yes</span></span> | <span data-ttu-id="44ead-155">None</span><span class="sxs-lookup"><span data-stu-id="44ead-155">None</span></span> |
| <span data-ttu-id="44ead-156">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="44ead-156">Project task dependency</span></span> | <span data-ttu-id="44ead-157">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-157">Yes</span></span> | <span data-ttu-id="44ead-158">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-158">Yes</span></span> | | <span data-ttu-id="44ead-159">Proiektuaren zereginen mendekotasun erregistroak ez dira eguneratu.</span><span class="sxs-lookup"><span data-stu-id="44ead-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="44ead-160">Horren ordez, erregistro zahar bat ezabatu eta erregistro berri bat sor daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="44ead-161">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="44ead-161">Resource assignment</span></span> | <span data-ttu-id="44ead-162">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-162">Yes</span></span> | <span data-ttu-id="44ead-163">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-163">Yes</span></span> | | <span data-ttu-id="44ead-164">Ez dira onartzen eremu hauek dituzten eragiketak: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** eta **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="44ead-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="44ead-165">Baliabideak esleitzeko erregistroak ez dira eguneratu.</span><span class="sxs-lookup"><span data-stu-id="44ead-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="44ead-166">Horren ordez, erregistro zaharra ezabatu eta erregistro berri bat sor daiteke.</span><span class="sxs-lookup"><span data-stu-id="44ead-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="44ead-167">Proiektuaren ontzia</span><span class="sxs-lookup"><span data-stu-id="44ead-167">Project bucket</span></span> | <span data-ttu-id="44ead-168">E/E</span><span class="sxs-lookup"><span data-stu-id="44ead-168">N/A</span></span> | <span data-ttu-id="44ead-169">E/E</span><span class="sxs-lookup"><span data-stu-id="44ead-169">N/A</span></span> | <span data-ttu-id="44ead-170">E/E</span><span class="sxs-lookup"><span data-stu-id="44ead-170">N/A</span></span> | <span data-ttu-id="44ead-171">Lehenetsitako ontzia fitxategia erabiliz sortzen da **CreateProjectV1** APIa.</span><span class="sxs-lookup"><span data-stu-id="44ead-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="44ead-172">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="44ead-172">Project team member</span></span> | <span data-ttu-id="44ead-173">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-173">Yes</span></span> | <span data-ttu-id="44ead-174">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-174">Yes</span></span> | <span data-ttu-id="44ead-175">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-175">Yes</span></span> | <span data-ttu-id="44ead-176">Eragiketa sortzeko, erabili **CreateTeamMemberV1** APIa.</span><span class="sxs-lookup"><span data-stu-id="44ead-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="44ead-177">Project</span><span class="sxs-lookup"><span data-stu-id="44ead-177">Project</span></span> | <span data-ttu-id="44ead-178">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-178">Yes</span></span> | <span data-ttu-id="44ead-179">Yes</span><span class="sxs-lookup"><span data-stu-id="44ead-179">Yes</span></span> | <span data-ttu-id="44ead-180">E/E</span><span class="sxs-lookup"><span data-stu-id="44ead-180">N/A</span></span> | <span data-ttu-id="44ead-181">Ez dira onartzen eremu hauek dituzten eragiketak: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** eta **Duration**.</span><span class="sxs-lookup"><span data-stu-id="44ead-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="44ead-182">API hauek eremu pertsonalizatuak dituzten entitate objektuekin dei daitezke.</span><span class="sxs-lookup"><span data-stu-id="44ead-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="44ead-183">Identifikazio propietatea aukerakoa da.</span><span class="sxs-lookup"><span data-stu-id="44ead-183">The ID property is optional.</span></span> <span data-ttu-id="44ead-184">Ematen bada, sistema erabiltzen saiatzen da eta salbuespen bat botatzen du ezin bada erabili.</span><span class="sxs-lookup"><span data-stu-id="44ead-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="44ead-185">Ematen ez bada, sistemak sortuko du.</span><span class="sxs-lookup"><span data-stu-id="44ead-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="44ead-186">Eremu mugatuak</span><span class="sxs-lookup"><span data-stu-id="44ead-186">Restricted fields</span></span>

<span data-ttu-id="44ead-187">Ondorengo tauletan mugatuta dauden eremuak zehazten dira **Sortu** eta **Editatu**.</span><span class="sxs-lookup"><span data-stu-id="44ead-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="44ead-188">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="44ead-188">Project task</span></span>

| <span data-ttu-id="44ead-189">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="44ead-189">**Logical name**</span></span>                       | <span data-ttu-id="44ead-190">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="44ead-190">**Can create**</span></span> | <span data-ttu-id="44ead-191">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="44ead-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="44ead-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="44ead-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="44ead-193">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-193">no</span></span>             | <span data-ttu-id="44ead-194">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-194">no</span></span>               |
| <span data-ttu-id="44ead-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="44ead-196">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-196">no</span></span>             | <span data-ttu-id="44ead-197">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-197">no</span></span>               |
| <span data-ttu-id="44ead-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="44ead-198">msdyn_actualend</span></span>                        | <span data-ttu-id="44ead-199">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-199">no</span></span>             | <span data-ttu-id="44ead-200">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-200">no</span></span>               |
| <span data-ttu-id="44ead-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="44ead-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="44ead-202">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-202">no</span></span>             | <span data-ttu-id="44ead-203">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-203">no</span></span>               |
| <span data-ttu-id="44ead-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="44ead-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="44ead-205">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-205">no</span></span>             | <span data-ttu-id="44ead-206">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-206">no</span></span>               |
| <span data-ttu-id="44ead-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="44ead-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="44ead-208">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-208">no</span></span>             | <span data-ttu-id="44ead-209">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-209">no</span></span>               |
| <span data-ttu-id="44ead-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="44ead-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="44ead-211">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-211">no</span></span>             | <span data-ttu-id="44ead-212">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-212">no</span></span>               |
| <span data-ttu-id="44ead-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="44ead-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="44ead-214">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-214">no</span></span>             | <span data-ttu-id="44ead-215">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-215">no</span></span>               |
| <span data-ttu-id="44ead-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="44ead-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="44ead-217">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-217">no</span></span>             | <span data-ttu-id="44ead-218">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-218">no</span></span>               |
| <span data-ttu-id="44ead-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="44ead-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="44ead-220">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-220">no</span></span>             | <span data-ttu-id="44ead-221">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-221">no</span></span>               |
| <span data-ttu-id="44ead-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="44ead-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="44ead-223">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-223">no</span></span>             | <span data-ttu-id="44ead-224">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-224">no</span></span>               |
| <span data-ttu-id="44ead-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="44ead-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="44ead-226">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-226">no</span></span>             | <span data-ttu-id="44ead-227">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-227">no</span></span>               |
| <span data-ttu-id="44ead-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="44ead-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="44ead-229">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-229">no</span></span>             | <span data-ttu-id="44ead-230">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-230">no</span></span>               |
| <span data-ttu-id="44ead-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="44ead-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="44ead-232">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-232">no</span></span>             | <span data-ttu-id="44ead-233">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-233">no</span></span>               |
| <span data-ttu-id="44ead-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="44ead-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="44ead-235">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-235">no</span></span>             | <span data-ttu-id="44ead-236">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-236">no</span></span>               |
| <span data-ttu-id="44ead-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="44ead-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="44ead-238">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-238">no</span></span>             | <span data-ttu-id="44ead-239">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-239">no</span></span>               |
| <span data-ttu-id="44ead-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="44ead-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="44ead-241">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-241">no</span></span>             | <span data-ttu-id="44ead-242">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-242">no</span></span>               |
| <span data-ttu-id="44ead-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="44ead-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="44ead-244">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-244">no</span></span>             | <span data-ttu-id="44ead-245">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-245">no</span></span>               |
| <span data-ttu-id="44ead-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="44ead-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="44ead-247">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-247">no</span></span>             | <span data-ttu-id="44ead-248">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-248">no</span></span>               |
| <span data-ttu-id="44ead-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="44ead-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="44ead-250">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-250">no</span></span>             | <span data-ttu-id="44ead-251">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-251">no</span></span>               |
| <span data-ttu-id="44ead-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="44ead-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="44ead-253">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-253">no</span></span>             | <span data-ttu-id="44ead-254">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-254">no</span></span>               |
| <span data-ttu-id="44ead-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="44ead-256">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-256">no</span></span>             | <span data-ttu-id="44ead-257">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-257">no</span></span>               |
| <span data-ttu-id="44ead-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="44ead-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="44ead-259">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-259">no</span></span>             | <span data-ttu-id="44ead-260">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-260">no</span></span>               |
| <span data-ttu-id="44ead-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="44ead-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="44ead-262">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-262">no</span></span>             | <span data-ttu-id="44ead-263">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-263">no</span></span>               |
| <span data-ttu-id="44ead-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="44ead-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="44ead-265">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-265">no</span></span>             | <span data-ttu-id="44ead-266">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-266">no</span></span>               |
| <span data-ttu-id="44ead-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="44ead-267">msdyn_progress</span></span>                         | <span data-ttu-id="44ead-268">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-268">no</span></span>             | <span data-ttu-id="44ead-269">ez (bai P4W-rako)</span><span class="sxs-lookup"><span data-stu-id="44ead-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="44ead-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="44ead-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="44ead-271">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-271">no</span></span>             | <span data-ttu-id="44ead-272">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-272">no</span></span>               |
| <span data-ttu-id="44ead-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="44ead-274">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-274">no</span></span>             | <span data-ttu-id="44ead-275">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-275">no</span></span>               |
| <span data-ttu-id="44ead-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="44ead-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="44ead-277">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-277">no</span></span>             | <span data-ttu-id="44ead-278">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-278">no</span></span>               |
| <span data-ttu-id="44ead-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="44ead-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="44ead-280">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-280">no</span></span>             | <span data-ttu-id="44ead-281">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-281">no</span></span>               |
| <span data-ttu-id="44ead-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="44ead-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="44ead-283">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-283">no</span></span>             | <span data-ttu-id="44ead-284">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-284">no</span></span>               |
| <span data-ttu-id="44ead-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="44ead-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="44ead-286">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-286">no</span></span>             | <span data-ttu-id="44ead-287">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-287">no</span></span>               |
| <span data-ttu-id="44ead-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="44ead-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="44ead-289">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-289">no</span></span>             | <span data-ttu-id="44ead-290">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-290">no</span></span>               |
| <span data-ttu-id="44ead-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="44ead-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="44ead-292">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-292">no</span></span>             | <span data-ttu-id="44ead-293">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-293">no</span></span>               |
| <span data-ttu-id="44ead-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="44ead-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="44ead-295">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-295">no</span></span>             | <span data-ttu-id="44ead-296">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-296">no</span></span>               |
| <span data-ttu-id="44ead-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="44ead-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="44ead-298">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-298">no</span></span>             | <span data-ttu-id="44ead-299">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-299">no</span></span>               |
| <span data-ttu-id="44ead-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="44ead-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="44ead-301">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-301">no</span></span>             | <span data-ttu-id="44ead-302">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-302">no</span></span>               |
| <span data-ttu-id="44ead-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="44ead-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="44ead-304">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-304">no</span></span>             | <span data-ttu-id="44ead-305">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-305">no</span></span>               |
| <span data-ttu-id="44ead-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="44ead-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="44ead-307">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-307">no</span></span>             | <span data-ttu-id="44ead-308">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-308">no</span></span>               |
| <span data-ttu-id="44ead-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="44ead-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="44ead-310">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-310">no</span></span>             | <span data-ttu-id="44ead-311">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-311">no</span></span>               |
| <span data-ttu-id="44ead-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="44ead-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="44ead-313">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-313">no</span></span>             | <span data-ttu-id="44ead-314">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-314">no</span></span>               |
| <span data-ttu-id="44ead-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="44ead-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="44ead-316">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-316">no</span></span>             | <span data-ttu-id="44ead-317">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-317">no</span></span>               |
| <span data-ttu-id="44ead-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="44ead-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="44ead-319">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-319">no</span></span>             | <span data-ttu-id="44ead-320">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-320">no</span></span>               |
| <span data-ttu-id="44ead-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="44ead-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="44ead-322">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-322">no</span></span>             | <span data-ttu-id="44ead-323">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-323">no</span></span>               |
| <span data-ttu-id="44ead-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="44ead-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="44ead-325">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-325">no</span></span>             | <span data-ttu-id="44ead-326">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-326">no</span></span>               |
| <span data-ttu-id="44ead-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="44ead-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="44ead-328">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-328">no</span></span>             | <span data-ttu-id="44ead-329">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-329">no</span></span>               |
| <span data-ttu-id="44ead-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="44ead-330">msdyn_summary</span></span>                          | <span data-ttu-id="44ead-331">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-331">no</span></span>             | <span data-ttu-id="44ead-332">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-332">no</span></span>               |
| <span data-ttu-id="44ead-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="44ead-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="44ead-334">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-334">no</span></span>             | <span data-ttu-id="44ead-335">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-335">no</span></span>               |
| <span data-ttu-id="44ead-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="44ead-337">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-337">no</span></span>             | <span data-ttu-id="44ead-338">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="44ead-339">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="44ead-339">Project task dependency</span></span>

| <span data-ttu-id="44ead-340">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="44ead-340">**Logical name**</span></span>              | <span data-ttu-id="44ead-341">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="44ead-341">**Can create**</span></span> | <span data-ttu-id="44ead-342">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="44ead-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="44ead-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="44ead-343">msdyn_linktype</span></span>                | <span data-ttu-id="44ead-344">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-344">no</span></span>             | <span data-ttu-id="44ead-345">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-345">no</span></span>           |
| <span data-ttu-id="44ead-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="44ead-346">msdyn_linktypename</span></span>            | <span data-ttu-id="44ead-347">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-347">no</span></span>             | <span data-ttu-id="44ead-348">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-348">no</span></span>           |
| <span data-ttu-id="44ead-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="44ead-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="44ead-350">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-350">yes</span></span>            | <span data-ttu-id="44ead-351">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-351">no</span></span>           |
| <span data-ttu-id="44ead-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="44ead-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="44ead-353">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-353">yes</span></span>            | <span data-ttu-id="44ead-354">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-354">no</span></span>           |
| <span data-ttu-id="44ead-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="44ead-355">msdyn_project</span></span>                 | <span data-ttu-id="44ead-356">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-356">yes</span></span>            | <span data-ttu-id="44ead-357">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-357">no</span></span>           |
| <span data-ttu-id="44ead-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="44ead-358">msdyn_projectname</span></span>             | <span data-ttu-id="44ead-359">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-359">yes</span></span>            | <span data-ttu-id="44ead-360">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-360">no</span></span>           |
| <span data-ttu-id="44ead-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="44ead-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="44ead-362">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-362">yes</span></span>            | <span data-ttu-id="44ead-363">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-363">no</span></span>           |
| <span data-ttu-id="44ead-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="44ead-364">msdyn_successortask</span></span>           | <span data-ttu-id="44ead-365">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-365">yes</span></span>            | <span data-ttu-id="44ead-366">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-366">no</span></span>           |
| <span data-ttu-id="44ead-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="44ead-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="44ead-368">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-368">yes</span></span>            | <span data-ttu-id="44ead-369">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="44ead-370">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="44ead-370">Resource assignment</span></span>

| <span data-ttu-id="44ead-371">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="44ead-371">**Logical name**</span></span>             | <span data-ttu-id="44ead-372">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="44ead-372">**Can create**</span></span> | <span data-ttu-id="44ead-373">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="44ead-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="44ead-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="44ead-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="44ead-375">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-375">yes</span></span>            | <span data-ttu-id="44ead-376">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-376">no</span></span>           |
| <span data-ttu-id="44ead-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="44ead-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="44ead-378">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-378">yes</span></span>            | <span data-ttu-id="44ead-379">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-379">no</span></span>           |
| <span data-ttu-id="44ead-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="44ead-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="44ead-381">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-381">no</span></span>             | <span data-ttu-id="44ead-382">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-382">no</span></span>           |
| <span data-ttu-id="44ead-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="44ead-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="44ead-384">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-384">no</span></span>             | <span data-ttu-id="44ead-385">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-385">no</span></span>           |
| <span data-ttu-id="44ead-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="44ead-386">msdyn_committype</span></span>             | <span data-ttu-id="44ead-387">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-387">no</span></span>             | <span data-ttu-id="44ead-388">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-388">no</span></span>           |
| <span data-ttu-id="44ead-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="44ead-389">msdyn_committypename</span></span>         | <span data-ttu-id="44ead-390">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-390">no</span></span>             | <span data-ttu-id="44ead-391">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-391">no</span></span>           |
| <span data-ttu-id="44ead-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="44ead-392">msdyn_effort</span></span>                 | <span data-ttu-id="44ead-393">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-393">no</span></span>             | <span data-ttu-id="44ead-394">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-394">no</span></span>           |
| <span data-ttu-id="44ead-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="44ead-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="44ead-396">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-396">no</span></span>             | <span data-ttu-id="44ead-397">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-397">no</span></span>           |
| <span data-ttu-id="44ead-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="44ead-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="44ead-399">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-399">no</span></span>             | <span data-ttu-id="44ead-400">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-400">no</span></span>           |
| <span data-ttu-id="44ead-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="44ead-401">msdyn_finish</span></span>                 | <span data-ttu-id="44ead-402">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-402">no</span></span>             | <span data-ttu-id="44ead-403">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-403">no</span></span>           |
| <span data-ttu-id="44ead-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="44ead-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="44ead-405">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-405">no</span></span>             | <span data-ttu-id="44ead-406">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-406">no</span></span>           |
| <span data-ttu-id="44ead-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="44ead-408">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-408">no</span></span>             | <span data-ttu-id="44ead-409">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-409">no</span></span>           |
| <span data-ttu-id="44ead-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="44ead-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="44ead-411">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-411">no</span></span>             | <span data-ttu-id="44ead-412">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-412">no</span></span>           |
| <span data-ttu-id="44ead-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="44ead-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="44ead-414">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-414">no</span></span>             | <span data-ttu-id="44ead-415">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-415">no</span></span>           |
| <span data-ttu-id="44ead-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="44ead-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="44ead-417">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-417">no</span></span>             | <span data-ttu-id="44ead-418">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-418">no</span></span>           |
| <span data-ttu-id="44ead-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="44ead-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="44ead-420">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-420">no</span></span>             | <span data-ttu-id="44ead-421">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-421">no</span></span>           |
| <span data-ttu-id="44ead-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="44ead-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="44ead-423">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-423">no</span></span>             | <span data-ttu-id="44ead-424">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-424">no</span></span>           |
| <span data-ttu-id="44ead-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="44ead-425">msdyn_projectid</span></span>              | <span data-ttu-id="44ead-426">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-426">yes</span></span>            | <span data-ttu-id="44ead-427">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-427">no</span></span>           |
| <span data-ttu-id="44ead-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="44ead-428">msdyn_projectidname</span></span>          | <span data-ttu-id="44ead-429">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-429">no</span></span>             | <span data-ttu-id="44ead-430">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-430">no</span></span>           |
| <span data-ttu-id="44ead-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="44ead-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="44ead-432">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-432">no</span></span>             | <span data-ttu-id="44ead-433">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-433">no</span></span>           |
| <span data-ttu-id="44ead-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="44ead-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="44ead-435">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-435">no</span></span>             | <span data-ttu-id="44ead-436">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-436">no</span></span>           |
| <span data-ttu-id="44ead-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="44ead-437">msdyn_start</span></span>                  | <span data-ttu-id="44ead-438">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-438">no</span></span>             | <span data-ttu-id="44ead-439">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-439">no</span></span>           |
| <span data-ttu-id="44ead-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="44ead-440">msdyn_taskid</span></span>                 | <span data-ttu-id="44ead-441">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-441">no</span></span>             | <span data-ttu-id="44ead-442">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-442">no</span></span>           |
| <span data-ttu-id="44ead-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="44ead-443">msdyn_taskidname</span></span>             | <span data-ttu-id="44ead-444">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-444">no</span></span>             | <span data-ttu-id="44ead-445">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-445">no</span></span>           |
| <span data-ttu-id="44ead-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="44ead-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="44ead-447">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-447">no</span></span>             | <span data-ttu-id="44ead-448">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="44ead-449">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="44ead-449">Project team member</span></span>

| <span data-ttu-id="44ead-450">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="44ead-450">**Logical name**</span></span>                                 | <span data-ttu-id="44ead-451">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="44ead-451">**Can create**</span></span> | <span data-ttu-id="44ead-452">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="44ead-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="44ead-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="44ead-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="44ead-454">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-454">no</span></span>             | <span data-ttu-id="44ead-455">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-455">no</span></span>           |
| <span data-ttu-id="44ead-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="44ead-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="44ead-457">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-457">no</span></span>             | <span data-ttu-id="44ead-458">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-458">no</span></span>           |
| <span data-ttu-id="44ead-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="44ead-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="44ead-460">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-460">no</span></span>             | <span data-ttu-id="44ead-461">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-461">no</span></span>           |
| <span data-ttu-id="44ead-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="44ead-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="44ead-463">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-463">no</span></span>             | <span data-ttu-id="44ead-464">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-464">no</span></span>           |
| <span data-ttu-id="44ead-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="44ead-465">msdyn_effort</span></span>                                     | <span data-ttu-id="44ead-466">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-466">no</span></span>             | <span data-ttu-id="44ead-467">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-467">no</span></span>           |
| <span data-ttu-id="44ead-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="44ead-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="44ead-469">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-469">no</span></span>             | <span data-ttu-id="44ead-470">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-470">no</span></span>           |
| <span data-ttu-id="44ead-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="44ead-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="44ead-472">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-472">no</span></span>             | <span data-ttu-id="44ead-473">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-473">no</span></span>           |
| <span data-ttu-id="44ead-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="44ead-474">msdyn_finish</span></span>                                     | <span data-ttu-id="44ead-475">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-475">no</span></span>             | <span data-ttu-id="44ead-476">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-476">no</span></span>           |
| <span data-ttu-id="44ead-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="44ead-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="44ead-478">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-478">no</span></span>             | <span data-ttu-id="44ead-479">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-479">no</span></span>           |
| <span data-ttu-id="44ead-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="44ead-480">msdyn_hours</span></span>                                      | <span data-ttu-id="44ead-481">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-481">no</span></span>             | <span data-ttu-id="44ead-482">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-482">no</span></span>           |
| <span data-ttu-id="44ead-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="44ead-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="44ead-484">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-484">no</span></span>             | <span data-ttu-id="44ead-485">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-485">no</span></span>           |
| <span data-ttu-id="44ead-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="44ead-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="44ead-487">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-487">no</span></span>             | <span data-ttu-id="44ead-488">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-488">no</span></span>           |
| <span data-ttu-id="44ead-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="44ead-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="44ead-490">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-490">no</span></span>             | <span data-ttu-id="44ead-491">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-491">no</span></span>           |
| <span data-ttu-id="44ead-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="44ead-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="44ead-493">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-493">no</span></span>             | <span data-ttu-id="44ead-494">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-494">no</span></span>           |
| <span data-ttu-id="44ead-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="44ead-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="44ead-496">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-496">no</span></span>             | <span data-ttu-id="44ead-497">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-497">no</span></span>           |
| <span data-ttu-id="44ead-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="44ead-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="44ead-499">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-499">no</span></span>             | <span data-ttu-id="44ead-500">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-500">no</span></span>           |
| <span data-ttu-id="44ead-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="44ead-501">msdyn_start</span></span>                                      | <span data-ttu-id="44ead-502">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-502">no</span></span>             | <span data-ttu-id="44ead-503">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="44ead-504">Project</span><span class="sxs-lookup"><span data-stu-id="44ead-504">Project</span></span>

| <span data-ttu-id="44ead-505">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="44ead-505">**Logical name**</span></span>                       | <span data-ttu-id="44ead-506">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="44ead-506">**Can create**</span></span> | <span data-ttu-id="44ead-507">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="44ead-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="44ead-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="44ead-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="44ead-509">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-509">no</span></span>             | <span data-ttu-id="44ead-510">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-510">no</span></span>           |
| <span data-ttu-id="44ead-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="44ead-512">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-512">no</span></span>             | <span data-ttu-id="44ead-513">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-513">no</span></span>           |
| <span data-ttu-id="44ead-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="44ead-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="44ead-515">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-515">no</span></span>             | <span data-ttu-id="44ead-516">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-516">no</span></span>           |
| <span data-ttu-id="44ead-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="44ead-518">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-518">no</span></span>             | <span data-ttu-id="44ead-519">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-519">no</span></span>           |
| <span data-ttu-id="44ead-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="44ead-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="44ead-521">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-521">no</span></span>             | <span data-ttu-id="44ead-522">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-522">no</span></span>           |
| <span data-ttu-id="44ead-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="44ead-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="44ead-524">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-524">no</span></span>             | <span data-ttu-id="44ead-525">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-525">no</span></span>           |
| <span data-ttu-id="44ead-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="44ead-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="44ead-527">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-527">yes</span></span>            | <span data-ttu-id="44ead-528">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-528">no</span></span>           |
| <span data-ttu-id="44ead-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="44ead-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="44ead-530">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-530">yes</span></span>            | <span data-ttu-id="44ead-531">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-531">no</span></span>           |
| <span data-ttu-id="44ead-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="44ead-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="44ead-533">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-533">yes</span></span>            | <span data-ttu-id="44ead-534">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-534">no</span></span>           |
| <span data-ttu-id="44ead-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="44ead-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="44ead-536">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-536">no</span></span>             | <span data-ttu-id="44ead-537">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-537">no</span></span>           |
| <span data-ttu-id="44ead-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="44ead-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="44ead-539">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-539">no</span></span>             | <span data-ttu-id="44ead-540">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-540">no</span></span>           |
| <span data-ttu-id="44ead-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="44ead-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="44ead-542">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-542">no</span></span>             | <span data-ttu-id="44ead-543">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-543">no</span></span>           |
| <span data-ttu-id="44ead-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="44ead-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="44ead-545">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-545">no</span></span>             | <span data-ttu-id="44ead-546">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-546">no</span></span>           |
| <span data-ttu-id="44ead-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="44ead-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="44ead-548">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-548">no</span></span>             | <span data-ttu-id="44ead-549">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-549">no</span></span>           |
| <span data-ttu-id="44ead-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="44ead-550">msdyn_duration</span></span>                         | <span data-ttu-id="44ead-551">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-551">no</span></span>             | <span data-ttu-id="44ead-552">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-552">no</span></span>           |
| <span data-ttu-id="44ead-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="44ead-553">msdyn_effort</span></span>                           | <span data-ttu-id="44ead-554">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-554">no</span></span>             | <span data-ttu-id="44ead-555">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-555">no</span></span>           |
| <span data-ttu-id="44ead-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="44ead-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="44ead-557">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-557">no</span></span>             | <span data-ttu-id="44ead-558">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-558">no</span></span>           |
| <span data-ttu-id="44ead-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="44ead-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="44ead-560">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-560">no</span></span>             | <span data-ttu-id="44ead-561">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-561">no</span></span>           |
| <span data-ttu-id="44ead-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="44ead-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="44ead-563">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-563">no</span></span>             | <span data-ttu-id="44ead-564">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-564">no</span></span>           |
| <span data-ttu-id="44ead-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="44ead-565">msdyn_finish</span></span>                           | <span data-ttu-id="44ead-566">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-566">yes</span></span>            | <span data-ttu-id="44ead-567">bai</span><span class="sxs-lookup"><span data-stu-id="44ead-567">yes</span></span>          |
| <span data-ttu-id="44ead-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="44ead-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="44ead-569">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-569">no</span></span>             | <span data-ttu-id="44ead-570">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-570">no</span></span>           |
| <span data-ttu-id="44ead-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="44ead-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="44ead-572">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-572">no</span></span>             | <span data-ttu-id="44ead-573">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-573">no</span></span>           |
| <span data-ttu-id="44ead-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="44ead-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="44ead-575">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-575">no</span></span>             | <span data-ttu-id="44ead-576">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-576">no</span></span>           |
| <span data-ttu-id="44ead-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="44ead-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="44ead-578">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-578">no</span></span>             | <span data-ttu-id="44ead-579">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-579">no</span></span>           |
| <span data-ttu-id="44ead-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="44ead-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="44ead-581">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-581">no</span></span>             | <span data-ttu-id="44ead-582">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-582">no</span></span>           |
| <span data-ttu-id="44ead-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="44ead-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="44ead-584">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-584">no</span></span>             | <span data-ttu-id="44ead-585">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-585">no</span></span>           |
| <span data-ttu-id="44ead-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="44ead-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="44ead-587">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-587">no</span></span>             | <span data-ttu-id="44ead-588">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-588">no</span></span>           |
| <span data-ttu-id="44ead-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="44ead-590">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-590">no</span></span>             | <span data-ttu-id="44ead-591">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-591">no</span></span>           |
| <span data-ttu-id="44ead-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="44ead-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="44ead-593">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-593">no</span></span>             | <span data-ttu-id="44ead-594">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-594">no</span></span>           |
| <span data-ttu-id="44ead-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="44ead-596">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-596">no</span></span>             | <span data-ttu-id="44ead-597">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-597">no</span></span>           |
| <span data-ttu-id="44ead-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="44ead-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="44ead-599">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-599">no</span></span>             | <span data-ttu-id="44ead-600">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-600">no</span></span>           |
| <span data-ttu-id="44ead-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="44ead-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="44ead-602">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-602">no</span></span>             | <span data-ttu-id="44ead-603">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-603">no</span></span>           |
| <span data-ttu-id="44ead-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="44ead-604">msdyn_progress</span></span>                         | <span data-ttu-id="44ead-605">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-605">no</span></span>             | <span data-ttu-id="44ead-606">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-606">no</span></span>           |
| <span data-ttu-id="44ead-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="44ead-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="44ead-608">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-608">no</span></span>             | <span data-ttu-id="44ead-609">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-609">no</span></span>           |
| <span data-ttu-id="44ead-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="44ead-611">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-611">no</span></span>             | <span data-ttu-id="44ead-612">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-612">no</span></span>           |
| <span data-ttu-id="44ead-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="44ead-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="44ead-614">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-614">no</span></span>             | <span data-ttu-id="44ead-615">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-615">no</span></span>           |
| <span data-ttu-id="44ead-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="44ead-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="44ead-617">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-617">no</span></span>             | <span data-ttu-id="44ead-618">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-618">no</span></span>           |
| <span data-ttu-id="44ead-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="44ead-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="44ead-620">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-620">no</span></span>             | <span data-ttu-id="44ead-621">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-621">no</span></span>           |
| <span data-ttu-id="44ead-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="44ead-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="44ead-623">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-623">no</span></span>             | <span data-ttu-id="44ead-624">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-624">no</span></span>           |
| <span data-ttu-id="44ead-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="44ead-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="44ead-626">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-626">no</span></span>             | <span data-ttu-id="44ead-627">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-627">no</span></span>           |
| <span data-ttu-id="44ead-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="44ead-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="44ead-629">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-629">no</span></span>             | <span data-ttu-id="44ead-630">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-630">no</span></span>           |
| <span data-ttu-id="44ead-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="44ead-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="44ead-632">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-632">no</span></span>             | <span data-ttu-id="44ead-633">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-633">no</span></span>           |
| <span data-ttu-id="44ead-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="44ead-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="44ead-635">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-635">no</span></span>             | <span data-ttu-id="44ead-636">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-636">no</span></span>           |
| <span data-ttu-id="44ead-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="44ead-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="44ead-638">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-638">no</span></span>             | <span data-ttu-id="44ead-639">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-639">no</span></span>           |
| <span data-ttu-id="44ead-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="44ead-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="44ead-641">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-641">no</span></span>             | <span data-ttu-id="44ead-642">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-642">no</span></span>           |
| <span data-ttu-id="44ead-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="44ead-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="44ead-644">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-644">no</span></span>             | <span data-ttu-id="44ead-645">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-645">no</span></span>           |
| <span data-ttu-id="44ead-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="44ead-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="44ead-647">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-647">no</span></span>             | <span data-ttu-id="44ead-648">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-648">no</span></span>           |
| <span data-ttu-id="44ead-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="44ead-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="44ead-650">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-650">no</span></span>             | <span data-ttu-id="44ead-651">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-651">no</span></span>           |
| <span data-ttu-id="44ead-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="44ead-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="44ead-653">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-653">no</span></span>             | <span data-ttu-id="44ead-654">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-654">no</span></span>           |
| <span data-ttu-id="44ead-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="44ead-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="44ead-656">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-656">no</span></span>             | <span data-ttu-id="44ead-657">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-657">no</span></span>           |
| <span data-ttu-id="44ead-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="44ead-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="44ead-659">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-659">no</span></span>             | <span data-ttu-id="44ead-660">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-660">no</span></span>           |
| <span data-ttu-id="44ead-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="44ead-662">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-662">no</span></span>             | <span data-ttu-id="44ead-663">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-663">no</span></span>           |
| <span data-ttu-id="44ead-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="44ead-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="44ead-665">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-665">no</span></span>             | <span data-ttu-id="44ead-666">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-666">no</span></span>           |
| <span data-ttu-id="44ead-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="44ead-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="44ead-668">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-668">no</span></span>             | <span data-ttu-id="44ead-669">ez</span><span class="sxs-lookup"><span data-stu-id="44ead-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="44ead-670">Mugak eta arazo ezagunak</span><span class="sxs-lookup"><span data-stu-id="44ead-670">Limitations and known issues</span></span>
<span data-ttu-id="44ead-671">Jarraian agertzen diren mugen eta arazo ezagunen zerrenda:</span><span class="sxs-lookup"><span data-stu-id="44ead-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="44ead-672">Project Schedule APIak soilik erabil ditzake **Microsoft Project lizentzia duten erabiltzaileek.**</span><span class="sxs-lookup"><span data-stu-id="44ead-672">Project Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="44ead-673">Ezin dute hauek erabili:</span><span class="sxs-lookup"><span data-stu-id="44ead-673">They can't be used by:</span></span>
    - <span data-ttu-id="44ead-674">Aplikazioaren erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="44ead-674">Application users</span></span>
    - <span data-ttu-id="44ead-675">Sistema-erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="44ead-675">System users</span></span>
    - <span data-ttu-id="44ead-676">Integrazio-erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="44ead-676">Integration users</span></span>
    - <span data-ttu-id="44ead-677">Beharrezko lizentzia ez duten beste erabiltzaile batzuk</span><span class="sxs-lookup"><span data-stu-id="44ead-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="44ead-678">**OperationSet** bakoitzak gehienez 100 eragiketa egin ditzake.</span><span class="sxs-lookup"><span data-stu-id="44ead-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="44ead-679">Erabiltzaile bakoitzak gehienez 10 **OperationSet** ireki eduki ditzake.</span><span class="sxs-lookup"><span data-stu-id="44ead-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="44ead-680">Gaur egun, Project Operations-ek gehienez 500 zeregin onartzen dituzte proiektu batean.</span><span class="sxs-lookup"><span data-stu-id="44ead-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="44ead-681">**OperationSet** hutsegiteen egoera eta hutsegiteen erregistroak ez daude erabilgarri une honetan.</span><span class="sxs-lookup"><span data-stu-id="44ead-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="44ead-682">Proiektuetako eta zereginetako mugak</span><span class="sxs-lookup"><span data-stu-id="44ead-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="44ead-683">Errore-kudeaketa</span><span class="sxs-lookup"><span data-stu-id="44ead-683">Error handling</span></span>

   - <span data-ttu-id="44ead-684">Eragiketa multzoetatik sortutako akatsak berrikusteko, joan **Ezarpenak** \> **Ordutegien integrazioa** \> **Eragiketa multzoak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="44ead-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="44ead-685">Proiektuaren programazio zerbitzutik sortutako akatsak berrikusteko, joan hona: **Ezarpenak** \> **Ordutegien integrazioa** \> **PSS erroreen erregistroak**.</span><span class="sxs-lookup"><span data-stu-id="44ead-685">To review errors generated from the Project schedule Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="44ead-686">Laginaren egoera</span><span class="sxs-lookup"><span data-stu-id="44ead-686">Sample scenario</span></span>

<span data-ttu-id="44ead-687">Eszenatoki honetan, proiektu bat, taldekide bat, lau ataza eta bi baliabide esleipen sortuko dituzu.</span><span class="sxs-lookup"><span data-stu-id="44ead-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="44ead-688">Ondoren, zeregin bat eguneratu, proiektua eguneratu, zeregin bat ezabatu, baliabideen esleipen bat ezabatu eta atazaren mendekotasuna sortuko duzu.</span><span class="sxs-lookup"><span data-stu-id="44ead-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="44ead-689">Lagin osagarriak</span><span class="sxs-lookup"><span data-stu-id="44ead-689">Additional samples</span></span>

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
