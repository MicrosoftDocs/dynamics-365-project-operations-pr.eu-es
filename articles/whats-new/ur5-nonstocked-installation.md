---
title: Eguneratu Project Operations zure Finantza ingurunean
description: Gai honek Project Operations Dynamics 365 Finance ingurunean nola eguneratu jakiteko informazioa eskaintzen du.
author: ruhercul
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d85a180aa094a048b4422605b25151d10785f67d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6011041"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="c0859-103">Eguneratu Project Operations zure Finantza ingurunean</span><span class="sxs-lookup"><span data-stu-id="c0859-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="c0859-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c0859-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="c0859-105">Gai honek Dynamics 365 Project Operations Dynamics 365 Finance ingurunean nola eguneratu jakiteko informazioa eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="c0859-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="c0859-106">Project Operations-ek 5 eguneratzera (UR5) eguneratzeko hiru prozedura behar dira:</span><span class="sxs-lookup"><span data-stu-id="c0859-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="c0859-107">Inportatu paketea aurrebista proiektuan</span><span class="sxs-lookup"><span data-stu-id="c0859-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="c0859-108">Aplikatu eguneratzea</span><span class="sxs-lookup"><span data-stu-id="c0859-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="c0859-109">Eguneratu Dataverse ingurunea</span><span class="sxs-lookup"><span data-stu-id="c0859-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="c0859-110">Inportatu paketea LCS proiektura</span><span class="sxs-lookup"><span data-stu-id="c0859-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="c0859-111">Hasi saioa [Lifecycle Services-en (LCS)](https://lcs.dynamics.com/) Proiektuaren jabe edo Ingurumen kudeatzaile gisa.</span><span class="sxs-lookup"><span data-stu-id="c0859-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="c0859-112">Proiektuen zerrendan, hautatu zure LCS proiektua.</span><span class="sxs-lookup"><span data-stu-id="c0859-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="c0859-113">**Proiektua** orrialdean, **Inguruneak** taldean, ireki eguneratu nahi duzun ingurunea.</span><span class="sxs-lookup"><span data-stu-id="c0859-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="c0859-114">Egiaztatu ingurunea martxan dagoela.</span><span class="sxs-lookup"><span data-stu-id="c0859-114">Verify that the environment is running.</span></span> <span data-ttu-id="c0859-115">Hasten ez bada, hasi ingurunea.</span><span class="sxs-lookup"><span data-stu-id="c0859-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="c0859-116">**Argitalpen berria** sekzioan, **Eguneratze erabilgarriak** atalean, hautatu **Ikusi eguneratzea** 10.0.15 bertsioarena.</span><span class="sxs-lookup"><span data-stu-id="c0859-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

![Ikusi eguneratzea botoia](media/view-update.png)

6. <span data-ttu-id="c0859-118">**Eguneratze bitarrak** orrialdean, hautatu **Gorde paketea**.</span><span class="sxs-lookup"><span data-stu-id="c0859-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="c0859-119">**Berrikusi eta gorde eguneratzeak** orrialdean, hautatu **Gorde paketea**.</span><span class="sxs-lookup"><span data-stu-id="c0859-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="c0859-120">Irekitzen den **Gorde paketea aktiboen liburutegian** panelean, sartu paketearen izena eta hautatu **Gorde paketea**.</span><span class="sxs-lookup"><span data-stu-id="c0859-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="c0859-121">LCS paketea gordetzen amaitutakoan, **Eginda** botoia gaituta dago.</span><span class="sxs-lookup"><span data-stu-id="c0859-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="c0859-122">Hautatu **Eginda**.</span><span class="sxs-lookup"><span data-stu-id="c0859-122">Select **Done**.</span></span> <span data-ttu-id="c0859-123">LCS-k paketea egiaztatuko du.</span><span class="sxs-lookup"><span data-stu-id="c0859-123">LCS will verify the package.</span></span> <span data-ttu-id="c0859-124">Egiaztapenak minutu batzuk edo gehienez ordubete iraun dezake.</span><span class="sxs-lookup"><span data-stu-id="c0859-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="c0859-125">Aplikatu pakete-eguneratzea</span><span class="sxs-lookup"><span data-stu-id="c0859-125">Apply the package update</span></span>

1. <span data-ttu-id="c0859-126">LCSn **Ingurumenaren xehetasunak** orrialdean, hautatu **Mantendu** > **Aplikatu eguneratzeak**.</span><span class="sxs-lookup"><span data-stu-id="c0859-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="c0859-127">Zerrendan, hautatu lehen gordetako paketea, eta hautatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="c0859-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="c0859-128">Aukeratu **Bai** paketea zabaldu nahi duzula baieztatzeko.</span><span class="sxs-lookup"><span data-stu-id="c0859-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![Berretsi paketeak inplementatzeko elkarrizketa-koadroa](media/confirm-package-deployment.png)

