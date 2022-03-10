---
title: Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko
description: Gai honek informazioa eta laginak eskaintzen ditu proiektuen programazio APIak erabiltzeko.
author: sigitac
ms.date: 09/09/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6be35b1c52996f4f94dc429974ef47343a027c8c
ms.sourcegitcommit: bbe484e58a77efe77d28b34709fb6661d5da00f9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/10/2021
ms.locfileid: "7487670"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_



## <a name="scheduling-entities"></a>Antolaketa-entitateak

Proiektuen programazio APIek eragiketak sortzeko, eguneratzeko eta ezabatzeko gaitasuna eskaintzen dute **Programazio entitateekin**. Entitate hauek Project for the Web-en antolaketa-motorearen bidez kudeatzen dira. Sortu, eguneratu eta ezabatu eragiketak honekin **Programazio entitateak** lehenago mugatu ziren Dynamics 365 Project Operations oharrak.

Hurrengo taulan Proiektuaren programazio entitateen zerrenda osoa ematen da.

| Entitatearen izena  | Entitatearen izen logikoa |
| --- | --- |
| Project | msdyn_project |
| Proiektuaren zeregina  | msdyn_projecttask  |
| Proiektuaren zereginen mendekotasuna  | msdyn_projecttaskdependency  |
| Baliabide-esleipena | msdyn_resourceassignment |
| Proiektuaren ontzia  | msdyn_projectbucket |
| Proiektu-taldeko kidea | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

OperationSet lan-unitate eredua da, eragiketen eskaerak eragiketen hainbat transakzio baten barruan prozesatu behar direnean erabil daitekeena.

## <a name="project-schedule-apis"></a>Proiektuen antolaketa APIak

Jarraian, proiektuaren antolaketaren APIen zerrenda dago.

- **msdyn_CreateProjectV1**: API hau proiektu bat sortzeko erabil daiteke. Proiektua eta lehenetsitako proiektua berehala sortzen dira.
- **msdyn_CreateTeamMemberV1**: API hau proiektuko taldekide bat sortzeko erabil daiteke. Taldekideen erregistroa berehala sortzen da.
- **msdyn_CreateOperationSetV1**: API hau transakzio baten barruan egin behar diren hainbat eskaera antolatzeko erabil daiteke.
- **msdyn_PSSCreateV1**: API hau entitate bat sortzeko erabil daiteke. Erakundea sortzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke.
- **msdyn_PSSUpdateV1**: API hau entitate bat eguneratzeko erabil daiteke. Erakundea eguneratzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke.
- **msdyn_PSSDeleteV1**: API hau entitate bat ezabatzeko erabil daiteke. Erakundea ezabatzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke.
- **msdyn_ExecuteOperationSetV1** : API hau emandako eragiketa multzoaren barneko eragiketa guztiak exekutatzeko erabiltzen da.

## <a name="using-project-schedule-apis-with-operationset"></a>ProjectSet programarekin APIak erabiltzea OperationSet-ekin

Biekin grabatzen delako **CreateProjectV1** eta **CreateTeamMemberV1** berehala sortzen dira, API horiek ezin dira **OperationSet** zuzenean. Hala ere, APIa erabil dezakezu beharrezko erregistroak sortzeko **OperationSet**, eta ondoren erabili aurrez sortutako erregistro hauek **OperationSet**.

## <a name="supported-operations"></a>Onartutako eragiketak

| Antolaketa-entitatea | Sortu | Eguneratzea | Ezabatu | Gogoeta garrantzitsuak |
| --- | --- | --- | --- | --- |
Proiektuaren zeregina | Yes | Yes | Yes | None |
| Proiektuaren zereginen mendekotasuna | Yes | Yes | | Proiektuaren zereginen mendekotasun erregistroak ez dira eguneratu. Horren ordez, erregistro zahar bat ezabatu eta erregistro berri bat sor daiteke. |
| Baliabide-esleipena | Yes | Yes | | Ez dira onartzen eremu hauek dituzten eragiketak: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** eta **PlannedWork**. Baliabideak esleitzeko erregistroak ez dira eguneratu. Horren ordez, erregistro zaharra ezabatu eta erregistro berri bat sor daiteke. |
| Proiektuaren ontzia | E/E | E/E | E/E | Lehenetsitako ontzia fitxategia erabiliz sortzen da **CreateProjectV1** APIa. |
| Proiektu-taldeko kidea | Yes | Yes | Yes | Eragiketa sortzeko, erabili **CreateTeamMemberV1** APIa. |
| Project | Yes | Yes | E/E | Ez dira onartzen eremu hauek dituzten eragiketak: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** eta **Duration**. |

