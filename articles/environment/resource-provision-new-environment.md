---
title: Eman ingurune berri bat
description: Gai honek Project Operations ingurune berri bat emateari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 9ee9e4c31d1972e3a75ad214071b31527f0ca826
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950519"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="20ddd-103">Eman ingurune berri bat</span><span class="sxs-lookup"><span data-stu-id="20ddd-103">Provision a new environment</span></span>

<span data-ttu-id="20ddd-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="20ddd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="20ddd-105">Gai honek baliabidean / pilatu gabeko egoeretako Dynamics 365 Project Operations ingurune berria emateko moduari buruzko informazioa ematen du.</span><span class="sxs-lookup"><span data-stu-id="20ddd-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="20ddd-106">Gaitu Project Operations hornidura automatikoa LCS proiektu batean</span><span class="sxs-lookup"><span data-stu-id="20ddd-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="20ddd-107">Erabili urrats hauek zure LCS proiekturako Project Operations hornidura-fluxu automatikoa gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="20ddd-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="20ddd-108">Joan [LCS](https://lcs.dynamics.com/v2) aukerara eta hautatu **Aurreikusi funtzioen kudeaketa** lauza.</span><span class="sxs-lookup"><span data-stu-id="20ddd-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="20ddd-109">**Aurrebista eginbidea** zerrendan, hautatu **Project Operations eginbidea** eta, ondoren, hautatu **Aurrebista eginbidea gaituta** Project Operations gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="20ddd-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="20ddd-110">Urrats hau LCS proiektu bakoitzeko behin bakarrik egiten da.</span><span class="sxs-lookup"><span data-stu-id="20ddd-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="20ddd-111">Project Operations ingurunea hornitzea</span><span class="sxs-lookup"><span data-stu-id="20ddd-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="20ddd-112">Ireki Dynamics 365 Finance [demo-ingurunea](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) edo [sandbox / produkzio ingurunea](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) inplementazioa.</span><span class="sxs-lookup"><span data-stu-id="20ddd-112">Open a new Dynamics 365 Finance [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="20ddd-113">**Ingurumen hornidura** morroia eramatea.</span><span class="sxs-lookup"><span data-stu-id="20ddd-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="20ddd-114">Ziurtatu hautatutako aplikazioaren bertsioa 10.0.13 edo berriagoa dela.</span><span class="sxs-lookup"><span data-stu-id="20ddd-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="20ddd-115">Project Operations hornitzeko, **Ezarpen aurreratuak** aukeran, hautatu **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="20ddd-116">Gaitu **Common Data Service ezarpena** **Bai** hautatuta, eta ondoren sartu informazioa beharrezko eremuetan:</span><span class="sxs-lookup"><span data-stu-id="20ddd-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="20ddd-117">Izena</span><span class="sxs-lookup"><span data-stu-id="20ddd-117">Name</span></span>
  - <span data-ttu-id="20ddd-118">Eskualdea</span><span class="sxs-lookup"><span data-stu-id="20ddd-118">Region</span></span>
  - <span data-ttu-id="20ddd-119">Hizkuntza</span><span class="sxs-lookup"><span data-stu-id="20ddd-119">Language</span></span>
  - <span data-ttu-id="20ddd-120">Moneta</span><span class="sxs-lookup"><span data-stu-id="20ddd-120">Currency</span></span>
 
5. <span data-ttu-id="20ddd-121">**Common Data Service txantiloia** eremuan, hautatu **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="20ddd-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="20ddd-122">Hautatu inplementazioaren ingurune mota.</span><span class="sxs-lookup"><span data-stu-id="20ddd-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="20ddd-123">Harpidetzan oinarritutako probak CDS ingurunea 30 egunez zabaltzen utziko dizu.</span><span class="sxs-lookup"><span data-stu-id="20ddd-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![Inplementazio-ezarpenak](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="20ddd-125">Aukeratu **Ados** zerbitzuaren baldintzak onartzeko eta ondoren hautatu **Eginda** inplementazio-ezarpenetara itzultzeko.</span><span class="sxs-lookup"><span data-stu-id="20ddd-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![Inplementazioaren onespena](./media/2DeploymentConsent.png)

