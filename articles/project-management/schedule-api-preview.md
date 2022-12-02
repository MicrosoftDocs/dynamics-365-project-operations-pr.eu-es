---
title: Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko
description: Artikulu honek informazioa eta laginak eskaintzen ditu proiektuen programazio APIak erabiltzeko.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541109"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


**Antolaketa-entitateak**

Proiektuen programazio APIek eragiketak sortzeko, eguneratzeko eta ezabatzeko gaitasuna eskaintzen dute **Programazio entitateekin**. Entitate hauek Project for the Web-en antolaketa-motorearen bidez kudeatzen dira. Sortu, eguneratu eta ezabatu eragiketak honekin **Programazio entitateak** lehenago mugatu ziren Dynamics 365 Project Operations oharrak.

Hurrengo taulan Proiektuaren programazio entitateen zerrenda osoa ematen da.

| **Entitatearen izena**         | **Entitatearen izen logikoa**     |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Proiektuaren zeregina            | msdyn_projecttask           |
| Proiektuaren zereginen mendekotasuna | msdyn_projecttaskdependency |
| Baliabide-esleipena     | msdyn_resourceassignment    |
| Proiektuaren ontzia          | msdyn_projectbucket         |
| Proiektu-taldeko kidea     | msdyn_projectteam           |
| Proiektuaren egiaztapen-zerrendak      | msdyn_projectchecklist      |
| Proiektuaren etiketa           | msdyn_projectlabel          |
| Etiketatzeko proiektuko zeregina   | msdyn_projecttasktolabel    |
| Proiektu-iterazioa          | msdyn_projectsprint         |

**OperationSet**

OperationSet lan-unitate eredua da, eragiketen eskaerak eragiketen hainbat transakzio baten barruan prozesatu behar direnean erabil daitekeena.

**Proiektuen antolaketa APIak**

Jarraian, proiektuaren antolaketaren APIen zerrenda dago.

| **API**                                 | Deskribapenak                                                                                                                       |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | API hau proiektua sortzeko erabiltzen da. Proiektua eta lehenetsitako proiektua berehala sortzen dira.                         |
| **msdyn_CreateTeamMemberV1**            | API hau proiektuaren taldeko kidea sortzeko erabiltzen da. Taldekideen erregistroa berehala sortzen da.                                  |
| **msdyn_CreateOperationSetV1**          | API hau transakzio baten barruan egin behar diren hainbat eskaera antolatzeko erabiltzen da.                                        |
| **msdyn_PssCreateV1**                   | API hau entitatea sortzeko erabiltzen da. Erakundea sortzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke. |
| **msdyn_PssUpdateV1**                   | API hau entitatea eguneratzeko erabiltzen da. Erakundea eguneratzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke  |
| **msdyn_PssDeleteV1**                   | API hau entitatea ezabatzeko erabiltzen da. Erakundea ezabatzeko eragiketa onartzen duten Proiektuak antolatzeko entitateetako edozein izan daiteke. |
| **msdyn_ExecuteOperationSetV1**         | API hau emandako eragiketa multzoaren barneko eragiketa guztiak exekutatzeko erabiltzen da.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | API hau Baliabide-esleipenaren planifikatutako lan-inguru bat eguneratzeko erabiltzen da.                                                        |



**ProjectSet programarekin APIak erabiltzea OperationSet-ekin**

Biekin grabatzen delako **CreateProjectV1** eta **CreateTeamMemberV1** berehala sortzen dira, API horiek ezin dira **OperationSet** zuzenean. Hala ere, APIa erabil dezakezu beharrezko erregistroak sortzeko **OperationSet**, eta ondoren erabili aurrez sortutako erregistro hauek **OperationSet**.

**Onartutako eragiketak**

| **Antolaketa-entitatea**   | **Sortu** | **Eguneratzea** | **Ezabatu** | **Gogoeta garrantzitsuak**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Proiektuaren zeregina            | Yes        | Yes        | Yes        | **Aurrerapena**, **EffortCompleted**, eta **EffortRemaining** eremuak Project for the Web-en edita daitezke, baina ezin dira editatu Project Operations-en.                                                                                                                                                                                             |
| Proiektuaren zereginen mendekotasuna | Yes        | No         | Yes        | Proiektuaren zereginen mendekotasun erregistroak ez dira eguneratu. Horren ordez, erregistro zahar bat ezabatu eta erregistro berri bat sor daiteke.                                                                                                                                                                                                                                 |
| Baliabide-esleipena     | Yes        | Bai\*      | Yes        | Ez dira onartzen eremu hauek dituzten eragiketak: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** eta **PlannedWork**. Baliabideak esleitzeko erregistroak ez dira eguneratu. Horren ordez, erregistro zaharra ezabatu eta erregistro berri bat sor daiteke. Aparteko API bat eman da Baliabideen Esleipenaren ingeradak eguneratzeko. |
| Proiektuaren ontzia          | Yes        | Yes        | Yes        | Lehenetsitako ontzia **CreateProjectV1** APIa erabiliz sortzen da. Proiektuen ontzia sortzeko eta ezabatzeko laguntza gehitu zen 16. bertsioan.                                                                                                                                                                                                   |
| Proiektu-taldeko kidea     | Yes        | Yes        | Yes        | Eragiketa sortzeko, erabili **CreateTeamMemberV1** APIa.                                                                                                                                                                                                                                                                                           |
| Project                 | Yes        | Yes        |            | Ez dira onartzen eremu hauek dituzten eragiketak: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** eta **Duration**.                                                                                       |
| Proiektuaren egiaztapen-zerrendak      | Yes        | Yes        | Yes        |                                                                                                                                                                                                                                                                                                                                                         |
| Proiektuaren etiketa           | No         | Yes        | No         | Etiketen izenak alda daitezke. Eginbide hori eskuragarri dago soilik Project for the Web-en                                                                                                                                                                                                                                                                      |
| Etiketatzeko proiektuko zeregina   | Yes        | No         | Yes        | Eginbide hori eskuragarri dago soilik Project for the Web-en                                                                                                                                                                                                                                                                                                  |
| Proiektu-iterazioa          | Yes        | Yes        | Yes        | **Hasi** eremuko datak **Amaitu** eremua baino lehenagokoa izan behar du. Proiektu bererako iterazioak ezin dira elkarren artean gainjarri. Eginbide hori eskuragarri dago soilik Project for the Web-en                                                                                                                                                                    |




