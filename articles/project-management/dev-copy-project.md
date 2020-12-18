---
title: Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin
description: Gai honek proiektuaren txantiloiak sortzeko proiektuari buruzko informazioa eskaintzen du Kopiatu proiektua ekintza pertsonalizatua erabiliz.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 22976730ef3c8c22ea028b27a6eb5f14fb88993e
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642393"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="9b0d7-103">Garatu proiektuaren txantiloiak Kopiatu proiektua eginbidearekin</span><span class="sxs-lookup"><span data-stu-id="9b0d7-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="9b0d7-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="9b0d7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="9b0d7-105">Dynamics 365 Project Operations proiektua kopiatu eta eginkizunak eginkizuna adierazten duten baliabide generikoetara itzultzeko gaitasuna onartzen du.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="9b0d7-106">Bezeroek funtzionalitate hau erabil dezakete oinarrizko proiektuen txantiloiak eraikitzeko.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="9b0d7-107">Hautatzen duzunean **Kopiatu proiektua**, helburuko proiektuaren egoera eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="9b0d7-108">Erabili **Egoeraren arrazoia** kopia ekintza noiz bukatu den jakiteko.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="9b0d7-109">**Kopiatu proiektua** hautatuz gero, proiektuaren hasiera-data uneko hasierako datara eguneratzen du xede-proiektuaren entitatean xede-datarik hautematen ez bada.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="9b0d7-110">Kopiatu proiektuaren ekintza pertsonalizatua</span><span class="sxs-lookup"><span data-stu-id="9b0d7-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="9b0d7-111">Eman izena</span><span class="sxs-lookup"><span data-stu-id="9b0d7-111">Name</span></span> 

<span data-ttu-id="9b0d7-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="9b0d7-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="9b0d7-113">Sarrerako parametroak</span><span class="sxs-lookup"><span data-stu-id="9b0d7-113">Input parameters</span></span>
<span data-ttu-id="9b0d7-114">Hiru sarrera-parametro daude:</span><span class="sxs-lookup"><span data-stu-id="9b0d7-114">There are three input parameters:</span></span>

| <span data-ttu-id="9b0d7-115">Parametroa</span><span class="sxs-lookup"><span data-stu-id="9b0d7-115">Parameter</span></span>          | <span data-ttu-id="9b0d7-116">Idatzi</span><span class="sxs-lookup"><span data-stu-id="9b0d7-116">Type</span></span>   | <span data-ttu-id="9b0d7-117">Balioak</span><span class="sxs-lookup"><span data-stu-id="9b0d7-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="9b0d7-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="9b0d7-118">ProjectCopyOption</span></span>  | <span data-ttu-id="9b0d7-119">String</span><span class="sxs-lookup"><span data-stu-id="9b0d7-119">String</span></span> | <span data-ttu-id="9b0d7-120">**{"removeNamedResources":true}** edo **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="9b0d7-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="9b0d7-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="9b0d7-121">SourceProject</span></span>      | <span data-ttu-id="9b0d7-122">Entitate-erreferentzia</span><span class="sxs-lookup"><span data-stu-id="9b0d7-122">Entity Reference</span></span> | <span data-ttu-id="9b0d7-123">Jatorriko proiektua</span><span class="sxs-lookup"><span data-stu-id="9b0d7-123">Source Project</span></span> |
| <span data-ttu-id="9b0d7-124">Helburua</span><span class="sxs-lookup"><span data-stu-id="9b0d7-124">Target</span></span>             | <span data-ttu-id="9b0d7-125">Entitate-erreferentzia</span><span class="sxs-lookup"><span data-stu-id="9b0d7-125">Entity Reference</span></span> | <span data-ttu-id="9b0d7-126">Helburu Proiektua</span><span class="sxs-lookup"><span data-stu-id="9b0d7-126">Target Project</span></span> |


- <span data-ttu-id="9b0d7-127">**{"clearTeamsAndAssignments":true}** : Lehenetsitako portaera duzu proiektuarentzako Weberako eta zeregin guztiak eta taldekideak kenduko ditu.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="9b0d7-128">**{"removeNamedResources":true}** Proiektuaren eragiketen portaera lehenetsia, eta zereginak baliabide generikoetara itzuliko ditu.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="9b0d7-129">Ekintzei buruzko informazio gehiagorako, ikusi [Erabili web API ekintzak](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="9b0d7-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="9b0d7-130">Zehaztu kopiatu beharreko eremuak</span><span class="sxs-lookup"><span data-stu-id="9b0d7-130">Specify fields to copy</span></span> 
<span data-ttu-id="9b0d7-131">Ekintza deitzen denean, **Kopiatu proiektua** proiektuaren ikuspegia aztertuko du **Kopiatu proiektuaren zutabeak** proiektua kopiatzerakoan zein eremu kopiatu zehazteko.</span><span class="sxs-lookup"><span data-stu-id="9b0d7-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
