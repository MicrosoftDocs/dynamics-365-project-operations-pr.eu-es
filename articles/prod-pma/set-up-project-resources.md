---
title: Konfiguratu proiektuan baliabideak
description: Gai honek proiektuko baliabideak konfiguratzeari edo eskatzeari buruzko informazioa ematen du.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0bf146c3bfb2fd558c471d8a9e980834cb1b87df
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288724"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="97866-103">Konfiguratu proiektuan baliabideak</span><span class="sxs-lookup"><span data-stu-id="97866-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="97866-104">Egutegia konfiguratu eta langile batekin edo langile batekin lotu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="97866-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="97866-105">Egutegia proiektua eta proiekturako gordetako baliabideen lanaldia antolatzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="97866-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="97866-106">Egutegia konfiguratzerakoan, proiektuen kudeatzaileek baliabideen berdinketa egin dezakete baliabideak optimizatzearen barruan.</span><span class="sxs-lookup"><span data-stu-id="97866-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="97866-107">Egutegiaren ordutegian oinarrituta, baliabideetan murrizketak jar daitezke.</span><span class="sxs-lookup"><span data-stu-id="97866-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="97866-108">Egutegia konfigura dezakezu **Egutegiak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="97866-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="97866-109">Langile bat proiektuaren baliabide gisa konfiguratzen duzunean, enpresan lan egiten duten langileen artean baliabideak konfiguratzen ari zarenetik hauta dezakezu.</span><span class="sxs-lookup"><span data-stu-id="97866-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="97866-110">Bestela, zure erakundeko beste enpresa batzuetako langileak hauta ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="97866-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="97866-111">Langile horiek enpresen arteko baliabideak bezala ezagutzen dira.</span><span class="sxs-lookup"><span data-stu-id="97866-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="97866-112">Ondorengo prozedurek langile bat zure enpresan proiektuaren baliabide gisa nola konfiguratu eta enpresen arteko proiektuaren baliabide bat nola konfiguratu azaltzen dute.</span><span class="sxs-lookup"><span data-stu-id="97866-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="97866-113">Konfiguratu langilea proiektuaren baliabide gisa</span><span class="sxs-lookup"><span data-stu-id="97866-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="97866-114">Gainean **Langileak** orrialdean, **Langileak** zerrenda, hautatu proiektuaren baliabide gisa gehitzen ari zaren langilea eta ireki langilearen erregistroa.</span><span class="sxs-lookup"><span data-stu-id="97866-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="97866-115">Ekintza panelean, hautatu **Proiektua** &gt; **Konfigurazioa** &gt; **Proiektuaren konfigurazioa**.</span><span class="sxs-lookup"><span data-stu-id="97866-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="97866-116">Aukeratu egutegi bat eta itxi orria.</span><span class="sxs-lookup"><span data-stu-id="97866-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="97866-117">Baliabide baterako proiektu lehenetsiak ere zehaztu ditzakezu aurrez esleitzeko mota gisa.</span><span class="sxs-lookup"><span data-stu-id="97866-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="97866-118">Aurrez esleipenak baliabideen kudeatzaileak edo proiektuaren kudeatzaileak baliabideak aldez aurretik zein proiektutan landuko dituen dakienean erabil daitezke.</span><span class="sxs-lookup"><span data-stu-id="97866-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="97866-119">Aurretiazko esleipenak proiektuaren babesle edo bezero baten eskaeran oinarrituta ere egin daitezke.</span><span class="sxs-lookup"><span data-stu-id="97866-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="97866-120">Proiektu bat aurrez esleitzeko, **Proiektuak esleitu** orrialdean, **Proiektuak** fitxan, **Gainerako proiektuak** zerrenda, hautatu proiektu egokia.</span><span class="sxs-lookup"><span data-stu-id="97866-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="97866-121">Konfiguratu enpresen arteko baliabide bat</span><span class="sxs-lookup"><span data-stu-id="97866-121">Set up an intercompany resource</span></span>

<span data-ttu-id="97866-122">Langilea enpresen arteko baliabide gisa konfiguratzen duzunean, konfigurazioa osatu behar duzu bai mailegu-enpresan bai mailegu-enpresan.</span><span class="sxs-lookup"><span data-stu-id="97866-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="97866-123">Mailegu-enpresan</span><span class="sxs-lookup"><span data-stu-id="97866-123">In the lending company</span></span>

