---
title: Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko
description: Gai honek Programazioa APIak erabiltzeko informazioa eta laginak eskaintzen ditu.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950789"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="74eef-103">Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko</span><span class="sxs-lookup"><span data-stu-id="74eef-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="74eef-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="74eef-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="74eef-105">Gai honetan zehaztutako funtzionaltasun batzuk edo guztiak erabilgarri dago aurrebista-bertsioaren zati gisa.</span><span class="sxs-lookup"><span data-stu-id="74eef-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="74eef-106">Edukia eta funtzionalitatea aldatu egin daitezke.</span><span class="sxs-lookup"><span data-stu-id="74eef-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="74eef-107">Antolaketa-entitateak</span><span class="sxs-lookup"><span data-stu-id="74eef-107">Scheduling entities</span></span>

<span data-ttu-id="74eef-108">Programatu APIek eragiketak sortu, eguneratu eta ezabatzeko gaitasuna eskaintzen dute **Programazio entitateak**.</span><span class="sxs-lookup"><span data-stu-id="74eef-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="74eef-109">Entitate hauek Project for the Web-en antolaketa-motorearen bidez kudeatzen dira.</span><span class="sxs-lookup"><span data-stu-id="74eef-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="74eef-110">Sortu, eguneratu eta ezabatu eragiketak honekin **Programazio entitateak** lehenago mugatu ziren Dynamics 365 Project Operations oharrak.</span><span class="sxs-lookup"><span data-stu-id="74eef-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="74eef-111">Ondorengo taulan zerrenda oso bat ematen da **Programazio entitateak**.</span><span class="sxs-lookup"><span data-stu-id="74eef-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="74eef-112">Entitatearen izena</span><span class="sxs-lookup"><span data-stu-id="74eef-112">Entity name</span></span>  | <span data-ttu-id="74eef-113">Entitatearen izen logikoa</span><span class="sxs-lookup"><span data-stu-id="74eef-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="74eef-114">Project</span><span class="sxs-lookup"><span data-stu-id="74eef-114">Project</span></span> | <span data-ttu-id="74eef-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="74eef-115">msdyn_project</span></span> |
| <span data-ttu-id="74eef-116">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="74eef-116">Project Task</span></span>  | <span data-ttu-id="74eef-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="74eef-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="74eef-118">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="74eef-118">Project Task Dependency</span></span>  | <span data-ttu-id="74eef-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="74eef-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="74eef-120">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="74eef-120">Resource Assignment</span></span> | <span data-ttu-id="74eef-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="74eef-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="74eef-122">Proiektuaren ontzia</span><span class="sxs-lookup"><span data-stu-id="74eef-122">Project Bucket</span></span>  | <span data-ttu-id="74eef-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="74eef-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="74eef-124">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="74eef-124">Project Team Member</span></span> | <span data-ttu-id="74eef-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="74eef-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="74eef-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="74eef-126">OperationSet</span></span>

<span data-ttu-id="74eef-127">OperationSet lan-unitate eredua da, eragiketen eskaerak eragiketen hainbat transakzio baten barruan prozesatu behar direnean erabil daitekeena.</span><span class="sxs-lookup"><span data-stu-id="74eef-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="74eef-128">Programatu APIak</span><span class="sxs-lookup"><span data-stu-id="74eef-128">Schedule APIs</span></span>

<span data-ttu-id="74eef-129">Jarraian uneko Programazio APIen zerrenda dago.</span><span class="sxs-lookup"><span data-stu-id="74eef-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="74eef-130">**msdyn_CreateProjectV1**: API hau proiektu bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="74eef-131">Proiektua eta lehenetsitako proiektua berehala sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="74eef-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="74eef-132">**msdyn_CreateTeamMemberV1**: API hau proiektuko taldekide bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="74eef-133">Taldekideen erregistroa berehala sortzen da.</span><span class="sxs-lookup"><span data-stu-id="74eef-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="74eef-134">**msdyn_CreateOperationSetV1**: API hau transakzio baten barruan egin behar diren hainbat eskaera antolatzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="74eef-135">**msdyn_PSSCreateV1**: API hau entitate bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="74eef-136">Erakundea sortu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="74eef-137">**msdyn_PSSUpdateV1**: API hau entitate bat eguneratzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="74eef-138">Erakundea eguneratu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="74eef-139">**msdyn_PSSDeleteV1**: API hau entitate bat ezabatzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="74eef-140">Erakundea ezabatu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="74eef-141">**msdyn_ExecuteOperationSetV1** : API hau emandako eragiketa multzoaren barneko eragiketa guztiak exekutatzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="74eef-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="74eef-142">Ordutegi APIak erabiliz OperationSet-ekin</span><span class="sxs-lookup"><span data-stu-id="74eef-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="74eef-143">Biekin grabatzen delako **CreateProjectV1** eta **CreateTeamMemberV1** berehala sortzen dira, API horiek ezin dira **OperationSet** zuzenean.</span><span class="sxs-lookup"><span data-stu-id="74eef-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="74eef-144">Hala ere, APIa erabil dezakezu beharrezko erregistroak sortzeko **OperationSet**, eta ondoren erabili aurrez sortutako erregistro hauek **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="74eef-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="74eef-145">Onartutako eragiketak</span><span class="sxs-lookup"><span data-stu-id="74eef-145">Supported operations</span></span>

