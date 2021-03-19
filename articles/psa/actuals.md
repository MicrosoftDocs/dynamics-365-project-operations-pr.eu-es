---
title: Benetako datuen ikuspegi orokorra
description: Gai honek benetako datuen antolaketari buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c4a3424bed704243dfb5524fa541c3fcc0899e57
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285603"
---
# <a name="actuals-overview"></a><span data-ttu-id="69dfb-103">Benetako datuen ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="69dfb-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="69dfb-104">Oraingoak proiektu batean burutu den lan kopurua da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="69dfb-105">Proiektuaren errealitateak jatorrizko dokumentuetara aurki daitezke.</span><span class="sxs-lookup"><span data-stu-id="69dfb-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="69dfb-106">Jatorri-dokumentu horiek denbora, gastua eta kutxako liburuko idazpen eta fakturak ere barne hartzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="69dfb-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Proiektuen errealitateak nola zuzentzen diren iturri dokumentuetara](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="69dfb-108">Bidali denbora-sarrera</span><span class="sxs-lookup"><span data-stu-id="69dfb-108">Submitting a time entry</span></span>

<span data-ttu-id="69dfb-109">PSAn, denboraren eta materialen kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi aldizkari-lerro sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="69dfb-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="69dfb-110">Lerro bat kostua da, eta bestea, berriz, fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="69dfb-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="69dfb-111">Prezio finkoa kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi kutxako liburuaren lerroa sortzen da kostuetarako bakarrik.</span><span class="sxs-lookup"><span data-stu-id="69dfb-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="69dfb-112">Prezio lehenetsiak sartzeko logika kutxako liburuaren lerroan dago.</span><span class="sxs-lookup"><span data-stu-id="69dfb-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="69dfb-113">Aldi bateko sarrera-eremuko balio guztiak kutxako liburuaren lerroan kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="69dfb-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="69dfb-114">Eremu hauetan daude transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezioen zerrenda egokian.</span><span class="sxs-lookup"><span data-stu-id="69dfb-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="69dfb-115">Prezio lehenetsiei eragiten dieten eremuak, adibidez **Funtzioa** eta **Organo Unitatea**, lehenetsitako kutxako liburuaren linean linean sartu behar izatea.</span><span class="sxs-lookup"><span data-stu-id="69dfb-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="69dfb-116">Denboraren sarreran eremu pertsonalizatu bat gehitzen baduzu eta eremuaren balioa aktualitatera hedatu nahi baduzu, sortu eremua Aktualitateko entitatean eta erabili eremuko mapak eremua kopiatzeko garaian benetako sarrerara.</span><span class="sxs-lookup"><span data-stu-id="69dfb-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="69dfb-117">Gastu sarrera aurkeztuz</span><span class="sxs-lookup"><span data-stu-id="69dfb-117">Submitting an expense entry</span></span>

