---
title: Eman ingurune berri bat
description: Gai honek Project Operations ingurune berri bat emateari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a43b947207b6d4276ef27ec996713bf3883e7906
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070923"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="e0971-103">Eman ingurune berri bat</span><span class="sxs-lookup"><span data-stu-id="e0971-103">Provision a new environment</span></span>

<span data-ttu-id="e0971-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="e0971-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e0971-105">Gai honek Dynamics 365 Project Operations ingurune berri bat emateko moduari buruzko informazioa eskaintzen du berreskuratutako / stockean oinarritutako eszenatokietarako.</span><span class="sxs-lookup"><span data-stu-id="e0971-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="e0971-106">Gaitu Project Operations hornidura automatikoa LCS proiektu batean</span><span class="sxs-lookup"><span data-stu-id="e0971-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="e0971-107">Erabili urrats hauek zure LCS proiekturako Project Operations hornidura-fluxu automatikoa gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="e0971-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="e0971-108">Joan [LCS](https://lcs.dynamics.com/v2) aukerara eta hautatu **Aurreikusi funtzioen kudeaketa** lauza.</span><span class="sxs-lookup"><span data-stu-id="e0971-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="e0971-109">**Aurrebista eginbidea** zerrendan, hautatu **Project Operations eginbidea** eta, ondoren, hautatu **Aurrebista eginbidea gaituta** Project Operations gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="e0971-109">In the **Preview feature** list, select **Project Operations Feature** , and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="e0971-110">Urrats hau LCS proiektu bakoitzeko behin bakarrik egiten da.</span><span class="sxs-lookup"><span data-stu-id="e0971-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="e0971-111">Project Operations ingurunea hornitzea</span><span class="sxs-lookup"><span data-stu-id="e0971-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="e0971-112">Ireki Dynamics 365 Finance [demo-ingurunea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) edo [sandbox / produkzio ingurunea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) inplementazioa.</span><span class="sxs-lookup"><span data-stu-id="e0971-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="e0971-113">**Ingurumen hornidura** morroia eramatea.</span><span class="sxs-lookup"><span data-stu-id="e0971-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="e0971-114">Ziurtatu hautatutako aplikazioaren bertsioa 10.0.13 edo berriagoa dela.</span><span class="sxs-lookup"><span data-stu-id="e0971-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="e0971-115">Project Operations hornitzeko, **Ezarpen aurreratuak** aukeran, hautatu **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="e0971-115">To provision Project Operations, under **Advance settings** , select **Common Data Service**.</span></span> 
4. <span data-ttu-id="e0971-116">Gaitu **Common Data Service ezarpena** **Bai** hautatuta, eta ondoren sartu informazioa beharrezko eremuetan:</span><span class="sxs-lookup"><span data-stu-id="e0971-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="e0971-117">Izena</span><span class="sxs-lookup"><span data-stu-id="e0971-117">Name</span></span>
  - <span data-ttu-id="e0971-118">Eskualdea</span><span class="sxs-lookup"><span data-stu-id="e0971-118">Region</span></span>
  - <span data-ttu-id="e0971-119">Hizkuntza</span><span class="sxs-lookup"><span data-stu-id="e0971-119">Language</span></span>
  - <span data-ttu-id="e0971-120">Moneta</span><span class="sxs-lookup"><span data-stu-id="e0971-120">Currency</span></span>
 
5. <span data-ttu-id="e0971-121">**Common Data Service txantiloia** eremuan, hautatu **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="e0971-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="e0971-122">Hautatu inplementazioaren ingurune mota.</span><span class="sxs-lookup"><span data-stu-id="e0971-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="e0971-123">Harpidetzan oinarritutako probak CDS ingurunea 30 egunez zabaltzen utziko dizu.</span><span class="sxs-lookup"><span data-stu-id="e0971-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Inplementazio-ezarpenak](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="e0971-125">Aukeratu **Ados** zerbitzuaren baldintzak onartzeko eta ondoren hautatu **Eginda** inplementazio-ezarpenetara itzultzeko.</span><span class="sxs-lookup"><span data-stu-id="e0971-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Inplementazioaren onespena](./media/2DeploymentConsent.png)

