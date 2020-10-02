---
title: Zuzenketa-egunkariak sortu eta berretsi
description: Gai honek zuzenketa-egunkari bat sortzeari eta hura berresteari buruzko informazioa ematen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 274f99527804b0db81b26201a22eb5a8cbe86c9a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896941"
---
# <a name="create-and-confirm-correction-journals"></a><span data-ttu-id="636f0-103">Zuzenketa-egunkariak sortu eta berretsi</span><span class="sxs-lookup"><span data-stu-id="636f0-103">Create and confirm Correction journals</span></span>

<span data-ttu-id="636f0-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="636f0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="636f0-105">Batzuetan, denbora edo gastuen sarrera bat okerra izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="636f0-105">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="636f0-106">Adibidez, baliteke aholkulari batek data okerra aukeratzea denbora-sarreran edo baliteke zenbakiekin nahastea gastu bat idaztean.</span><span class="sxs-lookup"><span data-stu-id="636f0-106">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="636f0-107">Aholkulari batek ezin badu bidalitako sarreren eguneratzeak egin, administratzaile batek zuzenean zuzendu dezake proiektuko sarrera.</span><span class="sxs-lookup"><span data-stu-id="636f0-107">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="636f0-108">Gai honetako prozedurak betetzeko, Administratzailearen baimenak beharko dituzu.</span><span class="sxs-lookup"><span data-stu-id="636f0-108">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="636f0-109">Zuzendu onartutako denbora-sarrerak</span><span class="sxs-lookup"><span data-stu-id="636f0-109">Correct approved time entries</span></span>     

<span data-ttu-id="636f0-110">Bete urrats hauek proiektu bateko denbora-sarrera bakarrak edo bat baino gehiago zuzentzeko.</span><span class="sxs-lookup"><span data-stu-id="636f0-110">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="636f0-111">**Salmentak**eremuan, hautatu **Transakzioak** eta, ondoren, hautatu **Onartutako ordua**.</span><span class="sxs-lookup"><span data-stu-id="636f0-111">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="636f0-112">**Onartutako ordua** zerrendan, kokatu eta hautatu onartutako denbora-sarrera bat edo gehiago zuzentzeko.</span><span class="sxs-lookup"><span data-stu-id="636f0-112">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="636f0-113">Lotutako sarrerak aurkitzeko iragazkia erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="636f0-113">You can use the filter to locate related entries.</span></span> <span data-ttu-id="636f0-114">Adibidez, Proiektuaren ID bat iragazi eta Proiektu ID horrekin onartutako denbora-sarrera guztiak hauta ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="636f0-114">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="636f0-115">Hautatu **Zuzendu sarrera**.</span><span class="sxs-lookup"><span data-stu-id="636f0-115">Select **Correct entries**.</span></span> <span data-ttu-id="636f0-116">Zuzenketa-aldizkari berri bat sortuko da automatikoki, esleitutako **Denboraren zuzenketa** motarekin.</span><span class="sxs-lookup"><span data-stu-id="636f0-116">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="636f0-117">Aukeratutako sarrerak aldizkarian gehituko dira.</span><span class="sxs-lookup"><span data-stu-id="636f0-117">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="636f0-118">**Aldizkari berria** orrian, sartu **Deskribapena** zuzenketa-aldizkarian eta, ondoren, hautatu **Ordu-sarreraren zuzenketak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="636f0-118">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  

5. <span data-ttu-id="636f0-119">**Denbora-sarreren balio berriak** atalean, eguneratu eremuak informazio egokiarekin behar ahala.</span><span class="sxs-lookup"><span data-stu-id="636f0-119">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="636f0-120">Adibidez, esleitutako proiektua edo baliabide eserbagarria alda dezakezu.</span><span class="sxs-lookup"><span data-stu-id="636f0-120">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="636f0-121">Hautatu **Aurrebista**.</span><span class="sxs-lookup"><span data-stu-id="636f0-121">Select **Preview**.</span></span> <span data-ttu-id="636f0-122">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="636f0-122">In the dialog box, select **OK**.</span></span> <span data-ttu-id="636f0-123">**Aldizkari-lerroak** fitxan, aldatu eta zuzendu diren hautatutako denbora-sarrerekin lotutako jatorrizko benetako datuen zerrenda ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="636f0-123">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="636f0-124">Zuzenketa osagarriak egin behar badira, errepikatu 5. eta 6. urratsak.</span><span class="sxs-lookup"><span data-stu-id="636f0-124">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="636f0-125">Zuzendutako benetako datuek **Denboraren sarrerako balio berriak** sekzioan hautatutako balio berak dituzte.</span><span class="sxs-lookup"><span data-stu-id="636f0-125">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="636f0-126">Zuzenketak espero bezala agertzen badira, hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="636f0-126">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="636f0-127">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="636f0-127">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="636f0-128">**Salmentak** eremuan, hautatu **Proiektuak** eta, ondoren, ireki denboraren sarrerak eguneratu dituzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="636f0-128">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="636f0-129">**Proiektuak** orrialdean, **Benetako datuak** fitxan, ikusi egin dituzun aldaketak.</span><span class="sxs-lookup"><span data-stu-id="636f0-129">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="636f0-130">**Benetako datuak** fitxa ez badago ikusgai, hautatu **Erlazionatutakoak** > **Benetako datuak** aukera.</span><span class="sxs-lookup"><span data-stu-id="636f0-130">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="636f0-131">**Ikuspegiaren erlazionatutako benetako datuak** zerrendan, aldatu den jatorrizko denbora-sarrerak zerrendatuta jarraitzen duela ikus dezakezu, dagozkion zuzendutako sarrerekin batera.</span><span class="sxs-lookup"><span data-stu-id="636f0-131">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="636f0-132">Adibidez, grafiko honetan, bi errenkada-elementu daude, Zenbatekoa zutabean 8,00 zenbatekoko zordunketak zerrendatuta dituenak.</span><span class="sxs-lookup"><span data-stu-id="636f0-132">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="636f0-133">Gainera, Zenbatekoa zutabean zordundutako zenbatekoak dituzten -8,00 zenbatekoko bi errenkada daude.</span><span class="sxs-lookup"><span data-stu-id="636f0-133">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="636f0-134">Horrela zuzenketarekin zenbatekoa zero da.</span><span class="sxs-lookup"><span data-stu-id="636f0-134">These corrections bring the quantity to zero.</span></span>

 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="636f0-135">Zuzendu onartutako gastuen sarrerak</span><span class="sxs-lookup"><span data-stu-id="636f0-135">Correct approved expense entries</span></span>

