---
title: Aplikatu demo-konfigurazioa eta konfigurazio-datuak
description: Gai honek Project Operations-eko demo-konfigurazioa eta konfigurazio datuak nola aplikatu jakiteko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 33b85115963f3561718b8951e5b518fd34de7723
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070901"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="f8c81-103">Aplikatu demo konfigurazio eta konfigurazio datuak Project Operations lite inplementazioan - aurre proforma fakturazioari</span><span class="sxs-lookup"><span data-stu-id="f8c81-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="f8c81-104">_\*\*Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="f8c81-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="f8c81-105">Deskargatu [Datu nagusien paketea](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="f8c81-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="f8c81-106">Joan *ProjOpsDemoDataSetupAndMaster - CMT integratua* karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="f8c81-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="f8c81-107">Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.</span><span class="sxs-lookup"><span data-stu-id="f8c81-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="f8c81-109">CMT morroiaren 2. orrian, hautatu **Microsoft 365** **Inplementazio mota** gisa.</span><span class="sxs-lookup"><span data-stu-id="f8c81-109">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="f8c81-110">Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.</span><span class="sxs-lookup"><span data-stu-id="f8c81-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="f8c81-111">Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="f8c81-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="f8c81-113">3. orrialdean, Maizterraren Erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="f8c81-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="f8c81-114">4. orrialdean, hautatu zip fitxategia, *MasterAndSetupData* paketatu gabeko karpetatik, *ProjOpsDemoDataSetupAndMaster - CMT integratua*.</span><span class="sxs-lookup"><span data-stu-id="f8c81-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Zip fitxategia](./media/3ZipFile.png)

![Hautatu fitxategia.](./media/4SelectAFile.png)

9. <span data-ttu-id="f8c81-117">Zip fitxategia hautatu ondoren, hautatu **Inportatu datuak**.</span><span class="sxs-lookup"><span data-stu-id="f8c81-117">After the zip file is selected, select **Import Data**.</span></span>

![Inportatu datuak](./media/5ImportData.png)

10. <span data-ttu-id="f8c81-119">Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera.</span><span class="sxs-lookup"><span data-stu-id="f8c81-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="f8c81-120">Bukatu ondoren, irten CMT morroitik.</span><span class="sxs-lookup"><span data-stu-id="f8c81-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="f8c81-121">Egiaztatu zure erakundeak 20 entitate hauetako datuak dituen:</span><span class="sxs-lookup"><span data-stu-id="f8c81-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="f8c81-122">Moneta</span><span class="sxs-lookup"><span data-stu-id="f8c81-122">Currency</span></span>
- <span data-ttu-id="f8c81-123">Erakundearen unitatea</span><span class="sxs-lookup"><span data-stu-id="f8c81-123">Organizational Unit</span></span>
- <span data-ttu-id="f8c81-124">Contact</span><span class="sxs-lookup"><span data-stu-id="f8c81-124">Contact</span></span>
- <span data-ttu-id="f8c81-125">Zerga Taldea</span><span class="sxs-lookup"><span data-stu-id="f8c81-125">Tax Group</span></span>
- <span data-ttu-id="f8c81-126">Bezero-taldea</span><span class="sxs-lookup"><span data-stu-id="f8c81-126">Customer Group</span></span>
- <span data-ttu-id="f8c81-127">Unitatea</span><span class="sxs-lookup"><span data-stu-id="f8c81-127">Unit</span></span>
- <span data-ttu-id="f8c81-128">Salmenta-unitatea</span><span class="sxs-lookup"><span data-stu-id="f8c81-128">Unit Group</span></span>
- <span data-ttu-id="f8c81-129">Prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="f8c81-129">Price List</span></span>
- <span data-ttu-id="f8c81-130">Proiektuaren parametroen prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="f8c81-130">Project Parameter Price List</span></span>
- <span data-ttu-id="f8c81-131">Fakturen maiztasuna</span><span class="sxs-lookup"><span data-stu-id="f8c81-131">Invoice Frequency</span></span>
- <span data-ttu-id="f8c81-132">Fakturen maiztasunaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="f8c81-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="f8c81-133">Baliabide erreserbagarriaren kategoria</span><span class="sxs-lookup"><span data-stu-id="f8c81-133">Bookable Resource Category</span></span>
- <span data-ttu-id="f8c81-134">Transakzio-kategoria</span><span class="sxs-lookup"><span data-stu-id="f8c81-134">Transaction Category</span></span>
- <span data-ttu-id="f8c81-135">Gastu-kategoria</span><span class="sxs-lookup"><span data-stu-id="f8c81-135">Expense Category</span></span>
- <span data-ttu-id="f8c81-136">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="f8c81-136">Role Price</span></span>
- <span data-ttu-id="f8c81-137">Transakzio-kategoriaren prezioa</span><span class="sxs-lookup"><span data-stu-id="f8c81-137">Transaction Category Price</span></span>
- <span data-ttu-id="f8c81-138">Ezaugarria</span><span class="sxs-lookup"><span data-stu-id="f8c81-138">Characteristic</span></span>
- <span data-ttu-id="f8c81-139">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="f8c81-139">Bookable Resource</span></span>
- <span data-ttu-id="f8c81-140">Baliabide erreserbagarriaren kategoriaren erlazioa</span><span class="sxs-lookup"><span data-stu-id="f8c81-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="f8c81-141">Baliabide erreserbagarriaren ezaugarria</span><span class="sxs-lookup"><span data-stu-id="f8c81-141">Bookable Resource Characteristic</span></span>

![Inportazio osoa](./media/6CompleteImport.png)
