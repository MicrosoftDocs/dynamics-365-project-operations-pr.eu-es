---
title: Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin
description: Gai honek proiektuaren txantiloiak sortzeko proiektuari buruzko informazioa eskaintzen du Kopiatu proiektua ekintza pertsonalizatua erabiliz.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 27847575e2d6ec9af77d24f756b13d3aeb0efea7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286908"
---
# <a name="develop-project-templates-with-copy-project"></a>Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations proiektua kopiatu eta eginkizunak eginkizuna adierazten duten baliabide generikoetara itzultzeko gaitasuna onartzen du. Bezeroek funtzionalitate hau erabil dezakete oinarrizko proiektuen txantiloiak eraikitzeko.

Hautatzen duzunean **Kopiatu proiektua**, helburuko proiektuaren egoera eguneratzen da. Erabili **Egoeraren arrazoia** kopia ekintza noiz bukatu den jakiteko. **Kopiatu proiektua** hautatuz gero, proiektuaren hasiera-data uneko hasierako datara eguneratzen du xede-proiektuaren entitatean xede-datarik hautematen ez bada.

## <a name="copy-project-custom-action"></a>Kopiatu proiektuaren ekintza pertsonalizatua 

### <a name="name"></a>Eman izena 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>Sarrerako parametroak
Hiru sarrera-parametro daude:

| Parametroa          | Idatzi   | Balioak                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** edo **{"clearTeamsAndAssignments":true}** |
| SourceProject      | Entitate-erreferentzia | Jatorriko proiektua |
| Helburua             | Entitate-erreferentzia | Helburu Proiektua |


- **{"clearTeamsAndAssignments":true}** : Lehenetsitako portaera duzu proiektuarentzako Weberako eta zeregin guztiak eta taldekideak kenduko ditu.
- **{"removeNamedResources":true}** Proiektuaren eragiketen portaera lehenetsia, eta zereginak baliabide generikoetara itzuliko ditu.

Ekintzei buruzko informazio gehiagorako, ikusi [Erabili web API ekintzak](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>Zehaztu kopiatu beharreko eremuak 
Ekintza deitzen denean, **Kopiatu proiektua** proiektuaren ikuspegia aztertuko du **Kopiatu proiektuaren zutabeak** proiektua kopiatzerakoan zein eremu kopiatu zehazteko.


### <a name="example"></a>Adibidez
Ondorengo adibidean **CopyProject** ekintza pertsonalizatua **removeNamedResources** parametro multzoarekin nola deitu erakusten da.
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