API hauek eremu pertsonalizatuak dituzten entitate objektuekin dei daitezke.

Identifikazio propietatea aukerakoa da. Ematen bada, sistema erabiltzen saiatzen da eta salbuespen bat botatzen du ezin bada erabili. Ematen ez bada, sistemak sortuko du.

## <a name="restricted-fields"></a>Eremu mugatuak

Ondorengo tauletan mugatuta dauden eremuak zehazten dira **Sortu** eta **Editatu**.

### <a name="project-task"></a>Proiektuaren zeregina

| **Izen logikoa**                       | **Ez da sortu** | **Edita daiteke**     |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | ez             | ez               |
| msdyn_actualcost_base                  | ez             | ez               |
| msdyn_actualend                        | ez             | ez               |
| msdyn_actualsales                      | ez             | ez               |
| msdyn_actualsales_base                 | ez             | ez               |
| msdyn_actualstart                      | ez             | ez               |
| msdyn_costatcompleteestimate           | ez             | ez               |
| msdyn_costatcompleteestimate_base      | ez             | ez               |
| msdyn_costconsumptionpercentage        | ez             | ez               |
| msdyn_effortcompleted                  | ez             | ez               |
| msdyn_effortestimateatcomplete         | ez             | ez               |
| msdyn_iscritical                       | ez             | ez               |
| msdyn_iscriticalname                   | ez             | ez               |
| msdyn_ismanual                         | ez             | ez               |
| msdyn_ismanualname                     | ez             | ez               |
| msdyn_ismilestone                      | ez             | ez               |
| msdyn_ismilestonename                  | ez             | ez               |
| msdyn_LinkStatus                       | ez             | ez               |
| msdyn_linkstatusname                   | ez             | ez               |
| msdyn_msprojectclientid                | ez             | ez               |
| msdyn_plannedcost                      | ez             | ez               |
| msdyn_plannedcost_base                 | ez             | ez               |
| msdyn_plannedsales                     | ez             | ez               |
| msdyn_plannedsales_base                | ez             | ez               |
| msdyn_pluginprocessingdata             | ez             | ez               |
| msdyn_progress                         | ez             | ez (bai P4W-rako) |
| msdyn_remainingcost                    | ez             | ez               |
| msdyn_remainingcost_base               | ez             | ez               |
| msdyn_remainingsales                   | ez             | ez               |
| msdyn_remainingsales_base              | ez             | ez               |
| msdyn_requestedhours                   | ez             | ez               |
| msdyn_resourcecategory                 | ez             | ez               |
| msdyn_resourcecategoryname             | ez             | ez               |
| msdyn_resourceorganizationalunitid     | ez             | ez               |
| msdyn_resourceorganizationalunitidname | ez             | ez               |
| msdyn_salesconsumptionpercentage       | ez             | ez               |
| msdyn_salesestimateatcomplete          | ez             | ez               |
| msdyn_salesestimateatcomplete_base     | ez             | ez               |
| msdyn_salesvariance                    | ez             | ez               |
| msdyn_salesvariance_base               | ez             | ez               |
| msdyn_scheduleddurationminutes         | ez             | ez               |
| msdyn_scheduledend                     | ez             | ez               |
| msdyn_scheduledstart                   | ez             | ez               |
| msdyn_schedulevariance                 | ez             | ez               |
| msdyn_skipupdateestimateline           | ez             | ez               |
| msdyn_skipupdateestimatelinename       | ez             | ez               |
| msdyn_summary                          | ez             | ez               |
| msdyn_varianceofcost                   | ez             | ez               |
| msdyn_varianceofcost_base              | ez             | ez               |

### <a name="project-task-dependency"></a>Proiektuaren zereginen mendekotasuna

