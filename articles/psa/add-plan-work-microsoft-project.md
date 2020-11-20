---
title: Erabili Project Service gehigarria Microsoft Project-ekin lanaren plangintza egiteko | MicrosoftDocs
description: Gai honek Microsoft Project gehigarria Microsoft Project Service-en nola gehitu, konfiguratu eta erabiltzeko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 6bc74442866caccc02e53afc913a55aab81f9629
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129663"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="0c2f0-103">Antolatu Microsoft Project lana formateatzeko, Project Service Automation Proiektua Gehitu add-in erabili</span><span class="sxs-lookup"><span data-stu-id="0c2f0-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="0c2f0-104">aplikazioak proiektuen plangintza egiten errazten du, baita gutxi gorabeherakoak ere.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-104">makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="0c2f0-105">Lana daitezen kostuen, ahalegina eta salmenta balio behin betiko proposamena bidali gisa markatu gabe zehatz ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="0c2f0-106">Orain [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] instalatu eta lanaren plangintza egin dezakezu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ingurune ezagunean.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="0c2f0-107">Erabili [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioaren antolatzeko eta kudeatzeko gaitasun indartsuak eta eguneratu proiektu-plana Project Service Automation-en.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="0c2f0-108">SharePoint dokumentu-kudeaketa [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektuetako zure [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] fitxategiak gordetzeko erabiltzeko, zure [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] administratzaileak dokumentu-kudeaketa aktibatu beharko du.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> 
> - <span data-ttu-id="0c2f0-109">[!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] bateragarria da [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-109">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="0c2f0-110">Deskargatu eta instalatu gehigarria</span><span class="sxs-lookup"><span data-stu-id="0c2f0-110">Download and install the add-in</span></span>  
 <span data-ttu-id="0c2f0-111">Izan zure [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] saioa hasteko informazioa prest.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-111">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="0c2f0-112">Informazio hau beharko duzu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikaziotik [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikaziora konektatzeko.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-112">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="0c2f0-113">Deskarga-zentrotik, deskargatu Project Service-en bertsioa onartzen duen gehigarria [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) edo [V3.4 +](https://www.microsoft.com/download/details.aspx?id=57956).</span><span class="sxs-lookup"><span data-stu-id="0c2f0-113">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="0c2f0-114">Sakatu deskargatu esteka.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-114">Click the download link.</span></span>  

3.  <span data-ttu-id="0c2f0-115">Deskarga amaitzen denean, sakatu **Bai** gehigarria instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-115">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="0c2f0-116">Konfiguratu osagarria</span><span class="sxs-lookup"><span data-stu-id="0c2f0-116">Configure the add-in</span></span>  

1. <span data-ttu-id="0c2f0-117">Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] eta sakatu **Project Service** fitxa.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-117">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="0c2f0-118">Sakatu **Konektatu**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-118">Click **Connect**.</span></span>  

3. <span data-ttu-id="0c2f0-119">Sartu zure saio-informazioa eta, ondoren, sakatu **Saioa**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-119">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="0c2f0-120">Orain erabiltzen has zaitezke gehigarria.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-120">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="0c2f0-121">Irakurri txantiloi bat</span><span class="sxs-lookup"><span data-stu-id="0c2f0-121">Read from a template</span></span>  
 <span data-ttu-id="0c2f0-122">Irakurri [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan sortu duzun txantiloi batetik eta kopiatu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan, proiektuaren plangintza hasteko.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-122">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0c2f0-123">[Sortu proiektu-txantiloia (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="0c2f0-123">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1.  <span data-ttu-id="0c2f0-124">**Project Service** fitxan, sakatu **Irakurri** > **Project Service Automation proiektu-txantiloia**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-124">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="0c2f0-125">Aukeratu proiektua txantiloi bat zerrendatik eta, ondoren, sakatu **Ireki**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-125">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="0c2f0-126">Modu lehenetsian, dira kopiatu txantiloiaren Proiektua zeregin gisa ezartzen dira eskuz gisa antolatu.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-126">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="0c2f0-127">Esleitu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] funtzioak proiektuaren baliabideei</span><span class="sxs-lookup"><span data-stu-id="0c2f0-127">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="0c2f0-128">Ireki proiektua bat eta sakatu **Zeregina** zinta.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-128">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="0c2f0-129">Sakatu **Gantt diagrama** menua eta, ondoren, aukeratu **Baliabide Orria**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-129">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="0c2f0-130">Baliabide-Orria, sakatu, **Project Service Automation Baliabide Funtzioak** goitibeherako menuan eta hautatu Project Service Automation funtzio bat.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-130">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="0c2f0-131">Zure proiektua baliabideekin staff</span><span class="sxs-lookup"><span data-stu-id="0c2f0-131">Staff your project with resources</span></span>  

1.  <span data-ttu-id="0c2f0-132">Project Service fitxan aurki daiteke, errenkada bat hautatu eta sakatu **Bilaketa-baliabideak**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-132">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="0c2f0-133">Atalean, **Liburua Baliabide** pantailan, hautatu proiektuan erabili nahi duzun baliabidea.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-133">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="0c2f0-134">Sakatu **Erreserbatu** eta, ondoren, sakatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-134">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="0c2f0-135">Zure proiektua argitaratu</span><span class="sxs-lookup"><span data-stu-id="0c2f0-135">Publish your project</span></span>  
<span data-ttu-id="0c2f0-136">Hurrengo urratsera inportatu eta argitaratzeko, atalean proiektua da antolamendu-proiektua zure bukatuta duzunean, [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0c2f0-136">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="0c2f0-137">Proiektuan inportatzeko da [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0c2f0-137">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="0c2f0-138">Prezioak eta taldeak sorrerako prozesu aplikatzen dira.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-138">The pricing and team generation process are applied.</span></span> <span data-ttu-id="0c2f0-139">Aplikazioan proiektua ireki [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] duzun taldea, proiektua estimates eta diren kanpaina-xehatzea egitura lan egin ikusteko sortu da.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-139">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="0c2f0-140">Taula honetan emaitzak non aurkit erakusten da:</span><span class="sxs-lookup"><span data-stu-id="0c2f0-140">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0c2f0-141">**Gantt diagrama**</span><span class="sxs-lookup"><span data-stu-id="0c2f0-141">**Gantt Chart**</span></span>   | <span data-ttu-id="0c2f0-142">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Zereginen xehetasunen egitura** pantailara inportatzen du.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-142">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0c2f0-143">**Baliabideen orria**</span><span class="sxs-lookup"><span data-stu-id="0c2f0-143">**Resource Sheet**</span></span> |   <span data-ttu-id="0c2f0-144">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Proiektuko taldekideak** pantailara inportatzen du.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-144">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0c2f0-145">**Erabili erabilera**</span><span class="sxs-lookup"><span data-stu-id="0c2f0-145">**Use Usage**</span></span>    |    <span data-ttu-id="0c2f0-146">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Proiektuaren aurreikuspenak** pantailara inportatzen du.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-146">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="0c2f0-147">**Proiektua inportatzeko eta argitaratzeko**</span><span class="sxs-lookup"><span data-stu-id="0c2f0-147">**To import and publish your project**</span></span>  
1. <span data-ttu-id="0c2f0-148">**Project Service** fitxan, sakatu **Argitaratu** > **Project Service Automation berria**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-148">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="0c2f0-149">Tresna-barran **Project Service-n proiektu berria argitaratu** elkarrizketa-koadroan, idatzi- **Proiektuaren izena** eta hautatu **Bezeroa**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-149">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="0c2f0-150">Egiaztatu nahi izanez gero, **Estekatu proiektu-plana Project Service Automation-era** Proiektua fitxategiaren plana Project Service Automation-era estekatzeko.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-150">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="0c2f0-151">Sakatu **Argitaratu**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-151">Click **Publish**.</span></span>  

   <span data-ttu-id="0c2f0-152">Esteka bat Project fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] nagusia fitxategi Proiektua eta lana diren kanpaina-xehatzea egitura [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] batera irakurtzeko soilik.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-152">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="0c2f0-153">Proiektu-planean aldaketak egiteko, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan egin eta eguneratze gisa argitaratu behar dituzu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-153">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="0c2f0-154">Editatu proiektua inportatzen dira</span><span class="sxs-lookup"><span data-stu-id="0c2f0-154">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="0c2f0-155">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikaziora inportatu den proiektu-planean aldaketak egiteko, bi aukera dituzu:</span><span class="sxs-lookup"><span data-stu-id="0c2f0-155">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="0c2f0-156">Ireki fitxategia nagusia eta editatu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-156">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="0c2f0-157">Kendu esteka fitxategiari eta editatu zuzenean Project Servicen.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-157">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="0c2f0-158">Modu lehenetsian, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikaziotik kargatu den proiektua blokeatuta dago eta Proiektua atalean soilik edita daiteke.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-158">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="0c2f0-159">Fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan editatzeko, fitxategiak askatuta izan behar da.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-159">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="0c2f0-160">Editatu [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan</span><span class="sxs-lookup"><span data-stu-id="0c2f0-160">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="0c2f0-161">Menu nagusian, sakatu **Project Service** > **Proiektuak**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-161">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="0c2f0-162">Proiektuen zerrendan, ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan sortu duzuna.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-162">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="0c2f0-163">Sakatu **Ireki MS Project** zintaren batetik.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-163">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="0c2f0-164">Estekatutako fitxategi nagusia irekiko da [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]-en.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-164">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="0c2f0-165">Kendu esteka fitxategiari eta editatu zuzenean [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]-n</span><span class="sxs-lookup"><span data-stu-id="0c2f0-165">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="0c2f0-166">Menu nagusian, sakatu **Project Service** > **Proiektuak**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-166">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="0c2f0-167">Proiektuen zerrendan, ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan sortu duzuna.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-167">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="0c2f0-168">Sakatu **Kendu esteka MS Project-ik** zintaren batetik.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-168">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="0c2f0-169">SharePoint-eko edo Office Taldeak aplikaziora proiektu-fitxategia kargatu</span><span class="sxs-lookup"><span data-stu-id="0c2f0-169">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="0c2f0-170">SharePoint-eko proiektu-fitxategia kargatu eta erlazionatutako dokumentuak atalean aurki dezakezu zure [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektua.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-170">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="0c2f0-171">Zure administratzaileak SharePoint dokumentu-kudeaketa konfiguratu eta aktibatu behar du Proiektua entitaterako.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-171">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> 

 <span data-ttu-id="0c2f0-172">Office Taldeak konfiguratuta baduzu ere karga dezakezu Proiektua fitxategia [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] aplikazioan.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-172">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span>

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="0c2f0-173">Kargatu fitxategi bat SharePoint-en</span><span class="sxs-lookup"><span data-stu-id="0c2f0-173">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="0c2f0-174">Menu nagusian, sakatu **Project Service** > **Kargatu**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-174">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="0c2f0-175">Hautatu **Project Service Automation proiektuaren dokumentuak**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-175">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="0c2f0-176">**Gaitu Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** elkarrizketan, hautatu **Bai** edo **Ez**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-176">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="0c2f0-177">**Bai** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**-en botoia hautatu ahal izango duzu Project Service Automation aplikazioan eta [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] abiarazi eta proiektu-fitxategia kargatu ahal izango duzu SharePoint dokumentu-liburutegian.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-177">If you click **Yes**, you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="0c2f0-178">**Ez** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** botoiaren estekak ez du funtzionatuko.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-178">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="0c2f0-179">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan ere aurki daiteke [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektuari dagokion **Dokumentuak** atalean.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-179">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="0c2f0-180">Fitxategi bat kargatzeko Office Taldeak</span><span class="sxs-lookup"><span data-stu-id="0c2f0-180">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="0c2f0-181">Menu nagusian, sakatu **Project Service** > **Kargatu**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-181">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="0c2f0-182">Hautatu **Project Service Automation proiektuaren dokumentuak**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-182">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="0c2f0-183">**Gaitu Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** elkarrizketan, hautatu **Bai** edo **Ez**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-183">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="0c2f0-184">**Bai** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**-en botoia hautatu ahal izango duzu Project Service Automation aplikazioan eta [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] abiarazi eta proiektu-fitxategia kargatu ahal izango duzu SharePoint dokumentu-liburutegian.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-184">If you click **Yes**, you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="0c2f0-185">**Ez** sakatzen baduzu, **Ireki [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** botoiaren estekak ez du funtzionatuko.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-185">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="0c2f0-186">[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan ere aurki daiteke [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] proiektuari dagokion **Dokumentuak** atalean.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-186">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="0c2f0-187">Zure proiektua txantiloi gisa argitaratu</span><span class="sxs-lookup"><span data-stu-id="0c2f0-187">Publish  your project as a template</span></span>  
 <span data-ttu-id="0c2f0-188">Zure proiektua gorde dezakezu eta aplikazioan proiektua txantiloi gisa gorde arabera erabiltzeko [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0c2f0-188">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="0c2f0-189">Aplikazioan antzekoentzat proiektua planak dira proiektua txantiloiak [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0c2f0-189">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0c2f0-190">[Sortu proiektu-txantiloia (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="0c2f0-190">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1. <span data-ttu-id="0c2f0-191">**Project Service** fitxan, sakatu **Argitaratu** > **Project Service Automation proiektuaren txantiloia**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-191">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="0c2f0-192">**Project Service-n proiektu txantiloia argitaratu** elkarrizketa-koadroan, idatzi- **Proiektu-txantiloiaren izena**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-192">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="0c2f0-193">Nahi izanez gero, egiaztatu **Estekatu proiektu-plana Project Service Automation-era** Proiektua fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]-ra estekatzeko.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-193">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="0c2f0-194">Sakatu **Argitaratu**.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-194">Click **Publish**.</span></span>  

<span data-ttu-id="0c2f0-195">Esteka bat Project fitxategia [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] nagusia fitxategi Proiektua eta lana diren kanpaina-xehatzea egitura [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] txantiloi batera irakurtzeko soilik.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-195">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="0c2f0-196">Proiektu-planean aldaketak egiteko, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] aplikazioan egin eta eguneratze gisa argitaratu behar dituzu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] aplikazioan.</span><span class="sxs-lookup"><span data-stu-id="0c2f0-196">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="0c2f0-197">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="0c2f0-197">See Also</span></span>  
 [<span data-ttu-id="0c2f0-198">Proiektu-kudeatzailearen gida</span><span class="sxs-lookup"><span data-stu-id="0c2f0-198">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
