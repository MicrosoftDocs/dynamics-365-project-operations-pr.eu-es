---
title: Aplikatu Project Operations demo-datuak Finance-ren hodeian ostatatutako ingurune batean
description: Gai honek Project Operations-etik demo datuak nola aplikatu azaltzen du Dynamics 365 Finance hodeian ostatatutako ingurunea.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 1a94862d5a024eb1630f33c0c96699e8b4b49bf2
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948735"
---
# <a name="apply-project-operations-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="6b700-103">Aplikatu Project Operations demo-datuak Finance-ren hodeian ostatatutako ingurune batean</span><span class="sxs-lookup"><span data-stu-id="6b700-103">Apply Project Operations demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="6b700-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="6b700-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

><span data-ttu-id="6b700-105">[Garrantzitsua] Gai hau Microsoft Dynamics 365 Finance 10.0.13 bertsioan soilik aplikatzen da eta hodeian ostatatutako ingurune batean bakarrik egin daiteke.</span><span class="sxs-lookup"><span data-stu-id="6b700-105">[Important] This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="6b700-106">Osatu gai honetako urratsak **AURRETIK** ingurumenari kalitatezko eguneratzeak aplikatzen dizkiozu.</span><span class="sxs-lookup"><span data-stu-id="6b700-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="6b700-107">Zure LCS proiektuan, ireki **Ingurumenaren xehetasunak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="6b700-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="6b700-108">Ohar zaitez urruneko mahaigaineko protokoloa (RDP) erabiliz ingurunearekin konektatzeko behar diren xehetasunak biltzen dituela.</span><span class="sxs-lookup"><span data-stu-id="6b700-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![ Ingurune-xehetasunak](./media/1EnvironmentDetails.png)

<span data-ttu-id="6b700-110">Nabarmendutako kredentzialen lehen multzoa tokiko kontuaren egiaztagiriak dira eta urruneko mahaigaineko konexiorako hiperesteka bat dute.</span><span class="sxs-lookup"><span data-stu-id="6b700-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="6b700-111">Kredentzialen artean, inguruneko administratzaile izena eta pasahitza daude.</span><span class="sxs-lookup"><span data-stu-id="6b700-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="6b700-112">Ingurune honetan SQL Server zerbitzuan saioa hasteko bigarren kredentzial multzoa erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="6b700-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="6b700-113">Konektatu ingurunearekin hiperesteka bidez **Tokiko kontuak**, eta erabili **Tokiko kontuaren egiaztagiriak** autentifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="6b700-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="6b700-114">Joan **Interneteko Informazio Zerbitzuak** > **Aplikazio multzoak** > **AOSZerbitzua** eta zerbitzua gelditu.</span><span class="sxs-lookup"><span data-stu-id="6b700-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="6b700-115">Une honetan zerbitzua gelditzen ari zara, SQL datu basea ordezkatzen jarrai dezazun.</span><span class="sxs-lookup"><span data-stu-id="6b700-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![Gelditu AOS](./media/2StopAOS.png)

4. <span data-ttu-id="6b700-117">Joan **Zerbitzuak** eta gelditu bi elementu hauek:</span><span class="sxs-lookup"><span data-stu-id="6b700-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="6b700-118">Microsoft Dynamics 365 Unified Operations: Loteen kudeaketa zerbitzua</span><span class="sxs-lookup"><span data-stu-id="6b700-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="6b700-119">Microsoft Dynamics 365 Unified Operations: Datuak Inportatzeko Esportazio Esparrua</span><span class="sxs-lookup"><span data-stu-id="6b700-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![Gelditu zerbitzuak](./media/3StopServices.png)

5. <span data-ttu-id="6b700-121">Ireki Microsoft SQL Server Management Studio.</span><span class="sxs-lookup"><span data-stu-id="6b700-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="6b700-122">Hasi saioa SQL zerbitzariaren egiaztagiriekin eta erabili axdbadmin erabiltzailea eta LCSko pasahitza **Inguruneen xehetasunak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="6b700-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server Management Studio](./media/4SSMS.png)

