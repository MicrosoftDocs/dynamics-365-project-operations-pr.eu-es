---
title: Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan
description: Gai honek Project Operations-era harpidetzeko eta hedatzeko moduari buruzko informazioa eskaintzen du berreskuratutako / stockean oinarritutako eszenatokietarako.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: da93fcf23ee3f255812842e31cb22b5d39daa963
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334812"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="cf2f3-103">Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan</span><span class="sxs-lookup"><span data-stu-id="cf2f3-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="cf2f3-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="cf2f3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="cf2f3-105">Gai honetan azaltzen da nola harpidetu probako eskaintzan eta nola zabaldu Project Operations ingurunea baliabideetan / stockean oinarritutako eszenatokietan.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-105">This topic explains how to subscribe to the trial offer and deploy Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf2f3-106">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="cf2f3-106">Prerequisites</span></span>
- <span data-ttu-id="cf2f3-107">Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="cf2f3-108">Maizterra sor dezakezu lehenengo eskaintzaren amortizazioan.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-108">You can create a tenant during the first offer redemption.</span></span> 
- <span data-ttu-id="cf2f3-109">Finantza ingurunea hedatzeko baliozko Azure harpidetza behar da ingurune bakoitzeko fakturatuko dena.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-109">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="cf2f3-110">Zure erakundeetan dagoen harpidetza erabil dezakezu edo [Azure proba](https://azure.microsoft.com/en-us/free/) erabiltzen hasteko.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-110">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="cf2f3-111">CDS ingurunea doan emango da 30 eguneko epean.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-111">The CDS environment will be provided free for a limited 30 day period.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cf2f3-112">Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-112">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="cf2f3-113">Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-113">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="cf2f3-114">Probak erabilera bakarrekoak dira maizterrean.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-114">Trials are single use in the tenant.</span></span> <span data-ttu-id="cf2f3-115">Probak behin bakarrik exekutatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-115">You can only run a trial one time.</span></span> <span data-ttu-id="cf2f3-116">Probarako helburuarekin maizter berri bat sortzea gomendatzen dizugu.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-116">We recommend that you create a new tenant for the purpose of the trial.</span></span>


### <a name="dynamics-365-project-operations-ce---preview-trial"></a><span data-ttu-id="cf2f3-117">Dynamics 365 Project Operations (CE) - Aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="cf2f3-117">Dynamics 365 Project Operations (CE) - Preview Trial</span></span> 

<span data-ttu-id="cf2f3-118">Hasi aurretik, ziurtatu proiektuaren eragiketen aurrebista nahi duzun maizterrean erabiltzailearen laneko kontua duen arakatzailean saioa hasi duzula.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-118">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="cf2f3-119">Erabili lehen eskaintza kodea, **Dynamics 365 Project Operations** hemen [Project Operations proba](https://aka.ms/try-po).</span><span class="sxs-lookup"><span data-stu-id="cf2f3-119">Redeem the first offer code, **Dynamics 365 Project Operations** here [Project Operations Trial](https://aka.ms/try-po).</span></span>
2. <span data-ttu-id="cf2f3-120">Berretsi eskaera.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-120">Confirm your order.</span></span>

  <span data-ttu-id="cf2f3-121">Baieztapen eskaintza behar bezala berreskuratu dela ikusiko duzu.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-121">You will see confirmation offer was successfully redeemed.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="cf2f3-122">Dynamics 365 Finance aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="cf2f3-122">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="cf2f3-123">Joan [Dynamics 365 for Finance aurrebista proba](https://aka.ms/trypoche) eta errepikatu aurreko ataleko urratsak eskaintzarekin, Erregistratu hodeian ostatatutako ingurunean.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-123">Go to [Dynamics 365 for Finance Preview Trial](https://aka.ms/trypoche) and repeat the steps from the previous section with the offer, Sign up for the Cloud Hosted Environment.</span></span>  

## <a name="assign-licenses"></a><span data-ttu-id="cf2f3-124">Esleitu lizentziak</span><span class="sxs-lookup"><span data-stu-id="cf2f3-124">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cf2f3-125">Zure erakundeko Microsoft 365 Portal-erako sarbide administratiboa beharko duzu urrats hauek burutzeko.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-125">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="cf2f3-126">Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) aukerara, zure erabiltzaileei lizentziak emateko.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-126">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

2. <span data-ttu-id="cf2f3-127">**Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-127">On the **Active users** page, select the users that you want to assign a license to.</span></span>

3. <span data-ttu-id="cf2f3-128">Egiaztatu **Dynamics 365 Project Operations** lizentzia hautatu dela eta hautatu **Aldaketak gorde**.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-128">Verify that the **Dynamics 365 Project Operations** license has been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="cf2f3-129">Finantza probako eskaintza ez zaio erabiltzaile bati esleitu behar.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-129">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="cf2f3-130">Sortu proiektua LCS-n</span><span class="sxs-lookup"><span data-stu-id="cf2f3-130">Start a new project in LCS</span></span>

<span data-ttu-id="cf2f3-131">Sortu LCS proiektu berria gaian azaltzen den moduan, [Hasi proiektu berri bat LCSn](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="cf2f3-131">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="cf2f3-132">Gehitu Azure harpidetza LCS proiektu batean</span><span class="sxs-lookup"><span data-stu-id="cf2f3-132">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="cf2f3-133">Zeregin hori burutzeko, jarraitu gaiaren urratsak, [Gehitu Azure harpidetza LCS proiektuari](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="cf2f3-133">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="cf2f3-134">Inplementatu Finantza demo ingurunea, Project Operations-ekin baliabideak/hornitu gabeko agertokietarako</span><span class="sxs-lookup"><span data-stu-id="cf2f3-134">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="cf2f3-135">Jarraitu gaiaren argibideak, [Ingurune berria hornitzea](resource-provision-new-environment.md) hedapena osatzeko.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-135">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="cf2f3-136">Erabili [demo-ingurunea](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) inplementazio mota aurrebistarako.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-136">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="cf2f3-137">Instalatu CDS konfigurazioa eta konfigurazio-datuak</span><span class="sxs-lookup"><span data-stu-id="cf2f3-137">Install CDS setup and configuration data</span></span>

<span data-ttu-id="cf2f3-138">Instalatu CDS konfigurazio eta konfigurazio datuak gaian deskribatutako moduan, [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="cf2f3-138">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="cf2f3-139">Egin urrats hau Finantzako demo ingurunea inplementatu eta demo datuak prest egon ondoren.</span><span class="sxs-lookup"><span data-stu-id="cf2f3-139">Complete this step only after Finance demo environment is deployed and demo data is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