4. <span data-ttu-id="c0859-130">Aukeratu **Bai** aplikazioa eguneratu nahi duzula baieztatzeko.</span><span class="sxs-lookup"><span data-stu-id="c0859-130">Select **Yes** to confirm that you want to update the application.</span></span>

![Berretsi aplikazioa eguneratzeko elkarrizketa-koadroa](media/confirm-application-update.png)

<span data-ttu-id="c0859-132">Inplementazioa eta aplikazioaren eguneratzea hasiko da.</span><span class="sxs-lookup"><span data-stu-id="c0859-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="c0859-133">**Ingurumenaren xehetasunak** orrialdean, goiko eskuineko izkinan, ingurunearen egoera **Zerbitzua ematea** aukerara eguneratuko da.</span><span class="sxs-lookup"><span data-stu-id="c0859-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="c0859-134">Bi ordutan gutxi gorabehera, eguneratzea osatuko da.</span><span class="sxs-lookup"><span data-stu-id="c0859-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="c0859-135">Aplikazioaren bertsioaren informazioa eguneratu egingo da **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** eta ingurunearen egoera eguneratu egingo da **Inplementatuta**.</span><span class="sxs-lookup"><span data-stu-id="c0859-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><a name="update"></a><span data-ttu-id="c0859-136">Eguneratu Dataverse ingurunea</span><span class="sxs-lookup"><span data-stu-id="c0859-136">Update your Dataverse environment</span></span>