<span data-ttu-id="69dfb-118">PSAn, gastu eta materialen kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi aldizkari-lerro sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="69dfb-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="69dfb-119">Lerro bat kostua da, eta bestea, berriz, fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="69dfb-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="69dfb-120">Gastua kontratu-lerro batera esleitutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi kutxako liburuaren lerroa sortzen da kostuetarako bakarrik.</span><span class="sxs-lookup"><span data-stu-id="69dfb-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="69dfb-121">Gastuen prezio lehenetsiak sartzeko logika, hautatutako gastu kategorian oinarritzen da **Sarrera gastua** orria.</span><span class="sxs-lookup"><span data-stu-id="69dfb-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="69dfb-122">Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="69dfb-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="69dfb-123">Hala ere, prezioarengatik, erabiltzaileak sartu duen zenbatekoa lehenetsitako gastu aldizkariaren lineetan kostua eta salmentak lehenetsiko dira.</span><span class="sxs-lookup"><span data-stu-id="69dfb-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="69dfb-124">PSAren gaur egungo bertsioan, gastu sarreretan unitate bakoitzeko prezioen lehenetsitako kategorien sarrera ez dago erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="69dfb-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="69dfb-125">Sarrerako aldizkariak erabiltzea kostuak erregistratzeko</span><span class="sxs-lookup"><span data-stu-id="69dfb-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="69dfb-126">PSAn, sarrerako aldizkariek kostua edo diru-sarrerak erregistratzen dizkizute material, kuota, denbora, gastu edo zerga transakzio klaseetan.</span><span class="sxs-lookup"><span data-stu-id="69dfb-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="69dfb-127">Aldizkari batek goiburua, lerroak eta a ditu **Berretsia** ekintza.</span><span class="sxs-lookup"><span data-stu-id="69dfb-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="69dfb-128">Hona hemen aldizkari bat erabil dezakezuen eszenatoki batzuk:</span><span class="sxs-lookup"><span data-stu-id="69dfb-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="69dfb-129">Proiektu batean benetako kostuak eta salmentak erregistratu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="69dfb-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="69dfb-130">Transakzioen egitateak beste sistema batetik PSAra eraman behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="69dfb-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="69dfb-131">Beste sistema batean gertatu diren kostuak erregistratu behar dituzu, hala nola kontratazioan edo azpikontratazioan.</span><span class="sxs-lookup"><span data-stu-id="69dfb-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="69dfb-132">Egunkariak sarrerako aldizkariak erabiltzea benetan proiektuan izan dezakeen eraginaz jabetzen den erabiltzaile batek bakarrik egin beharko du.</span><span class="sxs-lookup"><span data-stu-id="69dfb-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="69dfb-133">Izan ere, aplikazioak ez du aldizkari-lerro mota balioztatzen edo aldizkari-lerroan sartzen diren prezioak.</span><span class="sxs-lookup"><span data-stu-id="69dfb-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="69dfb-134">Aldizkari mota honen eragina dela eta, kontuz ibili behar da sarbidea nori sarbidea ematen dion.</span><span class="sxs-lookup"><span data-stu-id="69dfb-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="69dfb-135">Proiektuen gertaeretan oinarritutako errealitateak grabatu</span><span class="sxs-lookup"><span data-stu-id="69dfb-135">Recording actuals based on project events</span></span>

