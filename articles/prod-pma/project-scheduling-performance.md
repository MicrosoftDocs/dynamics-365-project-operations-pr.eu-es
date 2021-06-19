---
title: Proiektuko baliabideen antolaketa-errendimendua
description: Gai honetan proiektu ugarientzako baliabideen programazioaren errendimendua hobetzeko moduari buruzko informazioa ematen da.
author: Yowelle
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 113023909f88cb4dd498190ef21b6955482b25dd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010006"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="69d1d-103">Proiektuko baliabideen antolaketa-errendimendua</span><span class="sxs-lookup"><span data-stu-id="69d1d-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="69d1d-104">Baliabideen antolaketarekin lotutako errendimendu arazoak gerta daitezke proiektu kopurua milaka izatera iristen denean.</span><span class="sxs-lookup"><span data-stu-id="69d1d-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="69d1d-105">Baliabideen antolaketa errendimendua hobetzeko, erabiltzaileek baliabideen erabilgarritasun inprimakia abiarazteko behar duten denbora murriztu dezaketen funtzioa dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="69d1d-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="69d1d-106">Zehazki, honek baliabideen gaitasuna biltzeko sinkronizazio prozesua kentzen du eta **ResProjectResource** taula baliabideen bilaketa azkartzeko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="69d1d-107">Kontuan izan **ResRollup** mahaia ez da gehiago erabiliko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="69d1d-108">Baliabideen gaitasuna biltzeko sinkronizazio prozesuaren edo **ResProjectResource** taula, ez erabili funtzio hau.</span><span class="sxs-lookup"><span data-stu-id="69d1d-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="69d1d-109">Gaitu baliabideak antolatzeko errendimendua hobetzea</span><span class="sxs-lookup"><span data-stu-id="69d1d-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="69d1d-110">Baliabideen programazioaren errendimendua hobetzeko gaitu, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="69d1d-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="69d1d-111">Joan **Ezaugarrien kudeaketa** > **Guztiak**, eta eginbideen zerrendan, bilatu **Gaitu proiektuaren baliabideen antolaketa errendimendua hobetzeko eginbidea**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-111">Go to **Feature management** > **All**, and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="69d1d-112">Hautatu **Gaitu orain**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="69d1d-113">Eginbidea zerrendan aurkitzen ez baduzu, hautatu **Egiaztatu eguneratzeak** zerrenda freskatzeko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="69d1d-114">Freskatu arakatzailea eta joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Proiektuaren baliabideak** > **Sinkronizatu baliabideen egutegien gaitasuna enpresa guztietan**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="69d1d-115">Ezarri **Kendu dauden gaitasun erregistroak** **Bai** aurreko datuak kentzeko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="69d1d-116">Datu inkrementalak sortu nahi badituzu, ezarri **Ez**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="69d1d-117">**Garai-kodea** eremuan, hautatu datuak zein alditan sortu behar diren.</span><span class="sxs-lookup"><span data-stu-id="69d1d-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="69d1d-118">Garai kode bat hautatzen baduzu, ez da hasiera eta amaiera data zehaztu behar.</span><span class="sxs-lookup"><span data-stu-id="69d1d-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="69d1d-119">**Garai kodea** eremua hutsik uzten baduzu, hautatu hasiera eta amaiera data zehatzak datuak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="69d1d-120">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="69d1d-121">Honek datu orokorrak banatuko ditu **ResCalendarCapacity** zure inguruneko enpresa guztien artean egin ezazu, beraz, sorta lana pertsona juridiko bakarrean exekutatu behar da.</span><span class="sxs-lookup"><span data-stu-id="69d1d-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="69d1d-122">Loteko lan honetako datuak beharrezkoak dira baliabideen ahalmena lotutako egutegiaren bidez kalkulatzeko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="69d1d-123">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Proiektuaren baliabideak** > **Bideratu proiektuaren baliabideak enpresa guztietan** eta, ondoren, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="69d1d-124">Hau da datuen bertsio berriaren gidoia **ResProjectResource**, **ResCalendarDateTimeRange** eta **ResEffectiveDateTimeRange** mahaiak.</span><span class="sxs-lookup"><span data-stu-id="69d1d-124">This is the data upgrade script for general data in the **ResProjectResource**, **ResCalendarDateTimeRange**, and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="69d1d-125">**PSAPRojSchedRole.RootActivity** eremuko balioak ere eguneratu dira.</span><span class="sxs-lookup"><span data-stu-id="69d1d-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="69d1d-126">Hau exekutatzen ez bada, abisu bat jasoko duzu baliabideak antolatzeko eragiketak egiten saiatzean.</span><span class="sxs-lookup"><span data-stu-id="69d1d-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="69d1d-127">Desaktibatu baliabideak antolatzeko errendimendua hobetzea</span><span class="sxs-lookup"><span data-stu-id="69d1d-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="69d1d-128">Joan **Ezaugarrien kudeaketa** > **Guztiak** eta bilatu **Gaitu proiektuaren baliabideen antolaketa errendimendua hobetzeko eginbidea**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="69d1d-129">Aukeratu funtzioa eta, ondoren, hautatu **Desgaitu** botoia.</span><span class="sxs-lookup"><span data-stu-id="69d1d-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="69d1d-130">Freskatu arakatzailea.</span><span class="sxs-lookup"><span data-stu-id="69d1d-130">Refresh your browser.</span></span>
4. <span data-ttu-id="69d1d-131">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Edukiera sinkronizatzea** > **Sinkronizatu baliabideen ahalmenak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="69d1d-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="69d1d-132">**Edukiera biltzeko sinkronizazioa** orrialdean, ezarri **Kendu dauden gaitasun erregistroak** **Bai** aurreko datuak kentzeko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="69d1d-133">Datu inkrementalak sortu nahi badituzu, ezarri **Ez**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="69d1d-134">**Garai-kodea** eremuan, hautatu datuak zein alditan sortu behar diren.</span><span class="sxs-lookup"><span data-stu-id="69d1d-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="69d1d-135">Garai kode bat hautatzen baduzu, ez da hasiera eta amaiera data zehaztu behar.</span><span class="sxs-lookup"><span data-stu-id="69d1d-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="69d1d-136">**Garai kodea** eremua hutsik uzten baduzu, hautatu hasiera eta amaiera data zehatzak datuak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="69d1d-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="69d1d-137">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="69d1d-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="69d1d-138">Honek datu orokorrak banatuko ditu **ResRollup** zure inguruneko enpresa guztien artean egin ezazu, beraz, sorta lana pertsona juridiko bakarrean exekutatu behar da.</span><span class="sxs-lookup"><span data-stu-id="69d1d-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="69d1d-139">Batch lan hau beharrezkoa da guztientzat **Baliabideen erabilgarritasuna** ikuspegiak.</span><span class="sxs-lookup"><span data-stu-id="69d1d-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="69d1d-140">Batch lan hau exekutatzen ez bada, **ResRollup** datuak hegan sortuko dira eta horrek denbora behar dezake.</span><span class="sxs-lookup"><span data-stu-id="69d1d-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]