---
title: Konfiguratu parametro-ezarpen osagarriak
description: Nola konfiguratu parametro gehigarriaren ezarpenak Project Service-n
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bac484e29f1a0578042f350b1657a42e80b48cb4
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290749"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="a5990-103">Konfiguratu parametro gehigarriaren ezarpenak (Project Service)</span><span class="sxs-lookup"><span data-stu-id="a5990-103">Configure additional parameter settings (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="a5990-104">Aurreko gaiko elementuak konfiguratu ostean, proiektu-parametro osagarriak ezarri behar dituzu zure proiektuetarako.</span><span class="sxs-lookup"><span data-stu-id="a5990-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="a5990-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] instalatu ostean, [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] zerbitzuak funtzionatzeko behar diren erregistro guztien parametro-ezarpena sortu duzu.</span><span class="sxs-lookup"><span data-stu-id="a5990-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="a5990-106">Itzuli eta ezarpen horien eremu osagarriak konfiguratzeko unea da.</span><span class="sxs-lookup"><span data-stu-id="a5990-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="a5990-107">Ezarpen hauek konfiguratuta izan behar dituzu:</span><span class="sxs-lookup"><span data-stu-id="a5990-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="a5990-108">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="a5990-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="a5990-109">Fakturen maiztasuna</span><span class="sxs-lookup"><span data-stu-id="a5990-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="a5990-110">Lanorduen txantiloiak</span><span class="sxs-lookup"><span data-stu-id="a5990-110">Work hours template</span></span>  
  
-   <span data-ttu-id="a5990-111">Prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="a5990-111">Price list</span></span>  
 
<span data-ttu-id="a5990-112">Urrats honetan, zein baliabide-esleipen mota nahi duzun ere adierazi behar duzu:</span><span class="sxs-lookup"><span data-stu-id="a5990-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="a5990-113">**Erdialdekoa**.</span><span class="sxs-lookup"><span data-stu-id="a5990-113">**Central**.</span></span> <span data-ttu-id="a5990-114">Baliabide-kudeatzaileek soilik eslei ditzakete baliabideak proiektuei.</span><span class="sxs-lookup"><span data-stu-id="a5990-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="a5990-115">**Hibridoa**.</span><span class="sxs-lookup"><span data-stu-id="a5990-115">**Hybrid**.</span></span> <span data-ttu-id="a5990-116">Baliabide-kudeatzaileek, proiektu-kudeatzaileek eta kontu-kudeatzaileek eslei ditzakete baliabideak proiektuei.</span><span class="sxs-lookup"><span data-stu-id="a5990-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="a5990-117">Proiektu-parametroak ezartzeko:</span><span class="sxs-lookup"><span data-stu-id="a5990-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="a5990-118">Joan **Project Service > Parametroak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="a5990-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="a5990-119">Sakatu konfiguratu nahi duzun parametro-ezarpena ([!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] lehen aldiz instalatu ostean), edo sakatu **Berria** berri bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="a5990-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="a5990-120">**Orokorra** eremuan, ezarri zure proiektu-parametroaren aukera guztiak.</span><span class="sxs-lookup"><span data-stu-id="a5990-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="a5990-121">**Prezio-zerrenda** eremuan, sakatu **+** prezio-zerrendak gehitzeko, prezio-zerrendak hautzeko **Proiektu-parametroaren prezio-zerrenda** goitibeherako zerrendan eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="a5990-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="a5990-122">Sakatu **Gorde** pantailaren behe-eskuineko izkinako botoia.</span><span class="sxs-lookup"><span data-stu-id="a5990-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="a5990-123">Proiektuaren parametro-erregistroa mantendu behar da Project Service-rako zuzen funtziona dezan.</span><span class="sxs-lookup"><span data-stu-id="a5990-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="a5990-124">Erregistro hau ez da ezabatu behar.</span><span class="sxs-lookup"><span data-stu-id="a5990-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="a5990-125">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="a5990-125">See Also</span></span>  
 [<span data-ttu-id="a5990-126">Baliabideak konfiguratu</span><span class="sxs-lookup"><span data-stu-id="a5990-126">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]