---
title: Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko
description: Gai honek Programazioa APIak erabiltzeko informazioa eta laginak eskaintzen ditu.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4a032dc7bcbdf23fce3c3b2ca63c51d473bd8e26
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116782"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="f1640-103">Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko</span><span class="sxs-lookup"><span data-stu-id="f1640-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="f1640-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="f1640-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="f1640-105">Gai honetan zehaztutako funtzionaltasun batzuk edo guztiak erabilgarri dago aurrebista-bertsioaren zati gisa.</span><span class="sxs-lookup"><span data-stu-id="f1640-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="f1640-106">Edukia eta funtzionalitatea aldatu egin daitezke.</span><span class="sxs-lookup"><span data-stu-id="f1640-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="f1640-107">Antolaketa-entitateak</span><span class="sxs-lookup"><span data-stu-id="f1640-107">Scheduling entities</span></span>

<span data-ttu-id="f1640-108">Programatu APIek eragiketak sortu, eguneratu eta ezabatzeko gaitasuna eskaintzen dute **Programazio entitateak**.</span><span class="sxs-lookup"><span data-stu-id="f1640-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="f1640-109">Entitate hauek Project for the Web-en antolaketa-motorearen bidez kudeatzen dira.</span><span class="sxs-lookup"><span data-stu-id="f1640-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="f1640-110">Sortu, eguneratu eta ezabatu eragiketak honekin **Programazio entitateak** lehenago mugatu ziren Dynamics 365 Project Operations oharrak.</span><span class="sxs-lookup"><span data-stu-id="f1640-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="f1640-111">Ondorengo taulan zerrenda oso bat ematen da **Programazio entitateak**.</span><span class="sxs-lookup"><span data-stu-id="f1640-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="f1640-112">Entitatearen izena</span><span class="sxs-lookup"><span data-stu-id="f1640-112">Entity name</span></span>  | <span data-ttu-id="f1640-113">Entitatearen izen logikoa</span><span class="sxs-lookup"><span data-stu-id="f1640-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="f1640-114">Project</span><span class="sxs-lookup"><span data-stu-id="f1640-114">Project</span></span> | <span data-ttu-id="f1640-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="f1640-115">msdyn_project</span></span> |
| <span data-ttu-id="f1640-116">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="f1640-116">Project Task</span></span>  | <span data-ttu-id="f1640-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="f1640-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="f1640-118">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="f1640-118">Project Task Dependency</span></span>  | <span data-ttu-id="f1640-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="f1640-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="f1640-120">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="f1640-120">Resource Assignment</span></span> | <span data-ttu-id="f1640-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="f1640-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="f1640-122">Proiektuaren ontzia</span><span class="sxs-lookup"><span data-stu-id="f1640-122">Project Bucket</span></span>  | <span data-ttu-id="f1640-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="f1640-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="f1640-124">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="f1640-124">Project Team Member</span></span> | <span data-ttu-id="f1640-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="f1640-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="f1640-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="f1640-126">OperationSet</span></span>

<span data-ttu-id="f1640-127">OperationSet lan-unitate eredua da, eragiketen eskaerak eragiketen hainbat transakzio baten barruan prozesatu behar direnean erabil daitekeena.</span><span class="sxs-lookup"><span data-stu-id="f1640-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="f1640-128">Programatu APIak</span><span class="sxs-lookup"><span data-stu-id="f1640-128">Schedule APIs</span></span>

<span data-ttu-id="f1640-129">Jarraian uneko Programazio APIen zerrenda dago.</span><span class="sxs-lookup"><span data-stu-id="f1640-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="f1640-130">**msdyn_CreateProjectV1**: API hau proiektu bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="f1640-131">Proiektua eta lehenetsitako proiektua berehala sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="f1640-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="f1640-132">**msdyn_CreateTeamMemberV1**: API hau proiektuko taldekide bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="f1640-133">Taldekideen erregistroa berehala sortzen da.</span><span class="sxs-lookup"><span data-stu-id="f1640-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="f1640-134">**msdyn_CreateOperationSetV1**: API hau transakzio baten barruan egin behar diren hainbat eskaera antolatzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="f1640-135">**msdyn_PSSCreateV1**: API hau entitate bat sortzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="f1640-136">Erakundea sortu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="f1640-137">**msdyn_PSSUpdateV1**: API hau entitate bat eguneratzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="f1640-138">Erakundea eguneratu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="f1640-139">**msdyn_PSSDeleteV1**: API hau entitate bat ezabatzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="f1640-140">Erakundea ezabatu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="f1640-141">**msdyn_ExecuteOperationSetV1** : API hau emandako eragiketa multzoaren barneko eragiketa guztiak exekutatzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="f1640-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="f1640-142">Ordutegi APIak erabiliz OperationSet-ekin</span><span class="sxs-lookup"><span data-stu-id="f1640-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="f1640-143">Biekin grabatzen delako **CreateProjectV1** eta **CreateTeamMemberV1** berehala sortzen dira, API horiek ezin dira **OperationSet** zuzenean.</span><span class="sxs-lookup"><span data-stu-id="f1640-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="f1640-144">Hala ere, APIa erabil dezakezu beharrezko erregistroak sortzeko **OperationSet**, eta ondoren erabili aurrez sortutako erregistro hauek **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="f1640-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="f1640-145">Onartutako eragiketak</span><span class="sxs-lookup"><span data-stu-id="f1640-145">Supported operations</span></span>

