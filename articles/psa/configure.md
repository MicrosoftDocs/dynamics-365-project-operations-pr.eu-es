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
ms.openlocfilehash: 8a219ef0166565a550a7836ffeae37ffd514a001
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129168"
---
# <a name="configure-project-service"></a><span data-ttu-id="ae426-103">Konfiguratu Project Service</span><span class="sxs-lookup"><span data-stu-id="ae426-103">Configure Project Service</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="ae426-104">[!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] aplikazioan kontuak, proiektuak eta baliabideak kudeatzeko [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automatizazioaren gaitasunak erabili ahal izateko, konfigurazio-urrats batzuk bete behar dituzu [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] eta erakundearen beharrak bat datozela ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="ae426-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="ae426-105">Urratsak hauek dira:</span><span class="sxs-lookup"><span data-stu-id="ae426-105">These steps include:</span></span>  
  
-   <span data-ttu-id="ae426-106">[Konfiguratu denbora-unitateak](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="ae426-107">Konfiguratu denbora-unitateak proiektuak antolatzeko eta fakturatzeko oinarri gisa erabiliko duzun produktu-katalogoan.</span><span class="sxs-lookup"><span data-stu-id="ae426-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="ae426-108">[Konfiguratu monetak eta truke-tasak](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="ae426-109">Konfiguratu proiektuetan erabiltzeko monetak.</span><span class="sxs-lookup"><span data-stu-id="ae426-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="ae426-110">[Sortu erakunde-unitateak](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="ae426-111">Konfiguratu zure enpresan negozioak zatitzeko erabiltzen dituen taldeak, geografiaren, negozio-funtzioaren edo beste zatiketa-logika baten arabera.</span><span class="sxs-lookup"><span data-stu-id="ae426-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="ae426-112">[Konfiguratu fakturen maiztasunak](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="ae426-113">Konfiguratu bezeroak fakturatzeko erabili nahi dituzun denbora-epeak.</span><span class="sxs-lookup"><span data-stu-id="ae426-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="ae426-114">[Konfiguratu transakzio-kategoriak](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="ae426-115">Konfiguratu zure aholkulariek fakturatu ditzaketen eta fakturatu ezin ditzaketen transakzio-kategoriak.</span><span class="sxs-lookup"><span data-stu-id="ae426-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="ae426-116">[Konfiguratu gastu-kategoriak](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="ae426-117">Konfiguratu zure aholkulariek fakturatu ditzaketen eta fakturatu ezin ditzaketen kategoriak.</span><span class="sxs-lookup"><span data-stu-id="ae426-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="ae426-118">[Sortu produktu-katalogoko elementuak](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="ae426-119">Gehitu produktu-katalogoan saltzen dituzun produktuak, hala nola software-lizentziak.</span><span class="sxs-lookup"><span data-stu-id="ae426-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="ae426-120">[Sortu prezio-zerrenda](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="ae426-121">Konfiguratu prezio-zerrendak, bezeroek beren proeiktuetarako eskatzen dituzten funtzio bakoitzerako kobratu nahi diezun.</span><span class="sxs-lookup"><span data-stu-id="ae426-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="ae426-122">[Baliabideak konfiguratu](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="ae426-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="ae426-123">Gehitu zure proiektuetarako behar dituzun trebakuntzak, gaitasunak, baliabide-funtzioak eta bestelako baliabide-informazioa.</span><span class="sxs-lookup"><span data-stu-id="ae426-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="ae426-124">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="ae426-124">See Also</span></span>  
 <span data-ttu-id="ae426-125">[Project Service Automation-en ikuspegi orokorra](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="ae426-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="ae426-126">[Konfiguratu Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="ae426-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="ae426-127">[Kontu-kudeatzailearen gida](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae426-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="ae426-128">[Proiektu-kudeatzailearen gida](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae426-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="ae426-129">[Baliabide-kudeatzailearen gida](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae426-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="ae426-130">Denboraren, gastuen eta lankidetzaren gida</span><span class="sxs-lookup"><span data-stu-id="ae426-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)
