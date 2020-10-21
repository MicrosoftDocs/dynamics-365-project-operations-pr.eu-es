---
title: Konfiguratu eta aplikatu konfigurazio-datuak Project Operations-en Common Data Service-n
description: Gai honek Project Operations-eko konfigurazio-datuak konfiguratzeari eta aplikatzeari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d99ab4c7b2ebf6ba56b86a3e0151036c6247e484
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948730"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="5c915-103">Konfiguratu eta aplikatu konfigurazio-datuak Project Operations-en Common Data Service-n</span><span class="sxs-lookup"><span data-stu-id="5c915-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="5c915-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="5c915-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="5c915-105">Instalatu konfigurazioa eta konfigurazio-datuak</span><span class="sxs-lookup"><span data-stu-id="5c915-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="5c915-106">Deskargatu, desblokeatu eta deskonprimatu [Konfigurazio eta konfigurazio datu paketea](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="5c915-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="5c915-107">Joan deskonprimatutako karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="5c915-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="5c915-108">Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.</span><span class="sxs-lookup"><span data-stu-id="5c915-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="5c915-110">CMT morroiaren 2. orrian, hautatu **Office 365** **Inplementazio mota** gisa.</span><span class="sxs-lookup"><span data-stu-id="5c915-110">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="5c915-111">Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.</span><span class="sxs-lookup"><span data-stu-id="5c915-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="5c915-112">Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="5c915-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="5c915-114">3. orrialdean, maizterraren erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="5c915-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="5c915-115">4. orrialdean, hautatu zip fitxategia, *SampelSetupAndConfigData*, paketatu gabeko karpetatik.</span><span class="sxs-lookup"><span data-stu-id="5c915-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Zip fitxategien hautaketa](./media/3ZipFile.png)

![Hautatu fitxategia.](./media/4SelectAFile.png)

9. <span data-ttu-id="5c915-118">Zip fitxategia hautatu ondoren, hautatu**Inportatu datuak**.</span><span class="sxs-lookup"><span data-stu-id="5c915-118">After the zip file is selected, select **Import Data**.</span></span>

![Inportatu datuak](./media/5ImportData.png)

10. <span data-ttu-id="5c915-120">Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera.</span><span class="sxs-lookup"><span data-stu-id="5c915-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="5c915-121">Inportatu ondoren, irten CMT morroitik.</span><span class="sxs-lookup"><span data-stu-id="5c915-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="5c915-122">Egiaztatu zure erakundeak 19 entitate hauetako datuak dituen:</span><span class="sxs-lookup"><span data-stu-id="5c915-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="5c915-123">Moneta</span><span class="sxs-lookup"><span data-stu-id="5c915-123">Currency</span></span>
  - <span data-ttu-id="5c915-124">Erakundearen unitatea</span><span class="sxs-lookup"><span data-stu-id="5c915-124">Organizational Unit</span></span>
  - <span data-ttu-id="5c915-125">Contact</span><span class="sxs-lookup"><span data-stu-id="5c915-125">Contact</span></span>
  - <span data-ttu-id="5c915-126">Zerga Taldea</span><span class="sxs-lookup"><span data-stu-id="5c915-126">Tax Group</span></span>
  - <span data-ttu-id="5c915-127">Bezero-taldea</span><span class="sxs-lookup"><span data-stu-id="5c915-127">Customer Group</span></span>
  - <span data-ttu-id="5c915-128">Unitatea</span><span class="sxs-lookup"><span data-stu-id="5c915-128">Unit</span></span>
  - <span data-ttu-id="5c915-129">Salmenta-unitatea</span><span class="sxs-lookup"><span data-stu-id="5c915-129">Unit Group</span></span>
  - <span data-ttu-id="5c915-130">Prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="5c915-130">Price List</span></span>
  - <span data-ttu-id="5c915-131">Proiektuaren parametroen prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="5c915-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="5c915-132">Fakturen maiztasuna</span><span class="sxs-lookup"><span data-stu-id="5c915-132">Invoice Frequency</span></span>
  - <span data-ttu-id="5c915-133">Baliabide erreserbagarriaren kategoria</span><span class="sxs-lookup"><span data-stu-id="5c915-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="5c915-134">Transakzio-kategoria</span><span class="sxs-lookup"><span data-stu-id="5c915-134">Transaction Category</span></span>
  - <span data-ttu-id="5c915-135">Gastu-kategoria</span><span class="sxs-lookup"><span data-stu-id="5c915-135">Expense Category</span></span>
  - <span data-ttu-id="5c915-136">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="5c915-136">Role Price</span></span>
  - <span data-ttu-id="5c915-137">Transakzio-kategoriaren prezioa</span><span class="sxs-lookup"><span data-stu-id="5c915-137">Transaction Category Price</span></span>
  - <span data-ttu-id="5c915-138">Ezaugarria</span><span class="sxs-lookup"><span data-stu-id="5c915-138">Characteristic</span></span>
  - <span data-ttu-id="5c915-139">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="5c915-139">Bookable Resource</span></span>
  - <span data-ttu-id="5c915-140">Baliabide erreserbagarriaren kategoriaren erlazioa</span><span class="sxs-lookup"><span data-stu-id="5c915-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="5c915-141">Baliabide erreserbagarriaren ezaugarria</span><span class="sxs-lookup"><span data-stu-id="5c915-141">Bookable Resource Characteristic</span></span>