| <span data-ttu-id="f1640-146">Antolaketa-entitatea</span><span class="sxs-lookup"><span data-stu-id="f1640-146">Scheduling entity</span></span> | <span data-ttu-id="f1640-147">Sortu</span><span class="sxs-lookup"><span data-stu-id="f1640-147">Create</span></span> | <span data-ttu-id="f1640-148">Eguneratzea</span><span class="sxs-lookup"><span data-stu-id="f1640-148">Update</span></span> | <span data-ttu-id="f1640-149">Ezabatu</span><span class="sxs-lookup"><span data-stu-id="f1640-149">Delete</span></span> | <span data-ttu-id="f1640-150">Gogoeta garrantzitsuak</span><span class="sxs-lookup"><span data-stu-id="f1640-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="f1640-151">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="f1640-151">Project task</span></span> | <span data-ttu-id="f1640-152">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-152">Yes</span></span> | <span data-ttu-id="f1640-153">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-153">Yes</span></span> | <span data-ttu-id="f1640-154">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-154">Yes</span></span> | <span data-ttu-id="f1640-155">None</span><span class="sxs-lookup"><span data-stu-id="f1640-155">None</span></span> |
| <span data-ttu-id="f1640-156">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="f1640-156">Project task dependency</span></span> | <span data-ttu-id="f1640-157">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-157">Yes</span></span> | <span data-ttu-id="f1640-158">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-158">Yes</span></span> | | <span data-ttu-id="f1640-159">Proiektuaren zereginen mendekotasun erregistroak ez dira eguneratu.</span><span class="sxs-lookup"><span data-stu-id="f1640-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="f1640-160">Horren ordez, erregistro zahar bat ezabatu eta erregistro berri bat sor daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="f1640-161">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="f1640-161">Resource assignment</span></span> | <span data-ttu-id="f1640-162">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-162">Yes</span></span> | <span data-ttu-id="f1640-163">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-163">Yes</span></span> | | <span data-ttu-id="f1640-164">Ez dira onartzen eremu hauek dituzten eragiketak: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** eta **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="f1640-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="f1640-165">Baliabideak esleitzeko erregistroak ez dira eguneratu.</span><span class="sxs-lookup"><span data-stu-id="f1640-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="f1640-166">Horren ordez, erregistro zaharra ezabatu eta erregistro berri bat sor daiteke.</span><span class="sxs-lookup"><span data-stu-id="f1640-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="f1640-167">Proiektuaren ontzia</span><span class="sxs-lookup"><span data-stu-id="f1640-167">Project bucket</span></span> | <span data-ttu-id="f1640-168">E/E</span><span class="sxs-lookup"><span data-stu-id="f1640-168">N/A</span></span> | <span data-ttu-id="f1640-169">E/E</span><span class="sxs-lookup"><span data-stu-id="f1640-169">N/A</span></span> | <span data-ttu-id="f1640-170">E/E</span><span class="sxs-lookup"><span data-stu-id="f1640-170">N/A</span></span> | <span data-ttu-id="f1640-171">Lehenetsitako ontzia fitxategia erabiliz sortzen da **CreateProjectV1** APIa.</span><span class="sxs-lookup"><span data-stu-id="f1640-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="f1640-172">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="f1640-172">Project team member</span></span> | <span data-ttu-id="f1640-173">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-173">Yes</span></span> | <span data-ttu-id="f1640-174">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-174">Yes</span></span> | <span data-ttu-id="f1640-175">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-175">Yes</span></span> | <span data-ttu-id="f1640-176">Eragiketa sortzeko, erabili **CreateTeamMemberV1** APIa.</span><span class="sxs-lookup"><span data-stu-id="f1640-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="f1640-177">Project</span><span class="sxs-lookup"><span data-stu-id="f1640-177">Project</span></span> | <span data-ttu-id="f1640-178">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-178">Yes</span></span> | <span data-ttu-id="f1640-179">Yes</span><span class="sxs-lookup"><span data-stu-id="f1640-179">Yes</span></span> | <span data-ttu-id="f1640-180">E/E</span><span class="sxs-lookup"><span data-stu-id="f1640-180">N/A</span></span> | <span data-ttu-id="f1640-181">Ez dira onartzen eremu hauek dituzten eragiketak: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** eta **Duration**.</span><span class="sxs-lookup"><span data-stu-id="f1640-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="f1640-182">API hauek eremu pertsonalizatuak dituzten entitate objektuekin dei daitezke.</span><span class="sxs-lookup"><span data-stu-id="f1640-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="f1640-183">Identifikazio propietatea aukerakoa da.</span><span class="sxs-lookup"><span data-stu-id="f1640-183">The ID property is optional.</span></span> <span data-ttu-id="f1640-184">Ematen bada, sistema erabiltzen saiatzen da eta salbuespen bat botatzen du ezin bada erabili.</span><span class="sxs-lookup"><span data-stu-id="f1640-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="f1640-185">Ematen ez bada, sistemak sortuko du.</span><span class="sxs-lookup"><span data-stu-id="f1640-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="f1640-186">Eremu mugatuak</span><span class="sxs-lookup"><span data-stu-id="f1640-186">Restricted fields</span></span>

<span data-ttu-id="f1640-187">Ondorengo tauletan mugatuta dauden eremuak zehazten dira **Sortu** eta **Editatu**.</span><span class="sxs-lookup"><span data-stu-id="f1640-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="f1640-188">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="f1640-188">Project task</span></span>

