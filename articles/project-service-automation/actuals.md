---
title: Benetakoak
description: Gai honek benetako datuen antolaketari buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748927"
---
# <a name="actuals"></a><span data-ttu-id="e2323-103">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="e2323-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e2323-104">Oraingoak proiektu batean burutu den lan kopurua da.</span><span class="sxs-lookup"><span data-stu-id="e2323-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="e2323-105">Proiektuaren errealitateak jatorrizko dokumentuetara aurki daitezke.</span><span class="sxs-lookup"><span data-stu-id="e2323-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="e2323-106">Jatorri-dokumentu horiek denbora, gastua eta kutxako liburuko idazpen eta fakturak ere barne hartzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="e2323-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![Proiektuen errealitateak nola zuzentzen diren iturri dokumentuetara](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="e2323-108">Bidali denbora-sarrera</span><span class="sxs-lookup"><span data-stu-id="e2323-108">Submitting a time entry</span></span>

<span data-ttu-id="e2323-109">PSAn, denboraren eta materialen kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi aldizkari-lerro sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="e2323-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="e2323-110">Lerro bat kostua da, eta bestea, berriz, fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="e2323-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="e2323-111">Prezio finkoa kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi kutxako liburuaren lerroa sortzen da kostuetarako bakarrik.</span><span class="sxs-lookup"><span data-stu-id="e2323-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="e2323-112">Prezio lehenetsiak sartzeko logika kutxako liburuaren lerroan dago.</span><span class="sxs-lookup"><span data-stu-id="e2323-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="e2323-113">Aldi bateko sarrera-eremuko balio guztiak kutxako liburuaren lerroan kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="e2323-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="e2323-114">Eremu hauetan daude transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezioen zerrenda egokian.</span><span class="sxs-lookup"><span data-stu-id="e2323-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="e2323-115">Prezio lehenetsiei eragiten dieten eremuak, adibidez **Funtzioa** eta **Organo Unitatea**, lehenetsitako kutxako liburuaren linean linean sartu behar izatea.</span><span class="sxs-lookup"><span data-stu-id="e2323-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="e2323-116">Denboraren sarreran eremu pertsonalizatu bat gehitzen baduzu eta eremuaren balioa aktualitatera hedatu nahi baduzu, sortu eremua Aktualitateko entitatean eta erabili eremuko mapak eremua kopiatzeko garaian benetako sarrerara.</span><span class="sxs-lookup"><span data-stu-id="e2323-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="e2323-117">Gastu sarrera aurkeztuz</span><span class="sxs-lookup"><span data-stu-id="e2323-117">Submitting an expense entry</span></span>

<span data-ttu-id="e2323-118">PSAn, gastu eta materialen kontratu-lerro batera mapatutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi aldizkari-lerro sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="e2323-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="e2323-119">Lerro bat kostua da, eta bestea, berriz, fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="e2323-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="e2323-120">Gastua kontratu-lerro batera esleitutako proiektu baterako denbora-sarrera bat bidaltzen denean, bi kutxako liburuaren lerroa sortzen da kostuetarako bakarrik.</span><span class="sxs-lookup"><span data-stu-id="e2323-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="e2323-121">Gastuen prezio lehenetsiak sartzeko logika, hautatutako gastu kategorian oinarritzen da **Sarrera gastua** orria.</span><span class="sxs-lookup"><span data-stu-id="e2323-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="e2323-122">Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="e2323-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="e2323-123">Hala ere, prezioarengatik, erabiltzaileak sartu duen zenbatekoa lehenetsitako gastu aldizkariaren lineetan kostua eta salmentak lehenetsiko dira.</span><span class="sxs-lookup"><span data-stu-id="e2323-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="e2323-124">PSAren gaur egungo bertsioan, gastu sarreretan unitate bakoitzeko prezioen lehenetsitako kategorien sarrera ez dago erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="e2323-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="e2323-125">Aldizkariak erabiltzea kostuak erregistratzeko</span><span class="sxs-lookup"><span data-stu-id="e2323-125">Using journals to record costs</span></span>

<span data-ttu-id="e2323-126">PSAn, aldizkariek kostua edo diru-sarrerak erregistratzen dizkizute material, kuota, denbora, gastu edo zerga transakzio klaseetan.</span><span class="sxs-lookup"><span data-stu-id="e2323-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="e2323-127">Aldizkari batek goiburua, lerroak eta a ditu **Berretsia** ekintza.</span><span class="sxs-lookup"><span data-stu-id="e2323-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="e2323-128">Hona hemen aldizkari bat erabil dezakezuen eszenatoki batzuk:</span><span class="sxs-lookup"><span data-stu-id="e2323-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="e2323-129">Proiektu batean benetako kostuak eta salmentak erregistratu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="e2323-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="e2323-130">Transakzioen egitateak beste sistema batetik PSAra eraman behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="e2323-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="e2323-131">Beste sistema batean gertatu diren kostuak erregistratu behar dituzu, hala nola kontratazioan edo azpikontratazioan.</span><span class="sxs-lookup"><span data-stu-id="e2323-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="e2323-132">Proiektuen gertaeretan oinarritutako errealitateak grabatu</span><span class="sxs-lookup"><span data-stu-id="e2323-132">Recording actuals based on project events</span></span>