| **Izen logikoa**              | **Ez da sortu** | **Edita daiteke** |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | ez             | ez           |
| msdyn_linktypename            | ez             | ez           |
| msdyn_predecessortask         | bai            | ez           |
| msdyn_predecessortaskname     | bai            | ez           |
| msdyn_project                 | bai            | ez           |
| msdyn_projectname             | bai            | ez           |
| msdyn_projecttaskdependencyid | bai            | ez           |
| msdyn_successortask           | bai            | ez           |
| msdyn_successortaskname       | bai            | ez           |

### <a name="resource-assignment"></a>Baliabide-esleipena

| **Izen logikoa**             | **Ez da sortu** | **Edita daiteke** |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | bai            | ez           |
| msdyn_bookableresourceidname | bai            | ez           |
| msdyn_bookingstatusid        | ez             | ez           |
| msdyn_bookingstatusidname    | ez             | ez           |
| msdyn_committype             | ez             | ez           |
| msdyn_committypename         | ez             | ez           |
| msdyn_effort                 | ez             | ez           |
| msdyn_effortcompleted        | ez             | ez           |
| msdyn_effortremaining        | ez             | ez           |
| msdyn_finish                 | ez             | ez           |
| msdyn_plannedcost            | ez             | ez           |
| msdyn_plannedcost_base       | ez             | ez           |
| msdyn_plannedcostcontour     | ez             | ez           |
| msdyn_plannedsales           | ez             | ez           |
| msdyn_plannedsales_base      | ez             | ez           |
| msdyn_plannedsalescontour    | ez             | ez           |
| msdyn_plannedwork            | ez             | ez           |
| msdyn_projectid              | bai            | ez           |
| msdyn_projectidname          | ez             | ez           |
| msdyn_projectteamid          | ez             | ez           |
| msdyn_projectteamidname      | ez             | ez           |
| msdyn_start                  | ez             | ez           |
| msdyn_taskid                 | ez             | ez           |
| msdyn_taskidname             | ez             | ez           |
| msdyn_userresourceid         | ez             | ez           |

### <a name="project-team-member"></a>Proiektu-taldeko kidea

| **Izen logikoa**                                 | **Ez da sortu** | **Edita daiteke** |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | ez             | ez           |
| msdyn_creategenericteammemberwithrequirementname | ez             | ez           |
| msdyn_deletestatus                               | ez             | ez           |
| msdyn_deletestatusname                           | ez             | ez           |
| msdyn_effort                                     | ez             | ez           |
| msdyn_effortcompleted                            | ez             | ez           |
| msdyn_effortremaining                            | ez             | ez           |
| msdyn_finish                                     | ez             | ez           |
| msdyn_hardbookedhours                            | ez             | ez           |
| msdyn_hours                                      | ez             | ez           |
| msdyn_markedfordeletiontimer                     | ez             | ez           |
| msdyn_markedfordeletiontimestamp                 | ez             | ez           |
| msdyn_msprojectclientid                          | ez             | ez           |
| msdyn_percentage                                 | ez             | ez           |
| msdyn_requiredhours                              | ez             | ez           |
| msdyn_softbookedhours                            | ez             | ez           |
| msdyn_start                                      | ez             | ez           |

### <a name="project"></a>Project