| <span data-ttu-id="f1640-189">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="f1640-189">**Logical name**</span></span>                       | <span data-ttu-id="f1640-190">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="f1640-190">**Can create**</span></span> | <span data-ttu-id="f1640-191">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="f1640-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="f1640-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="f1640-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="f1640-193">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-193">no</span></span>             | <span data-ttu-id="f1640-194">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-194">no</span></span>               |
| <span data-ttu-id="f1640-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="f1640-196">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-196">no</span></span>             | <span data-ttu-id="f1640-197">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-197">no</span></span>               |
| <span data-ttu-id="f1640-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="f1640-198">msdyn_actualend</span></span>                        | <span data-ttu-id="f1640-199">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-199">no</span></span>             | <span data-ttu-id="f1640-200">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-200">no</span></span>               |
| <span data-ttu-id="f1640-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="f1640-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="f1640-202">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-202">no</span></span>             | <span data-ttu-id="f1640-203">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-203">no</span></span>               |
| <span data-ttu-id="f1640-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="f1640-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="f1640-205">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-205">no</span></span>             | <span data-ttu-id="f1640-206">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-206">no</span></span>               |
| <span data-ttu-id="f1640-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="f1640-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="f1640-208">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-208">no</span></span>             | <span data-ttu-id="f1640-209">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-209">no</span></span>               |
| <span data-ttu-id="f1640-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="f1640-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="f1640-211">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-211">no</span></span>             | <span data-ttu-id="f1640-212">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-212">no</span></span>               |
| <span data-ttu-id="f1640-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="f1640-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="f1640-214">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-214">no</span></span>             | <span data-ttu-id="f1640-215">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-215">no</span></span>               |
| <span data-ttu-id="f1640-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="f1640-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="f1640-217">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-217">no</span></span>             | <span data-ttu-id="f1640-218">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-218">no</span></span>               |
| <span data-ttu-id="f1640-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="f1640-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="f1640-220">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-220">no</span></span>             | <span data-ttu-id="f1640-221">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-221">no</span></span>               |
| <span data-ttu-id="f1640-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="f1640-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="f1640-223">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-223">no</span></span>             | <span data-ttu-id="f1640-224">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-224">no</span></span>               |
| <span data-ttu-id="f1640-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="f1640-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="f1640-226">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-226">no</span></span>             | <span data-ttu-id="f1640-227">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-227">no</span></span>               |
| <span data-ttu-id="f1640-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="f1640-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="f1640-229">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-229">no</span></span>             | <span data-ttu-id="f1640-230">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-230">no</span></span>               |
| <span data-ttu-id="f1640-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="f1640-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="f1640-232">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-232">no</span></span>             | <span data-ttu-id="f1640-233">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-233">no</span></span>               |
| <span data-ttu-id="f1640-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="f1640-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="f1640-235">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-235">no</span></span>             | <span data-ttu-id="f1640-236">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-236">no</span></span>               |
| <span data-ttu-id="f1640-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="f1640-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="f1640-238">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-238">no</span></span>             | <span data-ttu-id="f1640-239">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-239">no</span></span>               |
| <span data-ttu-id="f1640-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="f1640-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="f1640-241">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-241">no</span></span>             | <span data-ttu-id="f1640-242">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-242">no</span></span>               |
| <span data-ttu-id="f1640-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="f1640-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="f1640-244">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-244">no</span></span>             | <span data-ttu-id="f1640-245">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-245">no</span></span>               |
| <span data-ttu-id="f1640-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="f1640-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="f1640-247">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-247">no</span></span>             | <span data-ttu-id="f1640-248">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-248">no</span></span>               |
| <span data-ttu-id="f1640-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="f1640-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="f1640-250">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-250">no</span></span>             | <span data-ttu-id="f1640-251">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-251">no</span></span>               |
| <span data-ttu-id="f1640-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="f1640-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="f1640-253">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-253">no</span></span>             | <span data-ttu-id="f1640-254">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-254">no</span></span>               |
| <span data-ttu-id="f1640-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="f1640-256">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-256">no</span></span>             | <span data-ttu-id="f1640-257">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-257">no</span></span>               |
| <span data-ttu-id="f1640-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="f1640-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="f1640-259">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-259">no</span></span>             | <span data-ttu-id="f1640-260">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-260">no</span></span>               |
| <span data-ttu-id="f1640-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="f1640-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="f1640-262">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-262">no</span></span>             | <span data-ttu-id="f1640-263">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-263">no</span></span>               |
| <span data-ttu-id="f1640-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="f1640-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="f1640-265">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-265">no</span></span>             | <span data-ttu-id="f1640-266">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-266">no</span></span>               |
| <span data-ttu-id="f1640-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="f1640-267">msdyn_progress</span></span>                         | <span data-ttu-id="f1640-268">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-268">no</span></span>             | <span data-ttu-id="f1640-269">ez (bai P4W-rako)</span><span class="sxs-lookup"><span data-stu-id="f1640-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="f1640-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="f1640-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="f1640-271">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-271">no</span></span>             | <span data-ttu-id="f1640-272">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-272">no</span></span>               |
| <span data-ttu-id="f1640-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="f1640-274">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-274">no</span></span>             | <span data-ttu-id="f1640-275">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-275">no</span></span>               |
| <span data-ttu-id="f1640-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="f1640-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="f1640-277">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-277">no</span></span>             | <span data-ttu-id="f1640-278">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-278">no</span></span>               |
| <span data-ttu-id="f1640-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="f1640-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="f1640-280">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-280">no</span></span>             | <span data-ttu-id="f1640-281">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-281">no</span></span>               |
| <span data-ttu-id="f1640-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="f1640-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="f1640-283">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-283">no</span></span>             | <span data-ttu-id="f1640-284">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-284">no</span></span>               |
| <span data-ttu-id="f1640-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="f1640-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="f1640-286">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-286">no</span></span>             | <span data-ttu-id="f1640-287">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-287">no</span></span>               |
| <span data-ttu-id="f1640-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="f1640-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="f1640-289">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-289">no</span></span>             | <span data-ttu-id="f1640-290">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-290">no</span></span>               |
| <span data-ttu-id="f1640-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="f1640-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="f1640-292">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-292">no</span></span>             | <span data-ttu-id="f1640-293">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-293">no</span></span>               |
| <span data-ttu-id="f1640-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="f1640-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="f1640-295">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-295">no</span></span>             | <span data-ttu-id="f1640-296">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-296">no</span></span>               |
| <span data-ttu-id="f1640-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="f1640-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="f1640-298">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-298">no</span></span>             | <span data-ttu-id="f1640-299">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-299">no</span></span>               |
| <span data-ttu-id="f1640-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="f1640-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="f1640-301">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-301">no</span></span>             | <span data-ttu-id="f1640-302">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-302">no</span></span>               |
| <span data-ttu-id="f1640-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="f1640-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="f1640-304">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-304">no</span></span>             | <span data-ttu-id="f1640-305">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-305">no</span></span>               |
| <span data-ttu-id="f1640-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="f1640-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="f1640-307">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-307">no</span></span>             | <span data-ttu-id="f1640-308">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-308">no</span></span>               |
| <span data-ttu-id="f1640-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="f1640-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="f1640-310">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-310">no</span></span>             | <span data-ttu-id="f1640-311">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-311">no</span></span>               |
| <span data-ttu-id="f1640-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="f1640-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="f1640-313">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-313">no</span></span>             | <span data-ttu-id="f1640-314">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-314">no</span></span>               |
| <span data-ttu-id="f1640-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="f1640-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="f1640-316">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-316">no</span></span>             | <span data-ttu-id="f1640-317">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-317">no</span></span>               |
| <span data-ttu-id="f1640-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="f1640-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="f1640-319">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-319">no</span></span>             | <span data-ttu-id="f1640-320">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-320">no</span></span>               |
| <span data-ttu-id="f1640-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="f1640-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="f1640-322">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-322">no</span></span>             | <span data-ttu-id="f1640-323">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-323">no</span></span>               |
| <span data-ttu-id="f1640-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="f1640-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="f1640-325">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-325">no</span></span>             | <span data-ttu-id="f1640-326">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-326">no</span></span>               |
| <span data-ttu-id="f1640-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="f1640-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="f1640-328">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-328">no</span></span>             | <span data-ttu-id="f1640-329">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-329">no</span></span>               |
| <span data-ttu-id="f1640-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="f1640-330">msdyn_summary</span></span>                          | <span data-ttu-id="f1640-331">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-331">no</span></span>             | <span data-ttu-id="f1640-332">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-332">no</span></span>               |
| <span data-ttu-id="f1640-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="f1640-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="f1640-334">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-334">no</span></span>             | <span data-ttu-id="f1640-335">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-335">no</span></span>               |
| <span data-ttu-id="f1640-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="f1640-337">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-337">no</span></span>             | <span data-ttu-id="f1640-338">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="f1640-339">Proiektuaren zereginen mendekotasuna</span><span class="sxs-lookup"><span data-stu-id="f1640-339">Project task dependency</span></span>

