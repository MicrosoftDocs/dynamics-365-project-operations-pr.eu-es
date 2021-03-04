---
title: Konfiguratu Project Service Automation
description: Project Service konfiguratzeko urratsak
author: ruhercul
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
ms.openlocfilehash: ec5381f91b1fe5198bd93ac8d6015b1fea38738d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146918"
---
# <a name="configure-project-service"></a><span data-ttu-id="30cf0-103">Konfiguratu Project Service</span><span class="sxs-lookup"><span data-stu-id="30cf0-103">Configure Project Service</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="30cf0-104">[!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] aplikazioan kontuak, proiektuak eta baliabideak kudeatzeko [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automatizazioaren gaitasunak erabili ahal izateko, konfigurazio-urrats batzuk bete behar dituzu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] eta erakundearen beharrak bat datozela ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="30cf0-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="30cf0-105">Urratsak hauek dira:</span><span class="sxs-lookup"><span data-stu-id="30cf0-105">These steps include:</span></span>  
  
-   <span data-ttu-id="30cf0-106">[Konfiguratu denbora-unitateak](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="30cf0-107">Konfiguratu denbora-unitateak proiektuak antolatzeko eta fakturatzeko oinarri gisa erabiliko duzun produktu-katalogoan.</span><span class="sxs-lookup"><span data-stu-id="30cf0-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="30cf0-108">[Konfiguratu monetak eta truke-tasak](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="30cf0-109">Konfiguratu proiektuetan erabiltzeko monetak.</span><span class="sxs-lookup"><span data-stu-id="30cf0-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="30cf0-110">[Sortu erakunde-unitateak](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="30cf0-111">Konfiguratu zure enpresan negozioak zatitzeko erabiltzen dituen taldeak, geografiaren, negozio-funtzioaren edo beste zatiketa-logika baten arabera.</span><span class="sxs-lookup"><span data-stu-id="30cf0-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="30cf0-112">[Konfiguratu fakturen maiztasunak](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="30cf0-113">Konfiguratu bezeroak fakturatzeko erabili nahi dituzun denbora-epeak.</span><span class="sxs-lookup"><span data-stu-id="30cf0-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="30cf0-114">[Konfiguratu transakzio-kategoriak](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="30cf0-115">Konfiguratu zure aholkulariek fakturatu ditzaketen eta fakturatu ezin ditzaketen transakzio-kategoriak.</span><span class="sxs-lookup"><span data-stu-id="30cf0-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="30cf0-116">[Konfiguratu gastu-kategoriak](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="30cf0-117">Konfiguratu zure aholkulariek fakturatu ditzaketen eta fakturatu ezin ditzaketen kategoriak.</span><span class="sxs-lookup"><span data-stu-id="30cf0-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="30cf0-118">[Sortu produktu-katalogoko elementuak](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="30cf0-119">Gehitu produktu-katalogoan saltzen dituzun produktuak, hala nola software-lizentziak.</span><span class="sxs-lookup"><span data-stu-id="30cf0-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="30cf0-120">[Sortu prezio-zerrenda](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="30cf0-121">Konfiguratu prezio-zerrendak, bezeroek beren proeiktuetarako eskatzen dituzten funtzio bakoitzerako kobratu nahi diezun.</span><span class="sxs-lookup"><span data-stu-id="30cf0-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="30cf0-122">[Baliabideak konfiguratu](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="30cf0-123">Gehitu zure proiektuetarako behar dituzun trebakuntzak, gaitasunak, baliabide-funtzioak eta bestelako baliabide-informazioa.</span><span class="sxs-lookup"><span data-stu-id="30cf0-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="30cf0-124">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="30cf0-124">See Also</span></span>  
 <span data-ttu-id="30cf0-125">[Project Service Automation-en ikuspegi orokorra](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="30cf0-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="30cf0-126">[Konfiguratu Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="30cf0-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="30cf0-127">[Kontu-kudeatzailearen gida](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="30cf0-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="30cf0-128">[Proiektu-kudeatzailearen gida](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="30cf0-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="30cf0-129">[Baliabide-kudeatzailearen gida](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="30cf0-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="30cf0-130">Denboraren, gastuen eta lankidetzaren gida</span><span class="sxs-lookup"><span data-stu-id="30cf0-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)
