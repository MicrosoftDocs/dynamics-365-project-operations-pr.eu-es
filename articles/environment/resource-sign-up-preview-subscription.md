---
title: Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan
description: Gai honek Project Operations-era harpidetzeko eta hedatzeko moduari buruzko informazioa eskaintzen du berreskuratutako / stockean oinarritutako eszenatokietarako.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d35a8bf9e8a841b45808b26ae2587c5b7d99d72
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948732"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="406b7-103">Eman izena Project Operations-en aurrebista harpidetzak baliabideetan / hornitu gabeko agertokietan</span><span class="sxs-lookup"><span data-stu-id="406b7-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="406b7-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="406b7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="406b7-105">Gai honetan aurrebista/bazkide eskaintzara nola harpidetu eta Project Operations-en ingurunea nola hornitu azaltzen da baliabideetan/stockean oinarritutako eszenatokietan.</span><span class="sxs-lookup"><span data-stu-id="406b7-105">This topic explains how to subscribe to the preview/partner offer and deploy Project Operations environment for resource/ non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="406b7-106">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="406b7-106">Prerequisites</span></span>

- <span data-ttu-id="406b7-107">Mezu elektroniko bat jasoko duzu aurrebistan parte hartzera gonbidatzen zaituena.</span><span class="sxs-lookup"><span data-stu-id="406b7-107">You will receive an email inviting you to participate in the preview.</span></span> <span data-ttu-id="406b7-108">Aurreikuspena eska dezakezu [Project Operations webgunea](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span><span class="sxs-lookup"><span data-stu-id="406b7-108">You can request a preview on the [Project Operations website](https://dynamics.microsoft.com/en-us/project-operations/overview/).</span></span>
- <span data-ttu-id="406b7-109">Aurrebista zabaltzen duen erabiltzaileak Azure maizter administratzaile eskubide orokorrak izan behar ditu.</span><span class="sxs-lookup"><span data-stu-id="406b7-109">The user who deploys the preview must have Azure tenant global administrator rights.</span></span>
- <span data-ttu-id="406b7-110">Finantza ingurunea hedatzeko baliozko Azure harpidetza behar da ingurune bakoitzeko fakturatuko dena.</span><span class="sxs-lookup"><span data-stu-id="406b7-110">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="406b7-111">Zure erakundeetan dagoen harpidetza erabil dezakezu edo [Azure proba](https://azure.microsoft.com/en-us/free/) erabiltzen hasteko.</span><span class="sxs-lookup"><span data-stu-id="406b7-111">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="406b7-112">CDS ingurunea doan emango da 30 eguneko epean.</span><span class="sxs-lookup"><span data-stu-id="406b7-112">The CDS environment will be provided free for a limited 30 day period.</span></span>

## <a name="subscribe"></a><span data-ttu-id="406b7-113">Harpidetu</span><span class="sxs-lookup"><span data-stu-id="406b7-113">Subscribe</span></span>

<span data-ttu-id="406b7-114">Zure [aurrebista eskaera](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) onartuta dago, Microsoft-en bi eskaintza jasoko dituzu posta elektronikoz.</span><span class="sxs-lookup"><span data-stu-id="406b7-114">When your [preview request](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) is approved, you will receive two offers from Microsoft by email.</span></span> <span data-ttu-id="406b7-115">Eskaintza hauei esker, Project Operations-en aurrebista hedatu dezakezu:</span><span class="sxs-lookup"><span data-stu-id="406b7-115">These offers allow you to deploy the Project Operations Preview:</span></span>

- <span data-ttu-id="406b7-116">Dynamics 365 Project Operations - Aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="406b7-116">Dynamics 365 Project Operations – Preview Trial</span></span>
- <span data-ttu-id="406b7-117">Dynamics 365 for Finance and Operations Aurrebista proba.</span><span class="sxs-lookup"><span data-stu-id="406b7-117">Dynamics 365 for Finance and Operations Preview Trial.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="406b7-118">Erakunde bateko pertsona bakarrak, maizter administratzaileak, egin behar du zeregin hori.</span><span class="sxs-lookup"><span data-stu-id="406b7-118">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="406b7-119">Bertsio honen harpideduna ez bazara, itxaron zure erakundea erregistratu arte eta zure erabiltzaile kredentzialak jaso arte.</span><span class="sxs-lookup"><span data-stu-id="406b7-119">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>

### <a name="dynamics-365-project-operations--preview-trial"></a><span data-ttu-id="406b7-120">Dynamics 365 Project Operations - aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="406b7-120">Dynamics 365 Project Operations – Preview trial</span></span>

1. <span data-ttu-id="406b7-121">Erabili lehen eskaintza, **Dynamics 365 Project Operations Proba**, URLarekin ongi etorritako mezu elektronikoan.</span><span class="sxs-lookup"><span data-stu-id="406b7-121">Redeem the first offer, **Dynamics 365 Project Operations Trial**, with the URL provided in your welcome email.</span></span>

![Lehen Eskaintza](./media/1FirstOffer.png)

2. <span data-ttu-id="406b7-123">Egiaztatu zerbitzuan harpidetuko den erakundeko erabiltzaile gisa hasi duzula saioa.</span><span class="sxs-lookup"><span data-stu-id="406b7-123">Verify that you are logged in as the user who belongs to the organization who will be subscribing to the service.</span></span>
3. <span data-ttu-id="406b7-124">Jarrai ezazu eskaintza trukatzen.</span><span class="sxs-lookup"><span data-stu-id="406b7-124">Proceed with redeeming the offer.</span></span> 
4. <span data-ttu-id="406b7-125">Aukeratu **Bai, gehitu nire kontura**.</span><span class="sxs-lookup"><span data-stu-id="406b7-125">Select **Yes, add it to my account**.</span></span>

![Erabili Eskaintza](./media/2RedeemFirstOffer.png)

![Berretsi eskaintza](./media/3ConfirmFirstOffer.png)

![Erabili da eskaintza](./media/4OfferSuccessfulyRedeemed.png)

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="406b7-129">Dynamics 365 Finance aurrebista proba</span><span class="sxs-lookup"><span data-stu-id="406b7-129">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="406b7-130">Errepikatu urrats berdinak Ongietorri posta elektronikoko bigarren eskaintzarekin.</span><span class="sxs-lookup"><span data-stu-id="406b7-130">Repeat the same steps with the second offer from the Welcome email.</span></span>

## <a name="assign-licenses"></a><span data-ttu-id="406b7-131">Esleitu lizentziak</span><span class="sxs-lookup"><span data-stu-id="406b7-131">Assign Licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="406b7-132">Zure erakundeko Office 365 atarirako sarbide administratiboa beharko duzu urrats hauek burutzeko.</span><span class="sxs-lookup"><span data-stu-id="406b7-132">You will need administrative access to your organization's Office 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="406b7-133">Joan [Microsoft 365 administrazio zentroa](https://portal.office.com/) aukerara, zure erabiltzaileei lizentziak emateko.</span><span class="sxs-lookup"><span data-stu-id="406b7-133">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign licenses to your users.</span></span>

![Office administrazio-ataria](./media/5OfficeAdminPortal.png)

2. <span data-ttu-id="406b7-135">**Erabiltzaile aktiboak** orrian, hautatu lizentzia esleitu nahi diezun erabiltzaileak.</span><span class="sxs-lookup"><span data-stu-id="406b7-135">On the **Active users** page, select the users that you want to assign a license to.</span></span>

![Esleitu lizentziak](./media/6AssignLicenses.png)

3. <span data-ttu-id="406b7-137">Egiaztatu Project Operations lizentzia hautatu dela eta hautatu **Gorde aldaketak**.</span><span class="sxs-lookup"><span data-stu-id="406b7-137">Verify that the Project Operations license has been selected and select **Save changes**.</span></span> 

> [!NOTE]
> <span data-ttu-id="406b7-138">Finantza probako eskaintza ez zaio erabiltzaile bati esleitu behar.</span><span class="sxs-lookup"><span data-stu-id="406b7-138">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="406b7-139">Sortu proiektua LCS-n</span><span class="sxs-lookup"><span data-stu-id="406b7-139">Start a new project in LCS</span></span>

<span data-ttu-id="406b7-140">Sortu LCS proiektu berria gaian azaltzen den moduan, [Hasi proiektu berri bat LCSn](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="406b7-140">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="406b7-141">Gehitu Azure harpidetza LCS proiektu batean</span><span class="sxs-lookup"><span data-stu-id="406b7-141">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="406b7-142">Zeregin hori burutzeko, jarraitu gaiaren urratsak, [Gehitu Azure harpidetza LCS proiektuari](resource-add-azure-subscription-lcs-project.md).</span><span class="sxs-lookup"><span data-stu-id="406b7-142">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="406b7-143">Inplementatu Finantza demo ingurunea, Project Operations-ekin baliabideak/hornitu gabeko agertokietarako</span><span class="sxs-lookup"><span data-stu-id="406b7-143">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="406b7-144">Jarraitu gaiaren argibideak, [Ingurune berria hornitzea](resource-provision-new-environment.md) hedapena osatzeko.</span><span class="sxs-lookup"><span data-stu-id="406b7-144">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="406b7-145">Erabili [demo-ingurunea](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) inplementazio mota aurrebistarako.</span><span class="sxs-lookup"><span data-stu-id="406b7-145">Use the [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span>

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="406b7-146">Instalatu CDS konfigurazioa eta konfigurazio-datuak</span><span class="sxs-lookup"><span data-stu-id="406b7-146">Install CDS setup and configuration data</span></span>

<span data-ttu-id="406b7-147">Instalatu CDS konfigurazio eta konfigurazio datuak gaian deskribatutako moduan, [Konfiguratu eta aplikatu konfigurazio datuak Common Data Service](resource-apply-pro-setup-config-data.md).</span><span class="sxs-lookup"><span data-stu-id="406b7-147">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>