Identifikazio propietatea aukerakoa da. Ematen bada, sistema erabiltzen saiatzen da eta salbuespen bat botatzen du ezin bada erabili. Ematen ez bada, sistemak sortuko du.

**Mugak eta arazo ezagunak**

Jarraian agertzen diren mugen eta arazo ezagunen zerrenda:

-   Project Schedule APIak soilik erabil ditzake **Microsoft Project lizentzia duten erabiltzaileek**. Ezin dute hauek erabili:
    -   Aplikazioaren erabiltzaileak
    -   Sistema-erabiltzaileak
    -   Integrazio-erabiltzaileak
    -   Beharrezko lizentzia ez duten beste erabiltzaile batzuk
-   **OperationSet** bakoitzak gehienez 100 eragiketa egin ditzake.
-   Erabiltzaile bakoitzak gehienez 10 **OperationSet** ireki eduki ditzake.
-   Gaur egun, Project Operations-ek gehienez 500 zeregin onartzen dituzte proiektu batean.
-   Eguneratze baliabideen esleipenaren Ingerada eragiketa bakoitza eragiketa bakar gisa zenbatzen da.
-   Ingerada eguneratuen zerrenda bakoitzak gehienez 100 denbora zati izan ditzake.
-   **OperationSet** hutsegiteen egoera eta hutsegiteen erregistroak ez daude erabilgarri une honetan.
-   Proiektu bakoitzeko 400 iterazio daude gehienez.
-   [Proiektuetako eta zereginetako mugak](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   Etiketak eskuragarri daude soilik Project for the Web-en.

**Errore-kudeaketa**

-   Eragiketa multzoetatik sortutako akatsak berrikusteko, joan **Ezarpenak** \> **Ordutegien integrazioa** \> **Eragiketa multzoak** aukerara.
-   Proiektuaren programazio zerbitzutik sortutako akatsak berrikusteko, joan hona: **Ezarpenak** \> **Ordutegien integrazioa** \> **PSS erroreen erregistroak**.

**Baliabideak esleitzeko ingerada editatzea**

Entitate bat eguneratzen duten proiektuen antolakuntzako beste API guztiek ez bezala, baliabideen esleipenaren ingerada APIa eremu bakarreko, msdyn_plannedwork, entitate bakarreko, msydn_resourceassignment, eguneratzearen arduradun bakarra da.

Emandako antolaketa-modua hau da:

-   **unitate finkoak**
-   proiektuaren egutegia 9-5p da 9-5pst, astelehena, asteartea, osteguna, ostirala (ASTEAZKENEAN LANIK EZ)
-   eta baliabideen egutegia 9-1p PST da astelehenetik ostiralera

Lan hau astebetekoa da, eguneko lau ordukoa. Baliabideen egutegia 9-1 PST bitartekoa delako, edo egunean lau ordu.

| &nbsp;     | Zeregina | Hasiera-data | Amaiera-data  | Kantitatea | 2022/06/13 | 2022/06/14 | 2022/06/15 | 2022/06/16 | 2022/06/17 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 ordutegiko langile |  T1  | 2022/06/13  | 2022/06/17 | 20       | 4         | 4         | 4         | 4         | 4         |

Adibidez, langileak aste honetan egunero hiru ordu bakarrik lan egitea eta beste zereginetarako ordu bat ematea nahi baduzu.

#### <a name="updatedcontours-sample-payload"></a>UpdatedContours lagin karga:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

Ingeradaren antolaketa APIa exekutatu ondorengo esleipena da hau.

| &nbsp;     | Zeregina | Hasiera-data | Amaiera-data  | Kantitatea | 2022/06/13 | 2022/06/14 | 2022/06/15 | 2022/06/16 | 2022/06/17 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 ordutegiko langile | T1   | 2022/06/13  | 2022/06/17 | 15       | 3         | 3         | 3         | 3         | 3         |


**Laginaren egoera**

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

** Lagin osagarriak

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
