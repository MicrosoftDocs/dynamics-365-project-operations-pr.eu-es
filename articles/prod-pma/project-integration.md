---
title: Microsoft Project client integrazioa
description: Proiektuen egutegia planifikatzea eta mantentzea konplexua izan daiteke, beraz, proiektuen kudeatzaileek zeregin hori kudeatzen lagunduko dieten tresnak erabili behar dituzte. Microsoft Project Client-ekin integratzeak proiektuaren lanen banakako egitura irekitzeko eta kudeatzeko laguntza eskaintzen du.
author: Yowelle
ms.date: 12/11/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: 032d726bb6206c563b573f30d13fe2697a13c949
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999431"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="ab88f-104">Microsoft Project client integrazioa</span><span class="sxs-lookup"><span data-stu-id="ab88f-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="ab88f-105">Proiektuen egutegia planifikatzea eta mantentzea konplexua izan daiteke, beraz, proiektuen kudeatzaileek zeregin hori kudeatzen lagunduko dieten tresnak erabili behar dituzte.</span><span class="sxs-lookup"><span data-stu-id="ab88f-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="ab88f-106">Microsoft Project Client-ekin integratzeak proiektuaren lanen banakako egitura irekitzeko eta kudeatzeko laguntza eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="ab88f-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="ab88f-107">Proiektuaren kudeatzaileak edozein aldaketa argitaratu ahal izango ditu Dynamics 365 Finance proiektuaren zereginen xehetasunen egitura.</span><span class="sxs-lookup"><span data-stu-id="ab88f-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="ab88f-108">Uztaileko eguneratzea erabiltzen baduzu (10.0.4 bertsioa), KB 4054797 eta 4055884 instalatu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="ab88f-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="ab88f-109">Konfiguratu Microsoft Project Client gehigarria</span><span class="sxs-lookup"><span data-stu-id="ab88f-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="ab88f-110">Microsoft Project Client-ekin bateratzea ahalbidetzeko, a Microsoft Dynamics 365 gehigarriak erabiltzailearen bezero Microsoft Project aplikazioan instalatu behar dira.</span><span class="sxs-lookup"><span data-stu-id="ab88f-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="ab88f-111">Hau irekitzen da **Proiektuak kudeatzeko lan eremua**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="ab88f-112">•   Egin klik **Konfiguratu proiektuaren bezeroaren gehigarria** hurrengotik **Estekak** > **Konfigurazioa** lan-eremuko atala.</span><span class="sxs-lookup"><span data-stu-id="ab88f-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="ab88f-113">•   Egin klik **Ireki**, egin klik **Exekutatu** galdetutakoan.</span><span class="sxs-lookup"><span data-stu-id="ab88f-113">•   Click **Open**, then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="ab88f-114">Ireki eta editatu lehendik dagoen proiektuaren zirriborroen egitura Microsoft Project Client-en</span><span class="sxs-lookup"><span data-stu-id="ab88f-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="ab88f-115">Proiektu bat bada Dynamics 365 Finance dagoeneko zereginen xehetasunen egitura sortu da, zereginen xehetasunen egitura Microsoft Project Client aplikazioan ireki ahal izango da lan banakako egitura zirriborro egoeran badago.</span><span class="sxs-lookup"><span data-stu-id="ab88f-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="ab88f-116">Irekitzeko **Proiektua** orrialdean, egin klik **Ireki Microsoft Project-en** estekatik **Plana** fitxa. Orri hau Microsoft Project Client aplikazioaren barruan ere ireki daiteke klik eginez **Irekia** urtean **Microsoft Dynamics 365** fitxa. Aukeratu **Pertsona juridikoa** eta **Proiektua** zerrendatik.</span><span class="sxs-lookup"><span data-stu-id="ab88f-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="ab88f-117">Erabiltzen ari bazara Internet Explorer zure arakatzaile gisa, klik egin beharko duzu **Gorde** fitxategia deskargatu den kokapenetik eskuz irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="ab88f-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="ab88f-118">Edo, egin klik **Gorde eta ireki** fitxategia Microsoft Project Client-en irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="ab88f-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="ab88f-119">Ez aldatu izena gordetzean fitxategiaren izena.</span><span class="sxs-lookup"><span data-stu-id="ab88f-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="ab88f-120">Microsoft Project Client-ekin fitxategian aldaketak egin aurretik, egiaztatu egin behar duzu. Egin klik **Errebisatu** urtean **Microsoft Dynamics 365** fitxa. Horrek saihestuko du beste erabiltzaile batzuek lanaren banakako egitura aldi berean Finantza barrutik editatzea.</span><span class="sxs-lookup"><span data-stu-id="ab88f-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="ab88f-121">Edizioak egin ondoren lanaren banakako egitura argitaratzeko, egin klik **Sartu** gainean **Microsoft Dynamics 365** fitxa.</span><span class="sxs-lookup"><span data-stu-id="ab88f-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="ab88f-122">Finantza proiektuan proiektu talde bat dagoeneko gehitu bada, baliabideen zerrenda taldekideekin osatuko da.</span><span class="sxs-lookup"><span data-stu-id="ab88f-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="ab88f-123">Proiektu talde bat oraindik proiektuan gehitu ez bada, baliabideak hauta ditzakezu eta taldea Microsoft Project Client-en sortu dezakezu klik eginez **Baliabideak** botoian **Microsoft Dynamics 365** fitxa.</span><span class="sxs-lookup"><span data-stu-id="ab88f-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="ab88f-124">Datu hauek Finantzarekin sinkronizatuko dira check-in prozesuaren barruan:</span><span class="sxs-lookup"><span data-stu-id="ab88f-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="ab88f-125">•   Zereginaren izena</span><span class="sxs-lookup"><span data-stu-id="ab88f-125">•   Task name</span></span>

