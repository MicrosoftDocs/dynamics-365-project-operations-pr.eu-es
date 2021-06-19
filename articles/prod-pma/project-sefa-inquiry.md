---
title: Sari Federalen kontsulten gastuen egutegia
description: Gai honek Sari Federalen Gastuen Ordutegiari buruzko kontsultari buruzko informazioa eskaintzen du.
author: velofog
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: a16b0fb097124e26da09e220a1239cd6df303f98
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010051"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="1e80e-103">Sari Federalen kontsulten gastuen egutegia</span><span class="sxs-lookup"><span data-stu-id="1e80e-103">Schedule of Expenditures of Federal Awards inquiry</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1e80e-104">A-133 Bulegoko Kudeaketa eta Aurrekontuen Zirkularrak dioenez, funts federalak jasotzen dituzten agentziek ikuskaritza-eskakizunak betetzen dituzte, auditoria bakarra izenarekin ere ezagutzen direnak.</span><span class="sxs-lookup"><span data-stu-id="1e80e-104">According to Office of Management and Budget Circular A-133, agencies that receive federal funds are subject to audit requirements, which are also known as single audits.</span></span> <span data-ttu-id="1e80e-105">Ikuskaritza prozesua beka federalen sarreren eta gastuen berri emateko erabiltzen da behin eta berriz.</span><span class="sxs-lookup"><span data-stu-id="1e80e-105">The audit process is used to report on the revenues and expenditures of federal grants on a recurring basis.</span></span> <span data-ttu-id="1e80e-106">Ikuskaritza txosten bakarraren zati batek Sari Federalen Gastuen Egitaraua (SEFA) barne hartzen du.</span><span class="sxs-lookup"><span data-stu-id="1e80e-106">Part of the single audit report includes the Schedule of Expenditures of Federal Awards (SEFA).</span></span>

<span data-ttu-id="1e80e-107">Sari Federalen Gastuen Ordutegiak kontsultak barne hartzen ditu Etxe Laguntza Federalaren Katalogoa (CFDA) izenburua eta zenbakia, diru-laguntzaren zenbakia, diru-laguntzaren urtea, funtsak ematen dituen agentzia federalaren izena eta txartelaren izena. entitatearen bidez.</span><span class="sxs-lookup"><span data-stu-id="1e80e-107">The Schedule of Expenditures of Federal Awards inquiry includes the Catalog of Federal Domestic Assistance (CFDA) title and number, the grant number, the year of the grant, the name of the federal agency that provides the funds, and the name of the pass-through entity.</span></span> <span data-ttu-id="1e80e-108">Kontsulta epe zehatz baterako da.</span><span class="sxs-lookup"><span data-stu-id="1e80e-108">The inquiry is for a specific period.</span></span> <span data-ttu-id="1e80e-109">Normalean, epe hori finantza egoeraren aldiaren berdina da, hau da, urte fiskal.</span><span class="sxs-lookup"><span data-stu-id="1e80e-109">Typically, that period is the same as the financial statement period, which is a fiscal year.</span></span>

<span data-ttu-id="1e80e-110">Kontsultak hautatutako data tartean proiekzio datak dituzten laguntzak biltzen ditu.</span><span class="sxs-lookup"><span data-stu-id="1e80e-110">The inquiry includes grants that have projection dates in the selected date range.</span></span> <span data-ttu-id="1e80e-111">**Laguntzailea** kontsultaren zutabean, bekaren bezeroa edo, igarotako beka lortzeko, agentzia emailea agertzen da.</span><span class="sxs-lookup"><span data-stu-id="1e80e-111">The **Grantor agency** column of the inquiry shows the grant customer or, for a pass-through grant, the grantor agency.</span></span> <span data-ttu-id="1e80e-112">Diru-laguntza emateko, **Pass-through agentzia** zutabeak beka bezeroa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="1e80e-112">For a pass-through grant, the **Pass-through agency** column shows the grant customer.</span></span> <span data-ttu-id="1e80e-113">Diru-laguntza ematen ez bada, **Pass-through agentzia** zutabea hutsik geratuko da.</span><span class="sxs-lookup"><span data-stu-id="1e80e-113">If the grant isn't a pass-through grant, the **Pass-through agency** column is blank.</span></span>

## <a name="set-up-the-cfda-clusters"></a><span data-ttu-id="1e80e-114">Konfiguratu CFDA klusterrak</span><span class="sxs-lookup"><span data-stu-id="1e80e-114">Set up the CFDA clusters</span></span>