| <span data-ttu-id="f1640-340">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="f1640-340">**Logical name**</span></span>              | <span data-ttu-id="f1640-341">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="f1640-341">**Can create**</span></span> | <span data-ttu-id="f1640-342">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="f1640-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="f1640-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="f1640-343">msdyn_linktype</span></span>                | <span data-ttu-id="f1640-344">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-344">no</span></span>             | <span data-ttu-id="f1640-345">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-345">no</span></span>           |
| <span data-ttu-id="f1640-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="f1640-346">msdyn_linktypename</span></span>            | <span data-ttu-id="f1640-347">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-347">no</span></span>             | <span data-ttu-id="f1640-348">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-348">no</span></span>           |
| <span data-ttu-id="f1640-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="f1640-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="f1640-350">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-350">yes</span></span>            | <span data-ttu-id="f1640-351">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-351">no</span></span>           |
| <span data-ttu-id="f1640-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="f1640-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="f1640-353">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-353">yes</span></span>            | <span data-ttu-id="f1640-354">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-354">no</span></span>           |
| <span data-ttu-id="f1640-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="f1640-355">msdyn_project</span></span>                 | <span data-ttu-id="f1640-356">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-356">yes</span></span>            | <span data-ttu-id="f1640-357">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-357">no</span></span>           |
| <span data-ttu-id="f1640-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="f1640-358">msdyn_projectname</span></span>             | <span data-ttu-id="f1640-359">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-359">yes</span></span>            | <span data-ttu-id="f1640-360">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-360">no</span></span>           |
| <span data-ttu-id="f1640-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="f1640-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="f1640-362">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-362">yes</span></span>            | <span data-ttu-id="f1640-363">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-363">no</span></span>           |
| <span data-ttu-id="f1640-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="f1640-364">msdyn_successortask</span></span>           | <span data-ttu-id="f1640-365">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-365">yes</span></span>            | <span data-ttu-id="f1640-366">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-366">no</span></span>           |
| <span data-ttu-id="f1640-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="f1640-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="f1640-368">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-368">yes</span></span>            | <span data-ttu-id="f1640-369">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="f1640-370">Baliabide-esleipena</span><span class="sxs-lookup"><span data-stu-id="f1640-370">Resource assignment</span></span>

