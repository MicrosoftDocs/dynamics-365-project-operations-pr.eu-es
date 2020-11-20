---
title: Benetako datuak
description: Gai honek Microsoft Dynamics 365 Project Operations-en benetako datuekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 13c429763fa805fae5324e4dcf1bf7669e842281
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126288"
---
# <a name="actuals"></a><span data-ttu-id="5419c-103">Benetako datuak</span><span class="sxs-lookup"><span data-stu-id="5419c-103">Actuals</span></span> 

<span data-ttu-id="5419c-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="5419c-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="5419c-105">Oraingoak proiektu batean burutu den lan kopurua da.</span><span class="sxs-lookup"><span data-stu-id="5419c-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="5419c-106">Denbora eta gastuen sarreren, eta egunkariaren sarreren eta fakturen ondorioz sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="5419c-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="5419c-107">Aldizkari lerroak eta denbora bidaltzea</span><span class="sxs-lookup"><span data-stu-id="5419c-107">Journal lines and time submission</span></span>

<span data-ttu-id="5419c-108">Denbora sartzeari buruzko informazio gehiago lortzeko, ikusi [Denbora sartzeko ikuspegi orokorra](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5419c-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="5419c-109">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="5419c-109">Time and materials</span></span>

<span data-ttu-id="5419c-110">Aurkezten den denbora-sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="5419c-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="5419c-111">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="5419c-111">Fixed price</span></span>

<span data-ttu-id="5419c-112">Prezio finkoa kontratu-lerro batera lotutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kostuaren kutxako liburuaren lerro bat sortzen du.</span><span class="sxs-lookup"><span data-stu-id="5419c-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="5419c-113">Prezio lehenetsia</span><span class="sxs-lookup"><span data-stu-id="5419c-113">Default pricing</span></span>

<span data-ttu-id="5419c-114">Prezio lehenetsiak sortzeko logika kutxako liburuaren lerroan dago.</span><span class="sxs-lookup"><span data-stu-id="5419c-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="5419c-115">Aldi bateko sarrera-eremuko balioak kutxako liburuaren lerroan kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="5419c-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="5419c-116">Balio hauetan daude transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezioen zerrenda egokian.</span><span class="sxs-lookup"><span data-stu-id="5419c-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="5419c-117">Prezio lehenetsiei eragiten dieten eremuak, adibidez **Funtzioa** eta **Organo-unitatea**, kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="5419c-117">The fields that affect default pricing, such as **Role** and **Org Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="5419c-118">Eremu pertsonalizatua gehi dezakezu denbora-sarreran.</span><span class="sxs-lookup"><span data-stu-id="5419c-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="5419c-119">Eremuaren balioa aktualitatera hedatu nahi baduzu, sortu eremua Aktualitateko entitatean eta erabili eremuko mapak eremua kopiatzeko garaian benetako sarrerara.</span><span class="sxs-lookup"><span data-stu-id="5419c-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="5419c-120">Aldizkari lerroak eta oinarrizko gastuen aurkezpena</span><span class="sxs-lookup"><span data-stu-id="5419c-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="5419c-121">Gastuen sarrerari buruzko informazio gehiago lortzeko, ikusi [Gastuen ikuspegi orokorra](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5419c-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="5419c-122">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="5419c-122">Time and materials</span></span>

<span data-ttu-id="5419c-123">Aurkezten den oinarrizko gastuaren sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="5419c-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="5419c-124">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="5419c-124">Fixed price</span></span>

<span data-ttu-id="5419c-125">Prezio finkoa kontratu-lerro batera lotutako proiektu baterako oinarrizko gastuaren sarrera bat bidaltzen denean, sistemak kostuaren kutxako liburuaren lerro bat sortzen du.</span><span class="sxs-lookup"><span data-stu-id="5419c-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="5419c-126">Prezio lehenetsia</span><span class="sxs-lookup"><span data-stu-id="5419c-126">Default pricing</span></span>

<span data-ttu-id="5419c-127">Gastuetarako lehenetsitako prezioak sartzeko logika gastuen kategorian oinarritzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="5419c-128">Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="5419c-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="5419c-129">Hala ere, lehenespenez, prezio gisa ezarritako zenbatekoa gastu aldizkariaren lineetan kostua eta salmentak lehenetsiko dira.</span><span class="sxs-lookup"><span data-stu-id="5419c-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="5419c-130">Gastu-sarreretan unitate bakoitzeko prezioen lehenetsitako kategorien sarrera ez dago erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="5419c-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="5419c-131">Erabili sarreren aldizkariak kostuak erregistratzeko</span><span class="sxs-lookup"><span data-stu-id="5419c-131">Use entry journals to record costs</span></span>

<span data-ttu-id="5419c-132">Aldizkariek kostua edo diru-sarrerak erregistratzen dizkizute material, kuota, denbora, gastu edo zerga transakzio klaseetan.</span><span class="sxs-lookup"><span data-stu-id="5419c-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="5419c-133">Aldizkariak helburu hauetarako erabil daitezke:</span><span class="sxs-lookup"><span data-stu-id="5419c-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="5419c-134">Erregistratu proiektuko materialen eta salmenten benetako datuen kostua.</span><span class="sxs-lookup"><span data-stu-id="5419c-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="5419c-135">Eraman transakzioen benetako datuak beste sistema batetik Microsoft Dynamics 365 Project Operations-era.</span><span class="sxs-lookup"><span data-stu-id="5419c-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="5419c-136">Beste sistema batean gertatu diren kostuak erregistratu.</span><span class="sxs-lookup"><span data-stu-id="5419c-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="5419c-137">Kostu horien artean kontratazio edo azpikontratazio kostuak sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="5419c-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5419c-138">Aplikazioak ez ditu aldizkari lerro mota edo aldizkari lerroan sartutako erlazionatutako prezioak balioztatzen.</span><span class="sxs-lookup"><span data-stu-id="5419c-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="5419c-139">Hori dela eta, egiazkoek proiektuan duten kontabilitate-inpaktuaz guztiz jabetzen den erabiltzaileak soilik erabili beharko lituzke sarrera-aldizkariak egiazkoak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="5419c-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="5419c-140">Aldizkari mota honen eragina dela eta, arretaz aukeratu beharko zenuke nork duen sarbidea aldizkariak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="5419c-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="5419c-141">Erregistratu proiektuen gertaeretan oinarritutako benetako datuak</span><span class="sxs-lookup"><span data-stu-id="5419c-141">Record actuals based on project events</span></span>

<span data-ttu-id="5419c-142">Project Operations-ek proiektu batean gertatzen diren finantza-transakzioak erregistratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="5419c-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="5419c-143">Transakzio hauek honela erregistratzen dira: unekoak.</span><span class="sxs-lookup"><span data-stu-id="5419c-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="5419c-144">Hurrengo tauletan, sortzen diren errealitate mota desberdinak daude, proiektuaren denbora eta materialak, prezio finkoa edo barne proiektua den ala ez, edo aurrez aurreko fasean dagoen ala ez, edo barne-proiektua den.</span><span class="sxs-lookup"><span data-stu-id="5419c-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="5419c-145">Baliabidea proiektuaren kontratazio unitateko antolakuntza unitate bera da</span><span class="sxs-lookup"><span data-stu-id="5419c-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="5419c-146">Gertaera</span><span class="sxs-lookup"><span data-stu-id="5419c-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="5419c-147">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="5419c-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="5419c-148">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="5419c-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="5419c-149">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="5419c-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="5419c-150">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="5419c-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="5419c-151">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="5419c-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="5419c-152">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="5419c-152">Actuals</span></span></th>
<th><span data-ttu-id="5419c-153">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="5419c-153">Transaction currency</span></span></th>
<th><span data-ttu-id="5419c-154">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="5419c-154">Fixed price</span></span></th>
<th><span data-ttu-id="5419c-155">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="5419c-156">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="5419c-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="5419c-157">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="5419c-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-158">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="5419c-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="5419c-159">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="5419c-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="5419c-160">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="5419c-161">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-161">Cost actual</span></span></td>
<td><span data-ttu-id="5419c-162">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-163">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-164">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="5419c-165">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-166">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-167">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="5419c-168">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="5419c-169">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="5419c-170">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-170">Cost actual</span></span></td>
<td><span data-ttu-id="5419c-171">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-172">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-173">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-174">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-175">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-176">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="5419c-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="5419c-177">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-178">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="5419c-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="5419c-179">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="5419c-180">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="5419c-181">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="5419c-182">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-183">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="5419c-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-184">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-185">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-186">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-187">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="5419c-187">Billed sales</span></span></td>
<td><span data-ttu-id="5419c-188">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="5419c-189">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="5419c-190">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="5419c-191">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-192">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-193">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-194">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-195">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-196">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="5419c-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="5419c-197">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-198">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="5419c-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="5419c-199">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="5419c-200">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="5419c-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="5419c-201">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="5419c-202">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="5419c-203">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="5419c-204">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="5419c-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="5419c-205">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-206">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-207">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-208">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="5419c-208">Billed sales</span></span></td>
<td><span data-ttu-id="5419c-209">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="5419c-210">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="5419c-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="5419c-211">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="5419c-212">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-213">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="5419c-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="5419c-214">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-215">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="5419c-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="5419c-216">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="5419c-217">Baliabidea proiektuaren kontratazio unitateko antolakuntza ez da unitate bera da</span><span class="sxs-lookup"><span data-stu-id="5419c-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="5419c-218">Gertaera</span><span class="sxs-lookup"><span data-stu-id="5419c-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="5419c-219">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="5419c-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="5419c-220">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="5419c-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="5419c-221">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="5419c-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="5419c-222">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="5419c-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="5419c-223">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="5419c-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="5419c-224">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="5419c-224">Actuals</span></span></th>
<th><span data-ttu-id="5419c-225">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="5419c-225">Transaction currency</span></span></th>
<th><span data-ttu-id="5419c-226">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="5419c-226">Fixed price</span></span></th>
<th><span data-ttu-id="5419c-227">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="5419c-228">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="5419c-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="5419c-229">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="5419c-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-230">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="5419c-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="5419c-231">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="5419c-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="5419c-232">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="5419c-233">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-233">Cost actual</span></span></td>
<td><span data-ttu-id="5419c-234">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="5419c-235">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="5419c-236">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="5419c-237">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="5419c-238">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-239">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="5419c-240">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-241">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="5419c-242">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-243">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="5419c-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="5419c-244">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="5419c-245">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="5419c-246">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-246">Cost actual</span></span></td>
<td><span data-ttu-id="5419c-247">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-248">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-249">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-250">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-251">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-252">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="5419c-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="5419c-253">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-254">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="5419c-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="5419c-255">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-256">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="5419c-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="5419c-257">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-258">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="5419c-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="5419c-259">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="5419c-260">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="5419c-261">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="5419c-262">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-263">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="5419c-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-264">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-265">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="5419c-266">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-267">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="5419c-267">Billed sales</span></span></td>
<td><span data-ttu-id="5419c-268">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="5419c-269">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="5419c-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="5419c-270">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="5419c-271">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-272">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-273">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-274">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="5419c-275">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-276">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="5419c-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="5419c-277">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-278">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="5419c-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="5419c-279">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="5419c-280">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="5419c-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="5419c-281">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="5419c-282">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="5419c-283">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="5419c-284">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="5419c-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="5419c-285">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-286">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="5419c-287">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="5419c-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-288">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="5419c-288">Billed sales</span></span></td>
<td><span data-ttu-id="5419c-289">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="5419c-290">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="5419c-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="5419c-291">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="5419c-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="5419c-292">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-293">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="5419c-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="5419c-294">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="5419c-295">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="5419c-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="5419c-296">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="5419c-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