| <span data-ttu-id="74eef-146">Antolaketa-entitatea</span><span class="sxs-lookup"><span data-stu-id="74eef-146">Scheduling entity</span></span> | <span data-ttu-id="74eef-147">Sortu</span><span class="sxs-lookup"><span data-stu-id="74eef-147">Create</span></span> | <span data-ttu-id="74eef-148">Eguneratzea</span><span class="sxs-lookup"><span data-stu-id="74eef-148">Update</span></span> | <span data-ttu-id="74eef-149">Ezabatu</span><span class="sxs-lookup"><span data-stu-id="74eef-149">Delete</span></span> | <span data-ttu-id="74eef-150">Gogoeta garrantzitsuak</span><span class="sxs-lookup"><span data-stu-id="74eef-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="74eef-151">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="74eef-151">Project task</span></span> | <span data-ttu-id="74eef-152">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-152">Yes</span></span> | <span data-ttu-id="74eef-153">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-153">Yes</span></span> | <span data-ttu-id="74eef-154">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-154">Yes</span></span> | <span data-ttu-id="74eef-155">None</span><span class="sxs-lookup"><span data-stu-id="74eef-155">None</span></span> |
| <span data-ttu-id="74eef-156">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="74eef-156">Project task dependency</span></span> | <span data-ttu-id="74eef-157">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-157">Yes</span></span> | <span data-ttu-id="74eef-158">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-158">Yes</span></span> | | <span data-ttu-id="74eef-159">Proiektuaren zereginen mendekotasun erregistroak ez dira eguneratu.</span><span class="sxs-lookup"><span data-stu-id="74eef-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="74eef-160">Horren ordez, erregistro zahar bat ezabatu eta erregistro berri bat sor daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="74eef-161">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="74eef-161">Resource assignment</span></span> | <span data-ttu-id="74eef-162">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-162">Yes</span></span> | <span data-ttu-id="74eef-163">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-163">Yes</span></span> | | <span data-ttu-id="74eef-164">Ez dira onartzen eremu hauek dituzten eragiketak: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** eta **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="74eef-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="74eef-165">Baliabideak esleitzeko erregistroak ez dira eguneratu.</span><span class="sxs-lookup"><span data-stu-id="74eef-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="74eef-166">Horren ordez, erregistro zaharra ezabatu eta erregistro berri bat sor daiteke.</span><span class="sxs-lookup"><span data-stu-id="74eef-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="74eef-167">Proiektuaren ontzia</span><span class="sxs-lookup"><span data-stu-id="74eef-167">Project bucket</span></span> | <span data-ttu-id="74eef-168">E/E</span><span class="sxs-lookup"><span data-stu-id="74eef-168">N/A</span></span> | <span data-ttu-id="74eef-169">E/E</span><span class="sxs-lookup"><span data-stu-id="74eef-169">N/A</span></span> | <span data-ttu-id="74eef-170">E/E</span><span class="sxs-lookup"><span data-stu-id="74eef-170">N/A</span></span> | <span data-ttu-id="74eef-171">Lehenetsitako ontzia fitxategia erabiliz sortzen da **CreateProjectV1** APIa.</span><span class="sxs-lookup"><span data-stu-id="74eef-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="74eef-172">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="74eef-172">Project team member</span></span> | <span data-ttu-id="74eef-173">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-173">Yes</span></span> | <span data-ttu-id="74eef-174">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-174">Yes</span></span> | <span data-ttu-id="74eef-175">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-175">Yes</span></span> | <span data-ttu-id="74eef-176">Eragiketa sortzeko, erabili **CreateTeamMemberV1** APIa.</span><span class="sxs-lookup"><span data-stu-id="74eef-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="74eef-177">Project</span><span class="sxs-lookup"><span data-stu-id="74eef-177">Project</span></span> | <span data-ttu-id="74eef-178">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-178">Yes</span></span> | <span data-ttu-id="74eef-179">Yes</span><span class="sxs-lookup"><span data-stu-id="74eef-179">Yes</span></span> | <span data-ttu-id="74eef-180">E/E</span><span class="sxs-lookup"><span data-stu-id="74eef-180">N/A</span></span> | <span data-ttu-id="74eef-181">Ez dira onartzen eremu hauek dituzten eragiketak: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** eta **Duration**.</span><span class="sxs-lookup"><span data-stu-id="74eef-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="74eef-182">API hauek eremu pertsonalizatuak dituzten entitate objektuekin dei daitezke.</span><span class="sxs-lookup"><span data-stu-id="74eef-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="74eef-183">Identifikazio propietatea aukerakoa da.</span><span class="sxs-lookup"><span data-stu-id="74eef-183">The ID property is optional.</span></span> <span data-ttu-id="74eef-184">Ematen bada, sistema erabiltzen saiatzen da eta salbuespen bat botatzen du ezin bada erabili.</span><span class="sxs-lookup"><span data-stu-id="74eef-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="74eef-185">Ematen ez bada, sistemak sortuko du.</span><span class="sxs-lookup"><span data-stu-id="74eef-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="74eef-186">Eremu mugatuak</span><span class="sxs-lookup"><span data-stu-id="74eef-186">Restricted fields</span></span>

<span data-ttu-id="74eef-187">Ondorengo tauletan mugatuta dauden eremuak zehazten dira **Sortu** eta **Editatu**.</span><span class="sxs-lookup"><span data-stu-id="74eef-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="74eef-188">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="74eef-188">Project task</span></span>