| <span data-ttu-id="f1640-371">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="f1640-371">**Logical name**</span></span>             | <span data-ttu-id="f1640-372">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="f1640-372">**Can create**</span></span> | <span data-ttu-id="f1640-373">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="f1640-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="f1640-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="f1640-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="f1640-375">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-375">yes</span></span>            | <span data-ttu-id="f1640-376">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-376">no</span></span>           |
| <span data-ttu-id="f1640-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="f1640-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="f1640-378">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-378">yes</span></span>            | <span data-ttu-id="f1640-379">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-379">no</span></span>           |
| <span data-ttu-id="f1640-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="f1640-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="f1640-381">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-381">no</span></span>             | <span data-ttu-id="f1640-382">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-382">no</span></span>           |
| <span data-ttu-id="f1640-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="f1640-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="f1640-384">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-384">no</span></span>             | <span data-ttu-id="f1640-385">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-385">no</span></span>           |
| <span data-ttu-id="f1640-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="f1640-386">msdyn_committype</span></span>             | <span data-ttu-id="f1640-387">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-387">no</span></span>             | <span data-ttu-id="f1640-388">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-388">no</span></span>           |
| <span data-ttu-id="f1640-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="f1640-389">msdyn_committypename</span></span>         | <span data-ttu-id="f1640-390">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-390">no</span></span>             | <span data-ttu-id="f1640-391">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-391">no</span></span>           |
| <span data-ttu-id="f1640-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="f1640-392">msdyn_effort</span></span>                 | <span data-ttu-id="f1640-393">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-393">no</span></span>             | <span data-ttu-id="f1640-394">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-394">no</span></span>           |
| <span data-ttu-id="f1640-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="f1640-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="f1640-396">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-396">no</span></span>             | <span data-ttu-id="f1640-397">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-397">no</span></span>           |
| <span data-ttu-id="f1640-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="f1640-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="f1640-399">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-399">no</span></span>             | <span data-ttu-id="f1640-400">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-400">no</span></span>           |
| <span data-ttu-id="f1640-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="f1640-401">msdyn_finish</span></span>                 | <span data-ttu-id="f1640-402">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-402">no</span></span>             | <span data-ttu-id="f1640-403">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-403">no</span></span>           |
| <span data-ttu-id="f1640-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="f1640-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="f1640-405">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-405">no</span></span>             | <span data-ttu-id="f1640-406">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-406">no</span></span>           |
| <span data-ttu-id="f1640-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="f1640-408">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-408">no</span></span>             | <span data-ttu-id="f1640-409">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-409">no</span></span>           |
| <span data-ttu-id="f1640-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="f1640-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="f1640-411">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-411">no</span></span>             | <span data-ttu-id="f1640-412">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-412">no</span></span>           |
| <span data-ttu-id="f1640-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="f1640-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="f1640-414">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-414">no</span></span>             | <span data-ttu-id="f1640-415">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-415">no</span></span>           |
| <span data-ttu-id="f1640-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="f1640-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="f1640-417">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-417">no</span></span>             | <span data-ttu-id="f1640-418">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-418">no</span></span>           |
| <span data-ttu-id="f1640-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="f1640-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="f1640-420">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-420">no</span></span>             | <span data-ttu-id="f1640-421">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-421">no</span></span>           |
| <span data-ttu-id="f1640-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="f1640-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="f1640-423">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-423">no</span></span>             | <span data-ttu-id="f1640-424">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-424">no</span></span>           |
| <span data-ttu-id="f1640-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="f1640-425">msdyn_projectid</span></span>              | <span data-ttu-id="f1640-426">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-426">yes</span></span>            | <span data-ttu-id="f1640-427">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-427">no</span></span>           |
| <span data-ttu-id="f1640-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="f1640-428">msdyn_projectidname</span></span>          | <span data-ttu-id="f1640-429">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-429">no</span></span>             | <span data-ttu-id="f1640-430">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-430">no</span></span>           |
| <span data-ttu-id="f1640-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="f1640-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="f1640-432">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-432">no</span></span>             | <span data-ttu-id="f1640-433">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-433">no</span></span>           |
| <span data-ttu-id="f1640-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="f1640-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="f1640-435">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-435">no</span></span>             | <span data-ttu-id="f1640-436">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-436">no</span></span>           |
| <span data-ttu-id="f1640-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="f1640-437">msdyn_start</span></span>                  | <span data-ttu-id="f1640-438">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-438">no</span></span>             | <span data-ttu-id="f1640-439">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-439">no</span></span>           |
| <span data-ttu-id="f1640-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="f1640-440">msdyn_taskid</span></span>                 | <span data-ttu-id="f1640-441">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-441">no</span></span>             | <span data-ttu-id="f1640-442">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-442">no</span></span>           |
| <span data-ttu-id="f1640-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="f1640-443">msdyn_taskidname</span></span>             | <span data-ttu-id="f1640-444">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-444">no</span></span>             | <span data-ttu-id="f1640-445">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-445">no</span></span>           |
| <span data-ttu-id="f1640-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="f1640-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="f1640-447">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-447">no</span></span>             | <span data-ttu-id="f1640-448">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="f1640-449">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="f1640-449">Project team member</span></span>