7. <span data-ttu-id="20ddd-127">Aukerakoa - Aplikatu demo datuak inguruneari.</span><span class="sxs-lookup"><span data-stu-id="20ddd-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="20ddd-128">Joan **Ezarpen aurreratuak** aukerara, hautatu **Pertsonalizatu SQL datu basearen konfigurazioa**, eta ezarri **Zehaztu datu-basea aplikazioen datu-baserako** **Demoa** gisa.</span><span class="sxs-lookup"><span data-stu-id="20ddd-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="20ddd-129">Osatu morroian beharrezko gainerako eremuak eta berretsi inplementazioa.</span><span class="sxs-lookup"><span data-stu-id="20ddd-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="20ddd-130">Ingurunea hornitzeko denbora aldatu egiten da ingurune motaren arabera.</span><span class="sxs-lookup"><span data-stu-id="20ddd-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="20ddd-131">Hornidurak sei ordu behar izan ditzake.</span><span class="sxs-lookup"><span data-stu-id="20ddd-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="20ddd-132">Inplementazioa ondo burutu ondoren, ingurunea honela agertuko da **Inplementatuta**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="20ddd-133">Ingurunea behar bezala zabaldu dela baieztatzeko, hautatu **Hasi saioa** eta saioa hasi ingurunean berresteko.</span><span class="sxs-lookup"><span data-stu-id="20ddd-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![ Ingurune-xehetasunak](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="20ddd-135">Aplikatu eguneratzeak Finance ingurunean</span><span class="sxs-lookup"><span data-stu-id="20ddd-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="20ddd-136">Project Operations-ek Finance ingurunea behar dute aplikazioaren **10.0.13 (10.0.569.20009)** bertsioarekin edo berriagoarekin.</span><span class="sxs-lookup"><span data-stu-id="20ddd-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="20ddd-137">Baliteke kalitate-eguneratzeak aplikatzea zure Finance inguruneari bertsio hau jasotzeko.</span><span class="sxs-lookup"><span data-stu-id="20ddd-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="20ddd-138">LCSn **Ingurumenaren xehetasunak** orrialdean, **Eguneratze erabilgarriak** sekzioan, hautatu **Ikusi eguneratzea**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![Ikusi eguneratzeak](./media/5ViewUpdates.png)

2. <span data-ttu-id="20ddd-140">**Eguneratze bitarrak** orrialdean, hautatu **Gorde paketea.**</span><span class="sxs-lookup"><span data-stu-id="20ddd-140">On the **Binary updates** page, select **Save package.**</span></span>

![Gorde paketea](./media/6SavePackage.png)

3. <span data-ttu-id="20ddd-142">Sakatu **Hautatu guztiak** eta hautatu **Gorde paketea**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-142">Click **Select all** and then select **Save package**.</span></span>

![Berrikusi eta gorde eguneratzeak](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="20ddd-144">Idatzi paketearen izena eta deskribapena, eta hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="20ddd-145">Interneteko konexioaren arabera, baliteke prozesu honek denbora pixka bat behar izatea.</span><span class="sxs-lookup"><span data-stu-id="20ddd-145">Depending on the internet connection, this process might take some time.</span></span>

![Kargatu paketea Aktiboen liburutegira](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="20ddd-147">Paketea gorde ondoren, hautatu **Eginda** eta gorde pakete hau Aktiboen liburutegian zure LCS proiektuan.</span><span class="sxs-lookup"><span data-stu-id="20ddd-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="20ddd-148">Paketea gorde eta balioztatzeak ~ 15 minutu behar izan ditzake.</span><span class="sxs-lookup"><span data-stu-id="20ddd-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="20ddd-149">Eguneratzea aplikatzeko, joan **Ingurumenaren xehetasunak** orrialdea LCSn eta hautatu **Mantendu** > **Aplikatu eguneratzeak**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![Mantendu inguruneak](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="20ddd-151">Eguneratzeen zerrendan hautatu sortu duzun paketea eta hautatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-151">In the updates list select the package you created, and select **Apply**.</span></span>

![Aplikatu eguneraketak](./media/10ApplyUpdates.png)

<span data-ttu-id="20ddd-153">Ingurumena zaintzeko denbora pixka bat beharko da.</span><span class="sxs-lookup"><span data-stu-id="20ddd-153">Environment servicing will take some time.</span></span> <span data-ttu-id="20ddd-154">Bukatu ondoren, ingurunea hedatutako egoerara itzuliko da.</span><span class="sxs-lookup"><span data-stu-id="20ddd-154">After it is complete, the environment will return to a deployed state.</span></span>

![Inplementatutako inguruneak](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="20ddd-156">Ezarri idazketa dualeko konexioa</span><span class="sxs-lookup"><span data-stu-id="20ddd-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="20ddd-157">Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.</span><span class="sxs-lookup"><span data-stu-id="20ddd-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="20ddd-158">**Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="20ddd-159">Esteka osatu ondoren, hautatu **Estekatu aplikazioetarako CDS** berriro.</span><span class="sxs-lookup"><span data-stu-id="20ddd-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="20ddd-160">Finantzetan Idazketa Dualera bideratuko zaituzte.</span><span class="sxs-lookup"><span data-stu-id="20ddd-160">You will be redirected to Dual Write in Finance.</span></span>

![Estekatu CDSra](./media/12LinktoCDS.png)

4. <span data-ttu-id="20ddd-162">Aukeratu **Aplikatu irtenbidea** integrazioan mapatuko diren entitateetara sartzeko.</span><span class="sxs-lookup"><span data-stu-id="20ddd-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![Aplikatu soluzioak](./media/13ApplySolutions.png)

5. <span data-ttu-id="20ddd-164">Aukeratu bi irtenbideak, **Dynamics 365 Finance and Operations Idazketa bikoitzeko entitateen mapa** eta **Dynamics 365 Project Operations Idazketa bikoitzeko entitateen mapak** eta, ondoren, hautatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![Berretsi irtenbideak](./media/14ConfirmSolutions.png)

<span data-ttu-id="20ddd-166">Irtenbideak aplikatu ondoren, Idazketa Dualeko entitateak inguruneari aplikatuko zaizkio.</span><span class="sxs-lookup"><span data-stu-id="20ddd-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![Soluzioak aplikatzea](./media/15ApplyingSolutions.png)

<span data-ttu-id="20ddd-168">Entitateak aplikatu ondoren, erabilgarri dauden mapaketa guztiak ingurunean zerrendatzen dira.</span><span class="sxs-lookup"><span data-stu-id="20ddd-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![Idazketa dualaren esleipenak](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="20ddd-170">Freskatu datu-entitateak eguneratu ondoren</span><span class="sxs-lookup"><span data-stu-id="20ddd-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="20ddd-171">Finantzetan, joan **Datuen kudeaketa** lan eremua.</span><span class="sxs-lookup"><span data-stu-id="20ddd-171">In Finance, go to the **Data management** workspace.</span></span>

![Datu-kudeaketarren laneko area](./media/16DataManagement.png)

2. <span data-ttu-id="20ddd-173">Aukeratu **Esparru parametroak** lauza.</span><span class="sxs-lookup"><span data-stu-id="20ddd-173">Select the **Framework parameters** tile.</span></span>

![Esparru-parametroak](./media/17FrameworkParameters.png)

3. <span data-ttu-id="20ddd-175">**Entitatearen ezarpenak** orrialdean, hautatu **Freskatu entitate zerrenda**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![Freskatu entitate-zerrenda](./media/18RefreshEntityList.png)

<span data-ttu-id="20ddd-177">Freskatzeak 20 minutu inguru iraungo du.</span><span class="sxs-lookup"><span data-stu-id="20ddd-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="20ddd-178">Amaitutakoan alerta jasoko duzu.</span><span class="sxs-lookup"><span data-stu-id="20ddd-178">You will receive an alert when it is complete.</span></span>

![Freskatzeko berrespena](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="20ddd-180">Eguneratu Project Operations-eko segurtasun-ezarpenak aktibatuta Dataverse-n</span><span class="sxs-lookup"><span data-stu-id="20ddd-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="20ddd-181">Joan Project Operations aukerara, Dataverse ingurunean.</span><span class="sxs-lookup"><span data-stu-id="20ddd-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="20ddd-182">Joan **Ezarpenak** > **Segurtasuna** > **Segurtasun-funtzioak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="20ddd-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="20ddd-183">**Segurtasun-funtzioak** orrialdean, funtzioen zerrendan, hautatu **idazketa bikoitzeko aplikazioaren erabiltzailea** eta hautatu **Entitate pertsonalizatuak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="20ddd-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="20ddd-184">Egiaztatu rolak funtzioak badituela **Irakurri** eta **Erantsi honi** honetarako baimenak:</span><span class="sxs-lookup"><span data-stu-id="20ddd-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="20ddd-185">**Monetaren truke-tasaren mota**</span><span class="sxs-lookup"><span data-stu-id="20ddd-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="20ddd-186">**Kontuen sailkapena**</span><span class="sxs-lookup"><span data-stu-id="20ddd-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="20ddd-187">**Egutegi fiskala**</span><span class="sxs-lookup"><span data-stu-id="20ddd-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="20ddd-188">**Liburua**</span><span class="sxs-lookup"><span data-stu-id="20ddd-188">**Ledger**</span></span>

5. <span data-ttu-id="20ddd-189">Segurtasun-funtzio eguneratu ondoren, joan **Ezarpenak** > **Segurtasuna** > **Taldeak** aukerara, eta hautatu lehenetsitako taldea **Tokiko negozioaren jabea** taldearen ikuspegia.</span><span class="sxs-lookup"><span data-stu-id="20ddd-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="20ddd-190">Aukeratu **Kudeatu funtzioak** eta egiaztatu **idazketa bikoitzeko aplikazioaren erabiltzailea** segurtasun-pribilegioa talde honi aplikatzen zaio.</span><span class="sxs-lookup"><span data-stu-id="20ddd-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="20ddd-191">Exekutatu Proiektuaren eragiketen idazketa dualaren esleipenak</span><span class="sxs-lookup"><span data-stu-id="20ddd-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="20ddd-192">Zure LCS proiektuan, joan **Ingurumenaren xehetasunak** orrialdera.</span><span class="sxs-lookup"><span data-stu-id="20ddd-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="20ddd-193">**Common Data Service Ingurumenari buruzko informazioa** aukeran, hautatu **Lotu aplikazioetarako CDS**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="20ddd-194">Esteka hautatu ondoren, mapen entitateen zerrendara birbideratuko zaituzte.</span><span class="sxs-lookup"><span data-stu-id="20ddd-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="20ddd-195">Hasi esleipenak hurrengo taulan deskribatzen den bezala.</span><span class="sxs-lookup"><span data-stu-id="20ddd-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="20ddd-196">Ziurtatu zerrendatutako sekuentzia jarraitzen duzula.</span><span class="sxs-lookup"><span data-stu-id="20ddd-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="20ddd-197">**Entitate-esleipena**</span><span class="sxs-lookup"><span data-stu-id="20ddd-197">**Entity Map**</span></span> | <span data-ttu-id="20ddd-198">**Freskatu entitatea**</span><span class="sxs-lookup"><span data-stu-id="20ddd-198">**Refresh entity**</span></span> | <span data-ttu-id="20ddd-199">**Hasierako sinkronizazioa**</span><span class="sxs-lookup"><span data-stu-id="20ddd-199">**Initial sync**</span></span> | <span data-ttu-id="20ddd-200">**Hasierako sinkronizazioaren eredua**</span><span class="sxs-lookup"><span data-stu-id="20ddd-200">**Master for initial sync**</span></span> | <span data-ttu-id="20ddd-201">**Exekutatu aurrebaldintzak**</span><span class="sxs-lookup"><span data-stu-id="20ddd-201">**Run prerequisites**</span></span> | <span data-ttu-id="20ddd-202">**Aurrebaldintzen hasierako sinkronizazioa**</span><span class="sxs-lookup"><span data-stu-id="20ddd-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="20ddd-203">**Enpresa guztientzako proiektuaren baliabideen eginkizunak (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="20ddd-204">No</span><span class="sxs-lookup"><span data-stu-id="20ddd-204">No</span></span> | <span data-ttu-id="20ddd-205">Yes</span><span class="sxs-lookup"><span data-stu-id="20ddd-205">Yes</span></span> | <span data-ttu-id="20ddd-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="20ddd-206">Common Data Service</span></span> | <span data-ttu-id="20ddd-207">No</span><span class="sxs-lookup"><span data-stu-id="20ddd-207">No</span></span> | <span data-ttu-id="20ddd-208">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-208">N\A</span></span> |
| <span data-ttu-id="20ddd-209">**Legezko entitateak (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="20ddd-210">No</span><span class="sxs-lookup"><span data-stu-id="20ddd-210">No</span></span> | <span data-ttu-id="20ddd-211">Yes</span><span class="sxs-lookup"><span data-stu-id="20ddd-211">Yes</span></span> | <span data-ttu-id="20ddd-212">Finance and Operations aplikazioak</span><span class="sxs-lookup"><span data-stu-id="20ddd-212">Finance and Operations apps</span></span> | <span data-ttu-id="20ddd-213">No</span><span class="sxs-lookup"><span data-stu-id="20ddd-213">No</span></span> | <span data-ttu-id="20ddd-214">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-214">N\A</span></span> |
| <span data-ttu-id="20ddd-215">**Liburua (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="20ddd-216">No</span><span class="sxs-lookup"><span data-stu-id="20ddd-216">No</span></span> | <span data-ttu-id="20ddd-217">Yes</span><span class="sxs-lookup"><span data-stu-id="20ddd-217">Yes</span></span> | <span data-ttu-id="20ddd-218">Finance and Operations aplikazioak</span><span class="sxs-lookup"><span data-stu-id="20ddd-218">Finance and Operations apps</span></span> | <span data-ttu-id="20ddd-219">Yes</span><span class="sxs-lookup"><span data-stu-id="20ddd-219">Yes</span></span> | <span data-ttu-id="20ddd-220">Bai, Finance and Operations aplikazioak</span><span class="sxs-lookup"><span data-stu-id="20ddd-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="20ddd-221">**Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="20ddd-222">No</span><span class="sxs-lookup"><span data-stu-id="20ddd-222">No</span></span> | <span data-ttu-id="20ddd-223">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-223">No</span></span> | <span data-ttu-id="20ddd-224">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-224">N\A</span></span> | <span data-ttu-id="20ddd-225">Yes</span><span class="sxs-lookup"><span data-stu-id="20ddd-225">Yes</span></span> | <span data-ttu-id="20ddd-226">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-226">No</span></span> |
| <span data-ttu-id="20ddd-227">**Proiektuetako kontratuaren lerroak (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="20ddd-228">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-228">No</span></span> | <span data-ttu-id="20ddd-229">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-229">No</span></span> | <span data-ttu-id="20ddd-230">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-230">N\A</span></span> | <span data-ttu-id="20ddd-231">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-231">No</span></span> | <span data-ttu-id="20ddd-232">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-232">No</span></span> |
| <span data-ttu-id="20ddd-233">**Proiektuen transakzio harremanetarako integrazio entitatea (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="20ddd-234">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-234">No</span></span> | <span data-ttu-id="20ddd-235">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-235">No</span></span> | <span data-ttu-id="20ddd-236">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-236">N\A</span></span> | <span data-ttu-id="20ddd-237">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-237">No</span></span> | <span data-ttu-id="20ddd-238">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-238">N\A</span></span> |
| <span data-ttu-id="20ddd-239">**Project Operations-ek integratzeko kontratu lerroaren mugarriak (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="20ddd-240">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-240">No</span></span> | <span data-ttu-id="20ddd-241">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-241">No</span></span> | <span data-ttu-id="20ddd-242">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-242">N\A</span></span> | <span data-ttu-id="20ddd-243">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-243">No</span></span> | <span data-ttu-id="20ddd-244">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-244">N\A</span></span> |
| <span data-ttu-id="20ddd-245">**Project Operations-ek integratzeko entitatea gastuen kalkuluen arabera (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="20ddd-246">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-246">No</span></span> | <span data-ttu-id="20ddd-247">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-247">No</span></span> | <span data-ttu-id="20ddd-248">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-248">N\A</span></span> | <span data-ttu-id="20ddd-249">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-249">No</span></span> | <span data-ttu-id="20ddd-250">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-250">N\A</span></span> |
| <span data-ttu-id="20ddd-251">**Project Operations-ek integratzeko proiektuaren gastuak kategoriak esportatzeko entitatea (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="20ddd-252">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-252">No</span></span> | <span data-ttu-id="20ddd-253">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-253">No</span></span> | <span data-ttu-id="20ddd-254">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-254">N\A</span></span> | <span data-ttu-id="20ddd-255">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-255">No</span></span> | <span data-ttu-id="20ddd-256">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-256">N\A</span></span> |
| <span data-ttu-id="20ddd-257">**Project Operations-ek integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="20ddd-258">Yes</span><span class="sxs-lookup"><span data-stu-id="20ddd-258">Yes</span></span> | <span data-ttu-id="20ddd-259">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-259">No</span></span> | <span data-ttu-id="20ddd-260">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-260">N\A</span></span> | <span data-ttu-id="20ddd-261">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-261">No</span></span> | <span data-ttu-id="20ddd-262">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-262">N\A</span></span> |
| <span data-ttu-id="20ddd-263">**Project Operations-ek integratzeko entitatea orduen kalkuluen arabera (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="20ddd-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="20ddd-264">Yes</span><span class="sxs-lookup"><span data-stu-id="20ddd-264">Yes</span></span> | <span data-ttu-id="20ddd-265">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-265">No</span></span> | <span data-ttu-id="20ddd-266">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-266">N\A</span></span> | <span data-ttu-id="20ddd-267">+Ez</span><span class="sxs-lookup"><span data-stu-id="20ddd-267">No</span></span> | <span data-ttu-id="20ddd-268">E/E</span><span class="sxs-lookup"><span data-stu-id="20ddd-268">N\A</span></span> |


4. <span data-ttu-id="20ddd-269">Entitatea freskatzeko, hautatu maparen izena eta hautatu **Freskatu entitateak**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![Freskatu mapa](./media/20RefreshMapping.png)

5. <span data-ttu-id="20ddd-271">Freskatzen osatu eta gero, exekutatu mapa.</span><span class="sxs-lookup"><span data-stu-id="20ddd-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="20ddd-272">Hurrengo mapa gaitu aurretik, egiaztatu taulako mapa egoera batean dagoela **Exekutatzen**.</span><span class="sxs-lookup"><span data-stu-id="20ddd-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="20ddd-273">Aurrebaldintza kopuru handiagoa duten mapak exekutatzeak denbora pixka bat behar izan dezake.</span><span class="sxs-lookup"><span data-stu-id="20ddd-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="20ddd-274">Aurrebaldintzak dituen mapa exekutatzeko, gaitu **Erakutsi erlazionatutako entitateen mapak** txandakatu.</span><span class="sxs-lookup"><span data-stu-id="20ddd-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="20ddd-275">Taulak adierazten badu **Hasierako sinkronizazioa** da **Ez**, egiaztatu **Hasierako sinkronizazioa** bandera da **Desaktibatuta** exekutatu aurretik aurrebaldintza-mapa guztietan.</span><span class="sxs-lookup"><span data-stu-id="20ddd-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![Exekutatu mapa](./media/21RunMap.png)

6. <span data-ttu-id="20ddd-277">Balioztatu proiektuarekin lotutako mapa guztiak martxan daudenean.</span><span class="sxs-lookup"><span data-stu-id="20ddd-277">Validate all project related maps are in the running state.</span></span>

![Mapa guztiak martxan](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="20ddd-279">Aplikatu konfigurazio-datuak Project Operations-en CDS-n (aukerakoa)</span><span class="sxs-lookup"><span data-stu-id="20ddd-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="20ddd-280">Demo datuak Finantza inguruneari aplikatu badizkiozu, ikusi [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service Project Operations-erako](resource-apply-pro-setup-config-data.md) CDS inguruneari demo datuak aplikatzeko.</span><span class="sxs-lookup"><span data-stu-id="20ddd-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="20ddd-281">Zure Project Operations ingurunea hornitu eta konfiguratuta dago orain.</span><span class="sxs-lookup"><span data-stu-id="20ddd-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]