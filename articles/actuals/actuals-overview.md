---
title: Benetako datuak
description: Gai honek Microsoft Dynamics 365 Project Operations-en benetako datuekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 93a945ffbe9c6dd998456b506b95e717ab8fbab7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071026"
---
# <a name="actuals"></a><span data-ttu-id="a1dae-103">Benetako datuak</span><span class="sxs-lookup"><span data-stu-id="a1dae-103">Actuals</span></span> 

<span data-ttu-id="a1dae-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="a1dae-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a1dae-105">Oraingoak proiektu batean burutu den lan kopurua da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="a1dae-106">Denbora eta gastuen sarreren, eta egunkariaren sarreren eta fakturen ondorioz sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="a1dae-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="a1dae-107">Aldizkari lerroak eta denbora bidaltzea</span><span class="sxs-lookup"><span data-stu-id="a1dae-107">Journal lines and time submission</span></span>

<span data-ttu-id="a1dae-108">Denbora sartzeari buruzko informazio gehiago lortzeko, ikusi [Denbora sartzeko ikuspegi orokorra](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="a1dae-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="a1dae-109">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="a1dae-109">Time and materials</span></span>

<span data-ttu-id="a1dae-110">Aurkezten den denbora-sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="a1dae-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="a1dae-111">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="a1dae-111">Fixed price</span></span>

<span data-ttu-id="a1dae-112">Prezio finkoa kontratu-lerro batera lotutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kostuaren kutxako liburuaren lerro bat sortzen du.</span><span class="sxs-lookup"><span data-stu-id="a1dae-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="a1dae-113">Prezio lehenetsia</span><span class="sxs-lookup"><span data-stu-id="a1dae-113">Default pricing</span></span>

<span data-ttu-id="a1dae-114">Prezio lehenetsiak sortzeko logika kutxako liburuaren lerroan dago.</span><span class="sxs-lookup"><span data-stu-id="a1dae-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="a1dae-115">Aldi bateko sarrera-eremuko balioak kutxako liburuaren lerroan kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="a1dae-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="a1dae-116">Balio hauetan daude transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezioen zerrenda egokian.</span><span class="sxs-lookup"><span data-stu-id="a1dae-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="a1dae-117">Prezio lehenetsiei eragiten dieten eremuak, adibidez **Funtzioa** eta **Organo-unitatea** , kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="a1dae-117">The fields that affect default pricing, such as **Role** and **Org Unit** , are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="a1dae-118">Eremu pertsonalizatua gehi dezakezu denbora-sarreran.</span><span class="sxs-lookup"><span data-stu-id="a1dae-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="a1dae-119">Eremuaren balioa aktualitatera hedatu nahi baduzu, sortu eremua Aktualitateko entitatean eta erabili eremuko mapak eremua kopiatzeko garaian benetako sarrerara.</span><span class="sxs-lookup"><span data-stu-id="a1dae-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="a1dae-120">Aldizkari lerroak eta oinarrizko gastuen aurkezpena</span><span class="sxs-lookup"><span data-stu-id="a1dae-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="a1dae-121">Gastuen sarrerari buruzko informazio gehiago lortzeko, ikusi [Gastuen ikuspegi orokorra](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="a1dae-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="a1dae-122">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="a1dae-122">Time and materials</span></span>

<span data-ttu-id="a1dae-123">Aurkezten den oinarrizko gastuaren sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="a1dae-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="a1dae-124">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="a1dae-124">Fixed price</span></span>

<span data-ttu-id="a1dae-125">Prezio finkoa kontratu-lerro batera lotutako proiektu baterako oinarrizko gastuaren sarrera bat bidaltzen denean, sistemak kostuaren kutxako liburuaren lerro bat sortzen du.</span><span class="sxs-lookup"><span data-stu-id="a1dae-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="a1dae-126">Prezio lehenetsia</span><span class="sxs-lookup"><span data-stu-id="a1dae-126">Default pricing</span></span>

<span data-ttu-id="a1dae-127">Gastuetarako lehenetsitako prezioak sartzeko logika gastuen kategorian oinarritzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="a1dae-128">Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="a1dae-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="a1dae-129">Hala ere, lehenespenez, prezio gisa ezarritako zenbatekoa gastu aldizkariaren lineetan kostua eta salmentak lehenetsiko dira.</span><span class="sxs-lookup"><span data-stu-id="a1dae-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="a1dae-130">Gastu-sarreretan unitate bakoitzeko prezioen lehenetsitako kategorien sarrera ez dago erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="a1dae-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="a1dae-131">Erabili sarreren aldizkariak kostuak erregistratzeko</span><span class="sxs-lookup"><span data-stu-id="a1dae-131">Use entry journals to record costs</span></span>

<span data-ttu-id="a1dae-132">Aldizkariek kostua edo diru-sarrerak erregistratzen dizkizute material, kuota, denbora, gastu edo zerga transakzio klaseetan.</span><span class="sxs-lookup"><span data-stu-id="a1dae-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="a1dae-133">Aldizkariak helburu hauetarako erabil daitezke:</span><span class="sxs-lookup"><span data-stu-id="a1dae-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="a1dae-134">Erregistratu proiektuko materialen eta salmenten benetako datuen kostua.</span><span class="sxs-lookup"><span data-stu-id="a1dae-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="a1dae-135">Eraman transakzioen benetako datuak beste sistema batetik Microsoft Dynamics 365 Project Operations-era.</span><span class="sxs-lookup"><span data-stu-id="a1dae-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="a1dae-136">Beste sistema batean gertatu diren kostuak erregistratu.</span><span class="sxs-lookup"><span data-stu-id="a1dae-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="a1dae-137">Kostu horien artean kontratazio edo azpikontratazio kostuak sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="a1dae-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a1dae-138">Aplikazioak ez ditu aldizkari lerro mota edo aldizkari lerroan sartutako erlazionatutako prezioak balioztatzen.</span><span class="sxs-lookup"><span data-stu-id="a1dae-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="a1dae-139">Hori dela eta, egiazkoek proiektuan duten kontabilitate-inpaktuaz guztiz jabetzen den erabiltzaileak soilik erabili beharko lituzke sarrera-aldizkariak egiazkoak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="a1dae-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="a1dae-140">Aldizkari mota honen eragina dela eta, arretaz aukeratu beharko zenuke nork duen sarbidea aldizkariak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="a1dae-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="a1dae-141">Erregistratu proiektuen gertaeretan oinarritutako benetako datuak</span><span class="sxs-lookup"><span data-stu-id="a1dae-141">Record actuals based on project events</span></span>

<span data-ttu-id="a1dae-142">Project Operations-ek proiektu batean gertatzen diren finantza-transakzioak erregistratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="a1dae-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="a1dae-143">Transakzio hauek honela erregistratzen dira: unekoak.</span><span class="sxs-lookup"><span data-stu-id="a1dae-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="a1dae-144">Hurrengo tauletan, sortzen diren errealitate mota desberdinak daude, proiektuaren denbora eta materialak, prezio finkoa edo barne proiektua den ala ez, edo aurrez aurreko fasean dagoen ala ez, edo barne-proiektua den.</span><span class="sxs-lookup"><span data-stu-id="a1dae-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="a1dae-145">Baliabidea proiektuaren kontratazio unitateko antolakuntza unitate bera da</span><span class="sxs-lookup"><span data-stu-id="a1dae-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="a1dae-146">Gertaera</span><span class="sxs-lookup"><span data-stu-id="a1dae-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="a1dae-147">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="a1dae-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="a1dae-148">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="a1dae-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="a1dae-149">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="a1dae-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="a1dae-150">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="a1dae-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="a1dae-151">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="a1dae-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="a1dae-152">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="a1dae-152">Actuals</span></span></th>
<th><span data-ttu-id="a1dae-153">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="a1dae-153">Transaction currency</span></span></th>
<th><span data-ttu-id="a1dae-154">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="a1dae-154">Fixed price</span></span></th>
<th><span data-ttu-id="a1dae-155">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="a1dae-156">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="a1dae-157">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="a1dae-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-158">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="a1dae-159">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="a1dae-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="a1dae-160">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="a1dae-161">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-161">Cost actual</span></span></td>
<td><span data-ttu-id="a1dae-162">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-163">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-164">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="a1dae-165">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-166">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-167">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="a1dae-168">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="a1dae-169">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="a1dae-170">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-170">Cost actual</span></span></td>
<td><span data-ttu-id="a1dae-171">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-172">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-173">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-174">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-175">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-176">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="a1dae-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="a1dae-177">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-178">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="a1dae-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="a1dae-179">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="a1dae-180">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="a1dae-181">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="a1dae-182">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-183">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="a1dae-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-184">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-185">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-186">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-187">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="a1dae-187">Billed sales</span></span></td>
<td><span data-ttu-id="a1dae-188">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="a1dae-189">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="a1dae-190">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="a1dae-191">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-192">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-193">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-194">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-195">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-196">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="a1dae-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="a1dae-197">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-198">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="a1dae-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="a1dae-199">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="a1dae-200">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="a1dae-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="a1dae-201">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="a1dae-202">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="a1dae-203">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="a1dae-204">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="a1dae-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="a1dae-205">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-206">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-207">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-208">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="a1dae-208">Billed sales</span></span></td>
<td><span data-ttu-id="a1dae-209">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="a1dae-210">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="a1dae-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="a1dae-211">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="a1dae-212">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-213">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="a1dae-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="a1dae-214">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-215">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="a1dae-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="a1dae-216">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="a1dae-217">Baliabidea proiektuaren kontratazio unitateko antolakuntza ez da unitate bera da</span><span class="sxs-lookup"><span data-stu-id="a1dae-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="a1dae-218">Gertaera</span><span class="sxs-lookup"><span data-stu-id="a1dae-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="a1dae-219">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="a1dae-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="a1dae-220">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="a1dae-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="a1dae-221">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="a1dae-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="a1dae-222">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="a1dae-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="a1dae-223">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="a1dae-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="a1dae-224">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="a1dae-224">Actuals</span></span></th>
<th><span data-ttu-id="a1dae-225">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="a1dae-225">Transaction currency</span></span></th>
<th><span data-ttu-id="a1dae-226">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="a1dae-226">Fixed price</span></span></th>
<th><span data-ttu-id="a1dae-227">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="a1dae-228">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="a1dae-229">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="a1dae-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-230">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="a1dae-231">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="a1dae-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="a1dae-232">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="a1dae-233">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-233">Cost actual</span></span></td>
<td><span data-ttu-id="a1dae-234">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="a1dae-235">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="a1dae-236">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="a1dae-237">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="a1dae-238">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-239">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="a1dae-240">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-241">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="a1dae-242">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-243">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="a1dae-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="a1dae-244">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="a1dae-245">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="a1dae-246">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-246">Cost actual</span></span></td>
<td><span data-ttu-id="a1dae-247">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-248">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-249">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-250">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-251">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-252">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="a1dae-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="a1dae-253">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-254">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="a1dae-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="a1dae-255">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-256">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="a1dae-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="a1dae-257">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-258">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="a1dae-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="a1dae-259">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="a1dae-260">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="a1dae-261">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="a1dae-262">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-263">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="a1dae-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-264">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-265">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="a1dae-266">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-267">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="a1dae-267">Billed sales</span></span></td>
<td><span data-ttu-id="a1dae-268">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="a1dae-269">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="a1dae-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="a1dae-270">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="a1dae-271">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-272">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-273">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-274">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="a1dae-275">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-276">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="a1dae-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="a1dae-277">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-278">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="a1dae-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="a1dae-279">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="a1dae-280">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="a1dae-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="a1dae-281">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="a1dae-282">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="a1dae-283">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="a1dae-284">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="a1dae-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="a1dae-285">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-286">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="a1dae-287">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="a1dae-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-288">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="a1dae-288">Billed sales</span></span></td>
<td><span data-ttu-id="a1dae-289">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="a1dae-290">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="a1dae-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="a1dae-291">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="a1dae-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="a1dae-292">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-293">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="a1dae-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="a1dae-294">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="a1dae-295">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="a1dae-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="a1dae-296">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="a1dae-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
