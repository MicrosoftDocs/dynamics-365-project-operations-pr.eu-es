---
title: Konfiguratu parametro-ezarpen osagarriak
description: Nola konfiguratu parametro gehigarriaren ezarpenak Project Service-n
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: de2fe830-4313-4711-b03b-76d56bf56cb6
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: f3e110163088f8e3b78da9f273113d74775bf24c
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748958"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="cbf78-103">Konfiguratu parametro gehigarriaren ezarpenak (Project Service)</span><span class="sxs-lookup"><span data-stu-id="cbf78-103">Configure additional parameter settings (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="cbf78-104">Aurreko gaiko elementuak konfiguratu ostean, proiektu-parametro osagarriak ezarri behar dituzu zure proiektuetarako.</span><span class="sxs-lookup"><span data-stu-id="cbf78-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="cbf78-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] instalatu ostean, [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] zerbitzuak funtzionatzeko behar diren erregistro guztien parametro-ezarpena sortu duzu.</span><span class="sxs-lookup"><span data-stu-id="cbf78-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="cbf78-106">Itzuli eta ezarpen horien eremu osagarriak konfiguratzeko unea da.</span><span class="sxs-lookup"><span data-stu-id="cbf78-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="cbf78-107">Ezarpen hauek konfiguratuta izan behar dituzu:</span><span class="sxs-lookup"><span data-stu-id="cbf78-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="cbf78-108">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="cbf78-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="cbf78-109">Fakturen maiztasuna</span><span class="sxs-lookup"><span data-stu-id="cbf78-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="cbf78-110">Lanorduen txantiloiak</span><span class="sxs-lookup"><span data-stu-id="cbf78-110">Work hours template</span></span>  
  
-   <span data-ttu-id="cbf78-111">Prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="cbf78-111">Price list</span></span>  
 
<span data-ttu-id="cbf78-112">Urrats honetan, zein baliabide-esleipen mota nahi duzun ere adierazi behar duzu:</span><span class="sxs-lookup"><span data-stu-id="cbf78-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="cbf78-113">**Erdialdekoa**.</span><span class="sxs-lookup"><span data-stu-id="cbf78-113">**Central**.</span></span> <span data-ttu-id="cbf78-114">Baliabide-kudeatzaileek soilik eslei ditzakete baliabideak proiektuei.</span><span class="sxs-lookup"><span data-stu-id="cbf78-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="cbf78-115">**Hibridoa**.</span><span class="sxs-lookup"><span data-stu-id="cbf78-115">**Hybrid**.</span></span> <span data-ttu-id="cbf78-116">Baliabide-kudeatzaileek, proiektu-kudeatzaileek eta kontu-kudeatzaileek eslei ditzakete baliabideak proiektuei.</span><span class="sxs-lookup"><span data-stu-id="cbf78-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="cbf78-117">Proiektu-parametroak ezartzeko:</span><span class="sxs-lookup"><span data-stu-id="cbf78-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="cbf78-118">Joan **Project Service > Parametroak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="cbf78-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="cbf78-119">Sakatu konfiguratu nahi duzun parametro-ezarpena ([!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] lehen aldiz instalatu ostean), edo sakatu **Berria** berri bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="cbf78-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="cbf78-120">**Orokorra** eremuan, ezarri zure proiektu-parametroaren aukera guztiak.</span><span class="sxs-lookup"><span data-stu-id="cbf78-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="cbf78-121">**Prezio-zerrenda** eremuan, sakatu **+** prezio-zerrendak gehitzeko, prezio-zerrendak hautzeko **Proiektu-parametroaren prezio-zerrenda** goitibeherako zerrendan eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="cbf78-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="cbf78-122">Sakatu **Gorde** pantailaren behe-eskuineko izkinako botoia.</span><span class="sxs-lookup"><span data-stu-id="cbf78-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="cbf78-123">Proiektuaren parametro-erregistroa mantendu behar da Project Service-rako zuzen funtziona dezan.</span><span class="sxs-lookup"><span data-stu-id="cbf78-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="cbf78-124">Erregistro hau ez da ezabatu behar.</span><span class="sxs-lookup"><span data-stu-id="cbf78-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="cbf78-125">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="cbf78-125">See Also</span></span>  
 [<span data-ttu-id="cbf78-126">Baliabideak konfiguratu</span><span class="sxs-lookup"><span data-stu-id="cbf78-126">Set up resources</span></span>](../project-service/set-up-resources.md)