<span data-ttu-id="1e80e-115">CFDA zenbakiekin lotu daitezkeen CFDA klusterrak konfiguratu behar dituzu Sari Federalen Gastuen Egutegia kontsultan.</span><span class="sxs-lookup"><span data-stu-id="1e80e-115">You must set up the CFDA clusters that can be associated with CFDA numbers in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="1e80e-116">Joan **Proiektuen kudeaketa eta kontabilitatea\> Konfigurazioa\> Diru-laguntzak\> Barne Laguntza Federaleko klusterren katalogoa**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-116">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance clusters**.</span></span>
2. <span data-ttu-id="1e80e-117">Hautatu **Berria** CFDA klusterra sortzeko.</span><span class="sxs-lookup"><span data-stu-id="1e80e-117">Select **New** to create a CFDA cluster.</span></span>
3. <span data-ttu-id="1e80e-118">Idatzi klusterraren izena.</span><span class="sxs-lookup"><span data-stu-id="1e80e-118">Enter the cluster name.</span></span>
4. <span data-ttu-id="1e80e-119">Aldaketak gordetzeko, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-119">Select **Save** to save your changes.</span></span>

## <a name="set-up-cfda-numbers"></a><span data-ttu-id="1e80e-120">Konfiguratu CFDA zenbakiak</span><span class="sxs-lookup"><span data-stu-id="1e80e-120">Set up CFDA numbers</span></span>

<span data-ttu-id="1e80e-121">CFDA zenbakiekin lotu daitezkeen CFDA klusterrak diru-laguntzetan gehi daitezke eta konfiguratu behar dituzu Sari Federalen Gastuen Egutegia kontsultan.</span><span class="sxs-lookup"><span data-stu-id="1e80e-121">You must set up CFDA numbers that can be added to grants and included in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="1e80e-122">Joan **Proiektuen kudeaketa eta kontabilitatea \> Konfigurazioa \> Diru-laguntzak \> Barne Laguntza Federaleko zenbakien katalogoa**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-122">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance numbers**.</span></span>
2. <span data-ttu-id="1e80e-123">Hautatu **Berria** CFDA zenbaki bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="1e80e-123">Select **New** to create a CFDA number.</span></span>
3. <span data-ttu-id="1e80e-124">**Zenbakia** zutabean, idatzi CFDA zenbakia.</span><span class="sxs-lookup"><span data-stu-id="1e80e-124">In the **Number** column, enter the CFDA number.</span></span>
4. <span data-ttu-id="1e80e-125">Sakatu **Fitxa** gakoa.</span><span class="sxs-lookup"><span data-stu-id="1e80e-125">Press the **Tab** key.</span></span>
5. <span data-ttu-id="1e80e-126">**Azalpena** zutabean, idatzi CFDA izenburua.</span><span class="sxs-lookup"><span data-stu-id="1e80e-126">In the **Description** column, enter the CFDA title.</span></span>
6. <span data-ttu-id="1e80e-127">Sakatu **Fitxa** gakoa.</span><span class="sxs-lookup"><span data-stu-id="1e80e-127">Press the **Tab** key.</span></span>
7. <span data-ttu-id="1e80e-128">Aukerakoa: **Programa klusterra** eremuan, gehitu dagokion CFDA klusterra.</span><span class="sxs-lookup"><span data-stu-id="1e80e-128">Optional: In the **Program cluster** field, add the appropriate CFDA cluster.</span></span>
8. <span data-ttu-id="1e80e-129">Aldaketak gordetzeko, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-129">Select **Save** to save your changes.</span></span>

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="1e80e-130">Ezarri diru-laguntzak Sari Federalen Gastuen Egutegia kontsultatzeko</span><span class="sxs-lookup"><span data-stu-id="1e80e-130">Set up grants to report for the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="1e80e-131">Joan **Proiektuen kudeaketa eta kontabilitatea \> Diru-laguntzak \> Diru-laguntzak**, eta hautatu lehendik dagoen dirulaguntza.</span><span class="sxs-lookup"><span data-stu-id="1e80e-131">Go to **Project management and accounting \> Grants \> Grants**, and select an existing grant.</span></span>
2. <span data-ttu-id="1e80e-132">**Konfigurazioa** FastTab fitxategian **Barne Laguntza Federalaren Katalogoa** eremuan, esleitu CFDA zenbakia.</span><span class="sxs-lookup"><span data-stu-id="1e80e-132">On the **Setup** FastTab, in the **Catalog of Federal Domestic Assistance** field, assign the CFDA number.</span></span> <span data-ttu-id="1e80e-133">Bekaren CFDA zenbakiak CFDA klusterra zehazten du txostenak egiteko.</span><span class="sxs-lookup"><span data-stu-id="1e80e-133">The CFDA number on the grant determines the CFDA cluster for reporting.</span></span>
3. <span data-ttu-id="1e80e-134">**Harremanetarako informazioa** FastTab-en, idatzi emailearen informazioa urrats hauek jarraituz:</span><span class="sxs-lookup"><span data-stu-id="1e80e-134">On **Contact information** FastTab, enter the grantor information by following these steps:</span></span>

    1. <span data-ttu-id="1e80e-135">**Eman bezeroari** eremuan, sartu bekaren erantzule den bezeroa.</span><span class="sxs-lookup"><span data-stu-id="1e80e-135">In the **Grant customer** field, enter the customer who is responsible for the grant.</span></span> <span data-ttu-id="1e80e-136">Lehendik dagoen beka baterako, baliteke informazio hori jada sartzea.</span><span class="sxs-lookup"><span data-stu-id="1e80e-136">For an existing grant, this information might already be entered.</span></span>
    2. <span data-ttu-id="1e80e-137">Adierazi bekaren bezeroa finantzatzailea den.</span><span class="sxs-lookup"><span data-stu-id="1e80e-137">Indicate whether the grant customer is the funder.</span></span> <span data-ttu-id="1e80e-138">Bekaren bezeroa finantzatzailea bada, utzi **Pasabidea** kontrol laukia garbitu da.</span><span class="sxs-lookup"><span data-stu-id="1e80e-138">If the grant customer is the funder, leave the **Pass-through** check box cleared.</span></span> <span data-ttu-id="1e80e-139">Beste bezero bat finantzatzailea bada, eta diru-laguntza bezeroa dirua gastatzeaz eta jarraitzeaz arduratzen bada, hautatu **Pasabidea** kontrol-laukia.</span><span class="sxs-lookup"><span data-stu-id="1e80e-139">If another customer is the funder, and the grant customer is responsible for spending and tracking the money, select the **Pass-through** check box.</span></span>

