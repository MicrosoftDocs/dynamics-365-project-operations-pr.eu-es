---
title: Konfiguratu eta aplikatu konfigurazio-datuak Common Data Service-n
description: Gai honek Project Operations-eko konfigurazio-datuak konfiguratzeari eta aplikatzeari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7de8db5e91265c77c79f34a513bf27d9a55b789a
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401113"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="0adaf-103">Konfiguratu eta aplikatu konfigurazio-datuak Common Data Service-n</span><span class="sxs-lookup"><span data-stu-id="0adaf-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="0adaf-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="0adaf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0adaf-105">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="0adaf-105">Prerequisites</span></span>

<span data-ttu-id="0adaf-106">Fitxategian datuak konfiguratzeko eskatu aurretik Common Data Service (CDS), honako baldintza hauek bete behar dira:</span><span class="sxs-lookup"><span data-stu-id="0adaf-106">Before you beging to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="0adaf-107">CDS ingurunea eta Dynamics 365 Finance Project Operations-etarako ingurunea.</span><span class="sxs-lookup"><span data-stu-id="0adaf-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="0adaf-108">Pertsona juridikoen informazioa Dynamics 365 Finance CDS ingurunearekin partekatzen da.</span><span class="sxs-lookup"><span data-stu-id="0adaf-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="0adaf-109">Horrek esan nahi du **Enpresa** CDS erakundeak konpainiaren erregistro hauek ditu:</span><span class="sxs-lookup"><span data-stu-id="0adaf-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="0adaf-110">THPM</span><span class="sxs-lookup"><span data-stu-id="0adaf-110">THPM</span></span>
  - <span data-ttu-id="0adaf-111">USPM</span><span class="sxs-lookup"><span data-stu-id="0adaf-111">USPM</span></span>
  - <span data-ttu-id="0adaf-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="0adaf-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="0adaf-113">Instalatu konfigurazioa eta konfigurazio-datuak</span><span class="sxs-lookup"><span data-stu-id="0adaf-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="0adaf-114">Deskargatu, desblokeatu eta deskonprimatu [Konfigurazio eta konfigurazio datu paketea](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="0adaf-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="0adaf-115">Joan deskonprimatutako karpetara eta exekutatu fitxategi exekutagarria, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="0adaf-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="0adaf-116">Common Data Service konfigurazio-migrazioaren (CMT) morroiko 1. orrian, hautatu **Inportatu datuak** eta, ondoren, hautatu **Jarraitu**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![Konfigurazioaren migrazioa](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="0adaf-118">CMT morroiaren 2. orrian, hautatu **Microsoft 365** **Inplementazio mota** gisa.</span><span class="sxs-lookup"><span data-stu-id="0adaf-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="0adaf-119">Aukeratu **Erakutsi eskuragarri dauden erakundeen zerrenda** eta **Erakutsi aurreratua** kontrol-laukiak.</span><span class="sxs-lookup"><span data-stu-id="0adaf-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="0adaf-120">Aukeratu zure maizterraren eskualdea, sartu zure kredentzialak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![Konfigurazioaren saio-hasiera](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="0adaf-122">3. orrialdean, maizterraren erakundeen zerrendan, hautatu zein erakundetan inportatu nahi dituzun demo datuak eta hautatu **Saioa hasi**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="0adaf-123">4. orrialdean, hautatu zip fitxategia, *SampelSetupAndConfigData*, paketatu gabeko karpetatik.</span><span class="sxs-lookup"><span data-stu-id="0adaf-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![Zip fitxategien hautaketa](./media/3ZipFile.png)

![Hautatu fitxategia.](./media/4SelectAFile.png)

9. <span data-ttu-id="0adaf-126">Zip fitxategia hautatu ondoren, hautatu **Inportatu datuak**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-126">After the zip file is selected, select **Import Data**.</span></span>

![Inportatu datuak](./media/5ImportData.png)

