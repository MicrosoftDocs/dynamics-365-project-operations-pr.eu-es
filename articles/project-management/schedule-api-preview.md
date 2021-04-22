---
title: Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko
description: Gai honek Programazioa APIak erabiltzeko informazioa eta laginak eskaintzen ditu.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868114"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

> [!IMPORTANT] 
> Gai honetan zehaztutako funtzionaltasun batzuk edo guztiak erabilgarri dago aurrebista-bertsioaren zati gisa. Edukia eta funtzionalitatea aldatu egin daitezke. 

## <a name="scheduling-entities"></a>Antolaketa-entitateak

Programatu APIek eragiketak sortu, eguneratu eta ezabatzeko gaitasuna eskaintzen dute **Programazio entitateak**. Entitate hauek Project for the Web-en antolaketa-motorearen bidez kudeatzen dira. Sortu, eguneratu eta ezabatu eragiketak honekin **Programazio entitateak** lehenago mugatu ziren Dynamics 365 Project Operations oharrak.

Ondorengo taulan zerrenda oso bat ematen da **Programazio entitateak**.

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

## <a name="schedule-apis"></a>Programatu APIak

Jarraian uneko Programazio APIen zerrenda dago.

- **msdyn_CreateProjectV1**: API hau proiektu bat sortzeko erabil daiteke. Proiektua eta lehenetsitako proiektua berehala sortzen dira.
- **msdyn_CreateTeamMemberV1**: API hau proiektuko taldekide bat sortzeko erabil daiteke. Taldekideen erregistroa berehala sortzen da.
- **msdyn_CreateOperationSetV1**: API hau transakzio baten barruan egin behar diren hainbat eskaera antolatzeko erabil daiteke.
- **msdyn_PSSCreateV1**: API hau entitate bat sortzeko erabil daiteke. Erakundea sortu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.
- **msdyn_PSSUpdateV1**: API hau entitate bat eguneratzeko erabil daiteke. Erakundea eguneratu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.
- **msdyn_PSSDeleteV1**: API hau entitate bat ezabatzeko erabil daiteke. Erakundea ezabatu eragiketa onartzen duten Antolaketa-entitateetako edozein izan daiteke.
- **msdyn_ExecuteOperationSetV1** : API hau emandako eragiketa multzoaren barneko eragiketa guztiak exekutatzeko erabiltzen da.

## <a name="using-schedule-apis-with-operationset"></a>Ordutegi APIak erabiliz OperationSet-ekin

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

## <a name="limitations-and-known-issues"></a>Mugak eta arazo ezagunak
Jarraian agertzen diren mugen eta arazo ezagunen zerrenda:

- Programazio APIak soilik erabil ditzake **Microsoft Project lizentzia duten erabiltzaileak.** Ezin dute hauek erabili:
    - Aplikazioaren erabiltzaileak
    - Sistema-erabiltzaileak
    - Integrazio-erabiltzaileak
    - Beharrezko lizentzia ez duten beste erabiltzaile batzuk
- **OperationSet** bakoitzak gehienez 100 eragiketa egin ditzake.
- Erabiltzaile bakoitzak gehienez 10 **OperationSet** ireki eduki ditzake.
- Gaur egun, Project Operations-ek gehienez 500 zeregin onartzen dituzte proiektu batean.
- **OperationSet** hutsegiteen egoera eta hutsegiteen erregistroak ez daude erabilgarri une honetan.
- Antolaketa APIak aurreargitalpen publikoan daude. API hauek ekoizpen-ingurunean erabiltzea ez da Microsoft-ek onartzen.

## <a name="sample-scenario"></a>Laginaren egoera

Eszenatoki honetan, proiektu bat, taldekide bat, lau ataza eta bi baliabide esleipen sortuko dituzu. Ondoren, zeregin bat eguneratu, proiektua eguneratu, zeregin bat ezabatu, baliabideen esleipen bat ezabatu eta atazaren mendekotasuna sortuko duzu.

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>Lagin osagarriak

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