4. <span data-ttu-id="1e80e-140">Aukeratu baduzu **Pasabidea** markatu aurreko urratseko kontrol laukia **Laguntzailea** eremuan, idatzi beka eman duen bezeroa.</span><span class="sxs-lookup"><span data-stu-id="1e80e-140">If you selected the **Pass-through** check box in the previous step, in the **Grantor agency** field, enter the customer who provided the grant.</span></span> <span data-ttu-id="1e80e-141">Laguntza-agentzia eta beka-bezeroa ezin dira bezero bera izan.</span><span class="sxs-lookup"><span data-stu-id="1e80e-141">The grantor agency and the grant customer can't be the same customer.</span></span>

<span data-ttu-id="1e80e-142">Hona hemen igarotako beka baten adibidea:</span><span class="sxs-lookup"><span data-stu-id="1e80e-142">Here is an example of a pass-through grant:</span></span>

<span data-ttu-id="1e80e-143">Gobernu federalak estatu baterako azpiegitura proiektua finantzatu zuen.</span><span class="sxs-lookup"><span data-stu-id="1e80e-143">The federal government funded an infrastructure project for a state.</span></span> <span data-ttu-id="1e80e-144">Gobernu federalak dirua eman zion estatuari gastatzeko.</span><span class="sxs-lookup"><span data-stu-id="1e80e-144">The federal government gave the money to the state to spend.</span></span> <span data-ttu-id="1e80e-145">Kasu honetan, gobernu federala da laguntza-agentzia, eta estatua beka-bezeroa da.</span><span class="sxs-lookup"><span data-stu-id="1e80e-145">In this case, the federal government is the grantor agency, and the state is the grant customer.</span></span>

> [!NOTE] 
> <span data-ttu-id="1e80e-146">Ezaugarria lehen aldiz aktibatzen duzunean, hasierako CFDA zenbakiak diru-laguntzetan dauden zenbakiak erabiliz sartuko dira.</span><span class="sxs-lookup"><span data-stu-id="1e80e-146">When you first turn on the feature, initial CFDA numbers will be entered by using the existing numbers on grants.</span></span>

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a><span data-ttu-id="1e80e-147">Baztertu diru-laguntzak SEFA txostenetik diru-laguntza motaren arabera</span><span class="sxs-lookup"><span data-stu-id="1e80e-147">Exclude grants from SEFA reporting based on the grant type</span></span>