| <span data-ttu-id="f1640-450">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="f1640-450">**Logical name**</span></span>                                 | <span data-ttu-id="f1640-451">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="f1640-451">**Can create**</span></span> | <span data-ttu-id="f1640-452">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="f1640-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="f1640-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="f1640-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="f1640-454">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-454">no</span></span>             | <span data-ttu-id="f1640-455">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-455">no</span></span>           |
| <span data-ttu-id="f1640-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="f1640-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="f1640-457">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-457">no</span></span>             | <span data-ttu-id="f1640-458">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-458">no</span></span>           |
| <span data-ttu-id="f1640-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="f1640-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="f1640-460">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-460">no</span></span>             | <span data-ttu-id="f1640-461">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-461">no</span></span>           |
| <span data-ttu-id="f1640-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="f1640-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="f1640-463">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-463">no</span></span>             | <span data-ttu-id="f1640-464">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-464">no</span></span>           |
| <span data-ttu-id="f1640-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="f1640-465">msdyn_effort</span></span>                                     | <span data-ttu-id="f1640-466">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-466">no</span></span>             | <span data-ttu-id="f1640-467">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-467">no</span></span>           |
| <span data-ttu-id="f1640-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="f1640-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="f1640-469">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-469">no</span></span>             | <span data-ttu-id="f1640-470">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-470">no</span></span>           |
| <span data-ttu-id="f1640-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="f1640-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="f1640-472">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-472">no</span></span>             | <span data-ttu-id="f1640-473">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-473">no</span></span>           |
| <span data-ttu-id="f1640-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="f1640-474">msdyn_finish</span></span>                                     | <span data-ttu-id="f1640-475">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-475">no</span></span>             | <span data-ttu-id="f1640-476">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-476">no</span></span>           |
| <span data-ttu-id="f1640-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="f1640-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="f1640-478">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-478">no</span></span>             | <span data-ttu-id="f1640-479">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-479">no</span></span>           |
| <span data-ttu-id="f1640-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="f1640-480">msdyn_hours</span></span>                                      | <span data-ttu-id="f1640-481">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-481">no</span></span>             | <span data-ttu-id="f1640-482">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-482">no</span></span>           |
| <span data-ttu-id="f1640-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="f1640-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="f1640-484">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-484">no</span></span>             | <span data-ttu-id="f1640-485">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-485">no</span></span>           |
| <span data-ttu-id="f1640-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="f1640-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="f1640-487">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-487">no</span></span>             | <span data-ttu-id="f1640-488">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-488">no</span></span>           |
| <span data-ttu-id="f1640-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="f1640-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="f1640-490">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-490">no</span></span>             | <span data-ttu-id="f1640-491">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-491">no</span></span>           |
| <span data-ttu-id="f1640-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="f1640-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="f1640-493">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-493">no</span></span>             | <span data-ttu-id="f1640-494">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-494">no</span></span>           |
| <span data-ttu-id="f1640-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="f1640-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="f1640-496">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-496">no</span></span>             | <span data-ttu-id="f1640-497">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-497">no</span></span>           |
| <span data-ttu-id="f1640-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="f1640-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="f1640-499">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-499">no</span></span>             | <span data-ttu-id="f1640-500">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-500">no</span></span>           |
| <span data-ttu-id="f1640-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="f1640-501">msdyn_start</span></span>                                      | <span data-ttu-id="f1640-502">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-502">no</span></span>             | <span data-ttu-id="f1640-503">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="f1640-504">Project</span><span class="sxs-lookup"><span data-stu-id="f1640-504">Project</span></span>