| <span data-ttu-id="74eef-189">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="74eef-189">**Logical name**</span></span>                       | <span data-ttu-id="74eef-190">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="74eef-190">**Can create**</span></span> | <span data-ttu-id="74eef-191">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="74eef-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="74eef-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="74eef-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="74eef-193">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-193">no</span></span>             | <span data-ttu-id="74eef-194">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-194">no</span></span>               |
| <span data-ttu-id="74eef-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="74eef-196">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-196">no</span></span>             | <span data-ttu-id="74eef-197">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-197">no</span></span>               |
| <span data-ttu-id="74eef-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="74eef-198">msdyn_actualend</span></span>                        | <span data-ttu-id="74eef-199">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-199">no</span></span>             | <span data-ttu-id="74eef-200">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-200">no</span></span>               |
| <span data-ttu-id="74eef-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="74eef-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="74eef-202">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-202">no</span></span>             | <span data-ttu-id="74eef-203">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-203">no</span></span>               |
| <span data-ttu-id="74eef-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="74eef-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="74eef-205">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-205">no</span></span>             | <span data-ttu-id="74eef-206">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-206">no</span></span>               |
| <span data-ttu-id="74eef-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="74eef-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="74eef-208">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-208">no</span></span>             | <span data-ttu-id="74eef-209">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-209">no</span></span>               |
| <span data-ttu-id="74eef-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="74eef-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="74eef-211">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-211">no</span></span>             | <span data-ttu-id="74eef-212">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-212">no</span></span>               |
| <span data-ttu-id="74eef-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="74eef-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="74eef-214">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-214">no</span></span>             | <span data-ttu-id="74eef-215">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-215">no</span></span>               |
| <span data-ttu-id="74eef-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="74eef-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="74eef-217">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-217">no</span></span>             | <span data-ttu-id="74eef-218">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-218">no</span></span>               |
| <span data-ttu-id="74eef-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="74eef-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="74eef-220">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-220">no</span></span>             | <span data-ttu-id="74eef-221">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-221">no</span></span>               |
| <span data-ttu-id="74eef-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="74eef-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="74eef-223">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-223">no</span></span>             | <span data-ttu-id="74eef-224">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-224">no</span></span>               |
| <span data-ttu-id="74eef-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="74eef-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="74eef-226">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-226">no</span></span>             | <span data-ttu-id="74eef-227">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-227">no</span></span>               |
| <span data-ttu-id="74eef-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="74eef-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="74eef-229">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-229">no</span></span>             | <span data-ttu-id="74eef-230">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-230">no</span></span>               |
| <span data-ttu-id="74eef-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="74eef-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="74eef-232">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-232">no</span></span>             | <span data-ttu-id="74eef-233">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-233">no</span></span>               |
| <span data-ttu-id="74eef-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="74eef-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="74eef-235">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-235">no</span></span>             | <span data-ttu-id="74eef-236">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-236">no</span></span>               |
| <span data-ttu-id="74eef-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="74eef-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="74eef-238">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-238">no</span></span>             | <span data-ttu-id="74eef-239">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-239">no</span></span>               |
| <span data-ttu-id="74eef-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="74eef-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="74eef-241">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-241">no</span></span>             | <span data-ttu-id="74eef-242">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-242">no</span></span>               |
| <span data-ttu-id="74eef-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="74eef-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="74eef-244">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-244">no</span></span>             | <span data-ttu-id="74eef-245">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-245">no</span></span>               |
| <span data-ttu-id="74eef-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="74eef-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="74eef-247">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-247">no</span></span>             | <span data-ttu-id="74eef-248">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-248">no</span></span>               |
| <span data-ttu-id="74eef-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="74eef-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="74eef-250">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-250">no</span></span>             | <span data-ttu-id="74eef-251">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-251">no</span></span>               |
| <span data-ttu-id="74eef-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="74eef-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="74eef-253">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-253">no</span></span>             | <span data-ttu-id="74eef-254">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-254">no</span></span>               |
| <span data-ttu-id="74eef-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="74eef-256">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-256">no</span></span>             | <span data-ttu-id="74eef-257">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-257">no</span></span>               |
| <span data-ttu-id="74eef-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="74eef-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="74eef-259">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-259">no</span></span>             | <span data-ttu-id="74eef-260">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-260">no</span></span>               |
| <span data-ttu-id="74eef-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="74eef-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="74eef-262">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-262">no</span></span>             | <span data-ttu-id="74eef-263">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-263">no</span></span>               |
| <span data-ttu-id="74eef-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="74eef-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="74eef-265">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-265">no</span></span>             | <span data-ttu-id="74eef-266">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-266">no</span></span>               |
| <span data-ttu-id="74eef-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="74eef-267">msdyn_progress</span></span>                         | <span data-ttu-id="74eef-268">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-268">no</span></span>             | <span data-ttu-id="74eef-269">ez (bai P4W-rako)</span><span class="sxs-lookup"><span data-stu-id="74eef-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="74eef-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="74eef-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="74eef-271">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-271">no</span></span>             | <span data-ttu-id="74eef-272">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-272">no</span></span>               |
| <span data-ttu-id="74eef-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="74eef-274">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-274">no</span></span>             | <span data-ttu-id="74eef-275">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-275">no</span></span>               |
| <span data-ttu-id="74eef-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="74eef-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="74eef-277">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-277">no</span></span>             | <span data-ttu-id="74eef-278">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-278">no</span></span>               |
| <span data-ttu-id="74eef-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="74eef-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="74eef-280">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-280">no</span></span>             | <span data-ttu-id="74eef-281">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-281">no</span></span>               |
| <span data-ttu-id="74eef-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="74eef-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="74eef-283">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-283">no</span></span>             | <span data-ttu-id="74eef-284">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-284">no</span></span>               |
| <span data-ttu-id="74eef-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="74eef-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="74eef-286">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-286">no</span></span>             | <span data-ttu-id="74eef-287">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-287">no</span></span>               |
| <span data-ttu-id="74eef-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="74eef-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="74eef-289">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-289">no</span></span>             | <span data-ttu-id="74eef-290">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-290">no</span></span>               |
| <span data-ttu-id="74eef-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="74eef-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="74eef-292">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-292">no</span></span>             | <span data-ttu-id="74eef-293">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-293">no</span></span>               |
| <span data-ttu-id="74eef-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="74eef-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="74eef-295">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-295">no</span></span>             | <span data-ttu-id="74eef-296">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-296">no</span></span>               |
| <span data-ttu-id="74eef-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="74eef-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="74eef-298">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-298">no</span></span>             | <span data-ttu-id="74eef-299">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-299">no</span></span>               |
| <span data-ttu-id="74eef-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="74eef-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="74eef-301">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-301">no</span></span>             | <span data-ttu-id="74eef-302">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-302">no</span></span>               |
| <span data-ttu-id="74eef-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="74eef-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="74eef-304">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-304">no</span></span>             | <span data-ttu-id="74eef-305">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-305">no</span></span>               |
| <span data-ttu-id="74eef-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="74eef-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="74eef-307">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-307">no</span></span>             | <span data-ttu-id="74eef-308">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-308">no</span></span>               |
| <span data-ttu-id="74eef-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="74eef-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="74eef-310">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-310">no</span></span>             | <span data-ttu-id="74eef-311">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-311">no</span></span>               |
| <span data-ttu-id="74eef-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="74eef-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="74eef-313">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-313">no</span></span>             | <span data-ttu-id="74eef-314">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-314">no</span></span>               |
| <span data-ttu-id="74eef-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="74eef-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="74eef-316">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-316">no</span></span>             | <span data-ttu-id="74eef-317">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-317">no</span></span>               |
| <span data-ttu-id="74eef-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="74eef-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="74eef-319">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-319">no</span></span>             | <span data-ttu-id="74eef-320">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-320">no</span></span>               |
| <span data-ttu-id="74eef-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="74eef-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="74eef-322">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-322">no</span></span>             | <span data-ttu-id="74eef-323">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-323">no</span></span>               |
| <span data-ttu-id="74eef-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="74eef-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="74eef-325">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-325">no</span></span>             | <span data-ttu-id="74eef-326">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-326">no</span></span>               |
| <span data-ttu-id="74eef-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="74eef-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="74eef-328">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-328">no</span></span>             | <span data-ttu-id="74eef-329">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-329">no</span></span>               |
| <span data-ttu-id="74eef-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="74eef-330">msdyn_summary</span></span>                          | <span data-ttu-id="74eef-331">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-331">no</span></span>             | <span data-ttu-id="74eef-332">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-332">no</span></span>               |
| <span data-ttu-id="74eef-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="74eef-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="74eef-334">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-334">no</span></span>             | <span data-ttu-id="74eef-335">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-335">no</span></span>               |
| <span data-ttu-id="74eef-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="74eef-337">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-337">no</span></span>             | <span data-ttu-id="74eef-338">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="74eef-339">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="74eef-339">Project task dependency</span></span>

