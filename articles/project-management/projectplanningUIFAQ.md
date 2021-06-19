---
title: Zeregina saretan lan egiteko arazoak konpontzea
description: Gai honek Atazen saretan lan egitean behar diren arazoak konpontzeko informazioa eskaintzen du.
author: ruhercul
ms.date: 01/19/2021
ms.topic: article
ms.product: ''
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a15a4752de7537b3f60d5ee3269c846257a1fe4a
ms.sourcegitcommit: 72fa1f09fe406805f7009fc68e2f3eeeb9b7d5fc
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/09/2021
ms.locfileid: "6213385"
---
# <a name="troubleshoot-working-in-the-task-grid"></a><span data-ttu-id="5e4a8-103">Zeregina saretan lan egiteko arazoak konpontzea</span><span class="sxs-lookup"><span data-stu-id="5e4a8-103">Troubleshoot working in the Task grid</span></span> 

<span data-ttu-id="5e4a8-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="5e4a8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5e4a8-105">Gai honek kostuen kudeaketarekin lan egiterakoan topa ditzakezun arazoak nola konpondu deskribatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-105">This topic describes how to fix issues that you might encounter while working with cost management.</span></span>

## <a name="enable-cookies"></a><span data-ttu-id="5e4a8-106">Gaitu cookieak</span><span class="sxs-lookup"><span data-stu-id="5e4a8-106">Enable cookies</span></span>

<span data-ttu-id="5e4a8-107">Project Operations-ek hirugarrenen cookieak gaitzea eskatzen dute zereginen xehetasunen egitura bihurtzeko.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-107">Project Operations requires that third-party cookies be enabled in order to render the work breakdown structure.</span></span> <span data-ttu-id="5e4a8-108">Hirugarrenen cookieak gaituta ez daudenean, zereginak ikusi beharrean, orrialde huts bat ikusiko duzu **Zereginak** fitxan **Proiektua** orrialdean.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-108">When third-party cookies aren't enabled, instead of seeing tasks, you will see a blank page when you select the **Tasks** tab on the **Project** page.</span></span>

![Fitxa hutsa hirugarrenen cookieak gaituta ez daudenean](media/blankschedule.png)


### <a name="workaround"></a><span data-ttu-id="5e4a8-110">Irtenbidea</span><span class="sxs-lookup"><span data-stu-id="5e4a8-110">Workaround</span></span>
<span data-ttu-id="5e4a8-111">Microsoft Edge edo Google Chrome arakatzaileetarako, honako prozedura hauek azaltzen dute nola eguneratu zure arakatzailearen ezarpena hirugarrenen cookieak gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-111">For Microsoft Edge or Google Chrome browsers, the following procedures outline how to update your browser setting to enable third-party cookies.</span></span>

#### <a name="microsoft-edge"></a><span data-ttu-id="5e4a8-112">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="5e4a8-112">Microsoft Edge</span></span>

1. <span data-ttu-id="5e4a8-113">Ireki Edge arakatzailea.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-113">Open your Edge browser.</span></span>
2. <span data-ttu-id="5e4a8-114">Goiko eskuineko ertzean, hautatu **hiru puntuak** (...), eta hautatu **Ezarpenak**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-114">In the upper-right corner, select the **ellipsis** (...), and then select **Settings**.</span></span>
3. <span data-ttu-id="5e4a8-115">**Cookieak eta gune baimenak** aukeran, hautatu **Cookieak eta webguneko datuak**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-115">Under **Cookies and site permissions**, select **Cookies and site data**.</span></span>
4. <span data-ttu-id="5e4a8-116">Desaktibatu **Blokeatu hirugarrenen cookieak**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-116">Turn off **Block third-party cookies**.</span></span>

#### <a name="google-chrome"></a><span data-ttu-id="5e4a8-117">Google Chrome</span><span class="sxs-lookup"><span data-stu-id="5e4a8-117">Google Chrome</span></span>