![Inportazio osoa](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="5c915-143">Eguneratu Project Operations-en konfigurazioak</span><span class="sxs-lookup"><span data-stu-id="5c915-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="5c915-144">Nabigatu CE ingurunera.</span><span class="sxs-lookup"><span data-stu-id="5c915-144">Navigate to the CE environment.</span></span> <span data-ttu-id="5c915-145">Fitxategia irekita aurki dezakezu [Power Platform Administrazio zentroa](https://admin.powerplatform.microsoft.com/environments), ingurunea hautatuz, eta ondoren hautatuz **Ingurune irekia**.</span><span class="sxs-lookup"><span data-stu-id="5c915-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Ireki ingurunea](./media/7OpenEnvironment.png)

2. <span data-ttu-id="5c915-147">Joan **Proiektuak** > **Baliabideak** aukerara eta, ondoren, hautatu **Berria** zure erabiltzailearentzako baliabide erreserbagarria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="5c915-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Baliabide erreserbagarriak](./media/8BookableResources.png)

3. <span data-ttu-id="5c915-149">**Orokorra** fitxan, hautatu administratzailearen erabiltzailea.</span><span class="sxs-lookup"><span data-stu-id="5c915-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="5c915-150">Egiaztatu ordu-zona bat zarenarekin bat datorrela.</span><span class="sxs-lookup"><span data-stu-id="5c915-150">Verify that the time zone matches the one you are in.</span></span> 

![Baliabide erreserbagarri berria](./media/9NewBookableResource.png)

4. <span data-ttu-id="5c915-152">**Programazioa** fitxan, **Enpresa** eremuan, aukeratu **USPM** enpresa, eta gero hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="5c915-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Antolaketa fitxa](./media/10SchedulingTab.png)

5. <span data-ttu-id="5c915-154">Hautatu **Lanorduak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="5c915-154">Select the **Work hours** tab.</span></span>  

![Lanorduak](./media/11WorkHours.png)

6. <span data-ttu-id="5c915-156">Egin klik bikoitza egutegiko edozein balioetan eta hautatu **Editatu** > **Serieko gertaera guztiak**.</span><span class="sxs-lookup"><span data-stu-id="5c915-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Lan-egutegia](./media/12WorkCalendar.png)

7. <span data-ttu-id="5c915-158">Aldatu laneko orduak zortzi (8) orduko lanegunera, markatu asteburuak lanik gabeko egun gisa eta ziurtatu ordu-zona bat datorrenarekin.</span><span class="sxs-lookup"><span data-stu-id="5c915-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="5c915-159">Hautatu **Gorde eta itxi**.</span><span class="sxs-lookup"><span data-stu-id="5c915-159">Select **Save and close**.</span></span>

![Eguneratu egutegia](./media/13UpdateCalendar.png)

9. <span data-ttu-id="5c915-161">Joan **Ezarpenak** > **Egutegiaren txantiloiak** eta hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="5c915-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Egutegiaren txantiloiak](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="5c915-163">Idatzi izen bat, hautatu sortu duzun txantiloiaren baliabidea eta hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="5c915-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Gorde egutegiaren txantiloia](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="5c915-165">Joan **Parametroak** eta egin klik bikoitza erregistroan.</span><span class="sxs-lookup"><span data-stu-id="5c915-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Proiektuaren parametroak](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="5c915-167">Eguneratu eremu hauek:</span><span class="sxs-lookup"><span data-stu-id="5c915-167">Update the following fields:</span></span>

 - <span data-ttu-id="5c915-168">**Enpresa lehenetsia**: USPM</span><span class="sxs-lookup"><span data-stu-id="5c915-168">**Default company**: USPM</span></span>
 - <span data-ttu-id="5c915-169">**Antolakuntza Unitate Lehenetsia**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="5c915-169">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="5c915-170">**Fakturen maiztasuna**: Zazpigarren eta Azken eguna</span><span class="sxs-lookup"><span data-stu-id="5c915-170">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="5c915-171">**Lan orduko txantiloia**: Sortu duzun txantiloira aldatu.</span><span class="sxs-lookup"><span data-stu-id="5c915-171">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="5c915-172">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="5c915-172">Select **Save**.</span></span> 

![Proiektuen parametro eguneratuak](./media/17UpdatedProjectParameters.png)