| <span data-ttu-id="74eef-340">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="74eef-340">**Logical name**</span></span>              | <span data-ttu-id="74eef-341">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="74eef-341">**Can create**</span></span> | <span data-ttu-id="74eef-342">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="74eef-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="74eef-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="74eef-343">msdyn_linktype</span></span>                | <span data-ttu-id="74eef-344">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-344">no</span></span>             | <span data-ttu-id="74eef-345">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-345">no</span></span>           |
| <span data-ttu-id="74eef-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="74eef-346">msdyn_linktypename</span></span>            | <span data-ttu-id="74eef-347">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-347">no</span></span>             | <span data-ttu-id="74eef-348">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-348">no</span></span>           |
| <span data-ttu-id="74eef-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="74eef-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="74eef-350">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-350">yes</span></span>            | <span data-ttu-id="74eef-351">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-351">no</span></span>           |
| <span data-ttu-id="74eef-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="74eef-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="74eef-353">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-353">yes</span></span>            | <span data-ttu-id="74eef-354">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-354">no</span></span>           |
| <span data-ttu-id="74eef-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="74eef-355">msdyn_project</span></span>                 | <span data-ttu-id="74eef-356">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-356">yes</span></span>            | <span data-ttu-id="74eef-357">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-357">no</span></span>           |
| <span data-ttu-id="74eef-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="74eef-358">msdyn_projectname</span></span>             | <span data-ttu-id="74eef-359">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-359">yes</span></span>            | <span data-ttu-id="74eef-360">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-360">no</span></span>           |
| <span data-ttu-id="74eef-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="74eef-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="74eef-362">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-362">yes</span></span>            | <span data-ttu-id="74eef-363">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-363">no</span></span>           |
| <span data-ttu-id="74eef-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="74eef-364">msdyn_successortask</span></span>           | <span data-ttu-id="74eef-365">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-365">yes</span></span>            | <span data-ttu-id="74eef-366">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-366">no</span></span>           |
| <span data-ttu-id="74eef-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="74eef-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="74eef-368">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-368">yes</span></span>            | <span data-ttu-id="74eef-369">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="74eef-370">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="74eef-370">Resource assignment</span></span>

