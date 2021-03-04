---
title: Kalkulatu proiektuaren salmentak eta kostuak, erreserbatu daitekeen baliabide batek proiektu bateko eginkizun ugari betetzen dituenean
description: Gai honetan prezioen dimentsioak proiektu bateko eginkizun ugari betetzen dituen baliabide baten prezioei eta kostuei buruzko estimazioak onartzeko nola erabil daitekeen azaltzen da.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 67e24156e960b9b09cf92f7f0cd77f6c74a982b8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145028"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-for-a-project"></a><span data-ttu-id="1378e-103">Kalkulatu proiektuaren salmentak eta kostuak, erreserbatu daitekeen baliabide batek proiektu bateko eginkizun ugari betetzen dituenean</span><span class="sxs-lookup"><span data-stu-id="1378e-103">Estimate project sales and costs when a bookable resource fills multiple roles for a project</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="1378e-104">Proiektuetan oinarritutako enpresek baliabide baten beharra izaten dute proiektu batean eginkizun ugari egiteko.</span><span class="sxs-lookup"><span data-stu-id="1378e-104">Project-based companies often have the need for one resource to perform multiple roles on a project.</span></span> <span data-ttu-id="1378e-105">Eginkizun horietako bakoitzaren prezioak eta kostuak desberdinak izan litezke; horrek esan nahi du baliabide berdinak proiektuan izandako denborak finantza-estimazio desberdina lor dezakeela eginkizun bakoitzaren fakturaren eta kostuen tasen arabera.</span><span class="sxs-lookup"><span data-stu-id="1378e-105">Each of these roles could be priced and costed differently, which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="1378e-106">Project Service Automation-ek izendatutako baliabiderako taldekideen erregistroan dauden balioak konfiguratzea ahalbidetzen du eta taldekideari esleitutako zeregin bakoitzean gainidatziak egiteko aukera ematen du.</span><span class="sxs-lookup"><span data-stu-id="1378e-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="1378e-107">Ondorengo adibidean azaltzen da nola balio horren gainidazte soilak baliabide batek proiektu batean funtzio anitz izatea kostuen eta fakturen tasa desberdinekin.</span><span class="sxs-lookup"><span data-stu-id="1378e-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="1378e-108">Sortu zereginak</span><span class="sxs-lookup"><span data-stu-id="1378e-108">Create tasks</span></span>
<span data-ttu-id="1378e-109">Sortu 40 orduko bi proiektuetako zereginak, A zeregina eta B zeregina. Aukeratu A zeregina B zereginaren aurreko gisa.</span><span class="sxs-lookup"><span data-stu-id="1378e-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="1378e-110">Konfiguratu proiektuko talde-kide orokor baten Funtzioa eta Antolaketa-unitatea</span><span class="sxs-lookup"><span data-stu-id="1378e-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="1378e-111">**Antolaketa** orrian, hautatu A zereginaren **Zeregina** errenkada.</span><span class="sxs-lookup"><span data-stu-id="1378e-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="1378e-112">**Baliabideak** eremuan, hautatu **Sortu** goitibeherako zerrendan.</span><span class="sxs-lookup"><span data-stu-id="1378e-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="1378e-113">**Talde-kidearen sorrera azkarra** orrian, zehaztu zeregin hori egin dezakeen talde-kide orokorraren atributuak.</span><span class="sxs-lookup"><span data-stu-id="1378e-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="1378e-114">Hautatu funtzio eta antolaketa-unitate egokia, eta hautatu **Gorde eta itxi**.</span><span class="sxs-lookup"><span data-stu-id="1378e-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="1378e-115">Talde-kide orokor bat sortu eta zeregin horri esleitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="1378e-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="1378e-116">Errepikatu B zereginaren urrats horiek eta ziurtatu B zereginean sortutako talde-kide orokorreko funtzioa eta antolaketa-unitatea eta A zereginarenak desberdinak direla.</span><span class="sxs-lookup"><span data-stu-id="1378e-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="1378e-117">Konfiguratu proiektu-zereginaren funtzioa eta antolaketa-unitatea</span><span class="sxs-lookup"><span data-stu-id="1378e-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="1378e-118">A zeregina sortu ondoren, hautatu zeregina eta, ondoren, hautatu **Editatu zeregina**.</span><span class="sxs-lookup"><span data-stu-id="1378e-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="1378e-119">**Zereginaren xehetasunak** orrian, aurkitu **Funtzioa** eta **Antolaketa-unitatea** eremuak, gehitu zeregin hori egiteko behar den baliabide bat gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="1378e-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="1378e-120">Project Service Automation demo-datuak erabiliz agertoki hau osatzen ari bazara, hautatu funtzioaren **Aholkularitza-arduraduna**, eta **Fabrikam US** antolaketa-unitate gisa.</span><span class="sxs-lookup"><span data-stu-id="1378e-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="1378e-121">Hautatu B zeregina eta, ondoren, hautatu **Editatu zeregina**.</span><span class="sxs-lookup"><span data-stu-id="1378e-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="1378e-122">**Zereginaren xehetasunak** orrian, aurkitu **Funtzioa** eta **Antolaketa-unitatea** eremuak, gehitu zeregin hori egiteko behar den baliabide bat gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="1378e-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="1378e-123">Ziurtatu fitxategiko balioak **Funtzioa** eta **Antolakuntza-unitatea** eremuak desberdinak dira B ataza egiteko A ataza balioekin alderatuta.</span><span class="sxs-lookup"><span data-stu-id="1378e-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from the values for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="1378e-124">Project Service Automation demo-datuak erabiliz agertoki hau osatzen ari bazara, hautatu funtzioaren **Sare-teknikaria**, eta **Fabrikam US** antolaketa-unitate gisa.</span><span class="sxs-lookup"><span data-stu-id="1378e-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="1378e-125">Gorde eta itxi **Zereginaren xehetasunak** orria.</span><span class="sxs-lookup"><span data-stu-id="1378e-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behavior"></a><span data-ttu-id="1378e-126">Taldekidea eta portaera kalkulatzen du</span><span class="sxs-lookup"><span data-stu-id="1378e-126">Team member and estimates behavior</span></span> 

