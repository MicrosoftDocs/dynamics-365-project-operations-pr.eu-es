---
title: Gehitu Azure harpidetza LCS proiektu batean
description: Gai honek zure Azure harpidetza LCS proiektu batera konektatzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e741f35f9b229d2897cec06054d91ae620397228
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175786"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="4c736-103">Gehitu Azure harpidetza LCS proiektu batean</span><span class="sxs-lookup"><span data-stu-id="4c736-103">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="4c736-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="4c736-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="4c736-105">Hodeian ostatatutako inguruneak lehendik dagoen Azure harpidetza erabiliz inplementatu behar dira.</span><span class="sxs-lookup"><span data-stu-id="4c736-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="4c736-106">Gai honek zure lehendik duzun Azure harpidetza LCS proiektu batera konektatzeko moduari buruzko informazioa azaltzen du.</span><span class="sxs-lookup"><span data-stu-id="4c736-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="4c736-107">Eman administratzailearen baimena</span><span class="sxs-lookup"><span data-stu-id="4c736-107">Grant admin consent</span></span>

1. <span data-ttu-id="4c736-108">Zure LCS proiektuan, **Inguruneak** atala, hautatu **Microsoft Azure ezarpenak**.</span><span class="sxs-lookup"><span data-stu-id="4c736-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![Microsoft Azure ezarpenak](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="4c736-110">**Proiektuaren ezarpenak** orrialdean, **Azure konektoreak** fitxa, hautatu **Baimendu**.</span><span class="sxs-lookup"><span data-stu-id="4c736-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="4c736-111">Horri esker, inguruneak proiektu honetara zabaldu daitezke.</span><span class="sxs-lookup"><span data-stu-id="4c736-111">This allows environments to be deployed to this project.</span></span>

![Azure konektoreak](./media/2AzureConnectors.png)

3. <span data-ttu-id="4c736-113">Aukeratu **Baimendu** berriro administratzailearen baimena emateko.</span><span class="sxs-lookup"><span data-stu-id="4c736-113">Select **Authorize** again to provide admin consent.</span></span>

![Eman administratzailearen baimena](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="4c736-115">Onartu baimen eskaera.</span><span class="sxs-lookup"><span data-stu-id="4c736-115">Accept the permissions request.</span></span>

![Onartu baimen-eskaera](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="4c736-117">Baimena amaitu da.</span><span class="sxs-lookup"><span data-stu-id="4c736-117">The authorization is now complete.</span></span> 

![Baimena arrakastatsua da](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="4c736-119">Eman Dynamics Deployment Services sarbidea Azure harpidetzarako</span><span class="sxs-lookup"><span data-stu-id="4c736-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="4c736-120">Joan [Microsoft Azure fakturazioa](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) aukerara eta hautatu harpidetza.</span><span class="sxs-lookup"><span data-stu-id="4c736-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="4c736-121">Dynamics Deployment Services-ek harpidetza honetara sartu behar du inguruneak zabaldu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="4c736-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![Azure harpidetzaren xehetasunak](./media/6AzureSubscription.png)

2. <span data-ttu-id="4c736-123">Aukeratu **Sarbide kontrola (IAM)** nabigazio panelean, eta hautatu **Gehitu rol esleipena**.</span><span class="sxs-lookup"><span data-stu-id="4c736-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="4c736-124">Eskuineko aldean, hautatu **Laguntzaile-funtzioa**, eta emandako zerrendan, bilatu eta hautatu **Dynamics-en inplementazio-zerbitzuak**.</span><span class="sxs-lookup"><span data-stu-id="4c736-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="4c736-125">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="4c736-125">Select **Save**.</span></span>

![Harpidetzaren sarbidea](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="4c736-127">Gehitu harpidetzaren konektorea LCS proiektu batean</span><span class="sxs-lookup"><span data-stu-id="4c736-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="4c736-128">Zure LCS proiektuan **Microsoft Azure ezarpenak** orrialdean, hautatu **Gehitu** konektore berria gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="4c736-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="4c736-129">Idatzi zure Azure harpidetzaren IDa.</span><span class="sxs-lookup"><span data-stu-id="4c736-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="4c736-130">Zure Azure harpidetzaren IDa [Azure atarian](https://ms.portal.azure.com/), **Ezarpenak** pantailaren beheko ezkerrean.</span><span class="sxs-lookup"><span data-stu-id="4c736-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="4c736-131">**Konfiguratu Azure Resource Manager erabiltzeko** eremuan, hautatu **Bai**.</span><span class="sxs-lookup"><span data-stu-id="4c736-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="4c736-132">Ziurtatu Azure Harpidetzaren AAD maizter domeinua erabiltzen ari zaren domeinuaren jabe den Azure harpidetzarekin bat datorrela eta hautatu **Hurrengoa**.</span><span class="sxs-lookup"><span data-stu-id="4c736-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="4c736-133">**Microsoft Azure Konfigurazioa** pantailan, hautatu **Hurrengoa** baieztatzeko.</span><span class="sxs-lookup"><span data-stu-id="4c736-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="4c736-134">Pantaila honetan errore bat jasotzen baduzu, itzuli [Eman Dynamics Deployment Services sarbidea Azure harpidetzarako](#provide) atalera gai honetan eta ziurtatu urrats guztiak bete dituzula.</span><span class="sxs-lookup"><span data-stu-id="4c736-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="4c736-135">Deskargatu Azure kudeaketa ziurtagiria zure ordenagailuko karpeta lokal batera eta, ondoren, igo Azure kudeaketa atarira joan **Ezarpenak** >  **Kudeaketa ziurtagiriak**.</span><span class="sxs-lookup"><span data-stu-id="4c736-135">Download the Azure Management Certificate to a local folder on your computer, and then upload it to Azure Management Portal by going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="4c736-136">Ziurtagiri honi esker, LCSk Azure-rekin zure izenean komunikatzeko aukera emango du.</span><span class="sxs-lookup"><span data-stu-id="4c736-136">This certificate will enable LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="4c736-137">Urrats hau salta dezakezu zure erabiltzaileak harpidetzarako sarbidea badu.</span><span class="sxs-lookup"><span data-stu-id="4c736-137">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="4c736-138">Hautatu **Hurrengoa**.</span><span class="sxs-lookup"><span data-stu-id="4c736-138">Select  **Next**.</span></span>
8. <span data-ttu-id="4c736-139">Aukeratu zabaltzeko Azure eskualdea eta hautatu sistema hau erabiltzeko asmoa duzun tokitik gertu dagoen datu zentroa.</span><span class="sxs-lookup"><span data-stu-id="4c736-139">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="4c736-140">Hautatu **Konektatu**.</span><span class="sxs-lookup"><span data-stu-id="4c736-140">Select  **Connect**.</span></span>

<span data-ttu-id="4c736-141">Azure harpidetza behar bezala konektatu duzu.</span><span class="sxs-lookup"><span data-stu-id="4c736-141">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="4c736-142">Orain zabaldu dezakezu Dynamics 365 Finance hodeian ostatatutako inguruneak.</span><span class="sxs-lookup"><span data-stu-id="4c736-142">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>


