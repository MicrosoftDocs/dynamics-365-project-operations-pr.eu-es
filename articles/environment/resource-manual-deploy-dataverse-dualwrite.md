---
title: Inplementatu eskuz Project Operations-en Dataverse aplikazioa idazketa dualaren bateragarritasunarekin
description: Gai honetan Project Operations Dataverse aplikazioa nola inplementatu azaltzen da idazketa bikoitza onartzeko.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2021
ms.locfileid: "6273993"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a><span data-ttu-id="0ff92-103">Inplementatu eskuz Project Operations-en Dataverse aplikazioa idazketa dualaren bateragarritasunarekin</span><span class="sxs-lookup"><span data-stu-id="0ff92-103">Manually deploy the Project Operations Dataverse app with dual-write support</span></span>

<span data-ttu-id="0ff92-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="0ff92-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="0ff92-105">Gai honetan Microsoft Dataverse-ko Microsoft Dynamics 365 Project Operations nola inplementatu azaltzen da idazketa bikoitza onartzeko.</span><span class="sxs-lookup"><span data-stu-id="0ff92-105">This topic explains how to manually deploy Microsoft Dynamics 365 Project Operations in Microsoft Dataverse so that it supports dual-write.</span></span> <span data-ttu-id="0ff92-106">Project Operations-ek ingurunearen konfigurazioa hautematen dute eta idazketa bikoitzerako laguntza gehigarria gehitzen dute aurrez aurreko baldintzak betetzen badira.</span><span class="sxs-lookup"><span data-stu-id="0ff92-106">Project Operations detects the environment's configuration and adds additional support for dual-write if the prerequisites are met.</span></span>

<span data-ttu-id="0ff92-107">Microsoft Dynamics Lifecycle Services-en inplementazioan zehar (LCS), gai honetako argibideak jarraitu badituzu, Microsoft Power Platform integrazioaren inplementazioa salta dezakezu (aurretik Common Data Service ingurunea).</span><span class="sxs-lookup"><span data-stu-id="0ff92-107">During deployment through Microsoft Dynamics Lifecycle Services (LCS), if you've followed the instructions in this topic, you can skip the deployment of the Microsoft Power Platform integration (previously known as the Common Data Service environment).</span></span>

<span data-ttu-id="0ff92-108">Dataverse-ko Project Operations-ek idazketa bikoitza onartzeko inplementazio prozesuak du lau urrats nagusi ditu:</span><span class="sxs-lookup"><span data-stu-id="0ff92-108">The process of deploying Project Operations in Dataverse so that it supports dual-write has four main steps:</span></span>