1. <span data-ttu-id="97866-124">Finantzetan, egiaztatu enpresa mailegu-emailea hautatuta dagoela eta, ondoren, osatu aurreko ataleko prozedura, "Konfiguratu langilea proiektuaren baliabide gisa."</span><span class="sxs-lookup"><span data-stu-id="97866-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="97866-125">**Konpainia arteko kontua** orrian, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="97866-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="97866-126">**Pertsona juridikoaren IDa** eremuan, hautatu mailegu-enpresa.</span><span class="sxs-lookup"><span data-stu-id="97866-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="97866-127">Bete gainerako eremuak egoki gisa, eta gero hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="97866-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="97866-128">**Transferitzeko prezioa** orrian, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="97866-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="97866-129">**Hartu legezko entitatea** eremuan, hautatu konpainia egokia.</span><span class="sxs-lookup"><span data-stu-id="97866-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="97866-130">Mailegu-enpresari atal honen hasieran sortu zenituen baliabideak soilik emateko **Baliabidea** eremuan, hautatu sortu duzun baliabidearen izena.</span><span class="sxs-lookup"><span data-stu-id="97866-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="97866-131">Mailegu-enpresaren baliabide guztiak mailegu-enpresaren eskura jartzeko, utzi **Baliabidea** eremua hutsik.</span><span class="sxs-lookup"><span data-stu-id="97866-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="97866-132">Gainean **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, **Enpresa artekoa** fitxa, ezarri **Gaitu enpresen arteko baliabideen programazioa eta denbora-orriak** aukera **Bai**.</span><span class="sxs-lookup"><span data-stu-id="97866-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="97866-133">Hartutako konpainian</span><span class="sxs-lookup"><span data-stu-id="97866-133">In the borrowing company</span></span>

- <span data-ttu-id="97866-134">Gainean **Baliabideen zerrenda** orrian, bilaketa-iragazkian, idatzi mailegu-enpresarentzat sortu duzun baliabidearen izena, izena mailegu-enpresaren baliabideen zerrendan sartuta dagoela egiaztatzeko.</span><span class="sxs-lookup"><span data-stu-id="97866-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="97866-135">Proiektuaren baliabideen eskaera</span><span class="sxs-lookup"><span data-stu-id="97866-135">Request project resources</span></span>
<span data-ttu-id="97866-136">Proiektuaren baliabideen antolaketarako funtzionaltasunak baliabideen kudeatzaileek konpromiso edo proiektuetan pertsonaleko baliabideak banatu ditzaten soilik.</span><span class="sxs-lookup"><span data-stu-id="97866-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="97866-137">Funtzionalitate hau gaitzeko, burutu zeregin hauek edo egiaztatu egin direla:</span><span class="sxs-lookup"><span data-stu-id="97866-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="97866-138">Konfiguratu zenbaki sekuentziak.</span><span class="sxs-lookup"><span data-stu-id="97866-138">Set up number sequences.</span></span>
- <span data-ttu-id="97866-139">Konfiguratu proiektuen kudeaketa eta kontabilitate lan-fluxuak.</span><span class="sxs-lookup"><span data-stu-id="97866-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="97866-140">Gaitu baliabideen eskaera-fluxuak.</span><span class="sxs-lookup"><span data-stu-id="97866-140">Enable resource request workflows.</span></span>

<span data-ttu-id="97866-141">Aurreko zereginak amaitu ondoren, zeregin hauek bete ditzakezu nahi duzun moduan:</span><span class="sxs-lookup"><span data-stu-id="97866-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="97866-142">Sortu baliabide eskaera bat gordetako langileen baliabide batetik.</span><span class="sxs-lookup"><span data-stu-id="97866-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="97866-143">Monitorizatu baliabide-eskaerak.</span><span class="sxs-lookup"><span data-stu-id="97866-143">Monitor resource requests.</span></span>
- <span data-ttu-id="97866-144">Baliabide-eskaerak bete.</span><span class="sxs-lookup"><span data-stu-id="97866-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="97866-145">Eskatu baliabide pertsonal bat WBS bati.</span><span class="sxs-lookup"><span data-stu-id="97866-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="97866-146">Erreserbatu baliabideak proiektu batera, pertsonaleko baliabiderik eskatu gabe.</span><span class="sxs-lookup"><span data-stu-id="97866-146">Book resources to a project without having a request for a staffed resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]