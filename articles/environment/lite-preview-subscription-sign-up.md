---
title: Erregistratu aurrebista-harpidetzan - arina
description: Gai honek Project Operations lite-ra harpidetzeko eta hura inplementatzeko moduari buruzko informazioa eskaintzen du. Aurre egin fakturazio proformari.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2b5a65f5e29915c349d40400ebbf3e4923b36a67
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334767"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a><span data-ttu-id="70434-103">Erregistratu aurrebista-harpidetzan - arina</span><span class="sxs-lookup"><span data-stu-id="70434-103">Sign up for a preview subscription - lite</span></span> 

<span data-ttu-id="70434-104">Gai honek probako eskaintzan harpidetu eta nola inplementatu Dynamics 365 Project Operations lite inplementazioa azaltzen du - proforma fakturazioari aurre egin.</span><span class="sxs-lookup"><span data-stu-id="70434-104">This topic explains how to subscribe to the trial offer and deploy Dynamics 365 Project Operations lite deployment - deal to proforma invoicing.</span></span>

> [!NOTE]
> <span data-ttu-id="70434-105">Prozesu hau aldatu egingo da datozen Project Operations-en bertsioetan.</span><span class="sxs-lookup"><span data-stu-id="70434-105">This process will change in upcoming releases of Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70434-106">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="70434-106">Prerequisites</span></span>
- <span data-ttu-id="70434-107">Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu.</span><span class="sxs-lookup"><span data-stu-id="70434-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="70434-108">Maizterra sor dezakezu lehenengo eskaintzaren amortizazioan.</span><span class="sxs-lookup"><span data-stu-id="70434-108">You can create a tenant during the first offer redemption.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="70434-109">Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori.</span><span class="sxs-lookup"><span data-stu-id="70434-109">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="70434-110">Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.</span><span class="sxs-lookup"><span data-stu-id="70434-110">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="70434-111">Probak erabilera bakarrekoak dira maizterrean.</span><span class="sxs-lookup"><span data-stu-id="70434-111">Trials are single use in the tenant.</span></span> <span data-ttu-id="70434-112">Probak behin bakarrik exekutatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="70434-112">You can only run a trial one time.</span></span> <span data-ttu-id="70434-113">Probarako helburuarekin maizter berri bat sortzea gomendatzen dizugu.</span><span class="sxs-lookup"><span data-stu-id="70434-113">We recommend that you create a new tenant for the purpose of the trial.</span></span>

### <a name="dynamics-365-project-operations-trial"></a><span data-ttu-id="70434-114">Dynamics 365 Project Operations proba</span><span class="sxs-lookup"><span data-stu-id="70434-114">Dynamics 365 Project Operations trial</span></span> 

<span data-ttu-id="70434-115">Hasi aurretik, ziurtatu proiektuaren eragiketen aurrebista nahi duzun maizterrean erabiltzailearen laneko kontua duen arakatzailean saioa hasi duzula.</span><span class="sxs-lookup"><span data-stu-id="70434-115">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="70434-116">Joan [Project Operations probara](https://aka.ms/try-po) lehenengo eskaintza kodea erabiltzeko, **Dynamics 365 Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="70434-116">Go to [Project Operations Trial](https://aka.ms/try-po) to redeem the first offer code, **Dynamics 365 Project Operations**.</span></span>
2. <span data-ttu-id="70434-117">Berretsi eskaera.</span><span class="sxs-lookup"><span data-stu-id="70434-117">Confirm your order.</span></span>

  <span data-ttu-id="70434-118">Berrespen eskaintza behar bezala berreskuratu dela ikusiko duzu.</span><span class="sxs-lookup"><span data-stu-id="70434-118">You'll see the confirmation offer was successfully redeemed.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="70434-119">Esleitu lizentziak</span><span class="sxs-lookup"><span data-stu-id="70434-119">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="70434-120">Zure erakundeko Microsoft 365 Portal-erako sarbide administratiboa beharko duzu urrats hauek burutzeko.</span><span class="sxs-lookup"><span data-stu-id="70434-120">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>


1. <span data-ttu-id="70434-121">Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) aukerara, zure erabiltzaileei lizentziak emateko.</span><span class="sxs-lookup"><span data-stu-id="70434-121">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>
2. <span data-ttu-id="70434-122">**Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.</span><span class="sxs-lookup"><span data-stu-id="70434-122">On the **Active users** page, select the users that you want to assign a license to.</span></span>
3. <span data-ttu-id="70434-123">Egiaztatu **Dynamics 365 Project Operations** lizentzia hautatuta dagoela.</span><span class="sxs-lookup"><span data-stu-id="70434-123">Verify that the **Dynamics 365 Project Operations** license is selected.</span></span> 
4. <span data-ttu-id="70434-124">Hatatu **Gorde aldaketak**.</span><span class="sxs-lookup"><span data-stu-id="70434-124">Select **Save changes**.</span></span>

## <a name="create-a-new-dataverse-environment"></a><span data-ttu-id="70434-125">Sortu Dataverse ingurune berria</span><span class="sxs-lookup"><span data-stu-id="70434-125">Create a new Dataverse environment</span></span>

1. <span data-ttu-id="70434-126">Eman Project Operations Dataverse inplementazio ingurune berri bat gaiko argibideak jarraituz, [Dataverse inplementazio eredua](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="70434-126">Provision a new Project Operations Dataverse deployment environment by following instructions in the topic, [Dataverse deployment model](lite-deployment.md).</span></span> <span data-ttu-id="70434-127">Ingurune mota hautatzen duzunean, ziurtatu erabiltzen duzula **Proba (harpidetzan oinarrituta)**.</span><span class="sxs-lookup"><span data-stu-id="70434-127">When you select the environment type, make sure to use **Trial (Subscription based)**.</span></span>

  ![Ingurune berria](./media/19CreateEnvironment.png)

2. <span data-ttu-id="70434-129">Aukeratu **Gaitu Dynamics 365 aplikazioak** ezarpena, eta utzi **Aplikazio hauek automatikoki zabaldu** hutsik.</span><span class="sxs-lookup"><span data-stu-id="70434-129">Select the **Enable Dynamics 365 apps** setting, and leave **Automatically deploy these apps** blank.</span></span>  
3. <span data-ttu-id="70434-130">Hautatu **Gorde** ingurunea sortzeko.</span><span class="sxs-lookup"><span data-stu-id="70434-130">Select **Save** to create the environment.</span></span>

  ![Gehitu datu-basea](./media/20CreateEnvironment1.png)

4. <span data-ttu-id="70434-132">Ingurunea sortu ondoren, instalatu **Microsoft Dynamics 365 Project Operations** konponbidea.</span><span class="sxs-lookup"><span data-stu-id="70434-132">After the environment is created, install **Microsoft Dynamics 365 Project Operations** solution.</span></span> 

![Instalatu soluzioa](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a><span data-ttu-id="70434-134">Instalatu CDS konfigurazioa eta konfiguratu demo-datuak</span><span class="sxs-lookup"><span data-stu-id="70434-134">Install a CDS configuration and setup demo data</span></span>

<span data-ttu-id="70434-135">Instalatu CDS konfigurazioa eta konfiguratu demo datuak gaiko argibideak jarraituz, [Aplikatu demo konfigurazio eta konfigurazio datuak](lite-apply-demo-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="70434-135">Install the CDS configuration and set up demo data by following instructions in the topic, [Apply demo setup and configuration data](lite-apply-demo-setup-config-data.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
