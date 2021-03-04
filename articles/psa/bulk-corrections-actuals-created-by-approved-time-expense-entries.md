---
title: Benetako datuen zuzenketa masiboak onartutako denboraren eta gastuen sarrerek arabera
description: Gai honetan administratzaile batek aurrez onartutako orduaren edo gastuen sarreran zuzenketa bat edo masibo bat nola egin dezakeen azaltzen da, fakturazioa osatu gabe badago.
author: rumant
manager: AnnBe
ms.date: 04/02/2020
ms.topic: article
ms.service: dynamics-ax-applications
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
search.app:
- ProjectOperations
ms.openlocfilehash: 063c4d017f5904f09c3c239bfa432a128872e4d7
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144938"
---
# <a name="bulk-corrections-of-actuals-created-by-approved-time-and-expense-entries"></a><span data-ttu-id="41337-103">Benetako datuen zuzenketa masiboak onartutako denboraren eta gastuen sarrerek arabera</span><span class="sxs-lookup"><span data-stu-id="41337-103">Bulk corrections of actuals created by approved time and expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="41337-104">Batzuetan, denbora edo gastuen sarrera bat okerra izan daiteke.</span><span class="sxs-lookup"><span data-stu-id="41337-104">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="41337-105">Adibidez, baliteke aholkulari batek data okerra aukeratzea denbora-sarreran edo baliteke zenbakiekin nahastea gastu bat idaztean.</span><span class="sxs-lookup"><span data-stu-id="41337-105">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="41337-106">Aholkulari batek ezin badu bidalitako sarreren eguneratzeak egin, administratzaile batek zuzenean zuzendu dezake proiektuko sarrera.</span><span class="sxs-lookup"><span data-stu-id="41337-106">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="41337-107">Gai honetako prozedurak betetzeko, Administratzailearen baimenak beharko dituzu.</span><span class="sxs-lookup"><span data-stu-id="41337-107">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="41337-108">Zuzendu onartutako denbora-sarrerak</span><span class="sxs-lookup"><span data-stu-id="41337-108">Correct approved time entries</span></span>     

<span data-ttu-id="41337-109">Bete urrats hauek proiektu bateko denbora-sarrera bakarrak edo bat baino gehiago zuzentzeko.</span><span class="sxs-lookup"><span data-stu-id="41337-109">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="41337-110">**Salmentak** eremuan, hautatu **Transakzioak** eta, ondoren, hautatu **Onartutako ordua**.</span><span class="sxs-lookup"><span data-stu-id="41337-110">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="41337-111">**Onartutako ordua** zerrendan, kokatu eta hautatu onartutako denbora-sarrera bat edo gehiago zuzentzeko.</span><span class="sxs-lookup"><span data-stu-id="41337-111">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="41337-112">Lotutako sarrerak aurkitzeko iragazkia erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="41337-112">You can use the filter to locate related entries.</span></span> <span data-ttu-id="41337-113">Adibidez, Proiektuaren ID bat iragazi eta Proiektu ID horrekin onartutako denbora-sarrera guztiak hauta ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="41337-113">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="41337-114">Hautatu **Zuzendu sarrera**.</span><span class="sxs-lookup"><span data-stu-id="41337-114">Select **Correct entries**.</span></span> <span data-ttu-id="41337-115">Zuzenketa-aldizkari berri bat sortuko da automatikoki, esleitutako **Denboraren zuzenketa** motarekin.</span><span class="sxs-lookup"><span data-stu-id="41337-115">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="41337-116">Aukeratutako sarrerak aldizkarian gehituko dira.</span><span class="sxs-lookup"><span data-stu-id="41337-116">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="41337-117">**Aldizkari berria** orrian, sartu **Deskribapena** zuzenketa-aldizkarian eta, ondoren, hautatu **Ordu-sarreraren zuzenketak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="41337-117">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  
5. <span data-ttu-id="41337-118">**Denbora-sarreren balio berriak** atalean, eguneratu eremuak informazio egokiarekin behar ahala.</span><span class="sxs-lookup"><span data-stu-id="41337-118">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="41337-119">Adibidez, esleitutako proiektua edo baliabide eserbagarria alda dezakezu.</span><span class="sxs-lookup"><span data-stu-id="41337-119">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="41337-120">Hautatu **Aurrebista**.</span><span class="sxs-lookup"><span data-stu-id="41337-120">Select **Preview**.</span></span> <span data-ttu-id="41337-121">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="41337-121">In the dialog box, select **OK**.</span></span> <span data-ttu-id="41337-122">**Aldizkari-lerroak** fitxan, aldatu eta zuzendu diren hautatutako denbora-sarrerekin lotutako jatorrizko benetako datuen zerrenda ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="41337-122">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="41337-123">Zuzenketa osagarriak egin behar badira, errepikatu 5. eta 6. urratsak.</span><span class="sxs-lookup"><span data-stu-id="41337-123">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="41337-124">Zuzendutako benetako datuek **Denboraren sarrerako balio berriak** sekzioan hautatutako balio berak dituzte.</span><span class="sxs-lookup"><span data-stu-id="41337-124">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="41337-125">Zuzenketak espero bezala agertzen badira, hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="41337-125">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="41337-126">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="41337-126">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="41337-127">**Salmentak** eremuan, hautatu **Proiektuak** eta, ondoren, ireki denboraren sarrerak eguneratu dituzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="41337-127">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="41337-128">**Proiektuak** orrialdean, **Benetako datuak** fitxan, ikusi egin dituzun aldaketak.</span><span class="sxs-lookup"><span data-stu-id="41337-128">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="41337-129">**Benetako datuak** fitxa ez badago ikusgai, hautatu **Erlazionatutakoak** > **Benetako datuak** aukera.</span><span class="sxs-lookup"><span data-stu-id="41337-129">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="41337-130">**Ikuspegiaren erlazionatutako benetako datuak** zerrendan, aldatu den jatorrizko denbora-sarrerak zerrendatuta jarraitzen duela ikus dezakezu, dagozkion zuzendutako sarrerekin batera.</span><span class="sxs-lookup"><span data-stu-id="41337-130">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="41337-131">Adibidez, grafiko honetan, bi errenkada-elementu daude, Zenbatekoa zutabean 8,00 zenbatekoko zordunketak zerrendatuta dituenak.</span><span class="sxs-lookup"><span data-stu-id="41337-131">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="41337-132">Gainera, Zenbatekoa zutabean zordundutako zenbatekoak dituzten -8,00 zenbatekoko bi errenkada daude.</span><span class="sxs-lookup"><span data-stu-id="41337-132">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="41337-133">Horrela zuzenketarekin zenbatekoa zero da.</span><span class="sxs-lookup"><span data-stu-id="41337-133">These corrections bring the quantity to zero.</span></span>