| **Izen logikoa**                       | **Ez da sortu** | **Edita daiteke** |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | ez             | ez           |
| msdyn_actualexpensecost_base           | ez             | ez           |
| msdyn_actuallaborcost                  | ez             | ez           |
| msdyn_actuallaborcost_base             | ez             | ez           |
| msdyn_actualsales                      | ez             | ez           |
| msdyn_actualsales_base                 | ez             | ez           |
| msdyn_contractlineproject              | bai            | ez           |
| msdyn_contractorganizationalunitid     | bai            | ez           |
| msdyn_contractorganizationalunitidname | bai            | ez           |
| msdyn_costconsumption                  | ez             | ez           |
| msdyn_costestimateatcomplete           | ez             | ez           |
| msdyn_costestimateatcomplete_base      | ez             | ez           |
| msdyn_costvariance                     | ez             | ez           |
| msdyn_costvariance_base                | ez             | ez           |
| msdyn_duration                         | ez             | ez           |
| msdyn_effort                           | ez             | ez           |
| msdyn_effortcompleted                  | ez             | ez           |
| msdyn_effortestimateatcompleteeac      | ez             | ez           |
| msdyn_effortremaining                  | ez             | ez           |
| msdyn_finish                           | bai            | bai          |
| msdyn_globalrevisiontoken              | ez             | ez           |
| msdyn_islinkedtomsprojectclient        | ez             | ez           |
| msdyn_islinkedtomsprojectclientname    | ez             | ez           |
| msdyn_linkeddocumenturl                | ez             | ez           |
| msdyn_msprojectdocument                | ez             | ez           |
| msdyn_msprojectdocumentname            | ez             | ez           |
| msdyn_plannedexpensecost               | ez             | ez           |
| msdyn_plannedexpensecost_base          | ez             | ez           |
| msdyn_plannedlaborcost                 | ez             | ez           |
| msdyn_plannedlaborcost_base            | ez             | ez           |
| msdyn_plannedsales                     | ez             | ez           |
| msdyn_plannedsales_base                | ez             | ez           |
| msdyn_progress                         | ez             | ez           |
| msdyn_remainingcost                    | ez             | ez           |
| msdyn_remainingcost_base               | ez             | ez           |
| msdyn_remainingsales                   | ez             | ez           |
| msdyn_remainingsales_base              | ez             | ez           |
| msdyn_replaylogheader                  | ez             | ez           |
| msdyn_salesconsumption                 | ez             | ez           |
| msdyn_salesestimateatcompleteeac       | ez             | ez           |
| msdyn_salesestimateatcompleteeac_base  | ez             | ez           |
| msdyn_salesvariance                    | ez             | ez           |
| msdyn_salesvariance_base               | ez             | ez           |
| msdyn_scheduleperformance              | ez             | ez           |
| msdyn_scheduleperformancename          | ez             | ez           |
| msdyn_schedulevariance                 | ez             | ez           |
| msdyn_taskearlieststart                | ez             | ez           |
| msdyn_teamsize                         | ez             | ez           |
| msdyn_teamsize_date                    | ez             | ez           |
| msdyn_teamsize_state                   | ez             | ez           |
| msdyn_totalactualcost                  | ez             | ez           |
| msdyn_totalactualcost_base             | ez             | ez           |
| msdyn_totalplannedcost                 | ez             | ez           |
| msdyn_totalplannedcost_base            | ez             | ez           |


## <a name="limitations-and-known-issues"></a>Mugak eta arazo ezagunak
Jarraian agertzen diren mugen eta arazo ezagunen zerrenda:

- Project Schedule APIak soilik erabil ditzake **Microsoft Project lizentzia duten erabiltzaileek.** Ezin dute hauek erabili:
    - Aplikazioaren erabiltzaileak
    - Sistema-erabiltzaileak
    - Integrazio-erabiltzaileak
    - Beharrezko lizentzia ez duten beste erabiltzaile batzuk
- **OperationSet** bakoitzak gehienez 100 eragiketa egin ditzake.
- Erabiltzaile bakoitzak gehienez 10 **OperationSet** ireki eduki ditzake.
- Gaur egun, Project Operations-ek gehienez 500 zeregin onartzen dituzte proiektu batean.
- **OperationSet** hutsegiteen egoera eta hutsegiteen erregistroak ez daude erabilgarri une honetan.
- [Proiektuetako eta zereginetako mugak](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a>Errore-kudeaketa

   - Eragiketa multzoetatik sortutako akatsak berrikusteko, joan **Ezarpenak** \> **Ordutegien integrazioa** \> **Eragiketa multzoak** aukerara.
   - Proiektuaren programazio zerbitzutik sortutako akatsak berrikusteko, joan hona: **Ezarpenak** \> **Ordutegien integrazioa** \> **PSS erroreen erregistroak**.

## <a name="sample-scenario"></a>Laginaren egoera

Eszenatoki honetan, proiektu bat, taldekide bat, lau ataza eta bi baliabide esleipen sortuko dituzu. Ondoren, zeregin bat eguneratu, proiektua eguneratu, zeregin bat ezabatu, baliabideen esleipen bat ezabatu eta atazaren mendekotasuna sortuko duzu.

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

## <a name="additional-samples"></a>Lagin osagarriak

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