| <span data-ttu-id="74eef-371">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="74eef-371">**Logical name**</span></span>             | <span data-ttu-id="74eef-372">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="74eef-372">**Can create**</span></span> | <span data-ttu-id="74eef-373">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="74eef-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="74eef-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="74eef-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="74eef-375">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-375">yes</span></span>            | <span data-ttu-id="74eef-376">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-376">no</span></span>           |
| <span data-ttu-id="74eef-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="74eef-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="74eef-378">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-378">yes</span></span>            | <span data-ttu-id="74eef-379">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-379">no</span></span>           |
| <span data-ttu-id="74eef-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="74eef-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="74eef-381">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-381">no</span></span>             | <span data-ttu-id="74eef-382">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-382">no</span></span>           |
| <span data-ttu-id="74eef-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="74eef-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="74eef-384">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-384">no</span></span>             | <span data-ttu-id="74eef-385">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-385">no</span></span>           |
| <span data-ttu-id="74eef-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="74eef-386">msdyn_committype</span></span>             | <span data-ttu-id="74eef-387">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-387">no</span></span>             | <span data-ttu-id="74eef-388">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-388">no</span></span>           |
| <span data-ttu-id="74eef-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="74eef-389">msdyn_committypename</span></span>         | <span data-ttu-id="74eef-390">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-390">no</span></span>             | <span data-ttu-id="74eef-391">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-391">no</span></span>           |
| <span data-ttu-id="74eef-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="74eef-392">msdyn_effort</span></span>                 | <span data-ttu-id="74eef-393">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-393">no</span></span>             | <span data-ttu-id="74eef-394">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-394">no</span></span>           |
| <span data-ttu-id="74eef-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="74eef-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="74eef-396">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-396">no</span></span>             | <span data-ttu-id="74eef-397">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-397">no</span></span>           |
| <span data-ttu-id="74eef-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="74eef-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="74eef-399">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-399">no</span></span>             | <span data-ttu-id="74eef-400">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-400">no</span></span>           |
| <span data-ttu-id="74eef-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="74eef-401">msdyn_finish</span></span>                 | <span data-ttu-id="74eef-402">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-402">no</span></span>             | <span data-ttu-id="74eef-403">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-403">no</span></span>           |
| <span data-ttu-id="74eef-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="74eef-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="74eef-405">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-405">no</span></span>             | <span data-ttu-id="74eef-406">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-406">no</span></span>           |
| <span data-ttu-id="74eef-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="74eef-408">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-408">no</span></span>             | <span data-ttu-id="74eef-409">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-409">no</span></span>           |
| <span data-ttu-id="74eef-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="74eef-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="74eef-411">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-411">no</span></span>             | <span data-ttu-id="74eef-412">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-412">no</span></span>           |
| <span data-ttu-id="74eef-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="74eef-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="74eef-414">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-414">no</span></span>             | <span data-ttu-id="74eef-415">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-415">no</span></span>           |
| <span data-ttu-id="74eef-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="74eef-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="74eef-417">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-417">no</span></span>             | <span data-ttu-id="74eef-418">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-418">no</span></span>           |
| <span data-ttu-id="74eef-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="74eef-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="74eef-420">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-420">no</span></span>             | <span data-ttu-id="74eef-421">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-421">no</span></span>           |
| <span data-ttu-id="74eef-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="74eef-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="74eef-423">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-423">no</span></span>             | <span data-ttu-id="74eef-424">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-424">no</span></span>           |
| <span data-ttu-id="74eef-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="74eef-425">msdyn_projectid</span></span>              | <span data-ttu-id="74eef-426">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-426">yes</span></span>            | <span data-ttu-id="74eef-427">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-427">no</span></span>           |
| <span data-ttu-id="74eef-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="74eef-428">msdyn_projectidname</span></span>          | <span data-ttu-id="74eef-429">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-429">no</span></span>             | <span data-ttu-id="74eef-430">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-430">no</span></span>           |
| <span data-ttu-id="74eef-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="74eef-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="74eef-432">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-432">no</span></span>             | <span data-ttu-id="74eef-433">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-433">no</span></span>           |
| <span data-ttu-id="74eef-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="74eef-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="74eef-435">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-435">no</span></span>             | <span data-ttu-id="74eef-436">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-436">no</span></span>           |
| <span data-ttu-id="74eef-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="74eef-437">msdyn_start</span></span>                  | <span data-ttu-id="74eef-438">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-438">no</span></span>             | <span data-ttu-id="74eef-439">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-439">no</span></span>           |
| <span data-ttu-id="74eef-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="74eef-440">msdyn_taskid</span></span>                 | <span data-ttu-id="74eef-441">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-441">no</span></span>             | <span data-ttu-id="74eef-442">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-442">no</span></span>           |
| <span data-ttu-id="74eef-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="74eef-443">msdyn_taskidname</span></span>             | <span data-ttu-id="74eef-444">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-444">no</span></span>             | <span data-ttu-id="74eef-445">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-445">no</span></span>           |
| <span data-ttu-id="74eef-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="74eef-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="74eef-447">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-447">no</span></span>             | <span data-ttu-id="74eef-448">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="74eef-449">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="74eef-449">Project team member</span></span>