1. <span data-ttu-id="1378e-127">**Zereginaren xehetasunak** orrian, **Talde-kidea** atalean, hautatu bi talde-kide orokor eta hautatu **Sortu eskakizunak**.</span><span class="sxs-lookup"><span data-stu-id="1378e-127">On the **Task Details** page, on the **Team Member**, select the two generic team Members and then select **Generate Requirements**.</span></span> 
2. <span data-ttu-id="1378e-128">Hautatu **Aholkularitza-arduraduna** eginbidearen talde-kidea eta, ondoren, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="1378e-128">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="1378e-129">Antolaketa-panelak eskakizun horretarako baliabide bat irekitzen eta erreserbatzen du.</span><span class="sxs-lookup"><span data-stu-id="1378e-129">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="1378e-130">Hautatu **Sare-teknikaria** eginbidearen talde-kidea eta, ondoren, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="1378e-130">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="1378e-131">Antolaketa-panelak eskakizun horretako baliabide bera irekitzen eta erreserbatzen du.</span><span class="sxs-lookup"><span data-stu-id="1378e-131">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="1378e-132">Talde-kideen sareta</span><span class="sxs-lookup"><span data-stu-id="1378e-132">Team Member grid</span></span> 
<span data-ttu-id="1378e-133">**Talde-kidea** saretan, ikusi talde-kideen bi erregistro orokor ezabatu egin direla eta baliabide bat ordezkatu dela.</span><span class="sxs-lookup"><span data-stu-id="1378e-133">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="1378e-134">**Funtzioa** eta **Antolaketa-unitatea** eremuetako balioen multzo lehenetsia erakusten duen baliabidearen balio multzo bat dago.</span><span class="sxs-lookup"><span data-stu-id="1378e-134">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="1378e-135">Talde-kideen erregistro horren errenkada zabaltzen duzunean, bi zeregin horietako zeregin desberdinak ikus ditzakezu talde-kideen erregistroan.</span><span class="sxs-lookup"><span data-stu-id="1378e-135">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="1378e-136">Zereginen errenkada bakoitzak **Funtzioa** eta **Antolaketa-unitatea** funtzioen balio zehatzak ditu.</span><span class="sxs-lookup"><span data-stu-id="1378e-136">Each assignment row has task-specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="1378e-137">Aurreikuspenen sareta</span><span class="sxs-lookup"><span data-stu-id="1378e-137">Estimates grid</span></span> 
<span data-ttu-id="1378e-138">**Aurreikuspenak** sarera nabigatzen duzunean, baliabide beraren bi zereginek prezio desberdinak dituztela ohartuko zara.</span><span class="sxs-lookup"><span data-stu-id="1378e-138">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="1378e-139">A zeregineko baliabidearen esleipena **Aholkularitza-arduraduna** eremuaren **Funtzioa** atributuaren balioa erabiliz.</span><span class="sxs-lookup"><span data-stu-id="1378e-139">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="1378e-140">B zeregineko baliabide beraren esleipena **Sare-teknikaria** eremuaren **Funtzioa** atributuaren balioa erabiliz.</span><span class="sxs-lookup"><span data-stu-id="1378e-140">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>