1. <span data-ttu-id="5e4a8-118">Ireki Chrome arakatzailea.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-118">Open your Chrome browser.</span></span>
2. <span data-ttu-id="5e4a8-119">Goiko eskuineko ertzean, hautatu hiru puntu bertikalak, eta hautatu **Ezarpenak**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-119">In the upper-right corner, select the three vertical dots, and then select **Settings**.</span></span>
3. <span data-ttu-id="5e4a8-120">**Pribatutasuna eta segurtasuna** aukeran, hautatu **Cookieak eta webguneko beste datuak**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-120">Under **Privacy and security**, select **Cookies and other site data**.</span></span>
4. <span data-ttu-id="5e4a8-121">Hautatu **Baimendu cookie guztiak**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-121">Select **Allow all cookies**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5e4a8-122">Hirugarrenen cookieak blokeatzen badituzu, beste gune batzuetako cookieak eta webguneko datuak blokeatuko dira, nahiz eta gunea zure salbuespenen zerrendan onartzen den.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-122">If you block third-party cookies, all cookies and site data from other sites will be blocked, even if the site is allowed on your exceptions list.</span></span>

## <a name="pex-endpoint"></a><span data-ttu-id="5e4a8-123">PEX amaiera-puntua</span><span class="sxs-lookup"><span data-stu-id="5e4a8-123">PEX Endpoint</span></span>

<span data-ttu-id="5e4a8-124">Project Operations-ek proiektuaren parametro batek PEX amaiera puntua erreferentzia izatea eskatzen du.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-124">Project Operations requires that a project parameter reference the PEX Endpoint.</span></span> <span data-ttu-id="5e4a8-125">Amaierako puntu hau lanaren matxura egitura emateko erabiltzen den zerbitzuarekin komunikatzeko beharrezkoa da.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-125">This endpoint is required to communicate with the service used to render the work breakdown structure.</span></span> <span data-ttu-id="5e4a8-126">Parametroa gaituta ez badago, "Proiektuaren parametroak ez du balio" errorea jasoko duzu.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-126">If the parameter isn't enabled, you will receive the error, "The project parameter is not valid".</span></span> 

### <a name="workaround"></a><span data-ttu-id="5e4a8-127">Irtenbidea</span><span class="sxs-lookup"><span data-stu-id="5e4a8-127">Workaround</span></span>
 ![PEX amaiera-puntua eremua proiektuaren parametroan](media/projectparameter.png)

1. <span data-ttu-id="5e4a8-129">Gehitu **PEX amaiera puntua** eremua **Proiektuaren parametroak** orrialdean.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-129">Add the **PEX Endpoint** field to the **Project Parameters** page.</span></span>
2. <span data-ttu-id="5e4a8-130">Eguneratu eremua balio honekin: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=/<id>&type=2`</span><span class="sxs-lookup"><span data-stu-id="5e4a8-130">Update the field with the following value: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=/<id>&type=2`</span></span>
3. <span data-ttu-id="5e4a8-131">Kendu eremua **Proiektuaren parametroak** orrialdetik.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-131">Remove the field from the **Project Parameters** page.</span></span>

## <a name="privileges-for-project-for-the-web"></a><span data-ttu-id="5e4a8-132">Webgunearen proiektuaren pribilegioak</span><span class="sxs-lookup"><span data-stu-id="5e4a8-132">Privileges for Project for the Web</span></span>