| <span data-ttu-id="74eef-450">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="74eef-450">**Logical name**</span></span>                                 | <span data-ttu-id="74eef-451">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="74eef-451">**Can create**</span></span> | <span data-ttu-id="74eef-452">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="74eef-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="74eef-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="74eef-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="74eef-454">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-454">no</span></span>             | <span data-ttu-id="74eef-455">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-455">no</span></span>           |
| <span data-ttu-id="74eef-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="74eef-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="74eef-457">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-457">no</span></span>             | <span data-ttu-id="74eef-458">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-458">no</span></span>           |
| <span data-ttu-id="74eef-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="74eef-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="74eef-460">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-460">no</span></span>             | <span data-ttu-id="74eef-461">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-461">no</span></span>           |
| <span data-ttu-id="74eef-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="74eef-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="74eef-463">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-463">no</span></span>             | <span data-ttu-id="74eef-464">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-464">no</span></span>           |
| <span data-ttu-id="74eef-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="74eef-465">msdyn_effort</span></span>                                     | <span data-ttu-id="74eef-466">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-466">no</span></span>             | <span data-ttu-id="74eef-467">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-467">no</span></span>           |
| <span data-ttu-id="74eef-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="74eef-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="74eef-469">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-469">no</span></span>             | <span data-ttu-id="74eef-470">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-470">no</span></span>           |
| <span data-ttu-id="74eef-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="74eef-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="74eef-472">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-472">no</span></span>             | <span data-ttu-id="74eef-473">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-473">no</span></span>           |
| <span data-ttu-id="74eef-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="74eef-474">msdyn_finish</span></span>                                     | <span data-ttu-id="74eef-475">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-475">no</span></span>             | <span data-ttu-id="74eef-476">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-476">no</span></span>           |
| <span data-ttu-id="74eef-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="74eef-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="74eef-478">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-478">no</span></span>             | <span data-ttu-id="74eef-479">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-479">no</span></span>           |
| <span data-ttu-id="74eef-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="74eef-480">msdyn_hours</span></span>                                      | <span data-ttu-id="74eef-481">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-481">no</span></span>             | <span data-ttu-id="74eef-482">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-482">no</span></span>           |
| <span data-ttu-id="74eef-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="74eef-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="74eef-484">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-484">no</span></span>             | <span data-ttu-id="74eef-485">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-485">no</span></span>           |
| <span data-ttu-id="74eef-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="74eef-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="74eef-487">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-487">no</span></span>             | <span data-ttu-id="74eef-488">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-488">no</span></span>           |
| <span data-ttu-id="74eef-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="74eef-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="74eef-490">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-490">no</span></span>             | <span data-ttu-id="74eef-491">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-491">no</span></span>           |
| <span data-ttu-id="74eef-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="74eef-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="74eef-493">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-493">no</span></span>             | <span data-ttu-id="74eef-494">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-494">no</span></span>           |
| <span data-ttu-id="74eef-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="74eef-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="74eef-496">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-496">no</span></span>             | <span data-ttu-id="74eef-497">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-497">no</span></span>           |
| <span data-ttu-id="74eef-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="74eef-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="74eef-499">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-499">no</span></span>             | <span data-ttu-id="74eef-500">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-500">no</span></span>           |
| <span data-ttu-id="74eef-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="74eef-501">msdyn_start</span></span>                                      | <span data-ttu-id="74eef-502">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-502">no</span></span>             | <span data-ttu-id="74eef-503">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="74eef-504">Project</span><span class="sxs-lookup"><span data-stu-id="74eef-504">Project</span></span>