10. <span data-ttu-id="0adaf-128">Inportazioa gutxi gorabehera bi-hamar minutu iraungo du sareko abiaduraren arabera.</span><span class="sxs-lookup"><span data-stu-id="0adaf-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="0adaf-129">Inportatu ondoren, irten CMT morroitik.</span><span class="sxs-lookup"><span data-stu-id="0adaf-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="0adaf-130">Egiaztatu zure erakundeak 19 entitate hauetako datuak dituen:</span><span class="sxs-lookup"><span data-stu-id="0adaf-130">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="0adaf-131">Moneta</span><span class="sxs-lookup"><span data-stu-id="0adaf-131">Currency</span></span>
  - <span data-ttu-id="0adaf-132">Erakundearen unitatea</span><span class="sxs-lookup"><span data-stu-id="0adaf-132">Organizational Unit</span></span>
  - <span data-ttu-id="0adaf-133">Contact</span><span class="sxs-lookup"><span data-stu-id="0adaf-133">Contact</span></span>
  - <span data-ttu-id="0adaf-134">Zerga Taldea</span><span class="sxs-lookup"><span data-stu-id="0adaf-134">Tax Group</span></span>
  - <span data-ttu-id="0adaf-135">Bezero-taldea</span><span class="sxs-lookup"><span data-stu-id="0adaf-135">Customer Group</span></span>
  - <span data-ttu-id="0adaf-136">Unitatea</span><span class="sxs-lookup"><span data-stu-id="0adaf-136">Unit</span></span>
  - <span data-ttu-id="0adaf-137">Salmenta-unitatea</span><span class="sxs-lookup"><span data-stu-id="0adaf-137">Unit Group</span></span>
  - <span data-ttu-id="0adaf-138">Prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="0adaf-138">Price List</span></span>
  - <span data-ttu-id="0adaf-139">Proiektuaren parametroen prezio-zerrenda</span><span class="sxs-lookup"><span data-stu-id="0adaf-139">Project Parameter Price List</span></span>
  - <span data-ttu-id="0adaf-140">Fakturen maiztasuna</span><span class="sxs-lookup"><span data-stu-id="0adaf-140">Invoice Frequency</span></span>
  - <span data-ttu-id="0adaf-141">Baliabide erreserbagarriaren kategoria</span><span class="sxs-lookup"><span data-stu-id="0adaf-141">Bookable Resource Category</span></span>
  - <span data-ttu-id="0adaf-142">Transakzio-kategoria</span><span class="sxs-lookup"><span data-stu-id="0adaf-142">Transaction Category</span></span>
  - <span data-ttu-id="0adaf-143">Gastu-kategoria</span><span class="sxs-lookup"><span data-stu-id="0adaf-143">Expense Category</span></span>
  - <span data-ttu-id="0adaf-144">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="0adaf-144">Role Price</span></span>
  - <span data-ttu-id="0adaf-145">Transakzio-kategoriaren prezioa</span><span class="sxs-lookup"><span data-stu-id="0adaf-145">Transaction Category Price</span></span>
  - <span data-ttu-id="0adaf-146">Ezaugarria</span><span class="sxs-lookup"><span data-stu-id="0adaf-146">Characteristic</span></span>
  - <span data-ttu-id="0adaf-147">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="0adaf-147">Bookable Resource</span></span>
  - <span data-ttu-id="0adaf-148">Baliabide erreserbagarriaren kategoriaren erlazioa</span><span class="sxs-lookup"><span data-stu-id="0adaf-148">Bookable resource category Assn</span></span>
  - <span data-ttu-id="0adaf-149">Baliabide erreserbagarriaren ezaugarria</span><span class="sxs-lookup"><span data-stu-id="0adaf-149">Bookable Resource Characteristic</span></span>

