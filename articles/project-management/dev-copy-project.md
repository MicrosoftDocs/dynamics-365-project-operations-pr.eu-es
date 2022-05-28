---
title: Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin
description: Gai honek proiektuaren txantiloiak sortzeko proiektuari buruzko informazioa eskaintzen du Kopiatu proiektua ekintza pertsonalizatua erabiliz.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 72aa2db7c717eeab85ada448c673bf702087baeb
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8590883"
---
# <a name="develop-project-templates-with-copy-project"></a>Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations proiektua kopiatu eta eginkizunak eginkizuna adierazten duten baliabide generikoetara itzultzeko gaitasuna onartzen du. Bezeroek funtzionalitate hau erabil dezakete oinarrizko proiektuen txantiloiak eraikitzeko.

Hautatzen duzunean **Kopiatu proiektua**, helburuko proiektuaren egoera eguneratzen da. Erabili **Egoeraren arrazoia** kopia ekintza noiz bukatu den jakiteko. **Kopiatu proiektua** hautatuz gero, proiektuaren hasiera-data uneko hasierako datara eguneratzen du xede-proiektuaren entitatean xede-datarik hautematen ez bada.

## <a name="copy-project-custom-action"></a>Kopiatu proiektuaren ekintza pertsonalizatua

### <a name="name"></a>Eman izena 

msdyn\_ CopyProjectV3

### <a name="input-parameters"></a>Sarrerako parametroak

Hiru sarrera-parametro daude:

- **OrdezkatuNamedResources** edo **GarbituTeamsAndAssignments** – Ezarri aukeretako bakarra. Ez ezarri biak.

    - **\{"ReplaceNamedResources": egia\}** – Proiektuaren Eragiketen portaera lehenetsia. Izendatutako edozein baliabide baliabide generikoekin ordezkatzen dira.
    - **\{"ClearTeamsAndAssignments":egia\}** – Weberako Proiektuaren portaera lehenetsia. Zeregin eta taldekide guztiak kentzen dira.

- **IturburuProiektua** – Kopiatu nahi den iturburu-proiektuaren entitate-erreferentzia. Parametro hau ezin da nulua izan.
- **Helburua** – Kopiatu nahi den xede-proiektuaren entitate-erreferentzia. Parametro hau ezin da nulua izan.

Hurrengo taulak hiru parametroen laburpena eskaintzen du.

| Parametroa                | Idatzi             | Balioa                 |
|--------------------------|------------------|-----------------------|
| OrdezkatuNamedResources    | Boolean          | **Egia** edo **Gezurra** |
| GarbituTeamsAndAssignments | Boolean          | **Egia** edo **Gezurra** |
| SourceProject            | Entitate-erreferentzia | Iturburu proiektua    |
| Helburua                   | Entitate-erreferentzia | Helburuko proiektua    |

Ekintzei buruzko lehenespen gehiago lortzeko, ikus [Erabili Web API ekintzak](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>Balioztatzeak

Ondorengo balioztatzeak egiten dira.

1. Null-ek iturburu eta xede-proiektuak egiaztatzen eta berreskuratzen ditu erakundean bi proiektuen existentzia baieztatzeko.
2. Sistemak baliozkotzen du xede-proiektua kopiatzeko balio duela baldintza hauek egiaztatuz:

    - Proiektuan ez dago aurreko jarduerarik (hautaketa barne **Zereginak** fitxa), eta proiektua sortu berria da.
    - Ez dago aurreko kopiarik, ez da inportaziorik eskatu proiektu honetan, eta proiektuak ez du **Huts egin du** egoera.

3. Eragiketa ez da HTTP erabiliz deitzen.

## <a name="specify-fields-to-copy"></a>Zehaztu kopiatu beharreko eremuak

Ekintza deitzen denean, **Kopiatu proiektua** proiektuaren ikuspegia aztertuko du **Kopiatu proiektuaren zutabeak** proiektua kopiatzerakoan zein eremu kopiatu zehazteko.

### <a name="example"></a>Adibidez

Hurrengo adibidean nola deitzen den erakusten da **CopyProjectV3** ekintza pertsonalizatuarekin **kenduNamedResources** parametro multzoa.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

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
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