<span data-ttu-id="69dfb-136">Psak proiektu batean zehar gertatzen diren transakzio-ekonomiko guztiak erregistratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="69dfb-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="69dfb-137">Transakzio hauek honela erregistratzen dira: **unekoak**.</span><span class="sxs-lookup"><span data-stu-id="69dfb-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="69dfb-138">Hurrengo tauletan, sortzen diren errealitate mota desberdinak daude, proiektuaren denbora eta materialak, prezio finkoa edo barne proiektua den ala ez, edo aurrez aurreko fasean dagoen ala ez, edo barne-proiektua den.</span><span class="sxs-lookup"><span data-stu-id="69dfb-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="69dfb-139">**Baliabidea proiektuaren kontratazio unitateko antolakuntza unitate bera da**</span><span class="sxs-lookup"><span data-stu-id="69dfb-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="69dfb-140">Gertaera</span><span class="sxs-lookup"><span data-stu-id="69dfb-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="69dfb-141">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="69dfb-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="69dfb-142">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="69dfb-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="69dfb-143">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="69dfb-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="69dfb-144">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="69dfb-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="69dfb-145">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="69dfb-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="69dfb-146">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="69dfb-146">Actuals</span></span></th>
<th><span data-ttu-id="69dfb-147">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="69dfb-147">Transaction currency</span></span></th>
<th><span data-ttu-id="69dfb-148">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="69dfb-148">Fixed price</span></span></th>
<th><span data-ttu-id="69dfb-149">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="69dfb-150">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="69dfb-151">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="69dfb-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-152">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="69dfb-153">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="69dfb-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="69dfb-154">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="69dfb-155">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-155">Cost actual</span></span></td>
<td><span data-ttu-id="69dfb-156">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-157">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-158">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="69dfb-159">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-160">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-161">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="69dfb-162">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="69dfb-163">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="69dfb-164">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-164">Cost actual</span></span></td>
<td><span data-ttu-id="69dfb-165">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-166">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-167">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-168">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-169">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-170">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="69dfb-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="69dfb-171">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-172">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="69dfb-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="69dfb-173">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="69dfb-174">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="69dfb-175">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="69dfb-176">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-177">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="69dfb-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-178">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-179">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-180">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-181">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="69dfb-181">Billed sales</span></span></td>
<td><span data-ttu-id="69dfb-182">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="69dfb-183">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="69dfb-184">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="69dfb-185">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-186">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-187">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-188">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-189">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-190">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="69dfb-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="69dfb-191">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-192">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="69dfb-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="69dfb-193">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="69dfb-194">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="69dfb-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="69dfb-195">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="69dfb-196">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="69dfb-197">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="69dfb-198">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="69dfb-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="69dfb-199">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-200">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-201">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-202">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="69dfb-202">Billed sales</span></span></td>
<td><span data-ttu-id="69dfb-203">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="69dfb-204">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="69dfb-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="69dfb-205">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="69dfb-206">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-207">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="69dfb-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="69dfb-208">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-209">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="69dfb-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="69dfb-210">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="69dfb-211">**Baliabidea proiektuaren kontratazio unitateko antolakuntza ez da unitate bera da**</span><span class="sxs-lookup"><span data-stu-id="69dfb-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="69dfb-212">Gertaera</span><span class="sxs-lookup"><span data-stu-id="69dfb-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="69dfb-213">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="69dfb-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="69dfb-214">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="69dfb-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="69dfb-215">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="69dfb-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="69dfb-216">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="69dfb-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="69dfb-217">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="69dfb-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="69dfb-218">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="69dfb-218">Actuals</span></span></th>
<th><span data-ttu-id="69dfb-219">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="69dfb-219">Transaction currency</span></span></th>
<th><span data-ttu-id="69dfb-220">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="69dfb-220">Fixed price</span></span></th>
<th><span data-ttu-id="69dfb-221">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="69dfb-222">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="69dfb-223">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="69dfb-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-224">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="69dfb-225">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="69dfb-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="69dfb-226">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="69dfb-227">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-227">Cost actual</span></span></td>
<td><span data-ttu-id="69dfb-228">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="69dfb-229">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="69dfb-230">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="69dfb-231">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="69dfb-232">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-233">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="69dfb-234">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-235">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="69dfb-236">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-237">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="69dfb-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="69dfb-238">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="69dfb-239">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="69dfb-240">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-240">Cost actual</span></span></td>
<td><span data-ttu-id="69dfb-241">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-242">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-243">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-244">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-245">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-246">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="69dfb-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="69dfb-247">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-248">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="69dfb-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="69dfb-249">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-250">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="69dfb-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="69dfb-251">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-252">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="69dfb-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="69dfb-253">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="69dfb-254">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="69dfb-255">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="69dfb-256">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-257">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="69dfb-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-258">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-259">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="69dfb-260">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-261">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="69dfb-261">Billed sales</span></span></td>
<td><span data-ttu-id="69dfb-262">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="69dfb-263">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="69dfb-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="69dfb-264">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="69dfb-265">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-266">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-267">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-268">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="69dfb-269">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-270">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="69dfb-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="69dfb-271">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-272">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="69dfb-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="69dfb-273">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="69dfb-274">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="69dfb-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="69dfb-275">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="69dfb-276">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="69dfb-277">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="69dfb-278">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="69dfb-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="69dfb-279">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-280">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="69dfb-281">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="69dfb-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-282">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="69dfb-282">Billed sales</span></span></td>
<td><span data-ttu-id="69dfb-283">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="69dfb-284">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="69dfb-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="69dfb-285">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="69dfb-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="69dfb-286">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-287">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="69dfb-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="69dfb-288">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="69dfb-289">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="69dfb-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="69dfb-290">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="69dfb-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]