<span data-ttu-id="e2323-133">Psak proiektu batean zehar gertatzen diren transakzio-ekonomiko guztiak erregistratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="e2323-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="e2323-134">Transakzio hauek honela erregistratzen dira: **unekoak**.</span><span class="sxs-lookup"><span data-stu-id="e2323-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="e2323-135">Hurrengo tauletan, sortzen diren errealitate mota desberdinak daude, proiektuaren denbora eta materialak, prezio finkoa edo barne proiektua den ala ez, edo aurrez aurreko fasean dagoen ala ez, edo barne-proiektua den.</span><span class="sxs-lookup"><span data-stu-id="e2323-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="e2323-136">**Baliabidea proiektuaren kontratazio unitateko antolakuntza unitate bera da**</span><span class="sxs-lookup"><span data-stu-id="e2323-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="e2323-137">Gertaera</span><span class="sxs-lookup"><span data-stu-id="e2323-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="e2323-138">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="e2323-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="e2323-139">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="e2323-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="e2323-140">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="e2323-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="e2323-141">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="e2323-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="e2323-142">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="e2323-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="e2323-143">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="e2323-143">Actuals</span></span></th>
<th><span data-ttu-id="e2323-144">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="e2323-144">Transaction currency</span></span></th>
<th><span data-ttu-id="e2323-145">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="e2323-145">Fixed price</span></span></th>
<th><span data-ttu-id="e2323-146">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="e2323-147">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="e2323-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="e2323-148">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="e2323-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-149">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="e2323-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="e2323-150">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="e2323-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e2323-151">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e2323-152">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-152">Cost actual</span></span></td>
<td><span data-ttu-id="e2323-153">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-154">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-155">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="e2323-156">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-157">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-158">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="e2323-159">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e2323-160">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e2323-161">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-161">Cost actual</span></span></td>
<td><span data-ttu-id="e2323-162">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-163">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-164">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-165">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-166">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-167">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="e2323-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e2323-168">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-169">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="e2323-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e2323-170">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e2323-171">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e2323-172">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e2323-173">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-174">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="e2323-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-175">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-176">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-177">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-178">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="e2323-178">Billed sales</span></span></td>
<td><span data-ttu-id="e2323-179">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e2323-180">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e2323-181">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e2323-182">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-183">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-184">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-185">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-186">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-187">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="e2323-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e2323-188">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-189">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="e2323-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e2323-190">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e2323-191">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="e2323-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e2323-192">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e2323-193">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="e2323-194">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="e2323-195">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="e2323-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="e2323-196">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-197">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-198">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-199">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="e2323-199">Billed sales</span></span></td>
<td><span data-ttu-id="e2323-200">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e2323-201">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="e2323-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e2323-202">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e2323-203">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-204">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="e2323-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="e2323-205">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-206">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="e2323-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="e2323-207">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="e2323-208">**Baliabidea proiektuaren kontratazio unitateko antolakuntza ez da unitate bera da**</span><span class="sxs-lookup"><span data-stu-id="e2323-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="e2323-209">Gertaera</span><span class="sxs-lookup"><span data-stu-id="e2323-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="e2323-210">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="e2323-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="e2323-211">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="e2323-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="e2323-212">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="e2323-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="e2323-213">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="e2323-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="e2323-214">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="e2323-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="e2323-215">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="e2323-215">Actuals</span></span></th>
<th><span data-ttu-id="e2323-216">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="e2323-216">Transaction currency</span></span></th>
<th><span data-ttu-id="e2323-217">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="e2323-217">Fixed price</span></span></th>
<th><span data-ttu-id="e2323-218">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="e2323-219">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="e2323-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="e2323-220">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="e2323-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-221">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="e2323-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="e2323-222">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="e2323-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="e2323-223">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e2323-224">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-224">Cost actual</span></span></td>
<td><span data-ttu-id="e2323-225">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="e2323-226">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="e2323-227">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="e2323-228">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="e2323-229">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-230">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="e2323-231">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-232">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="e2323-233">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-234">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="e2323-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="e2323-235">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="e2323-236">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e2323-237">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-237">Cost actual</span></span></td>
<td><span data-ttu-id="e2323-238">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-239">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-240">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-241">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-242">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-243">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="e2323-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="e2323-244">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-245">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="e2323-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="e2323-246">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-247">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="e2323-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e2323-248">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-249">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="e2323-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e2323-250">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e2323-251">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e2323-252">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e2323-253">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-254">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="e2323-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-255">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-256">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="e2323-257">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-258">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="e2323-258">Billed sales</span></span></td>
<td><span data-ttu-id="e2323-259">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e2323-260">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="e2323-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e2323-261">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e2323-262">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-263">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-264">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-265">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e2323-266">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-267">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="e2323-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e2323-268">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-269">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="e2323-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e2323-270">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e2323-271">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="e2323-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e2323-272">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e2323-273">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="e2323-274">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="e2323-275">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="e2323-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="e2323-276">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-277">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="e2323-278">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="e2323-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-279">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="e2323-279">Billed sales</span></span></td>
<td><span data-ttu-id="e2323-280">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e2323-281">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="e2323-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e2323-282">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="e2323-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e2323-283">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-284">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="e2323-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="e2323-285">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e2323-286">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="e2323-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="e2323-287">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="e2323-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