<span data-ttu-id="5e4a8-133">Project Operations kanpoko planifikazio-zerbitzu batean oinarritzen da.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-133">Project Operations relies on an external scheduling service.</span></span> <span data-ttu-id="5e4a8-134">Zerbitzuak eskatzen du erabiltzaile batek hainbat funtzio esleituta izatea lanaren banakako egiturarekin lotutako entitateei irakurtzeko eta idazteko.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-134">The service requires that a user have several roles assigned to read and write to entities related to the work breakdown structure.</span></span> <span data-ttu-id="5e4a8-135">Entitate horien artean daude proiektuaren zereginak, baliabideen esleipenak eta atazen mendekotasunak.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-135">These entities include project tasks, resource assignments, and task dependencies.</span></span> <span data-ttu-id="5e4a8-136">Erabiltzaile batek ezin badu zereginen xehetasunen egitura errendatu **Zereginak** fitxa, ziurrenik Project Operations-erako proiektua gaituta ez dagoelako izango da.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-136">If a user can't render the work breakdown structure when they go to the **Tasks** tab, it's probably because Project for Project Operations hasn't been enabled.</span></span> <span data-ttu-id="5e4a8-137">Erabiltzaile batek segurtasun-funtzio errorea edo sarbidea ukatzearekin lotutako errorea jaso dezake.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-137">A user might receive either a security role error, or an error related to a denial of access.</span></span>


## <a name="workaround"></a><span data-ttu-id="5e4a8-138">Irtenbidea</span><span class="sxs-lookup"><span data-stu-id="5e4a8-138">Workaround</span></span>

1. <span data-ttu-id="5e4a8-139">Joan **Ezarpena > Segurtasuna > Erabiltzaileak > Aplikazioaren erabiltzaileak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-139">Go to **Setting > Security > Users > Application Users**.</span></span>  

   ![Aplikazio-irakurgailua](media/applicationuser.jpg)
   
2. <span data-ttu-id="5e4a8-141">Egin klik bikoitza aplikazioaren erabiltzaile erregistroan hau egiaztatzeko:</span><span class="sxs-lookup"><span data-stu-id="5e4a8-141">Double-click the application user record to verify the following:</span></span>

 - <span data-ttu-id="5e4a8-142">Erabiltzaileak sarbidea du proiektuan.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-142">The user has access to the project.</span></span> <span data-ttu-id="5e4a8-143">Egiaztapen hau normalean erabiltzaileak ziurtatzen du **Proiektu-kudeatzailea** segurtasun-funtzioa daukala.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-143">This verification is typically done by ensuring that the user has **Project Manager** security role.</span></span>
 - <span data-ttu-id="5e4a8-144">Microsoft Project aplikazioaren erabiltzailea badago eta behar bezala konfiguratuta dago.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-144">The Microsoft Project application user exists and is configured correctly.</span></span>
 
3. <span data-ttu-id="5e4a8-145">Erabiltzailea ez bada existitzen, erabiltzaile-erregistro bat sor dezakezu.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-145">If this user doesn't exist, you can create a new user record.</span></span> <span data-ttu-id="5e4a8-146">Hautatu **Erabiltzaile berriak**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-146">Select **New Users**.</span></span> <span data-ttu-id="5e4a8-147">Aldatu sarrera-inprimakia **Aplikazioaren erabiltzailea** aukeran, eta gehitu **Aplikazioaren IDa**.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-147">Change the entry form to **Application User**, and then add the **Application ID**.</span></span>

   ![Aplikazioaren erabiltzaile-xehetasunak](media/applicationuserdetails.jpg)

4. <span data-ttu-id="5e4a8-149">Egiaztatu erabiltzaileari lizentzia zuzena esleitu zaiola eta zerbitzua lizentziaren zerbitzu planen xehetasunetan gaituta dagoela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-149">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
5. <span data-ttu-id="5e4a8-150">Egiaztatu erabiltzaileak project.microsoft.com ireki dezakeela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-150">Verify that the user can open project.microsoft.com.</span></span>
6. <span data-ttu-id="5e4a8-151">Egiaztatu proiektuaren parametroen bidez sistemak proiektuaren amaierako puntu zuzena adierazten duela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-151">Verify through the project parameters that the system is pointing to the correct project endpoint.</span></span>
7. <span data-ttu-id="5e4a8-152">Egiaztatu proiektuaren aplikazioaren erabiltzailea sortu dela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-152">Verify that the project application user is created.</span></span>
8. <span data-ttu-id="5e4a8-153">Aplikatu segurtasun rol hauek erabiltzaileari:</span><span class="sxs-lookup"><span data-stu-id="5e4a8-153">Apply the following security roles to the user:</span></span>

  - <span data-ttu-id="5e4a8-154">Dataverse erabiltzailea</span><span class="sxs-lookup"><span data-stu-id="5e4a8-154">Dataverse User</span></span>
  - <span data-ttu-id="5e4a8-155">Project Operations sistema</span><span class="sxs-lookup"><span data-stu-id="5e4a8-155">Project Operations System</span></span>
  - <span data-ttu-id="5e4a8-156">Proiektuaren sistema</span><span class="sxs-lookup"><span data-stu-id="5e4a8-156">Project System</span></span>