| <span data-ttu-id="f1640-505">**Izen logikoa**</span><span class="sxs-lookup"><span data-stu-id="f1640-505">**Logical name**</span></span>                       | <span data-ttu-id="f1640-506">**Ez da sortu**</span><span class="sxs-lookup"><span data-stu-id="f1640-506">**Can create**</span></span> | <span data-ttu-id="f1640-507">**Edita daiteke**</span><span class="sxs-lookup"><span data-stu-id="f1640-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="f1640-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="f1640-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="f1640-509">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-509">no</span></span>             | <span data-ttu-id="f1640-510">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-510">no</span></span>           |
| <span data-ttu-id="f1640-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="f1640-512">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-512">no</span></span>             | <span data-ttu-id="f1640-513">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-513">no</span></span>           |
| <span data-ttu-id="f1640-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="f1640-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="f1640-515">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-515">no</span></span>             | <span data-ttu-id="f1640-516">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-516">no</span></span>           |
| <span data-ttu-id="f1640-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="f1640-518">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-518">no</span></span>             | <span data-ttu-id="f1640-519">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-519">no</span></span>           |
| <span data-ttu-id="f1640-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="f1640-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="f1640-521">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-521">no</span></span>             | <span data-ttu-id="f1640-522">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-522">no</span></span>           |
| <span data-ttu-id="f1640-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="f1640-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="f1640-524">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-524">no</span></span>             | <span data-ttu-id="f1640-525">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-525">no</span></span>           |
| <span data-ttu-id="f1640-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="f1640-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="f1640-527">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-527">yes</span></span>            | <span data-ttu-id="f1640-528">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-528">no</span></span>           |
| <span data-ttu-id="f1640-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="f1640-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="f1640-530">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-530">yes</span></span>            | <span data-ttu-id="f1640-531">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-531">no</span></span>           |
| <span data-ttu-id="f1640-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="f1640-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="f1640-533">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-533">yes</span></span>            | <span data-ttu-id="f1640-534">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-534">no</span></span>           |
| <span data-ttu-id="f1640-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="f1640-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="f1640-536">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-536">no</span></span>             | <span data-ttu-id="f1640-537">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-537">no</span></span>           |
| <span data-ttu-id="f1640-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="f1640-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="f1640-539">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-539">no</span></span>             | <span data-ttu-id="f1640-540">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-540">no</span></span>           |
| <span data-ttu-id="f1640-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="f1640-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="f1640-542">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-542">no</span></span>             | <span data-ttu-id="f1640-543">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-543">no</span></span>           |
| <span data-ttu-id="f1640-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="f1640-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="f1640-545">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-545">no</span></span>             | <span data-ttu-id="f1640-546">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-546">no</span></span>           |
| <span data-ttu-id="f1640-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="f1640-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="f1640-548">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-548">no</span></span>             | <span data-ttu-id="f1640-549">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-549">no</span></span>           |
| <span data-ttu-id="f1640-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="f1640-550">msdyn_duration</span></span>                         | <span data-ttu-id="f1640-551">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-551">no</span></span>             | <span data-ttu-id="f1640-552">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-552">no</span></span>           |
| <span data-ttu-id="f1640-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="f1640-553">msdyn_effort</span></span>                           | <span data-ttu-id="f1640-554">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-554">no</span></span>             | <span data-ttu-id="f1640-555">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-555">no</span></span>           |
| <span data-ttu-id="f1640-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="f1640-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="f1640-557">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-557">no</span></span>             | <span data-ttu-id="f1640-558">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-558">no</span></span>           |
| <span data-ttu-id="f1640-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="f1640-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="f1640-560">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-560">no</span></span>             | <span data-ttu-id="f1640-561">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-561">no</span></span>           |
| <span data-ttu-id="f1640-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="f1640-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="f1640-563">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-563">no</span></span>             | <span data-ttu-id="f1640-564">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-564">no</span></span>           |
| <span data-ttu-id="f1640-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="f1640-565">msdyn_finish</span></span>                           | <span data-ttu-id="f1640-566">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-566">yes</span></span>            | <span data-ttu-id="f1640-567">bai</span><span class="sxs-lookup"><span data-stu-id="f1640-567">yes</span></span>          |
| <span data-ttu-id="f1640-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="f1640-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="f1640-569">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-569">no</span></span>             | <span data-ttu-id="f1640-570">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-570">no</span></span>           |
| <span data-ttu-id="f1640-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="f1640-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="f1640-572">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-572">no</span></span>             | <span data-ttu-id="f1640-573">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-573">no</span></span>           |
| <span data-ttu-id="f1640-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="f1640-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="f1640-575">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-575">no</span></span>             | <span data-ttu-id="f1640-576">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-576">no</span></span>           |
| <span data-ttu-id="f1640-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="f1640-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="f1640-578">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-578">no</span></span>             | <span data-ttu-id="f1640-579">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-579">no</span></span>           |
| <span data-ttu-id="f1640-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="f1640-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="f1640-581">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-581">no</span></span>             | <span data-ttu-id="f1640-582">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-582">no</span></span>           |
| <span data-ttu-id="f1640-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="f1640-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="f1640-584">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-584">no</span></span>             | <span data-ttu-id="f1640-585">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-585">no</span></span>           |
| <span data-ttu-id="f1640-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="f1640-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="f1640-587">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-587">no</span></span>             | <span data-ttu-id="f1640-588">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-588">no</span></span>           |
| <span data-ttu-id="f1640-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="f1640-590">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-590">no</span></span>             | <span data-ttu-id="f1640-591">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-591">no</span></span>           |
| <span data-ttu-id="f1640-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="f1640-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="f1640-593">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-593">no</span></span>             | <span data-ttu-id="f1640-594">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-594">no</span></span>           |
| <span data-ttu-id="f1640-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="f1640-596">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-596">no</span></span>             | <span data-ttu-id="f1640-597">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-597">no</span></span>           |
| <span data-ttu-id="f1640-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="f1640-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="f1640-599">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-599">no</span></span>             | <span data-ttu-id="f1640-600">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-600">no</span></span>           |
| <span data-ttu-id="f1640-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="f1640-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="f1640-602">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-602">no</span></span>             | <span data-ttu-id="f1640-603">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-603">no</span></span>           |
| <span data-ttu-id="f1640-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="f1640-604">msdyn_progress</span></span>                         | <span data-ttu-id="f1640-605">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-605">no</span></span>             | <span data-ttu-id="f1640-606">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-606">no</span></span>           |
| <span data-ttu-id="f1640-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="f1640-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="f1640-608">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-608">no</span></span>             | <span data-ttu-id="f1640-609">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-609">no</span></span>           |
| <span data-ttu-id="f1640-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="f1640-611">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-611">no</span></span>             | <span data-ttu-id="f1640-612">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-612">no</span></span>           |
| <span data-ttu-id="f1640-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="f1640-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="f1640-614">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-614">no</span></span>             | <span data-ttu-id="f1640-615">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-615">no</span></span>           |
| <span data-ttu-id="f1640-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="f1640-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="f1640-617">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-617">no</span></span>             | <span data-ttu-id="f1640-618">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-618">no</span></span>           |
| <span data-ttu-id="f1640-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="f1640-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="f1640-620">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-620">no</span></span>             | <span data-ttu-id="f1640-621">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-621">no</span></span>           |
| <span data-ttu-id="f1640-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="f1640-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="f1640-623">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-623">no</span></span>             | <span data-ttu-id="f1640-624">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-624">no</span></span>           |
| <span data-ttu-id="f1640-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="f1640-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="f1640-626">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-626">no</span></span>             | <span data-ttu-id="f1640-627">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-627">no</span></span>           |
| <span data-ttu-id="f1640-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="f1640-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="f1640-629">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-629">no</span></span>             | <span data-ttu-id="f1640-630">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-630">no</span></span>           |
| <span data-ttu-id="f1640-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="f1640-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="f1640-632">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-632">no</span></span>             | <span data-ttu-id="f1640-633">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-633">no</span></span>           |
| <span data-ttu-id="f1640-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="f1640-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="f1640-635">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-635">no</span></span>             | <span data-ttu-id="f1640-636">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-636">no</span></span>           |
| <span data-ttu-id="f1640-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="f1640-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="f1640-638">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-638">no</span></span>             | <span data-ttu-id="f1640-639">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-639">no</span></span>           |
| <span data-ttu-id="f1640-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="f1640-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="f1640-641">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-641">no</span></span>             | <span data-ttu-id="f1640-642">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-642">no</span></span>           |
| <span data-ttu-id="f1640-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="f1640-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="f1640-644">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-644">no</span></span>             | <span data-ttu-id="f1640-645">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-645">no</span></span>           |
| <span data-ttu-id="f1640-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="f1640-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="f1640-647">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-647">no</span></span>             | <span data-ttu-id="f1640-648">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-648">no</span></span>           |
| <span data-ttu-id="f1640-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="f1640-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="f1640-650">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-650">no</span></span>             | <span data-ttu-id="f1640-651">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-651">no</span></span>           |
| <span data-ttu-id="f1640-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="f1640-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="f1640-653">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-653">no</span></span>             | <span data-ttu-id="f1640-654">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-654">no</span></span>           |
| <span data-ttu-id="f1640-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="f1640-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="f1640-656">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-656">no</span></span>             | <span data-ttu-id="f1640-657">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-657">no</span></span>           |
| <span data-ttu-id="f1640-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="f1640-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="f1640-659">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-659">no</span></span>             | <span data-ttu-id="f1640-660">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-660">no</span></span>           |
| <span data-ttu-id="f1640-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="f1640-662">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-662">no</span></span>             | <span data-ttu-id="f1640-663">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-663">no</span></span>           |
| <span data-ttu-id="f1640-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="f1640-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="f1640-665">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-665">no</span></span>             | <span data-ttu-id="f1640-666">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-666">no</span></span>           |
| <span data-ttu-id="f1640-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="f1640-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="f1640-668">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-668">no</span></span>             | <span data-ttu-id="f1640-669">ez</span><span class="sxs-lookup"><span data-stu-id="f1640-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="f1640-670">Mugak eta arazo ezagunak</span><span class="sxs-lookup"><span data-stu-id="f1640-670">Limitations and known issues</span></span>
<span data-ttu-id="f1640-671">Jarraian agertzen diren mugen eta arazo ezagunen zerrenda:</span><span class="sxs-lookup"><span data-stu-id="f1640-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="f1640-672">Programazio APIak soilik erabil ditzake **Microsoft Project lizentzia duten erabiltzaileak.**</span><span class="sxs-lookup"><span data-stu-id="f1640-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="f1640-673">Ezin dute hauek erabili:</span><span class="sxs-lookup"><span data-stu-id="f1640-673">They can't be used by:</span></span>
    - <span data-ttu-id="f1640-674">Aplikazioaren erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="f1640-674">Application users</span></span>
    - <span data-ttu-id="f1640-675">Sistema-erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="f1640-675">System users</span></span>
    - <span data-ttu-id="f1640-676">Integrazio-erabiltzaileak</span><span class="sxs-lookup"><span data-stu-id="f1640-676">Integration users</span></span>
    - <span data-ttu-id="f1640-677">Beharrezko lizentzia ez duten beste erabiltzaile batzuk</span><span class="sxs-lookup"><span data-stu-id="f1640-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="f1640-678">**OperationSet** bakoitzak gehienez 100 eragiketa egin ditzake.</span><span class="sxs-lookup"><span data-stu-id="f1640-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="f1640-679">Erabiltzaile bakoitzak gehienez 10 **OperationSet** ireki eduki ditzake.</span><span class="sxs-lookup"><span data-stu-id="f1640-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="f1640-680">Gaur egun, Project Operations-ek gehienez 500 zeregin onartzen dituzte proiektu batean.</span><span class="sxs-lookup"><span data-stu-id="f1640-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="f1640-681">**OperationSet** hutsegiteen egoera eta hutsegiteen erregistroak ez daude erabilgarri une honetan.</span><span class="sxs-lookup"><span data-stu-id="f1640-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="f1640-682">Proiektuetako eta zereginetako mugak</span><span class="sxs-lookup"><span data-stu-id="f1640-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="f1640-683">Errore-kudeaketa</span><span class="sxs-lookup"><span data-stu-id="f1640-683">Error handling</span></span>

   - <span data-ttu-id="f1640-684">Eragiketa multzoetatik sortutako akatsak berrikusteko, joan **Ezarpenak** \> **Ordutegien integrazioa** \> **Eragiketa multzoak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="f1640-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="f1640-685">Proiektua Antolatzeko Zerbitzutik sortutako akatsak berrikusteko, joan **Ezarpenak** \> **Ordutegien integrazioa** \> **PSS erroreen erregistroak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="f1640-685">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="f1640-686">Laginaren egoera</span><span class="sxs-lookup"><span data-stu-id="f1640-686">Sample scenario</span></span>

<span data-ttu-id="f1640-687">Eszenatoki honetan, proiektu bat, taldekide bat, lau ataza eta bi baliabide esleipen sortuko dituzu.</span><span class="sxs-lookup"><span data-stu-id="f1640-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="f1640-688">Ondoren, zeregin bat eguneratu, proiektua eguneratu, zeregin bat ezabatu, baliabideen esleipen bat ezabatu eta atazaren mendekotasuna sortuko duzu.</span><span class="sxs-lookup"><span data-stu-id="f1640-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="f1640-689">Lagin osagarriak</span><span class="sxs-lookup"><span data-stu-id="f1640-689">Additional samples</span></span>

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