| <span data-ttu-id="74eef-505">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="74eef-505">**Logical name**</span></span>                       | <span data-ttu-id="74eef-506">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="74eef-506">**Can create**</span></span> | <span data-ttu-id="74eef-507">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="74eef-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="74eef-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="74eef-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="74eef-509">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-509">no</span></span>             | <span data-ttu-id="74eef-510">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-510">no</span></span>           |
| <span data-ttu-id="74eef-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="74eef-512">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-512">no</span></span>             | <span data-ttu-id="74eef-513">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-513">no</span></span>           |
| <span data-ttu-id="74eef-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="74eef-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="74eef-515">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-515">no</span></span>             | <span data-ttu-id="74eef-516">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-516">no</span></span>           |
| <span data-ttu-id="74eef-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="74eef-518">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-518">no</span></span>             | <span data-ttu-id="74eef-519">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-519">no</span></span>           |
| <span data-ttu-id="74eef-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="74eef-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="74eef-521">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-521">no</span></span>             | <span data-ttu-id="74eef-522">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-522">no</span></span>           |
| <span data-ttu-id="74eef-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="74eef-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="74eef-524">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-524">no</span></span>             | <span data-ttu-id="74eef-525">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-525">no</span></span>           |
| <span data-ttu-id="74eef-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="74eef-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="74eef-527">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-527">yes</span></span>            | <span data-ttu-id="74eef-528">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-528">no</span></span>           |
| <span data-ttu-id="74eef-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="74eef-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="74eef-530">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-530">yes</span></span>            | <span data-ttu-id="74eef-531">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-531">no</span></span>           |
| <span data-ttu-id="74eef-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="74eef-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="74eef-533">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-533">yes</span></span>            | <span data-ttu-id="74eef-534">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-534">no</span></span>           |
| <span data-ttu-id="74eef-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="74eef-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="74eef-536">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-536">no</span></span>             | <span data-ttu-id="74eef-537">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-537">no</span></span>           |
| <span data-ttu-id="74eef-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="74eef-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="74eef-539">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-539">no</span></span>             | <span data-ttu-id="74eef-540">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-540">no</span></span>           |
| <span data-ttu-id="74eef-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="74eef-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="74eef-542">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-542">no</span></span>             | <span data-ttu-id="74eef-543">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-543">no</span></span>           |
| <span data-ttu-id="74eef-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="74eef-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="74eef-545">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-545">no</span></span>             | <span data-ttu-id="74eef-546">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-546">no</span></span>           |
| <span data-ttu-id="74eef-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="74eef-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="74eef-548">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-548">no</span></span>             | <span data-ttu-id="74eef-549">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-549">no</span></span>           |
| <span data-ttu-id="74eef-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="74eef-550">msdyn_duration</span></span>                         | <span data-ttu-id="74eef-551">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-551">no</span></span>             | <span data-ttu-id="74eef-552">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-552">no</span></span>           |
| <span data-ttu-id="74eef-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="74eef-553">msdyn_effort</span></span>                           | <span data-ttu-id="74eef-554">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-554">no</span></span>             | <span data-ttu-id="74eef-555">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-555">no</span></span>           |
| <span data-ttu-id="74eef-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="74eef-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="74eef-557">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-557">no</span></span>             | <span data-ttu-id="74eef-558">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-558">no</span></span>           |
| <span data-ttu-id="74eef-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="74eef-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="74eef-560">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-560">no</span></span>             | <span data-ttu-id="74eef-561">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-561">no</span></span>           |
| <span data-ttu-id="74eef-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="74eef-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="74eef-563">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-563">no</span></span>             | <span data-ttu-id="74eef-564">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-564">no</span></span>           |
| <span data-ttu-id="74eef-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="74eef-565">msdyn_finish</span></span>                           | <span data-ttu-id="74eef-566">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-566">yes</span></span>            | <span data-ttu-id="74eef-567">bai</span><span class="sxs-lookup"><span data-stu-id="74eef-567">yes</span></span>          |
| <span data-ttu-id="74eef-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="74eef-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="74eef-569">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-569">no</span></span>             | <span data-ttu-id="74eef-570">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-570">no</span></span>           |
| <span data-ttu-id="74eef-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="74eef-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="74eef-572">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-572">no</span></span>             | <span data-ttu-id="74eef-573">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-573">no</span></span>           |
| <span data-ttu-id="74eef-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="74eef-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="74eef-575">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-575">no</span></span>             | <span data-ttu-id="74eef-576">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-576">no</span></span>           |
| <span data-ttu-id="74eef-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="74eef-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="74eef-578">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-578">no</span></span>             | <span data-ttu-id="74eef-579">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-579">no</span></span>           |
| <span data-ttu-id="74eef-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="74eef-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="74eef-581">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-581">no</span></span>             | <span data-ttu-id="74eef-582">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-582">no</span></span>           |
| <span data-ttu-id="74eef-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="74eef-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="74eef-584">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-584">no</span></span>             | <span data-ttu-id="74eef-585">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-585">no</span></span>           |
| <span data-ttu-id="74eef-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="74eef-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="74eef-587">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-587">no</span></span>             | <span data-ttu-id="74eef-588">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-588">no</span></span>           |
| <span data-ttu-id="74eef-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="74eef-590">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-590">no</span></span>             | <span data-ttu-id="74eef-591">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-591">no</span></span>           |
| <span data-ttu-id="74eef-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="74eef-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="74eef-593">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-593">no</span></span>             | <span data-ttu-id="74eef-594">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-594">no</span></span>           |
| <span data-ttu-id="74eef-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="74eef-596">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-596">no</span></span>             | <span data-ttu-id="74eef-597">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-597">no</span></span>           |
| <span data-ttu-id="74eef-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="74eef-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="74eef-599">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-599">no</span></span>             | <span data-ttu-id="74eef-600">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-600">no</span></span>           |
| <span data-ttu-id="74eef-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="74eef-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="74eef-602">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-602">no</span></span>             | <span data-ttu-id="74eef-603">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-603">no</span></span>           |
| <span data-ttu-id="74eef-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="74eef-604">msdyn_progress</span></span>                         | <span data-ttu-id="74eef-605">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-605">no</span></span>             | <span data-ttu-id="74eef-606">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-606">no</span></span>           |
| <span data-ttu-id="74eef-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="74eef-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="74eef-608">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-608">no</span></span>             | <span data-ttu-id="74eef-609">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-609">no</span></span>           |
| <span data-ttu-id="74eef-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="74eef-611">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-611">no</span></span>             | <span data-ttu-id="74eef-612">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-612">no</span></span>           |
| <span data-ttu-id="74eef-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="74eef-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="74eef-614">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-614">no</span></span>             | <span data-ttu-id="74eef-615">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-615">no</span></span>           |
| <span data-ttu-id="74eef-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="74eef-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="74eef-617">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-617">no</span></span>             | <span data-ttu-id="74eef-618">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-618">no</span></span>           |
| <span data-ttu-id="74eef-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="74eef-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="74eef-620">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-620">no</span></span>             | <span data-ttu-id="74eef-621">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-621">no</span></span>           |
| <span data-ttu-id="74eef-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="74eef-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="74eef-623">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-623">no</span></span>             | <span data-ttu-id="74eef-624">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-624">no</span></span>           |
| <span data-ttu-id="74eef-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="74eef-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="74eef-626">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-626">no</span></span>             | <span data-ttu-id="74eef-627">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-627">no</span></span>           |
| <span data-ttu-id="74eef-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="74eef-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="74eef-629">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-629">no</span></span>             | <span data-ttu-id="74eef-630">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-630">no</span></span>           |
| <span data-ttu-id="74eef-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="74eef-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="74eef-632">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-632">no</span></span>             | <span data-ttu-id="74eef-633">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-633">no</span></span>           |
| <span data-ttu-id="74eef-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="74eef-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="74eef-635">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-635">no</span></span>             | <span data-ttu-id="74eef-636">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-636">no</span></span>           |
| <span data-ttu-id="74eef-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="74eef-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="74eef-638">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-638">no</span></span>             | <span data-ttu-id="74eef-639">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-639">no</span></span>           |
| <span data-ttu-id="74eef-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="74eef-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="74eef-641">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-641">no</span></span>             | <span data-ttu-id="74eef-642">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-642">no</span></span>           |
| <span data-ttu-id="74eef-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="74eef-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="74eef-644">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-644">no</span></span>             | <span data-ttu-id="74eef-645">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-645">no</span></span>           |
| <span data-ttu-id="74eef-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="74eef-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="74eef-647">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-647">no</span></span>             | <span data-ttu-id="74eef-648">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-648">no</span></span>           |
| <span data-ttu-id="74eef-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="74eef-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="74eef-650">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-650">no</span></span>             | <span data-ttu-id="74eef-651">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-651">no</span></span>           |
| <span data-ttu-id="74eef-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="74eef-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="74eef-653">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-653">no</span></span>             | <span data-ttu-id="74eef-654">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-654">no</span></span>           |
| <span data-ttu-id="74eef-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="74eef-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="74eef-656">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-656">no</span></span>             | <span data-ttu-id="74eef-657">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-657">no</span></span>           |
| <span data-ttu-id="74eef-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="74eef-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="74eef-659">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-659">no</span></span>             | <span data-ttu-id="74eef-660">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-660">no</span></span>           |
| <span data-ttu-id="74eef-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="74eef-662">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-662">no</span></span>             | <span data-ttu-id="74eef-663">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-663">no</span></span>           |
| <span data-ttu-id="74eef-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="74eef-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="74eef-665">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-665">no</span></span>             | <span data-ttu-id="74eef-666">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-666">no</span></span>           |
| <span data-ttu-id="74eef-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="74eef-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="74eef-668">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-668">no</span></span>             | <span data-ttu-id="74eef-669">ez</span><span class="sxs-lookup"><span data-stu-id="74eef-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="74eef-670">Mugak eta arazo ezagunak</span><span class="sxs-lookup"><span data-stu-id="74eef-670">Limitations and known issues</span></span>
<span data-ttu-id="74eef-671">Jarraian agertzen diren mugen eta arazo ezagunen zerrenda:</span><span class="sxs-lookup"><span data-stu-id="74eef-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="74eef-672">Programazio APIak soilik erabil ditzake **Microsoft Project lizentzia duten erabiltzaileak.**</span><span class="sxs-lookup"><span data-stu-id="74eef-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="74eef-673">Ezin dute hauek erabili:</span><span class="sxs-lookup"><span data-stu-id="74eef-673">They can't be used by:</span></span>
    - <span data-ttu-id="74eef-674">Aplikazioaren erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="74eef-674">Application users</span></span>
    - <span data-ttu-id="74eef-675">Sistema-erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="74eef-675">System users</span></span>
    - <span data-ttu-id="74eef-676">Integrazio-erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="74eef-676">Integration users</span></span>
    - <span data-ttu-id="74eef-677">Beharrezko lizentzia ez duten beste erabiltzaile batzuk</span><span class="sxs-lookup"><span data-stu-id="74eef-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="74eef-678">**OperationSet** bakoitzak gehienez 100 eragiketa egin ditzake.</span><span class="sxs-lookup"><span data-stu-id="74eef-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="74eef-679">Erabiltzaile bakoitzak gehienez 10 **OperationSet** ireki eduki ditzake.</span><span class="sxs-lookup"><span data-stu-id="74eef-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="74eef-680">Gaur egun, Project Operations-ek gehienez 500 zeregin onartzen dituzte proiektu batean.</span><span class="sxs-lookup"><span data-stu-id="74eef-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="74eef-681">**OperationSet** hutsegiteen egoera eta hutsegiteen erregistroak ez daude erabilgarri une honetan.</span><span class="sxs-lookup"><span data-stu-id="74eef-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="74eef-682">Antolaketa APIak aurreargitalpen publikoan daude.</span><span class="sxs-lookup"><span data-stu-id="74eef-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="74eef-683">API hauek ekoizpen-ingurunean erabiltzea ez da Microsoft-ek onartzen.</span><span class="sxs-lookup"><span data-stu-id="74eef-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="74eef-684">Proiektuetako eta zereginetako mugak</span><span class="sxs-lookup"><span data-stu-id="74eef-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="74eef-685">Errore-kudeaketa</span><span class="sxs-lookup"><span data-stu-id="74eef-685">Error handling</span></span>

   - <span data-ttu-id="74eef-686">Eragiketa multzoetatik sortutako akatsak berrikusteko, joan **Ezarpenak** \> **Ordutegien integrazioa** \> **Eragiketa multzoak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="74eef-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="74eef-687">Proiektua Antolatzeko Zerbitzutik sortutako akatsak berrikusteko, joan **Ezarpenak** \> **Ordutegien integrazioa** \> **PSS erroreen erregistroak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="74eef-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="74eef-688">Laginaren egoera</span><span class="sxs-lookup"><span data-stu-id="74eef-688">Sample scenario</span></span>

<span data-ttu-id="74eef-689">Eszenatoki honetan, proiektu bat, taldekide bat, lau ataza eta bi baliabide esleipen sortuko dituzu.</span><span class="sxs-lookup"><span data-stu-id="74eef-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="74eef-690">Ondoren, zeregin bat eguneratu, proiektua eguneratu, zeregin bat ezabatu, baliabideen esleipen bat ezabatu eta atazaren mendekotasuna sortuko duzu.</span><span class="sxs-lookup"><span data-stu-id="74eef-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="74eef-691">Lagin osagarriak</span><span class="sxs-lookup"><span data-stu-id="74eef-691">Additional samples</span></span>

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