7. <span data-ttu-id="e0971-127">Osatu morroian beharrezko gainerako eremuak eta berretsi inplementazioa.</span><span class="sxs-lookup"><span data-stu-id="e0971-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="e0971-128">Ingurumena hornitzeko denbora aldatu egiten da ingurune motaren arabera.</span><span class="sxs-lookup"><span data-stu-id="e0971-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="e0971-129">Hornidurak sei ordu behar izan ditzake.</span><span class="sxs-lookup"><span data-stu-id="e0971-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="e0971-130">Inplementazioa ondo burutu ondoren, ingurunea honela agertuko da **Inplementatuta**.</span><span class="sxs-lookup"><span data-stu-id="e0971-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="e0971-131">Ingurunea ondo zabaldu dela ziurtatzeko, hautatu **Saioa hasi** eta saioa hasi ingurunean berresteko.</span><span class="sxs-lookup"><span data-stu-id="e0971-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![ Ingurune-xehetasunak](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="e0971-133">Aplikatu Project Operations Finance demo-datuak (aukerako urratsa)</span><span class="sxs-lookup"><span data-stu-id="e0971-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="e0971-134">Aplikatu Project Operations Finance demo-datuak 10.0.13 zerbitzuaren bertsioan Hodeian ostatatutako ingurunean deskribatutako moduan [artikulu hau](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="e0971-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="e0971-135">Aplikatu eguneratzeak Finance ingurunean</span><span class="sxs-lookup"><span data-stu-id="e0971-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="e0971-136">Project Operations-ek Finance ingurunea behar dute aplikazioaren **10.0.13 (10.0.569.20009)** bertsioarekin edo berriagoarekin.</span><span class="sxs-lookup"><span data-stu-id="e0971-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="e0971-137">Baliteke kalitate-eguneratzeak aplikatzea zure Finance inguruneari bertsio hau jasotzeko.</span><span class="sxs-lookup"><span data-stu-id="e0971-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="e0971-138">LCSn **Ingurumenaren xehetasunak** orrialdean, **Eguneratze erabilgarriak** sekzioan, hautatu **Ikusi eguneratzea**.</span><span class="sxs-lookup"><span data-stu-id="e0971-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Ikusi eguneratzeak](./media/5ViewUpdates.png)

2. <span data-ttu-id="e0971-140">**Eguneratze bitarrak** orrialdean, hautatu **Gorde paketea.**</span><span class="sxs-lookup"><span data-stu-id="e0971-140">On the **Binary updates** page, select **Save package.**</span></span>

![Gorde paketea](./media/6SavePackage.png)

3. <span data-ttu-id="e0971-142">Sakatu **Hautatu guztiak** eta hautatu **Gorde paketea**.</span><span class="sxs-lookup"><span data-stu-id="e0971-142">Click **Select all** and then select **Save package**.</span></span>

![Berrikusi eta gorde eguneratzeak](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="e0971-144">Idatzi paketearen izena eta deskribapena, eta hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="e0971-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="e0971-145">Interneteko konexioaren arabera, baliteke prozesu honek denbora pixka bat behar izatea.</span><span class="sxs-lookup"><span data-stu-id="e0971-145">Depending on the internet connection, this process might take some time.</span></span>

![Kargatu paketea Aktiboen liburutegira](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="e0971-147">Paketea gorde ondoren, hautatu **Eginda** eta gorde pakete hau Aktiboen liburutegian zure LCS proiektuan.</span><span class="sxs-lookup"><span data-stu-id="e0971-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="e0971-148">Paketea gorde eta balioztatzeak ~ 15 minutu behar izan ditzake.</span><span class="sxs-lookup"><span data-stu-id="e0971-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="e0971-149">Eguneratzea aplikatzeko, joan **Ingurumenaren xehetasunak** orrialdea LCSn eta hautatu **Mantendu** > **Aplikatu eguneratzeak**.</span><span class="sxs-lookup"><span data-stu-id="e0971-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Mantendu inguruneak](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="e0971-151">Eguneratzeen zerrendan hautatu sortu duzun paketea eta hautatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="e0971-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Aplikatu eguneraketak](./media/10ApplyUpdates.png)

<span data-ttu-id="e0971-153">Ingurumena zaintzeko denbora pixka bat beharko da.</span><span class="sxs-lookup"><span data-stu-id="e0971-153">Environment servicing will take some time.</span></span> <span data-ttu-id="e0971-154">Bukatu ondoren, ingurunea hedatutako egoerara itzuliko da.</span><span class="sxs-lookup"><span data-stu-id="e0971-154">After it is complete, the environment will return to a deployed state.</span></span>

![Inplementatutako inguruneak](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="e0971-156">Ezarri idazketa dualeko konexioa</span><span class="sxs-lookup"><span data-stu-id="e0971-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="e0971-157">Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.</span><span class="sxs-lookup"><span data-stu-id="e0971-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="e0971-158">**Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**.</span><span class="sxs-lookup"><span data-stu-id="e0971-158">Under **Common Data Service Environment Information** , select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="e0971-159">Esteka osatu ondoren, hautatu **Estekatu aplikazioetarako CDS** berriro.</span><span class="sxs-lookup"><span data-stu-id="e0971-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="e0971-160">Finantzetan Idazketa Dualera bideratuko zaituzte.</span><span class="sxs-lookup"><span data-stu-id="e0971-160">You will be redirected to Dual Write in Finance.</span></span>

![Estekatu CDSra](./media/12LinktoCDS.png)

4. <span data-ttu-id="e0971-162">Aukeratu **Aplikatu irtenbidea** integrazioan mapatuko diren entitateetara sartzeko.</span><span class="sxs-lookup"><span data-stu-id="e0971-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Aplikatu soluzioak](./media/13ApplySolutions.png)

5. <span data-ttu-id="e0971-164">Aukeratu bi irtenbideak, **Dynamics 365 Finance and Operations Idazketa bikoitzeko entitateen mapa** eta **Dynamics 365 Project Operations Idazketa bikoitzeko entitateen mapak** eta, ondoren, hautatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="e0971-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps** , and then select **Apply**.</span></span>

![Berretsi irtenbideak](./media/14ConfirmSolutions.png)

<span data-ttu-id="e0971-166">Irtenbideak aplikatu ondoren, Idazketa Dualeko entitateak inguruneari aplikatuko zaizkio.</span><span class="sxs-lookup"><span data-stu-id="e0971-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Soluzioak aplikatzea](./media/15ApplyingSolutions.png)

<span data-ttu-id="e0971-168">Entitateak aplikatu ondoren, erabilgarri dauden mapaketa guztiak ingurunean zerrendatzen dira.</span><span class="sxs-lookup"><span data-stu-id="e0971-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Idazketa dualaren esleipenak](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="e0971-170">Freskatu datu-entitateak eguneratu ondoren</span><span class="sxs-lookup"><span data-stu-id="e0971-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="e0971-171">Finantzetan, joan **Datuen kudeaketa** lan eremua.</span><span class="sxs-lookup"><span data-stu-id="e0971-171">In Finance, go to the **Data management** workspace.</span></span>

![Datu-kudeaketarren laneko area](./media/16DataManagement.png)

2. <span data-ttu-id="e0971-173">Aukeratu **Esparru parametroak** lauza.</span><span class="sxs-lookup"><span data-stu-id="e0971-173">Select the **Framework parameters** tile.</span></span>

![Esparru-parametroak](./media/17FrameworkParameters.png)

3. <span data-ttu-id="e0971-175">**Entitatearen ezarpenak** orrialdean, hautatu **Freskatu entitate zerrenda**.</span><span class="sxs-lookup"><span data-stu-id="e0971-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Freskatu entitate-zerrenda](./media/18RefreshEntityList.png)

<span data-ttu-id="e0971-177">Freskatzeak 20 minutu inguru iraungo du.</span><span class="sxs-lookup"><span data-stu-id="e0971-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="e0971-178">Amaitutakoan alerta jasoko duzu.</span><span class="sxs-lookup"><span data-stu-id="e0971-178">You will receive an alert when it is complete.</span></span>

![Freskatzeko berrespena](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="e0971-180">Exekutatu Proiektuaren eragiketen idazketa dualaren esleipenak</span><span class="sxs-lookup"><span data-stu-id="e0971-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="e0971-181">Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.</span><span class="sxs-lookup"><span data-stu-id="e0971-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="e0971-182">**Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**.</span><span class="sxs-lookup"><span data-stu-id="e0971-182">Under **Common Data Service Environment Information** , select **Link to CDS for Apps.**</span></span> <span data-ttu-id="e0971-183">Esteka hautatu ondoren, mapen entitateen zerrendara birbideratuko zaituzte.</span><span class="sxs-lookup"><span data-stu-id="e0971-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="e0971-184">Hasi esleipenak hurrengo taulan deskribatzen den bezala.</span><span class="sxs-lookup"><span data-stu-id="e0971-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="e0971-185">Ziurtatu zerrendatutako sekuentzia jarraitzen duzula.</span><span class="sxs-lookup"><span data-stu-id="e0971-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="e0971-186">**Entitate-esleipena**</span><span class="sxs-lookup"><span data-stu-id="e0971-186">**Entity Map**</span></span> | <span data-ttu-id="e0971-187">**Freskatu entitatea**</span><span class="sxs-lookup"><span data-stu-id="e0971-187">**Refresh entity**</span></span> | <span data-ttu-id="e0971-188">**Hasierako sinkronizazioa**</span><span class="sxs-lookup"><span data-stu-id="e0971-188">**Initial sync**</span></span> | <span data-ttu-id="e0971-189">**Hasierako sinkronizazioaren eredua**</span><span class="sxs-lookup"><span data-stu-id="e0971-189">**Master for initial sync**</span></span> | <span data-ttu-id="e0971-190">**Exekutatu aurrebaldintzak**</span><span class="sxs-lookup"><span data-stu-id="e0971-190">**Run prerequisites**</span></span> | <span data-ttu-id="e0971-191">**Aurrebaldintzen hasierako sinkronizazioa**</span><span class="sxs-lookup"><span data-stu-id="e0971-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="e0971-192">**Enpresa guztientzako proiektuaren baliabideen eginkizunak (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="e0971-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="e0971-193">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-193">No</span></span> | <span data-ttu-id="e0971-194">Yes</span><span class="sxs-lookup"><span data-stu-id="e0971-194">Yes</span></span> | <span data-ttu-id="e0971-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="e0971-195">Common Data Service</span></span> | <span data-ttu-id="e0971-196">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-196">No</span></span> | <span data-ttu-id="e0971-197">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-197">N\A</span></span> |
| <span data-ttu-id="e0971-198">**Legezko entitateak (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="e0971-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="e0971-199">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-199">No</span></span> | <span data-ttu-id="e0971-200">Yes</span><span class="sxs-lookup"><span data-stu-id="e0971-200">Yes</span></span> | <span data-ttu-id="e0971-201">Finance and Operations aplikazioak</span><span class="sxs-lookup"><span data-stu-id="e0971-201">Finance and Operations apps</span></span> | <span data-ttu-id="e0971-202">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-202">No</span></span> | <span data-ttu-id="e0971-203">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-203">N\A</span></span> |
| <span data-ttu-id="e0971-204">**Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="e0971-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="e0971-205">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-205">No</span></span> | <span data-ttu-id="e0971-206">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-206">No</span></span> | <span data-ttu-id="e0971-207">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-207">N\A</span></span> | <span data-ttu-id="e0971-208">Yes</span><span class="sxs-lookup"><span data-stu-id="e0971-208">Yes</span></span> | <span data-ttu-id="e0971-209">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-209">No</span></span> |
| <span data-ttu-id="e0971-210">**Proiektuetako kontratuaren lerroak (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="e0971-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="e0971-211">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-211">No</span></span> | <span data-ttu-id="e0971-212">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-212">No</span></span> | <span data-ttu-id="e0971-213">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-213">N\A</span></span> | <span data-ttu-id="e0971-214">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-214">No</span></span> | <span data-ttu-id="e0971-215">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-215">No</span></span> |
| <span data-ttu-id="e0971-216">**Proiektuen transakzio harremanetarako integrazio entitatea (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="e0971-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="e0971-217">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-217">No</span></span> | <span data-ttu-id="e0971-218">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-218">No</span></span> | <span data-ttu-id="e0971-219">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-219">N\A</span></span> | <span data-ttu-id="e0971-220">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-220">No</span></span> | <span data-ttu-id="e0971-221">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-221">N\A</span></span> |
| <span data-ttu-id="e0971-222">**Project Operations-ek integratzeko kontratu lerroaren mugarriak (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="e0971-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="e0971-223">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-223">No</span></span> | <span data-ttu-id="e0971-224">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-224">No</span></span> | <span data-ttu-id="e0971-225">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-225">N\A</span></span> | <span data-ttu-id="e0971-226">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-226">No</span></span> | <span data-ttu-id="e0971-227">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-227">N\A</span></span> |
| <span data-ttu-id="e0971-228">**Project Operations-ek integratzeko entitatea gastuen kalkuluen arabera (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="e0971-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="e0971-229">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-229">No</span></span> | <span data-ttu-id="e0971-230">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-230">No</span></span> | <span data-ttu-id="e0971-231">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-231">N\A</span></span> | <span data-ttu-id="e0971-232">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-232">No</span></span> | <span data-ttu-id="e0971-233">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-233">N\A</span></span> |
| <span data-ttu-id="e0971-234">**Project Operations-ek integratzeko proiektuaren gastuak kategoriak esportatzeko entitatea (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="e0971-234">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="e0971-235">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-235">No</span></span> | <span data-ttu-id="e0971-236">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-236">No</span></span> | <span data-ttu-id="e0971-237">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-237">N\A</span></span> | <span data-ttu-id="e0971-238">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-238">No</span></span> | <span data-ttu-id="e0971-239">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-239">N\A</span></span> |
| <span data-ttu-id="e0971-240">**Project Operations-ek integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="e0971-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="e0971-241">Yes</span><span class="sxs-lookup"><span data-stu-id="e0971-241">Yes</span></span> | <span data-ttu-id="e0971-242">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-242">No</span></span> | <span data-ttu-id="e0971-243">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-243">N\A</span></span> | <span data-ttu-id="e0971-244">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-244">No</span></span> | <span data-ttu-id="e0971-245">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-245">N\A</span></span> |
| <span data-ttu-id="e0971-246">**Project Operations-ek integratzeko entitatea orduen kalkuluen arabera (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="e0971-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="e0971-247">Yes</span><span class="sxs-lookup"><span data-stu-id="e0971-247">Yes</span></span> | <span data-ttu-id="e0971-248">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-248">No</span></span> | <span data-ttu-id="e0971-249">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-249">N\A</span></span> | <span data-ttu-id="e0971-250">+Ez</span><span class="sxs-lookup"><span data-stu-id="e0971-250">No</span></span> | <span data-ttu-id="e0971-251">E/E</span><span class="sxs-lookup"><span data-stu-id="e0971-251">N\A</span></span> |


4. <span data-ttu-id="e0971-252">Entitatea freskatzeko, hautatu maparen izena eta hautatu **Freskatu entitateak**.</span><span class="sxs-lookup"><span data-stu-id="e0971-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Freskatu mapa](./media/20RefreshMapping.png)

5. <span data-ttu-id="e0971-254">Freskatzen osatu eta gero, exekutatu mapa.</span><span class="sxs-lookup"><span data-stu-id="e0971-254">After the refresh is complete, run the map.</span></span> <span data-ttu-id="e0971-255">Hurrengo mapa gaitu aurretik, egiaztatu taulako mapa egoera batean dagoela **Exekutatzen**.</span><span class="sxs-lookup"><span data-stu-id="e0971-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="e0971-256">Aurrebaldintza kopuru handiagoa duten mapak exekutatzeak denbora pixka bat behar izan dezake.</span><span class="sxs-lookup"><span data-stu-id="e0971-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="e0971-257">Aurrebaldintzak dituen mapa exekutatzeko, gaitu **Erakutsi erlazionatutako entitateen mapak** txandakatu.</span><span class="sxs-lookup"><span data-stu-id="e0971-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="e0971-258">Taulak adierazten badu **Hasierako sinkronizazioa** da **Ez** , egiaztatu **Hasierako sinkronizazioa** bandera da **Desaktibatuta** exekutatu aurretik aurrebaldintza-mapa guztietan.</span><span class="sxs-lookup"><span data-stu-id="e0971-258">If the table indicates **Prerequisite initial sync** is **No** , verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Exekutatu mapa](./media/21RunMap.png)

6. <span data-ttu-id="e0971-260">Balioztatu proiektuarekin lotutako mapa guztiak martxan daudenean.</span><span class="sxs-lookup"><span data-stu-id="e0971-260">Validate all project related maps are in the running state.</span></span>

![Mapa guztiak martxan](./media/22AllMapsRunning.png)

<span data-ttu-id="e0971-262">Zure Project Operations ingurunea hornitu eta konfiguratuta dago orain.</span><span class="sxs-lookup"><span data-stu-id="e0971-262">Your Project Operations environment is now provisioned and configured.</span></span>