![Benetako datuekin erlazionatutako ikuspegi-zerrenda](https://github.com/MicrosoftDocs/dynamics-365-customer-engagement-pr/blob/bulk-corrections-actuals-created-by-approved-time-expense-entries.md/time-actuals.png)
 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="41337-135">Zuzendu onartutako gastuen sarrerak</span><span class="sxs-lookup"><span data-stu-id="41337-135">Correct approved expense entries</span></span>

<span data-ttu-id="41337-136">Bete urrats hauek gastuen sarrera bat edo gehiago zuzentzeko.</span><span class="sxs-lookup"><span data-stu-id="41337-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="41337-137">**Salmentak** eremuan, ezkerreko nabigazio-panelean, **Transakzioak** aukeraren azpian, hautatu **Onartutako gastuak**.</span><span class="sxs-lookup"><span data-stu-id="41337-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="41337-138">**Onartutako gastuak** zerrendan, hautatu zuzendu nahi duzun proiektua eta hautatu **Zuzendu sarrerak**.</span><span class="sxs-lookup"><span data-stu-id="41337-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="41337-139">Zuzenketa-aldizkari berri bat sortuko da automatikoki esleitutako **Gastuen zuzenketa** motarekin.</span><span class="sxs-lookup"><span data-stu-id="41337-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="41337-140">**Aldizkari berria** orrialdean, idatzi zuzenketaren **Deskribapena** eta **Gastuen zuzenketa** fitxan, **Gastuen balio berriak** sekzioan, hautatu hautatutako gastuen zerrenden zuzendu nahi dituzun datu-eremuetan.</span><span class="sxs-lookup"><span data-stu-id="41337-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="41337-141">Adibidez, gastua beste **Proiektu** bati eslei dakiokezu edo **Gastu-kategoria**, **Gastu-data** edo **Erreserbatzeko baliabidea** zuzen dezakezu.</span><span class="sxs-lookup"><span data-stu-id="41337-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="41337-142">Hautatu **Aurrebista**.</span><span class="sxs-lookup"><span data-stu-id="41337-142">Select **Preview**.</span></span> <span data-ttu-id="41337-143">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="41337-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="41337-144">Egiaztatu **Aldizkari-lerroak** fitxako zuzenketak. Aldatu eta zuzendu diren hautatutako denbora-sarrerekin lotutako jatorrizko benetako gastuen zerrenda ikus dezakezu.</span><span class="sxs-lookup"><span data-stu-id="41337-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="41337-145">Zuzendutako balioak espero bezala agertzen badira, hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="41337-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="41337-146">Elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="41337-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="41337-147">Balioak ez badira espero bezala erakusten, hautatu **Utzi** **Onartutako gastuak** zerrendara itzultzeko.</span><span class="sxs-lookup"><span data-stu-id="41337-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="41337-148">Errepikatu 2. urratsetik 5. urratsera.</span><span class="sxs-lookup"><span data-stu-id="41337-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="41337-149">Zuzendutako benetako datuek **Gastuen balio berriak** sekzioan hautatutako balio berak dituzte.</span><span class="sxs-lookup"><span data-stu-id="41337-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="41337-150">Zuzenketa-aldizkaria berretsi ondoren, zoaz eguneratu dituzun proiektuetara, aldaketak ikusteko.</span><span class="sxs-lookup"><span data-stu-id="41337-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="41337-151">Proiektuaren orrian, **Benetako datuak** fitxan, berrikusi **Ikuspegiarekin erlazionatutako benetako datuak**.</span><span class="sxs-lookup"><span data-stu-id="41337-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="41337-152">Jatorrizko sarrerak eta zuzendutako sarrerak zerrendatzen dira.</span><span class="sxs-lookup"><span data-stu-id="41337-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="41337-153">Grafiko hauetan jatorrizko gastuen sarrera-zenbatekoak eta dagozkion zuzendutako gastuen sarrera-zenbatekoak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="41337-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 

![Gastuen benetako datuak](https://user-images.githubusercontent.com/60806505/77122219-4cd52900-69fa-11ea-8349-ccd2ffebf640.png)
