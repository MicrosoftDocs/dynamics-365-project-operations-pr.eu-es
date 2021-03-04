---
title: Aplikatu demo-konfigurazioa eta konfigurazio-datuak - arina
description: Gai honek Project Operations-eko demo-konfigurazioa eta konfigurazio datuak nola aplikatu jakiteko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 762b0cf317d442565a033f56033a53a5b5cc435c
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089104"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="1d19f-103">Aplikatu Project Operations-erako demo-konfigurazioa eta konfigurazio-datuak - arina</span><span class="sxs-lookup"><span data-stu-id="1d19f-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="1d19f-104">_\*\*Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="1d19f-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="1d19f-105">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="1d19f-105">Prerequisites</span></span>

<span data-ttu-id="1d19f-106">Konfigurazioa hasi aurretik, hau eduki behar duzu Common Data Service (CDS) ingurunea Dynamics 365 Project Operations-etarako hornituta.</span><span class="sxs-lookup"><span data-stu-id="1d19f-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="1d19f-107">Instrukzioak</span><span class="sxs-lookup"><span data-stu-id="1d19f-107">Instructions</span></span>

1. <span data-ttu-id="1d19f-108">Deskargatu [Datu nagusien paketea](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="1d19f-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="1d19f-109">Joan *ProjOpsDemoDataSetupAndMaster - CMT integratua* karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="1d19f-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="1d19f-110">Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.</span><span class="sxs-lookup"><span data-stu-id="1d19f-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="1d19f-112">CMT morroiaren 2. orrian, hautatu **Microsoft 365** **Inplementazio mota** gisa.</span><span class="sxs-lookup"><span data-stu-id="1d19f-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="1d19f-113">Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.</span><span class="sxs-lookup"><span data-stu-id="1d19f-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="1d19f-114">Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="1d19f-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="1d19f-116">3. orrialdean, Maizterraren Erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="1d19f-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="1d19f-117">4. orrialdean, hautatu zip fitxategia, *MasterAndSetupData* paketatu gabeko karpetatik, *ProjOpsDemoDataSetupAndMaster - CMT integratua*.</span><span class="sxs-lookup"><span data-stu-id="1d19f-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

   ![Zip fitxategia](./media/3ZipFile.png)

   ![Hautatu fitxategia.](./media/4SelectAFile.png)

9. <span data-ttu-id="1d19f-120">Zip fitxategia hautatu ondoren, hautatu **Inportatu datuak**.</span><span class="sxs-lookup"><span data-stu-id="1d19f-120">After the zip file is selected, select **Import Data**.</span></span>

   ![Inportatu datuak](./media/5ImportData.png)

10. <span data-ttu-id="1d19f-122">Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera.</span><span class="sxs-lookup"><span data-stu-id="1d19f-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="1d19f-123">Bukatu ondoren, irten CMT morroitik.</span><span class="sxs-lookup"><span data-stu-id="1d19f-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="1d19f-124">Egiaztatu zure erakundeak 20 entitate hauetako datuak dituen:</span><span class="sxs-lookup"><span data-stu-id="1d19f-124">Check your organization for data in the following 20 entities:</span></span>

    -   <span data-ttu-id="1d19f-125">Moneta</span><span class="sxs-lookup"><span data-stu-id="1d19f-125">Currency</span></span>
    -   <span data-ttu-id="1d19f-126">Account</span><span class="sxs-lookup"><span data-stu-id="1d19f-126">Account</span></span>
    -   <span data-ttu-id="1d19f-127">Erakundearen unitatea</span><span class="sxs-lookup"><span data-stu-id="1d19f-127">Organizational Unit</span></span>
    -   <span data-ttu-id="1d19f-128">Contact</span><span class="sxs-lookup"><span data-stu-id="1d19f-128">Contact</span></span>
    -   <span data-ttu-id="1d19f-129">Unitatea</span><span class="sxs-lookup"><span data-stu-id="1d19f-129">Unit</span></span>
    -   <span data-ttu-id="1d19f-130">Salmenta-unitatea</span><span class="sxs-lookup"><span data-stu-id="1d19f-130">Unit Group</span></span>
    -   <span data-ttu-id="1d19f-131">Prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="1d19f-131">Price List</span></span>
    -   <span data-ttu-id="1d19f-132">Proiektuaren parametroen prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="1d19f-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="1d19f-133">Fakturen maiztasuna</span><span class="sxs-lookup"><span data-stu-id="1d19f-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="1d19f-134">Baliabide erreserbagarriaren kategoria</span><span class="sxs-lookup"><span data-stu-id="1d19f-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="1d19f-135">Transakzio-kategoria</span><span class="sxs-lookup"><span data-stu-id="1d19f-135">Transaction Category</span></span>
    -   <span data-ttu-id="1d19f-136">Gastu-kategoria</span><span class="sxs-lookup"><span data-stu-id="1d19f-136">Expense Category</span></span>
    -   <span data-ttu-id="1d19f-137">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="1d19f-137">Role Price</span></span>
    -   <span data-ttu-id="1d19f-138">Transakzio-kategoriaren prezioa</span><span class="sxs-lookup"><span data-stu-id="1d19f-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="1d19f-139">Ezaugarria</span><span class="sxs-lookup"><span data-stu-id="1d19f-139">Characteristic</span></span>
    -   <span data-ttu-id="1d19f-140">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="1d19f-140">Bookable Resource</span></span>
    -   <span data-ttu-id="1d19f-141">Baliabide erreserbagarriaren kategoriaren erlazioa</span><span class="sxs-lookup"><span data-stu-id="1d19f-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="1d19f-142">Baliabide erreserbagarriaren ezaugarria</span><span class="sxs-lookup"><span data-stu-id="1d19f-142">Bookable Resource Characteristic</span></span>

    ![Inportazio osoa](./media/6CompleteImport.png)