1. <span data-ttu-id="0ff92-109">[Ingurune berri bat sortu Dataverse-n idazketa bikoitza onartzen duena](#create).</span><span class="sxs-lookup"><span data-stu-id="0ff92-109">[Create a new environment in Dataverse that supports dual-write](#create).</span></span>
2. <span data-ttu-id="0ff92-110">[Gehitu idazketa bikoitzaren aurrebaldintzak inguruneari](#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="0ff92-110">[Add dual-write prerequisites to the environment](#prerequisites).</span></span>
3. <span data-ttu-id="0ff92-111">[Gehitu Project Operations Dataverse aplikazioan](#dataverse).</span><span class="sxs-lookup"><span data-stu-id="0ff92-111">[Add the Project Operations Dataverse app](#dataverse).</span></span>
4. <span data-ttu-id="0ff92-112">[Estekatu inguruneak](#link).</span><span class="sxs-lookup"><span data-stu-id="0ff92-112">[Link your environments](#link).</span></span>

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a><span data-ttu-id="0ff92-113">Sortu ingurune bat Dataverse-n idazketa bikoitza onartzen duena</span><span class="sxs-lookup"><span data-stu-id="0ff92-113">Create a new environment in Dataverse that supports dual-write</span></span>

<span data-ttu-id="0ff92-114">Prozedura hau osatzeko, administratzaile gisa hasi behar duzu saioa.</span><span class="sxs-lookup"><span data-stu-id="0ff92-114">To complete this procedure, you must sign in as an administrator.</span></span>

1. <span data-ttu-id="0ff92-115">Ireki [Power Platform administratzaile zentroa](https://admin.powerplatform.com), eta hasi saioa administratzaile gisa.</span><span class="sxs-lookup"><span data-stu-id="0ff92-115">Open the [Power Platform admin center](https://admin.powerplatform.com), and sign in as an administrator.</span></span>
2. <span data-ttu-id="0ff92-116">Sortu ingurune bat eta jarri izena.</span><span class="sxs-lookup"><span data-stu-id="0ff92-116">Create a new environment, and name it.</span></span>
3. <span data-ttu-id="0ff92-117">Hautatu ingurune mota.</span><span class="sxs-lookup"><span data-stu-id="0ff92-117">Select the environment type.</span></span> <span data-ttu-id="0ff92-118">Probako eskaintzan izena eman baduzu, hautatu **Proba (harpidetzan oinarrituta)**.</span><span class="sxs-lookup"><span data-stu-id="0ff92-118">If you signed up for the trial offer, select **Trial (subscription-based)**.</span></span>
4. <span data-ttu-id="0ff92-119">Berretsi inplementazioaren eskualdea.</span><span class="sxs-lookup"><span data-stu-id="0ff92-119">Confirm the deployment region.</span></span>
5. <span data-ttu-id="0ff92-120">Gaitu **Sortu datu-base bat ingurune honetarako** aukera.</span><span class="sxs-lookup"><span data-stu-id="0ff92-120">Enable the **Create a database for this environment** option.</span></span> 
6. <span data-ttu-id="0ff92-121">Berretsi hizkuntza eta, ondoren, baieztatu moneta Finance and Operations aplikaziorako bat datorrela zure monetarekin.</span><span class="sxs-lookup"><span data-stu-id="0ff92-121">Confirm the language, and then confirm that the currency matches the currency for your Finance and Operations apps.</span></span>
7. <span data-ttu-id="0ff92-122">Gaitu **Dynamics 365 aplikazioak** aukera, eta baieztatu **Aplikazio hauek automatikoki zabaldu** eremua ezarrita dagoela **Bat ere ez** gisa.</span><span class="sxs-lookup"><span data-stu-id="0ff92-122">Enable the **Dynamics 365 apps** option, and confirm that the **Automatically deploy these apps** field is set to **None**.</span></span>
8. <span data-ttu-id="0ff92-123">Gehitu segurtasun taldea, segurtasun taldea beharrezkoa bada.</span><span class="sxs-lookup"><span data-stu-id="0ff92-123">Add a security group, if a security group is required.</span></span>
9. <span data-ttu-id="0ff92-124">Hautatu **Gorde** ingurunea sortzeko.</span><span class="sxs-lookup"><span data-stu-id="0ff92-124">Select **Save** to create the environment.</span></span>
10. <span data-ttu-id="0ff92-125">Itxaron inplementazioa amaitu arte eta ingurunea **Prest** egoeran egon arte.</span><span class="sxs-lookup"><span data-stu-id="0ff92-125">Wait until the deployment is completed and the environment reaches the **Ready** state.</span></span>

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a><span data-ttu-id="0ff92-126">Gehitu idazketa bikoitzaren aurrebaldintzak inguruneari</span><span class="sxs-lookup"><span data-stu-id="0ff92-126">Add dual-write prerequisites to the environment</span></span>

<span data-ttu-id="0ff92-127">Idazketa dualaren euskarriak funtsezko entitateei gehitzen zaizkien eremu osagarriak biltzen ditu, adibidez **Enpresa** entitatea.</span><span class="sxs-lookup"><span data-stu-id="0ff92-127">Dual-write support includes additional fields that are added to key entities, such as the **Company** entity.</span></span> <span data-ttu-id="0ff92-128">Lehendik dagoen ingurune bati idazketa bikoitzeko laguntza gehitzen ari bazara, baliteke datuak eguneratu beharko izatea laguntza gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="0ff92-128">If you're adding dual-write support to an existing environment, you might have to update the data to enable the support.</span></span> <span data-ttu-id="0ff92-129">Datuak abiarazteko moduari buruzko informazioa lortzeko, ikusi [Bootstrap enpresaren datuak](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span><span class="sxs-lookup"><span data-stu-id="0ff92-129">For information about how to bootstrap the data, see [Bootstrap company data](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span></span> <span data-ttu-id="0ff92-130">Idazketa bikoitzari buruzko informazio gehiago lortzeko, ikusi [Idazketa bikoitzeko sistemaren eskakizunak](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span><span class="sxs-lookup"><span data-stu-id="0ff92-130">For more information about dual-write, see [Dual-write system requirements](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span></span>

<span data-ttu-id="0ff92-131">Osatu prozedura hau idazketa bikoitzaren aurrebaldintzak zure inguruneari gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="0ff92-131">Complete this procedure to add the dual-write prerequisites to your environment.</span></span>

1. <span data-ttu-id="0ff92-132">Ireki sortu berri duzun ingurunea eta joan hona **Baliabidea** \> **Dynamics 365 aplikazioak**.</span><span class="sxs-lookup"><span data-stu-id="0ff92-132">Open the environment that you just created, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="0ff92-133">Aukeratu **Idazketa dualeko oinarrizko soluzioa** aplikazioen zerrendan eta instalatu.</span><span class="sxs-lookup"><span data-stu-id="0ff92-133">Select **Dual-write core solution** in the app list, and install it.</span></span>
3. <span data-ttu-id="0ff92-134">Itxaron instalazioa amaitu arte.</span><span class="sxs-lookup"><span data-stu-id="0ff92-134">Wait until the installation is completed.</span></span> <span data-ttu-id="0ff92-135">Aukeratu **Idazketa dualaren aplikazioa antolatzeko soluzioa** aplikazioen zerrendan eta instalatu.</span><span class="sxs-lookup"><span data-stu-id="0ff92-135">Then select **Dual-write application orchestration solution** in the app list, and install it.</span></span>

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a><span data-ttu-id="0ff92-136">Gehitu Project Operations Dataverse aplikazioan</span><span class="sxs-lookup"><span data-stu-id="0ff92-136">Add the Project Operations Dataverse app</span></span>

<span data-ttu-id="0ff92-137">Project Operations instalatu aurretik aurreko izapideak burutu badituzu soilik egin dezakezu prozedura hau.</span><span class="sxs-lookup"><span data-stu-id="0ff92-137">You can complete this procedure only if you completed the previous procedures before you installed Project Operations.</span></span> <span data-ttu-id="0ff92-138">Instalazioan zehar, sistemak ingurumenaren konfigurazioa aztertzen du eta beharrezkoa bada idazketa bikoitzeko laguntza gehitzen du.</span><span class="sxs-lookup"><span data-stu-id="0ff92-138">During installation, the system analyzes the environment configuration and adds support for dual-write if it's required.</span></span>

1. <span data-ttu-id="0ff92-139">Ireki sortu duzun ingurunea eta joan hona **Baliabidea** \> **Dynamics 365 aplikazioak**.</span><span class="sxs-lookup"><span data-stu-id="0ff92-139">Open the environment that you created earlier, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="0ff92-140">Aukeratu **Microsoft Dynamics 365 Project Operations** aplikazioen zerrendan eta instalatu.</span><span class="sxs-lookup"><span data-stu-id="0ff92-140">Select **Microsoft Dynamics 365 Project Operations** in the app list, and install it.</span></span>

## <a name="link-your-environments"></a><a name="link"></a><span data-ttu-id="0ff92-141">Estekatu inguruneak</span><span class="sxs-lookup"><span data-stu-id="0ff92-141">Link your environments</span></span>

<span data-ttu-id="0ff92-142">Dataverse ingurunea inplementatu dago, esteka konfigura dezakezu Finance and Operations aplikazioarena.</span><span class="sxs-lookup"><span data-stu-id="0ff92-142">After the Dataverse environment is deployed, you can set up the link in your Finance and Operations apps.</span></span> <span data-ttu-id="0ff92-143">Jarraitu urratsak: [Erabili idazketa bikoitzeko morroia zure inguruneak lotzeko](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span><span class="sxs-lookup"><span data-stu-id="0ff92-143">Follow the steps in [Use the dual-write wizard to link your environments](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span></span>