## <a name="error-when-updating-the-work-breakdown-structure"></a><span data-ttu-id="5e4a8-157">Errorea lanaren matxura egitura eguneratzean</span><span class="sxs-lookup"><span data-stu-id="5e4a8-157">Error when updating the work breakdown structure</span></span>

<span data-ttu-id="5e4a8-158">Lanaren banakako egiturari eguneratze bat edo gehiago egiten zaizkionean, azkenean aldaketak huts egiten dira eta ez dira gordetzen.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-158">When one or more updates are made to the work breakdown structure, the changes eventually fail and aren't saved.</span></span> <span data-ttu-id="5e4a8-159">Akats bat gertatu da programazio-saretan "Egindako azken aldaketa ezin izan dela gorde".</span><span class="sxs-lookup"><span data-stu-id="5e4a8-159">An error occurs in the schedule grid noting that “Recent change you’ve made couldn’t be saved.”</span></span>

### <a name="workaround"></a><span data-ttu-id="5e4a8-160">Irtenbidea</span><span class="sxs-lookup"><span data-stu-id="5e4a8-160">Workaround</span></span>

1. <span data-ttu-id="5e4a8-161">Egiaztatu erabiltzaileari lizentzia zuzena esleitu zaiola eta zerbitzua lizentziaren zerbitzu planen xehetasunetan gaituta dagoela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-161">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
2. <span data-ttu-id="5e4a8-162">Egiaztatu erabiltzaileak project.microsoft.com ireki dezakeela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-162">Verify that the user can open project.microsoft.com.</span></span>
3. <span data-ttu-id="5e4a8-163">Egiaztatu sistemak proiektuaren amaierako puntu zuzena adierazten duela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-163">Verify that the system is pointing to the correct project endpoint,.</span></span>
4. <span data-ttu-id="5e4a8-164">Egiaztatu Proiektuaren aplikazioaren erabiltzailea sortu dela.</span><span class="sxs-lookup"><span data-stu-id="5e4a8-164">Verify that the Project Application user has been created.</span></span>
5. <span data-ttu-id="5e4a8-165">Aplikatu segurtasun rol hauek erabiltzaileari:</span><span class="sxs-lookup"><span data-stu-id="5e4a8-165">Apply the following security roles to the user:</span></span>
  
  - <span data-ttu-id="5e4a8-166">Dataverse erabiltzailea edo Base erabiltzailea</span><span class="sxs-lookup"><span data-stu-id="5e4a8-166">Dataverse user or Base user</span></span>
  - <span data-ttu-id="5e4a8-167">Project Operations sistema</span><span class="sxs-lookup"><span data-stu-id="5e4a8-167">Project Operations System</span></span>
  - <span data-ttu-id="5e4a8-168">Proiektuaren sistema</span><span class="sxs-lookup"><span data-stu-id="5e4a8-168">Project System</span></span>
  - <span data-ttu-id="5e4a8-169">Project Operations-en idazketa bikoitzeko sistema (funtzio hau beharrezkoa da Project Operations-en baliabidea/biltegiratu gabeko oinarritutako egoera hedatzen ari bazara.)</span><span class="sxs-lookup"><span data-stu-id="5e4a8-169">Project Operations Dual Write System (This role is required if you are deploying the resource/non-stocked based scenario of Project Operations.)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