<span data-ttu-id="ab88f-126">•   Hasiera data</span><span class="sxs-lookup"><span data-stu-id="ab88f-126">•   Start date</span></span>

<span data-ttu-id="ab88f-127">•   Amaieraren data</span><span class="sxs-lookup"><span data-stu-id="ab88f-127">•   Finish date</span></span>

<span data-ttu-id="ab88f-128">•   Aurrekoak</span><span class="sxs-lookup"><span data-stu-id="ab88f-128">•   Predecessors</span></span>

<span data-ttu-id="ab88f-129">•   Baliabide izenak</span><span class="sxs-lookup"><span data-stu-id="ab88f-129">•   Resource names</span></span>

<span data-ttu-id="ab88f-130">•   Kategoria</span><span class="sxs-lookup"><span data-stu-id="ab88f-130">•   Category</span></span>

<span data-ttu-id="ab88f-131">•   Baliabide kategoria</span><span class="sxs-lookup"><span data-stu-id="ab88f-131">•   Resource category</span></span>

<span data-ttu-id="ab88f-132">•   Lan-orduak</span><span class="sxs-lookup"><span data-stu-id="ab88f-132">•   Work hours</span></span>

<span data-ttu-id="ab88f-133">•   Oharrak</span><span class="sxs-lookup"><span data-stu-id="ab88f-133">•   Notes</span></span>

<span data-ttu-id="ab88f-134">•   Lehentasuna</span><span class="sxs-lookup"><span data-stu-id="ab88f-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="ab88f-135">Microsoft Project Client fitxategian beste zutabe batzuk gehitzen badituzu, ez dira fitxategian gordeko eta ez dira bistaratuko fitxategia berriro irekitzen denean.</span><span class="sxs-lookup"><span data-stu-id="ab88f-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="ab88f-136">Sortu lehendik dagoen proiektu baterako lanen banaketa egitura Microsoft Project Client erabiliz</span><span class="sxs-lookup"><span data-stu-id="ab88f-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="ab88f-137">Sortzeko zereginen xehetasunen egitura berria erabiliz Microsoft Project Client hurrengo pauso hauek:</span><span class="sxs-lookup"><span data-stu-id="ab88f-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="ab88f-138">Ireki Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="ab88f-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="ab88f-139">**Microsoft Dynamics 365** fitxan, klik egin **Ireki**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="ab88f-140">Hautatu **Legezko entitatea** proiektuarentzat.</span><span class="sxs-lookup"><span data-stu-id="ab88f-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="ab88f-141">Hautatu **Proiektua**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="ab88f-142">Klik egin **Bilatu** hurrengoan **Microsoft Dynamics 365** fitxan.</span><span class="sxs-lookup"><span data-stu-id="ab88f-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="ab88f-143">Finantzan argitaratzeko prest zaudenean, egin klik **Sartu** gainean **Microsoft Dynamics 365** fitxa.</span><span class="sxs-lookup"><span data-stu-id="ab88f-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="ab88f-144">Ordezkatu existitzen den proiektu baterako lanen banaketa egitura Microsoft Project Client erabiliz</span><span class="sxs-lookup"><span data-stu-id="ab88f-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="ab88f-145">Microsoft Project Client erabiliz lanaren banakako egitura berria sortzeko eta lehendik dagoen proiektu baten lehendik dagoen banakako egitura ordezkatzeko, jarraitu urrats hauei:</span><span class="sxs-lookup"><span data-stu-id="ab88f-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="ab88f-146">Ireki Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="ab88f-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="ab88f-147">Sortu antolaketa Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="ab88f-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="ab88f-148">Gainean **Microsoft Dynamics 365** fitxa, egin klik **Aldaketak gorde** > **Ordeztu dagoen proiektua**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="ab88f-149">Hautatu **Legezko entitatea** proiektuarentzat.</span><span class="sxs-lookup"><span data-stu-id="ab88f-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="ab88f-150">Hautatu **Proiektua**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="ab88f-151">Sakatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="ab88f-152">Sortu proiektu berria Microsoft Project Client-etik</span><span class="sxs-lookup"><span data-stu-id="ab88f-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="ab88f-153">Ireki Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="ab88f-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="ab88f-154">Sortu antolaketa Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="ab88f-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="ab88f-155">Gainean **Microsoft Dynamics 365** fitxa, egin klik **Aldaketak gorde** > **Gorde proiektu berria**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="ab88f-156">Hautatu **Legezko entitatea** proiektuarentzat.</span><span class="sxs-lookup"><span data-stu-id="ab88f-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="ab88f-157">Sartu **Proiektuaren IDa**, Beharrezkoa bada.</span><span class="sxs-lookup"><span data-stu-id="ab88f-157">Enter the **Project ID**, if necessary.</span></span>

6.  <span data-ttu-id="ab88f-158">Idatzi **Proiektuaren izena**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="ab88f-159">Aukeratu **Proiektu mota**, **Proiektu taldea** eta **Proiektuaren kontratuaren IDa**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-159">Select the **Project type**, **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="ab88f-160">Bestela, proiektuaren kontratu berria sor dezakezu klik eginez **Berria**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="ab88f-161">Aukeratu **Egutegia** baliabideetarako erabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="ab88f-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="ab88f-162">Sakatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="ab88f-162">Click **OK**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]