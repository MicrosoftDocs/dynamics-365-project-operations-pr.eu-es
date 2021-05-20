---
title: Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan
description: Gai honek Project Operations-era harpidetzeko eta hedatzeko moduari buruzko informazioa eskaintzen du berreskuratutako / stockean oinarritutako eszenatokietarako.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 917ead8ff6d9d3ef8374f8ccde608b6cebd50c8c
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948449"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="2640a-103">Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan</span><span class="sxs-lookup"><span data-stu-id="2640a-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="2640a-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="2640a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="2640a-105">Gai honetan aurrebista/bazkide eskaintzara nola harpidetu eta Project Operations-en ingurunea nola hornitu azaltzen da baliabideetan/stockean oinarritutako eszenatokietan.</span><span class="sxs-lookup"><span data-stu-id="2640a-105">This topic explains how to subscribe to the preview/partner offer and deploy Project Operations environment for resource/ non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2640a-106">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="2640a-106">Prerequisites</span></span>

- <span data-ttu-id="2640a-107">Mezu elektroniko bat jasoko duzu aurrebistan parte hartzera gonbidatzen zaituena.</span><span class="sxs-lookup"><span data-stu-id="2640a-107">You will receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="2640a-108">Aurreikuspena eska dezakezu [Project Operations webgunea](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span><span class="sxs-lookup"><span data-stu-id="2640a-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="2640a-109">Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu.</span><span class="sxs-lookup"><span data-stu-id="2640a-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="2640a-110">Finantza ingurunea hedatzeko baliozko Azure harpidetza behar da ingurune bakoitzeko fakturatuko dena.</span><span class="sxs-lookup"><span data-stu-id="2640a-110">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="2640a-111">Zure erakundeetan dagoen harpidetza erabil dezakezu edo [Azure proba](https://azure.microsoft.com/en-us/free/) erabiltzen hasteko.</span><span class="sxs-lookup"><span data-stu-id="2640a-111">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="2640a-112">CDS ingurunea doan emango da 30 eguneko epean.</span><span class="sxs-lookup"><span data-stu-id="2640a-112">The CDS environment will be provided free for a limited 30 day period.</span></span>

## <a name="subscribe"></a><span data-ttu-id="2640a-113">Harpidetu</span><span class="sxs-lookup"><span data-stu-id="2640a-113">Subscribe</span></span>

<span data-ttu-id="2640a-114">Zure [aurrebista eskaera](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) onartuta dago, Microsoft-en hiru eskaintza jasoko dituzu posta elektronikoz.</span><span class="sxs-lookup"><span data-stu-id="2640a-114">When your [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) is approved, you will receive three offers from Microsoft by email.</span></span> <span data-ttu-id="2640a-115">Eskaintza hauei esker, Project Operations-en aurrebista hedatu dezakezu:</span><span class="sxs-lookup"><span data-stu-id="2640a-115">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="2640a-116">Dynamics 365 Project Operations (CRM) - Aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="2640a-116">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span>
- <span data-ttu-id="2640a-117">Office 365 Project Operations - Aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="2640a-117">Office 365 Project Operations - Preview Trial</span></span>
- <span data-ttu-id="2640a-118">Dynamics 365 Finance - Aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="2640a-118">Dynamics 365 Finance - Preview Trial</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2640a-119">Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori.</span><span class="sxs-lookup"><span data-stu-id="2640a-119">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="2640a-120">Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.</span><span class="sxs-lookup"><span data-stu-id="2640a-120">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations-crm---preview-trial"></a><span data-ttu-id="2640a-121">Dynamics 365 Project Operations (CRM) - Aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="2640a-121">Dynamics 365 Project Operations (CRM) - Preview Trial</span></span> 

<span data-ttu-id="2640a-122">Hasi aurretik, ziurtatu proiektuaren eragiketen aurrebista nahi duzun maizterrean erabiltzailearen laneko kontua duen arakatzailean saioa hasi duzula.</span><span class="sxs-lookup"><span data-stu-id="2640a-122">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="2640a-123">Erabili lehen eskaintza kodea, **Dynamics 365 Project Operations (CRM) - Aurrebista proba** arakatzailearen URLan itsatsita.</span><span class="sxs-lookup"><span data-stu-id="2640a-123">Redeem the first offer code, **Dynamics 365 Project Operations (CRM) - Preview Trial** by pasting it into the browser URL.</span></span>

![Erabili Eskaintza](./media/16RedeemFirstOfferNew.png)

2. <span data-ttu-id="2640a-125">Berretsi eskaera.</span><span class="sxs-lookup"><span data-stu-id="2640a-125">Confirm your order.</span></span>

![Berretsi eskaera](./media/17ConfirmOrderNew.png)

<span data-ttu-id="2640a-127">Baieztapen eskaintza behar bezala berreskuratu dela ikusiko duzu.</span><span class="sxs-lookup"><span data-stu-id="2640a-127">You will see confirmation offer was successfully redeemed.</span></span>

![Berrespena](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a><span data-ttu-id="2640a-129">Office 365 Project Operations - Aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="2640a-129">Office 365 Project Operations - Preview Trial</span></span>

<span data-ttu-id="2640a-130">Errepikatu eskaintzaren lehen kodearen urrats berdinak.</span><span class="sxs-lookup"><span data-stu-id="2640a-130">Repeat the same steps as with the first offer code.</span></span> <span data-ttu-id="2640a-131">Ziurtatu bigarren eskaintza kodea gehitzen duzula lehen eskaintza kodearekin erabilitako erabiltzaile kontu bera erabiliz.</span><span class="sxs-lookup"><span data-stu-id="2640a-131">Make sure to add the second offer code using the same user account that was used with the first offer code.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="2640a-132">Dynamics 365 Finance aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="2640a-132">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="2640a-133">Errepikatu urrats berdinak Ongietorri posta elektronikoko azken eskaintzarekin.</span><span class="sxs-lookup"><span data-stu-id="2640a-133">Repeat the same steps with the last offer from the Welcome email.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="2640a-134">Esleitu lizentziak</span><span class="sxs-lookup"><span data-stu-id="2640a-134">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2640a-135">Zure erakundeko Microsoft 365 Portal-erako sarbide administratiboa beharko duzu urrats hauek burutzeko.</span><span class="sxs-lookup"><span data-stu-id="2640a-135">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="2640a-136">Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) aukerara, zure erabiltzaileei lizentziak emateko.</span><span class="sxs-lookup"><span data-stu-id="2640a-136">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

![Administrazio zentroaren hasierako orria](./media/14AdminPortal.png)

2. <span data-ttu-id="2640a-138">**Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.</span><span class="sxs-lookup"><span data-stu-id="2640a-138">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![Esleitu lizentziak](./media/15AssignLicenses.png)

3. <span data-ttu-id="2640a-140">Egiaztatu **Dynamics 365 Project Operations (CRM) Aurrebista** eta **Office 365 Proiektuaren eragiketak - Aurrebista** lizentzia hautatu eta hautatu **Aldaketak gorde**.</span><span class="sxs-lookup"><span data-stu-id="2640a-140">Verify that the **Dynamics 365 Project Operations (CRM) Preview** and **Office 365 Project Operations - Preview** license have been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="2640a-141">Finantza probako eskaintza ez zaio erabiltzaile bati esleitu behar.</span><span class="sxs-lookup"><span data-stu-id="2640a-141">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="2640a-142">Sortu proiektua LCS-n</span><span class="sxs-lookup"><span data-stu-id="2640a-142">Start a new project in LCS</span></span>

<span data-ttu-id="2640a-143">Sortu LCS proiektu berria gaian azaltzen den moduan, [Hasi proiektu berri bat LCSn](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="2640a-143">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="2640a-144">Gehitu Azure harpidetza LCS proiektu batean</span><span class="sxs-lookup"><span data-stu-id="2640a-144">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="2640a-145">Zeregin hori burutzeko, jarraitu gaiaren urratsak, [Gehitu Azure harpidetza LCS proiektuari](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="2640a-145">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="2640a-146">Inplementatu Finantza demo ingurunea, Project Operations-ekin baliabideak/hornitu gabeko agertokietarako</span><span class="sxs-lookup"><span data-stu-id="2640a-146">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="2640a-147">Jarraitu gaiaren argibideak, [Ingurune berria hornitzea](resource-provision-new-environment.md) hedapena osatzeko.</span><span class="sxs-lookup"><span data-stu-id="2640a-147">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="2640a-148">Erabili [demo-ingurunea](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) inplementazio mota aurrebistarako.</span><span class="sxs-lookup"><span data-stu-id="2640a-148">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="2640a-149">Instalatu CDS konfigurazioa eta konfigurazio-datuak</span><span class="sxs-lookup"><span data-stu-id="2640a-149">Install CDS setup and configuration data</span></span>

<span data-ttu-id="2640a-150">Instalatu CDS konfigurazio eta konfigurazio datuak gaian deskribatutako moduan, [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="2640a-150">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="2640a-151">Osatu urrats hau Finantza demo ingurunea zabaldu eta FOko demo datuak prest egon ondoren.</span><span class="sxs-lookup"><span data-stu-id="2640a-151">Complete this step only after Finance demo environment is deployed and demo data in FO is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]