6. <span data-ttu-id="6b700-124">Object Explorer-en, **Datu-baseak** eta kokatu **AXDB**.</span><span class="sxs-lookup"><span data-stu-id="6b700-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="6b700-125">Datu-basea datu-basean ordeztuko duzu [Deskarga-zentroan](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span><span class="sxs-lookup"><span data-stu-id="6b700-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="6b700-126">Kopiatu zip fitxategia urrun zauden VM-ra eta atera zip edukia.</span><span class="sxs-lookup"><span data-stu-id="6b700-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="6b700-127">SQL Server Management Studio-n, egin klik eskuineko botoiaz **AxDB** eta, ondoren, hautatu **Zereginak** > **Berreskuratu** > **Datu basea**.</span><span class="sxs-lookup"><span data-stu-id="6b700-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![Leheneratu datu-basea](./media/5RestoreDatabase.png)

9. <span data-ttu-id="6b700-129">Aukeratu **Iturburu-gailua** eta joan kopiatu duzun zip-etik ateratako fitxategira.</span><span class="sxs-lookup"><span data-stu-id="6b700-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![Iturri gailuak](./media/6SourceDevice.png)

10. <span data-ttu-id="6b700-131">Aukeratu **Aukerak** eta, ondoren, hautatu **Gainidatzi lehendik dagoen datu basea** eta **Itxi dauden konexioak helmugako datu basera**.</span><span class="sxs-lookup"><span data-stu-id="6b700-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="6b700-132">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="6b700-132">Select **OK**.</span></span>

![Leheneratu ezarpenak](./media/7RestoreSetting.png)

<span data-ttu-id="6b700-134">AXDB berreskurapena arrakastatsua izan dela baieztatuko duzu.</span><span class="sxs-lookup"><span data-stu-id="6b700-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="6b700-135">Baieztapen hau jaso ondoren, SQL Services Management Studio itxi dezakezu.</span><span class="sxs-lookup"><span data-stu-id="6b700-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="6b700-136">Itzuli **Interneteko Informazio Zerbitzuak** > **Aplikazio multzoak** > **AOSZerbitzua** aukerara eta hasi AOSZerbitzua.</span><span class="sxs-lookup"><span data-stu-id="6b700-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="6b700-137">Joan **Zerbitzuak** eta hasi lehen gelditu zenituen bi zerbitzuak.</span><span class="sxs-lookup"><span data-stu-id="6b700-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="6b700-138">Aurkitu AdminUserProvisioning tresna VM honetan.</span><span class="sxs-lookup"><span data-stu-id="6b700-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="6b700-139">Begiratu azpian, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span><span class="sxs-lookup"><span data-stu-id="6b700-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="6b700-140">Exekutatu .ext fitxategia zure erabiltzailearen helbidea erabiliz **Helbide elektronikoa** eremua.</span><span class="sxs-lookup"><span data-stu-id="6b700-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="6b700-141">Hautatu **Bidali**.</span><span class="sxs-lookup"><span data-stu-id="6b700-141">Select **Submit**.</span></span>

![Administratzaile-erabiltzailearen hornitzea](./media/8AdminUserProvisioning.png)

<span data-ttu-id="6b700-143">Minutu pare bat behar dira.</span><span class="sxs-lookup"><span data-stu-id="6b700-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="6b700-144">Admin erabiltzailea ondo eguneratu dela baieztatzeko mezua jaso beharko zenuke.</span><span class="sxs-lookup"><span data-stu-id="6b700-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="6b700-145">Azkenean, exekutatu komando-gonbita administratzaile gisa eta burutu iisreset</span><span class="sxs-lookup"><span data-stu-id="6b700-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![IIS berrezartzea](./media/9IISReset.png)

18. <span data-ttu-id="6b700-147">Itxi urruneko mahaigaineko saioa eta erabili LCS **Ingurumenaren xehetasunak** orria ingurunean saioa hasteko espero bezala funtzionatzen duela baieztatzeko.</span><span class="sxs-lookup"><span data-stu-id="6b700-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)
