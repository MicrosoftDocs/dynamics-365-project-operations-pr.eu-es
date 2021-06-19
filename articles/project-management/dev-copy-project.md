---
title: Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin
description: Gai honek proiektuaren txantiloiak sortzeko proiektuari buruzko informazioa eskaintzen du Kopiatu proiektua ekintza pertsonalizatua erabiliz.
author: stsporen
ms.date: 01/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 7a1f602e789e07014fd6c742940f52341ce6c672
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005641"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="d5875-103">Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin</span><span class="sxs-lookup"><span data-stu-id="d5875-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="d5875-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="d5875-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="d5875-105">Dynamics 365 Project Operations proiektua kopiatu eta eginkizunak eginkizuna adierazten duten baliabide generikoetara itzultzeko gaitasuna onartzen du.</span><span class="sxs-lookup"><span data-stu-id="d5875-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="d5875-106">Bezeroek funtzionalitate hau erabil dezakete oinarrizko proiektuen txantiloiak eraikitzeko.</span><span class="sxs-lookup"><span data-stu-id="d5875-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="d5875-107">Hautatzen duzunean **Kopiatu proiektua**, helburuko proiektuaren egoera eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="d5875-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="d5875-108">Erabili **Egoeraren arrazoia** kopia ekintza noiz bukatu den jakiteko.</span><span class="sxs-lookup"><span data-stu-id="d5875-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="d5875-109">**Kopiatu proiektua** hautatuz gero, proiektuaren hasiera-data uneko hasierako datara eguneratzen du xede-proiektuaren entitatean xede-datarik hautematen ez bada.</span><span class="sxs-lookup"><span data-stu-id="d5875-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="d5875-110">Kopiatu proiektuaren ekintza pertsonalizatua</span><span class="sxs-lookup"><span data-stu-id="d5875-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="d5875-111">Eman izena</span><span class="sxs-lookup"><span data-stu-id="d5875-111">Name</span></span> 

<span data-ttu-id="d5875-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="d5875-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="d5875-113">Sarrerako parametroak</span><span class="sxs-lookup"><span data-stu-id="d5875-113">Input parameters</span></span>
<span data-ttu-id="d5875-114">Hiru sarrera-parametro daude:</span><span class="sxs-lookup"><span data-stu-id="d5875-114">There are three input parameters:</span></span>

| <span data-ttu-id="d5875-115">Parametroa</span><span class="sxs-lookup"><span data-stu-id="d5875-115">Parameter</span></span>          | <span data-ttu-id="d5875-116">Idatzi</span><span class="sxs-lookup"><span data-stu-id="d5875-116">Type</span></span>   | <span data-ttu-id="d5875-117">Balioak</span><span class="sxs-lookup"><span data-stu-id="d5875-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="d5875-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="d5875-118">ProjectCopyOption</span></span>  | <span data-ttu-id="d5875-119">String</span><span class="sxs-lookup"><span data-stu-id="d5875-119">String</span></span> | <span data-ttu-id="d5875-120">**{"removeNamedResources":true}** edo **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="d5875-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="d5875-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="d5875-121">SourceProject</span></span>      | <span data-ttu-id="d5875-122">Entitate-erreferentzia</span><span class="sxs-lookup"><span data-stu-id="d5875-122">Entity Reference</span></span> | <span data-ttu-id="d5875-123">Jatorriko proiektua</span><span class="sxs-lookup"><span data-stu-id="d5875-123">Source Project</span></span> |
| <span data-ttu-id="d5875-124">Helburua</span><span class="sxs-lookup"><span data-stu-id="d5875-124">Target</span></span>             | <span data-ttu-id="d5875-125">Entitate-erreferentzia</span><span class="sxs-lookup"><span data-stu-id="d5875-125">Entity Reference</span></span> | <span data-ttu-id="d5875-126">Helburu Proiektua</span><span class="sxs-lookup"><span data-stu-id="d5875-126">Target Project</span></span> |


- <span data-ttu-id="d5875-127">**{"clearTeamsAndAssignments":true}** : Lehenetsitako portaera duzu proiektuarentzako Weberako eta zeregin guztiak eta taldekideak kenduko ditu.</span><span class="sxs-lookup"><span data-stu-id="d5875-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="d5875-128">**{"removeNamedResources":true}** Proiektuaren eragiketen portaera lehenetsia, eta zereginak baliabide generikoetara itzuliko ditu.</span><span class="sxs-lookup"><span data-stu-id="d5875-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="d5875-129">Ekintzei buruzko informazio gehiagorako, ikusi [Erabili web API ekintzak](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="d5875-129">For more defaults on actions, see [Use Web API actions](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="d5875-130">Zehaztu kopiatu beharreko eremuak</span><span class="sxs-lookup"><span data-stu-id="d5875-130">Specify fields to copy</span></span> 
<span data-ttu-id="d5875-131">Ekintza deitzen denean, **Kopiatu proiektua** proiektuaren ikuspegia aztertuko du **Kopiatu proiektuaren zutabeak** proiektua kopiatzerakoan zein eremu kopiatu zehazteko.</span><span class="sxs-lookup"><span data-stu-id="d5875-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="d5875-132">Adibidez</span><span class="sxs-lookup"><span data-stu-id="d5875-132">Example</span></span>
<span data-ttu-id="d5875-133">Ondorengo adibidean **CopyProject** ekintza pertsonalizatua **removeNamedResources** parametro multzoarekin nola deitu erakusten da.</span><span class="sxs-lookup"><span data-stu-id="d5875-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]