<span data-ttu-id="636f0-136">Bete urrats hauek gastuen sarrera bat edo gehiago zuzentzeko.</span><span class="sxs-lookup"><span data-stu-id="636f0-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="636f0-137">**Salmentak** eremuan, ezkerreko nabigazio-panelean, **Transakzioak** aukeraren azpian, hautatu **Onartutako gastuak**.</span><span class="sxs-lookup"><span data-stu-id="636f0-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="636f0-138">**Onartutako gastuak** zerrendan, hautatu zuzendu nahi duzun proiektua eta hautatu **Zuzendu sarrerak**.</span><span class="sxs-lookup"><span data-stu-id="636f0-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="636f0-139">Zuzenketa-aldizkari berri bat sortuko da automatikoki esleitutako **Gastuen zuzenketa** motarekin.</span><span class="sxs-lookup"><span data-stu-id="636f0-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="636f0-140">**Aldizkari berria** orrialdean, idatzi zuzenketaren **Deskribapena** eta **Gastuen zuzenketa** fitxan, **Gastuen balio berriak** sekzioan, hautatu hautatutako gastuen zerrenden zuzendu nahi dituzun datu-eremuetan.</span><span class="sxs-lookup"><span data-stu-id="636f0-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="636f0-141">Adibidez, gastua beste **Proiektu** bati eslei dakiokezu edo **Gastu-kategoria**, **Gastu-data** edo **Erreserbatzeko baliabidea** zuzen dezakezu.</span><span class="sxs-lookup"><span data-stu-id="636f0-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="636f0-142">Hautatu **Aurrebista**.</span><span class="sxs-lookup"><span data-stu-id="636f0-142">Select **Preview**.</span></span> <span data-ttu-id="636f0-143">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="636f0-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="636f0-144">Egiaztatu **Aldizkari-lerroak** fitxako zuzenketak. Aldatu eta zuzendu diren hautatutako denbora-sarrerekin lotutako jatorrizko benetako gastuen zerrenda ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="636f0-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="636f0-145">Zuzendutako balioak espero bezala agertzen badira, hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="636f0-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="636f0-146">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="636f0-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="636f0-147">Balioak ez badira espero bezala erakusten, hautatu **Utzi** **Onartutako gastuak** zerrendara itzultzeko.</span><span class="sxs-lookup"><span data-stu-id="636f0-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="636f0-148">Errepikatu 2. urratsetik 5. urratsera.</span><span class="sxs-lookup"><span data-stu-id="636f0-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="636f0-149">Zuzendutako benetako datuek **Gastuen balio berriak** sekzioan hautatutako balio berak dituzte.</span><span class="sxs-lookup"><span data-stu-id="636f0-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="636f0-150">Zuzenketa-aldizkaria berretsi ondoren, zoaz eguneratu dituzun proiektuetara, aldaketak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="636f0-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="636f0-151">Proiektuaren orrian, **Benetako datuak** fitxan, berrikusi **Ikuspegiarekin erlazionatutako benetako datuak**.</span><span class="sxs-lookup"><span data-stu-id="636f0-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="636f0-152">Jatorrizko sarrerak eta zuzendutako sarrerak zerrendatzen dira.</span><span class="sxs-lookup"><span data-stu-id="636f0-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="636f0-153">Grafiko hauetan jatorrizko gastuen sarrera-zenbatekoak eta dagozkion zuzendutako gastuen sarrera-zenbatekoak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="636f0-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 


