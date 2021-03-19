---
title: Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera
description: Gai honek Project Operations-eko legezko entitatearen integrazioa konfiguratzeari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ccdbdce6b7d006adc9be2b5f3573dd8e79dd2b8d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276963"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="54bb3-103">Konfiguratu Project Operations-en integrazioa legezko entitatearen arabera</span><span class="sxs-lookup"><span data-stu-id="54bb3-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="54bb3-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="54bb3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="54bb3-105">Gai honek konfiguratzeko beharrezko pausoak ematen dizkizu Dynamics 365 Project Operations pertsona juridiko bakoitzeko.</span><span class="sxs-lookup"><span data-stu-id="54bb3-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="54bb3-106">Gaitu gako nagusiak Dynamics 365 Finance-n</span><span class="sxs-lookup"><span data-stu-id="54bb3-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="54bb3-107">Bete urrats hauek beharrezko eginbideak gaitzeko.</span><span class="sxs-lookup"><span data-stu-id="54bb3-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="54bb3-108">Dynamics 365 Finance-n, joan **Eginbideen kudeaketa** lan-eremura.</span><span class="sxs-lookup"><span data-stu-id="54bb3-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="54bb3-109">**Ezaugarrien zerrenda**, aurkitu eta gaitu ezaugarri hauek:</span><span class="sxs-lookup"><span data-stu-id="54bb3-109">In **Feature list**, find and enable the following features:</span></span>
  
    - <span data-ttu-id="54bb3-110">**Gaitu proiektu baterako hainbat kontratu lerro**</span><span class="sxs-lookup"><span data-stu-id="54bb3-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="54bb3-111">**Gaitu Project Operations Dynamics 365 Customer Engagement**</span><span class="sxs-lookup"><span data-stu-id="54bb3-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="54bb3-112">**Ezaugarri teklak** zerrendatuta ikusten ez baduzu, egiaztatu zure Finantza bertsioak gutxieneko bertsioaren baldintza betetzen duela (10.0.13 bertsioaren aplikazioa kalitate eguneratze guztiekin aplikatuta edo berriagoa).</span><span class="sxs-lookup"><span data-stu-id="54bb3-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="54bb3-113">Aukeratu **Egiaztatu eguneratzeak** funtzioen zerrenda freskatzeko.</span><span class="sxs-lookup"><span data-stu-id="54bb3-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="54bb3-114">Definitu Project Operations-ek hedatzeko agertokia pertsona juridiko baterako</span><span class="sxs-lookup"><span data-stu-id="54bb3-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="54bb3-115">Project Operations-en gaitu ditzakezu Dynamics 365 Customer Engagement entitate juridiko mailan.</span><span class="sxs-lookup"><span data-stu-id="54bb3-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="54bb3-116">Project Operations-eko Dynamics 365 Customer Engagement baliabideetan / stockean oinarritutako eszenatokietarako.</span><span class="sxs-lookup"><span data-stu-id="54bb3-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="54bb3-117">Ingurune berean, beste entitate juridiko bat izan dezakezu Proiektuaren eragiketak erabiliz, hornitutako / ekoizteko eskaeren agertokietarako.</span><span class="sxs-lookup"><span data-stu-id="54bb3-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="54bb3-118">Dynamics 365 Finance-n, joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa orokorra eta kontabilitate parametroak**.</span><span class="sxs-lookup"><span data-stu-id="54bb3-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="54bb3-119">Eskuragarri dauden pertsona juridikoen zerrendan, hautatu kontratu-lerro ugari eta proiektuaren eragiketak dauden entitateak Dynamics 365 Customer Engagement funtzioak gaituta egongo dira.</span><span class="sxs-lookup"><span data-stu-id="54bb3-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="54bb3-120">Utzi hautatutako proiektuen eragiketak erabiliko dituzten pertsona juridikoak biltegiratzeko / ekoizteko eskaera agertokietarako.</span><span class="sxs-lookup"><span data-stu-id="54bb3-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="54bb3-121">Pertsona juridikoa lehendik proiekturik ez badu soilik hauta daiteke.</span><span class="sxs-lookup"><span data-stu-id="54bb3-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="54bb3-122">Konfiguratu Proiektuaren kudeaketa eta kontabilitatearen parametroak</span><span class="sxs-lookup"><span data-stu-id="54bb3-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="54bb3-123">Proiektuaren eragiketak erabiltzen dituen pertsona juridiko bakoitza Dynamics 365 Customer Engagement parametro lehenetsien multzo bat behar du.</span><span class="sxs-lookup"><span data-stu-id="54bb3-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="54bb3-124">Parametro hauek **Proiektuaren eragiketak** fitxako **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean.</span><span class="sxs-lookup"><span data-stu-id="54bb3-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="54bb3-125">Parametroak dira:</span><span class="sxs-lookup"><span data-stu-id="54bb3-125">The parameters are:</span></span>

  - <span data-ttu-id="54bb3-126">**Fakturazio mota lehenetsiak**: Project Operations-ek fakturazio mota lehenetsien multzo finko bat erabiltzen du, Finantza lineako propietateekin mapatu behar dena.</span><span class="sxs-lookup"><span data-stu-id="54bb3-126">**Billing type defaults**: Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="54bb3-127">Sortu erregistro bat fakturazio mota bakoitzerako: **Zehaztu gabea**, **Kargagarria**, **Ez da ordaindu behar**, **Osagarria** eta **Ez dago erabilgarri**.</span><span class="sxs-lookup"><span data-stu-id="54bb3-127">Create a record for each billing type: **Not specified**, **Chargeable**, **Non-chargeable**, **Complimentary**, and **Not available**.</span></span>
  - <span data-ttu-id="54bb3-128">**Proiektuaren kategoria lehenetsiak**: Hautatu transakzio mota bakoitzerako erabiliko diren lehenetsitako proiektuen kategoriak.</span><span class="sxs-lookup"><span data-stu-id="54bb3-128">**Project category defaults**: Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="54bb3-129">Lehenetsi hauek fitxategian erabiliko dira **Project Operations Integration aldizkaria** eta proiektuaren benetako transakzio kategoriarik zehazten ez den estimazioetan.</span><span class="sxs-lookup"><span data-stu-id="54bb3-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="54bb3-130">**Iragarpenak**: Aukeratu iragarpen eredua denbora eta gastuen kalkuluak egiteko.</span><span class="sxs-lookup"><span data-stu-id="54bb3-130">**Forecasts**: Select the forecast model to be used for time and expense estimates.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]