1. <span data-ttu-id="c0859-137">Hasi saioa hurrengoan [Power Platform administrazio-zentroa](https://admin.powerplatform.com/).</span><span class="sxs-lookup"><span data-stu-id="c0859-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="c0859-138">Zerrendan, bilatu eta ireki Project Operations instalatzeko erabili zenuen ingurunea.</span><span class="sxs-lookup"><span data-stu-id="c0859-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="c0859-139">**Inguruneak** orrialdean, hautatu **Baliabidea** > **Dynamics 365 aplikazioak**.</span><span class="sxs-lookup"><span data-stu-id="c0859-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="c0859-140">Zerrendan, bilatu **Microsoft Dynamics 365 Project Operations**, eta **Egoera** zutabean, hautatu **Eguneratzea eskuragarri**.</span><span class="sxs-lookup"><span data-stu-id="c0859-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="c0859-141">Aukeratu **Zerbitzu baldintzak onartzen ditut** kontrol laukia eta, ondoren, hautatu **Eguneratu**.</span><span class="sxs-lookup"><span data-stu-id="c0859-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="c0859-142">Soluzioaren azken bertsioa instalatuko da.</span><span class="sxs-lookup"><span data-stu-id="c0859-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="c0859-143">Instalazioa amaitu ondoren, 4.5.0.134 bertsioa instalatuta izango duzu.</span><span class="sxs-lookup"><span data-stu-id="c0859-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="c0859-144">Konfiguratu eginbide berriak</span><span class="sxs-lookup"><span data-stu-id="c0859-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="c0859-145">Gaitu idazketa dualaren esleipenak</span><span class="sxs-lookup"><span data-stu-id="c0859-145">Enable dual-write mapping</span></span>

<span data-ttu-id="c0859-146">Finance eta Dataverse inguruneak eguneratu eta gero, beharrezko idazketa bikoitzeko mapak gaitu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="c0859-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="c0859-147">Osatu prozedura hauek, idazketa dualerako esleipenak gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="c0859-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="c0859-148">Eguneratu segurtasun-ezarpenak Customer Engagement ingurunean</span><span class="sxs-lookup"><span data-stu-id="c0859-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="c0859-149">Freskatu datu-entitateak</span><span class="sxs-lookup"><span data-stu-id="c0859-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="c0859-150">Eguneratu eta exekutatu idazketa bikoitzeko mapak</span><span class="sxs-lookup"><span data-stu-id="c0859-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="c0859-151">Eguneratu segurtasun-ezarpenak Dataverse ingurunean</span><span class="sxs-lookup"><span data-stu-id="c0859-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="c0859-152">Entitateen segurtasun pribilegioen eguneratze hauek beharrezkoak dira UR5 eguneratzearen barruan.</span><span class="sxs-lookup"><span data-stu-id="c0859-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="c0859-153">Dataverse ingurunean, joan **Ezarpenak** aukerara, eta **Sistema** taldean, hautatu **Segurtasuna**.</span><span class="sxs-lookup"><span data-stu-id="c0859-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![Dataverse ingurunearen ezarpenak](media/Picture21.png)

2. <span data-ttu-id="c0859-155">Hautatu **Segurtasun-funtzioak**.</span><span class="sxs-lookup"><span data-stu-id="c0859-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="c0859-156">Funtzioen zerrendan, hautatu **idazketa bikoitzeko aplikazioaren erabiltzailea** eta hautatu **Entitate pertsonalizatuak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="c0859-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="c0859-157">Egiaztatu rolak funtzioak badituela **Irakurri** eta **Erantsi honi** honetarako baimenak:</span><span class="sxs-lookup"><span data-stu-id="c0859-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="c0859-158">**Monetaren truke-tasaren mota**</span><span class="sxs-lookup"><span data-stu-id="c0859-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="c0859-159">**Kontuen sailkapena**</span><span class="sxs-lookup"><span data-stu-id="c0859-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="c0859-160">**Egutegi fiskala**</span><span class="sxs-lookup"><span data-stu-id="c0859-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="c0859-161">**Liburua**</span><span class="sxs-lookup"><span data-stu-id="c0859-161">**Ledger**</span></span>

5. <span data-ttu-id="c0859-162">Segurtasun-funtzio eguneratu ondoren, joan **Ezarpenak** > **Segurtasuna** > **Taldeak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="c0859-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="c0859-163">Egiaztatu **idazketa bikoitzeko aplikazioaren erabiltzailea** funtzioa aplikatu zaio taldeari.</span><span class="sxs-lookup"><span data-stu-id="c0859-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="c0859-164">Freskatu datu entitateak eguneratzetik</span><span class="sxs-lookup"><span data-stu-id="c0859-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="c0859-165">Zure Finance ingurunean, ireki **Datuen kudeaketa** laneko eremua eta, ondoren, ireki **Esparru parametroak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="c0859-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="c0859-166">**Entitatearen ezarpenak** fitxan, hautatu **Freskatu entitate zerrenda**.</span><span class="sxs-lookup"><span data-stu-id="c0859-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="c0859-167">Aukeratu **Itxi** entitatearen freskatzea baieztatzeko.</span><span class="sxs-lookup"><span data-stu-id="c0859-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="c0859-168">Prozesu horrek 20 bat minutu artean iraun dezake.</span><span class="sxs-lookup"><span data-stu-id="c0859-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="c0859-169">Freskapena amaitutakoan jakinaraziko zaizu.</span><span class="sxs-lookup"><span data-stu-id="c0859-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="c0859-170">Eguneratu idazketa dualaren esleipenak</span><span class="sxs-lookup"><span data-stu-id="c0859-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="c0859-171">**Datuen kudeaketa** lan-eremuan, hautatu **Idazketa bikoitza**.</span><span class="sxs-lookup"><span data-stu-id="c0859-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="c0859-172">Aukeratu **Aplikatu soluzioak**, hautatu bi irtenbideak zerrendan eta, ondoren, hautatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="c0859-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="c0859-173">**Idazketa bikoitza** orrialdean, hautatu taula-esleipen hauek eta hautatu **Gelditu**.</span><span class="sxs-lookup"><span data-stu-id="c0859-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="c0859-174">**Project Operations-en integrazioaren benetako datuak (msdynactuals)**</span><span class="sxs-lookup"><span data-stu-id="c0859-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="c0859-175">**Project Operations-en integratzeko proiektuaren gastuen kategoriak (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="c0859-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="c0859-176">**Project Operations-en integratzeko benetako datuen proiektuaren gastuen esportazio-entitatea (msdyn_expenses)**</span><span class="sxs-lookup"><span data-stu-id="c0859-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="c0859-177">**Taula-esleipenaren bertsioa** orrian, aplikatu maparen bertsio berria hiru entitate bakoitzari.</span><span class="sxs-lookup"><span data-stu-id="c0859-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="c0859-178">**Idazketa bikoitza** orrian, hautatu exekutatu mapak berrabiarazteko.</span><span class="sxs-lookup"><span data-stu-id="c0859-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="c0859-179">Mapen zerrendan, hautatu **Liburua (msdyn_ledgers)** mapa aurrebaldintza guztiekin eta hautatu **Hasierako sinkronizazioa** kontrol-laukia.</span><span class="sxs-lookup"><span data-stu-id="c0859-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="c0859-180">**Hasierako sinkronizaziorako nagusia** eremuan, hautatu **Finance and Operations aplikazioak** eta, ondoren, hautatu **Exekutatu**.</span><span class="sxs-lookup"><span data-stu-id="c0859-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![Liburuaren esleipenaren sinkronizazioa](media/DW6.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]