![Inportazio osoa](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="0adaf-151">Eguneratu Project Operations-en konfigurazioak</span><span class="sxs-lookup"><span data-stu-id="0adaf-151">Update Project Operations configurations</span></span>

1. <span data-ttu-id="0adaf-152">Nabigatu CE ingurunera.</span><span class="sxs-lookup"><span data-stu-id="0adaf-152">Navigate to the CE environment.</span></span> <span data-ttu-id="0adaf-153">Fitxategia irekita aurki dezakezu [Power Platform Administrazio zentroa](https://admin.powerplatform.microsoft.com/environments), ingurunea hautatuz, eta ondoren hautatuz **Ingurune irekia**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-153">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![Ireki ingurunea](./media/7OpenEnvironment.png)

2. <span data-ttu-id="0adaf-155">Joan **Proiektuak** > **Baliabideak** aukerara eta, ondoren, hautatu **Berria** zure erabiltzailearentzako baliabide erreserbagarria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="0adaf-155">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![Baliabide erreserbagarriak](./media/8BookableResources.png)

3. <span data-ttu-id="0adaf-157">**Orokorra** fitxan, hautatu administratzailearen erabiltzailea.</span><span class="sxs-lookup"><span data-stu-id="0adaf-157">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="0adaf-158">Egiaztatu ordu-zona bat zarenarekin bat datorrela.</span><span class="sxs-lookup"><span data-stu-id="0adaf-158">Verify that the time zone matches the one you are in.</span></span> 

![Baliabide erreserbagarri berria](./media/9NewBookableResource.png)

4. <span data-ttu-id="0adaf-160">**Programazioa** fitxan, **Enpresa** eremuan, aukeratu **USPM** enpresa, eta gero hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-160">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![Antolaketa fitxa](./media/10SchedulingTab.png)

5. <span data-ttu-id="0adaf-162">Hautatu **Lanorduak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="0adaf-162">Select the **Work hours** tab.</span></span>  

![Lanorduak](./media/11WorkHours.png)

6. <span data-ttu-id="0adaf-164">Egin klik bikoitza egutegiko edozein balioetan eta hautatu **Editatu** > **Serieko gertaera guztiak**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-164">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![Lan-egutegia](./media/12WorkCalendar.png)

7. <span data-ttu-id="0adaf-166">Aldatu laneko orduak zortzi (8) orduko lanegunera, markatu asteburuak lanik gabeko egun gisa eta ziurtatu ordu-zona bat datorrenarekin.</span><span class="sxs-lookup"><span data-stu-id="0adaf-166">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="0adaf-167">Hautatu **Gorde eta itxi**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-167">Select **Save and close**.</span></span>

![Eguneratu egutegia](./media/13UpdateCalendar.png)

9. <span data-ttu-id="0adaf-169">Joan **Ezarpenak** > **Egutegiaren txantiloiak** eta hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-169">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![Egutegiaren txantiloiak](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="0adaf-171">Idatzi izen bat, hautatu sortu duzun txantiloiaren baliabidea eta hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-171">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![Gorde egutegiaren txantiloia](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="0adaf-173">Joan **Parametroak** eta egin klik bikoitza erregistroan.</span><span class="sxs-lookup"><span data-stu-id="0adaf-173">Go to **Parameters** and double-click the record.</span></span> 
 
 ![Proiektuaren parametroak](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="0adaf-175">Eguneratu eremu hauek:</span><span class="sxs-lookup"><span data-stu-id="0adaf-175">Update the following fields:</span></span>

 - <span data-ttu-id="0adaf-176">**Enpresa lehenetsia**: USPM</span><span class="sxs-lookup"><span data-stu-id="0adaf-176">**Default company**: USPM</span></span>
 - <span data-ttu-id="0adaf-177">**Antolakuntza Unitate Lehenetsia**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="0adaf-177">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="0adaf-178">**Fakturen maiztasuna**: Zazpigarren eta Azken eguna</span><span class="sxs-lookup"><span data-stu-id="0adaf-178">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="0adaf-179">**Lan orduko txantiloia**: Sortu duzun txantiloira aldatu.</span><span class="sxs-lookup"><span data-stu-id="0adaf-179">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="0adaf-180">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="0adaf-180">Select **Save**.</span></span> 

![Proiektuen parametro eguneratuak](./media/17UpdatedProjectParameters.png)
