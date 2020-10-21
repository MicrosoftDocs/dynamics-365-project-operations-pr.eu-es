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
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948727"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="c0575-103">Aplikatu demo konfigurazio eta konfigurazio datuak Project Operations lite inplementazioan - aurre proforma fakturazioari</span><span class="sxs-lookup"><span data-stu-id="c0575-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="c0575-104">_\*\*Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="c0575-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="c0575-105">Deskargatu [Datu nagusien paketea](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="c0575-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="c0575-106">Joan *ProjOpsDemoDataSetupAndMaster - CMT integratua* karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="c0575-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="c0575-107">Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.</span><span class="sxs-lookup"><span data-stu-id="c0575-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="c0575-109">CMT morroiaren 2. orrian, hautatu **Office 365** **Inplementazio mota** gisa.</span><span class="sxs-lookup"><span data-stu-id="c0575-109">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="c0575-110">Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.</span><span class="sxs-lookup"><span data-stu-id="c0575-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="c0575-111">Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="c0575-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="c0575-113">3. orrialdean, Maizterraren Erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="c0575-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="c0575-114">4. orrialdean, hautatu zip fitxategia, *MasterAndSetupData* paketatu gabeko karpetatik, *ProjOpsDemoDataSetupAndMaster - CMT integratua*.</span><span class="sxs-lookup"><span data-stu-id="c0575-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![Zip fitxategia](./media/3ZipFile.png)

![Hautatu fitxategia.](./media/4SelectAFile.png)

9. <span data-ttu-id="c0575-117">Zip fitxategia hautatu ondoren, hautatu**Inportatu datuak**.</span><span class="sxs-lookup"><span data-stu-id="c0575-117">After the zip file is selected, select **Import Data**.</span></span>

![Inportatu datuak](./media/5ImportData.png)

10. <span data-ttu-id="c0575-119">Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera.</span><span class="sxs-lookup"><span data-stu-id="c0575-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="c0575-120">Bukatu ondoren, irten CMT morroitik.</span><span class="sxs-lookup"><span data-stu-id="c0575-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="c0575-121">Egiaztatu zure erakundeak 20 entitate hauetako datuak dituen:</span><span class="sxs-lookup"><span data-stu-id="c0575-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="c0575-122">Moneta</span><span class="sxs-lookup"><span data-stu-id="c0575-122">Currency</span></span>
- <span data-ttu-id="c0575-123">Erakundearen unitatea</span><span class="sxs-lookup"><span data-stu-id="c0575-123">Organizational Unit</span></span>
- <span data-ttu-id="c0575-124">Contact</span><span class="sxs-lookup"><span data-stu-id="c0575-124">Contact</span></span>
- <span data-ttu-id="c0575-125">Zerga Taldea</span><span class="sxs-lookup"><span data-stu-id="c0575-125">Tax Group</span></span>
- <span data-ttu-id="c0575-126">Bezero-taldea</span><span class="sxs-lookup"><span data-stu-id="c0575-126">Customer Group</span></span>
- <span data-ttu-id="c0575-127">Unitatea</span><span class="sxs-lookup"><span data-stu-id="c0575-127">Unit</span></span>
- <span data-ttu-id="c0575-128">Salmenta-unitatea</span><span class="sxs-lookup"><span data-stu-id="c0575-128">Unit Group</span></span>
- <span data-ttu-id="c0575-129">Prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="c0575-129">Price List</span></span>
- <span data-ttu-id="c0575-130">Proiektuaren parametroen prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="c0575-130">Project Parameter Price List</span></span>
- <span data-ttu-id="c0575-131">Fakturen maiztasuna</span><span class="sxs-lookup"><span data-stu-id="c0575-131">Invoice Frequency</span></span>
- <span data-ttu-id="c0575-132">Fakturen maiztasunaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="c0575-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="c0575-133">Baliabide erreserbagarriaren kategoria</span><span class="sxs-lookup"><span data-stu-id="c0575-133">Bookable Resource Category</span></span>
- <span data-ttu-id="c0575-134">Transakzio-kategoria</span><span class="sxs-lookup"><span data-stu-id="c0575-134">Transaction Category</span></span>
- <span data-ttu-id="c0575-135">Gastu-kategoria</span><span class="sxs-lookup"><span data-stu-id="c0575-135">Expense Category</span></span>
- <span data-ttu-id="c0575-136">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="c0575-136">Role Price</span></span>
- <span data-ttu-id="c0575-137">Transakzio-kategoriaren prezioa</span><span class="sxs-lookup"><span data-stu-id="c0575-137">Transaction Category Price</span></span>
- <span data-ttu-id="c0575-138">Ezaugarria</span><span class="sxs-lookup"><span data-stu-id="c0575-138">Characteristic</span></span>
- <span data-ttu-id="c0575-139">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="c0575-139">Bookable Resource</span></span>
- <span data-ttu-id="c0575-140">Baliabide erreserbagarriaren kategoriaren erlazioa</span><span class="sxs-lookup"><span data-stu-id="c0575-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="c0575-141">Baliabide erreserbagarriaren ezaugarria</span><span class="sxs-lookup"><span data-stu-id="c0575-141">Bookable Resource Characteristic</span></span>

![Inportazio osoa](./media/6CompleteImport.png)