1. <span data-ttu-id="1e80e-148">Joan **Proiektuen kudeaketa eta kontabilitatea \> Konfigurazioa \> Diru-laguntzak \> Beka motak**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-148">Go to **Project management and accounting \> Setup \> Grants \> Grant types**.</span></span>
2. <span data-ttu-id="1e80e-149">**Informazio lehenetsia** FastTab-en, hautatu **Sari Federalen Gastuen Ordutegitik kanpo utzi** kontrol-laukia.</span><span class="sxs-lookup"><span data-stu-id="1e80e-149">On the **Default information** FastTab, select the **Exclude from Schedule of Expenditures of Federal Awards** check box.</span></span>
3. <span data-ttu-id="1e80e-150">Aldaketak gordetzeko, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-150">Select **Save** to save your changes.</span></span>

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="1e80e-151">Exekutatu Sari Federalen kontsulten gastuen egutegia</span><span class="sxs-lookup"><span data-stu-id="1e80e-151">Run the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="1e80e-152">Joan **Proiektuen kudeaketa eta kontabilitatea \> Kontsultak eta txostenak \> Beka kontsulta \> Sari Federalen Gastuen Egitaraua**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-152">Go to **Project management and accounting \> Inquiries and reports \> Grant inquiry \> Schedule of Expenditures of Federal Awards**.</span></span>
2. <span data-ttu-id="1e80e-153">**Parametroak** sekzioan, ondorengo pausoak jarraitu:</span><span class="sxs-lookup"><span data-stu-id="1e80e-153">In the **Parameters** section, follow these steps:</span></span>

    1. <span data-ttu-id="1e80e-154">**Data tartea** eremuan, hautatu data tartearen kodea.</span><span class="sxs-lookup"><span data-stu-id="1e80e-154">In the **Date interval** field, select the code for the date interval.</span></span> <span data-ttu-id="1e80e-155">Bestela, **Datatik aurrera** eta **Orain arte** eremuak, zehaztu data tartea.</span><span class="sxs-lookup"><span data-stu-id="1e80e-155">Alternatively, in the **From date** and **To date** fields, define the date interval.</span></span>
    2. <span data-ttu-id="1e80e-156">Aukerakoa: kontsultan diru-sarrera gisa fakturatutako transakzioak soilik sartzeko, ezarri **Sartu fakturatutako diru-sarrerak soilik** aukera **Bai**.</span><span class="sxs-lookup"><span data-stu-id="1e80e-156">Optional: To include only billed transactions as revenue in the inquiry, set the **Include only billed revenues** option to **Yes**.</span></span>

## <a name="columns"></a><span data-ttu-id="1e80e-157">Zutabeak</span><span class="sxs-lookup"><span data-stu-id="1e80e-157">Columns</span></span>

<span data-ttu-id="1e80e-158">Sari Federalen Gastuen Ordutegiak kontsultak honako zutabe hauek ditu:</span><span class="sxs-lookup"><span data-stu-id="1e80e-158">The Schedule of Expenditures of Federal Awards inquiry includes the following columns:</span></span>

- <span data-ttu-id="1e80e-159">Barne Laguntza Federalaren klusterren katalogoa</span><span class="sxs-lookup"><span data-stu-id="1e80e-159">Catalog of Federal Domestic Assistance cluster name</span></span>
- <span data-ttu-id="1e80e-160">Laguntzailea</span><span class="sxs-lookup"><span data-stu-id="1e80e-160">Grantor agency</span></span>
- <span data-ttu-id="1e80e-161">Pasabide-agentzia</span><span class="sxs-lookup"><span data-stu-id="1e80e-161">Pass-through agency</span></span>
- <span data-ttu-id="1e80e-162">Eman izena</span><span class="sxs-lookup"><span data-stu-id="1e80e-162">Grant name</span></span>
- <span data-ttu-id="1e80e-163">Eman IDa</span><span class="sxs-lookup"><span data-stu-id="1e80e-163">Grant ID</span></span>
- <span data-ttu-id="1e80e-164">Diru-laguntza eskaeraren IDa</span><span class="sxs-lookup"><span data-stu-id="1e80e-164">Grant application ID</span></span>
- <span data-ttu-id="1e80e-165">Barne Laguntza Federalaren katalogoa</span><span class="sxs-lookup"><span data-stu-id="1e80e-165">Catalog of Federal Domestic Assistance</span></span>
- <span data-ttu-id="1e80e-166">Agiriak</span><span class="sxs-lookup"><span data-stu-id="1e80e-166">Receipts</span></span>
- <span data-ttu-id="1e80e-167">Gastuak</span><span class="sxs-lookup"><span data-stu-id="1e80e-167">Expenditures</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]