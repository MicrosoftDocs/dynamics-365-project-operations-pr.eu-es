---
title: Benetako datuak
description: Gai honek Microsoft Dynamics 365 Project Operations-en errealitateekin lan egiteko moduari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 78c7a9486d0338adfd7770447f21d17509e654f7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996596"
---
# <a name="actuals"></a><span data-ttu-id="ed5f7-103">Benetako datuak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-103">Actuals</span></span> 

<span data-ttu-id="ed5f7-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="ed5f7-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ed5f7-105">Eguneratzeek proiektu batean berrikusitako eta onartutako finantza eta egutegia adierazten dute.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="ed5f7-106">Denbora, gastua, materialaren erabileraren sarrerak eta egunkarietako sarrerak eta fakturak onartzearen ondorioz sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="ed5f7-107">Aldizkari lerroak eta denbora bidaltzea</span><span class="sxs-lookup"><span data-stu-id="ed5f7-107">Journal lines and time submission</span></span>

<span data-ttu-id="ed5f7-108">Denbora sartzeari buruzko informazio gehiago lortzeko, ikusi [Denbora sartzeko ikuspegi orokorra](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="ed5f7-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="ed5f7-109">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-109">Time and materials</span></span>

<span data-ttu-id="ed5f7-110">Aurkezten den denbora-sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="ed5f7-111">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-111">Fixed price</span></span>

<span data-ttu-id="ed5f7-112">Prezio finkoa kontratu-lerro batera lotutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kostuaren kutxako liburuaren lerro bat sortzen du.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="ed5f7-113">Prezio lehenetsia</span><span class="sxs-lookup"><span data-stu-id="ed5f7-113">Default pricing</span></span>

<span data-ttu-id="ed5f7-114">Prezio lehenetsiak sortzeko logika kutxako liburuaren lerroan dago.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="ed5f7-115">Aldi bateko sarrera-eremuko balioak kutxako liburuaren lerroan kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="ed5f7-116">Balio hauetan daude transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezioen zerrenda egokian.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="ed5f7-117">Prezio lehenetsiei eragiten dieten eremuak, adibidez **Funtzioa** eta **Baliabide-unitatea**, kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="ed5f7-118">Eremu pertsonalizatua gehi dezakezu denbora-sarreran.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="ed5f7-119">Eremuaren balioa benetakoetara hedatzea nahi baduzu, sortu eremua **Benetako datuak** eta **Kutxako liburuaren lerroa** taulak.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="ed5f7-120">Erabili kode pertsonalizatua hautatutako eremuaren balioa Denbora-sarreratik Eguneraino aldizkariaren lerroaren bidez transakzio-jatorriak erabiliz hedatzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="ed5f7-121">Transakzioen jatorriari eta konexioei buruzko informazio gehiago lortzeko, ikusi [Benetakoak jatorrizko erregistroekin lotzea](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="ed5f7-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="ed5f7-122">Aldizkari lerroak eta oinarrizko gastuen aurkezpena</span><span class="sxs-lookup"><span data-stu-id="ed5f7-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="ed5f7-123">Gastuen sarrerari buruzko informazio gehiago lortzeko, ikusi [Gastuen ikuspegi orokorra](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="ed5f7-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="ed5f7-124">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-124">Time and materials</span></span>

<span data-ttu-id="ed5f7-125">Aurkezten den oinarrizko gastuaren sarrera bat denbora eta materialen kontratu-lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak bi aldizkari-lerro sortzen ditu, bata kosturako eta bestea fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="ed5f7-126">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-126">Fixed price</span></span>

<span data-ttu-id="ed5f7-127">Bidalitako oinarrizko gastua kontratu-lerro batera esleitutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kutxako liburuaren lerro bat sortzen du kostuetarako.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="ed5f7-128">Prezio lehenetsia</span><span class="sxs-lookup"><span data-stu-id="ed5f7-128">Default pricing</span></span>

<span data-ttu-id="ed5f7-129">Gastuetarako lehenetsitako prezioak sartzeko logika gastuen kategorian oinarritzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="ed5f7-130">Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="ed5f7-131">Prezio lehenetsiei eragiten dieten eremuak, adibidez **Transakzioaren kategoria** eta **Unitatea**, kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="ed5f7-132">Hala ere, honek prezioen zerrendako prezioen metodoa dagoenean bakarrik funtzionatzen du **Unitateko prezioa**.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="ed5f7-133">Prezioen metodoa bada **Kostuan** edo **Markaketa kostuaren gainetik**, gastu sarrera sortzerakoan sartutako prezioa kosturako erabiltzen da eta salmenta egunkariaren lerroan prezioa prezio metodoaren arabera kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="ed5f7-134">Gastu sarreran eremu pertsonalizatua gehi dezakezu.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="ed5f7-135">Eremuaren balioa benetakoetara hedatzea nahi baduzu, sortu eremua **Benetako datuak** eta **Kutxako liburuaren lerroa** taulak.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="ed5f7-136">Erabili kode pertsonalizatua hautatutako eremuaren balioa Denbora-sarreratik Eguneraino aldizkariaren lerroaren bidez transakzio-jatorriak erabiliz hedatzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="ed5f7-137">Transakzioen jatorriari eta konexioei buruzko informazio gehiago lortzeko, ikusi [Benetakoak jatorrizko erregistroekin lotzea](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="ed5f7-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="ed5f7-138">Aldizkari lerroak eta materialaren erabilera erregistroa bidaltzea</span><span class="sxs-lookup"><span data-stu-id="ed5f7-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="ed5f7-139">Gastuen sarrerari buruzko informazio gehiago lortzeko, ikusi [Materialaren erabilera erregistroa](../material/material-usage-log.md).</span><span class="sxs-lookup"><span data-stu-id="ed5f7-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="ed5f7-140">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-140">Time and materials</span></span>

<span data-ttu-id="ed5f7-141">Aurkeztutako materialaren erabilera erregistroaren sarrera denbora eta materialen kontratu lerro batera mapatuta dagoen proiektuarekin lotzen denean, sistemak aldizkari lerro bi sortzen ditu, bata kostuarena eta bestea fakturatu gabeko salmentetarako.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="ed5f7-142">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-142">Fixed price</span></span>

<span data-ttu-id="ed5f7-143">Bidalitako materialaren erabilera-erregistroaren sarrera kontratu-lerro batera esleitutako proiektu baterako denbora-sarrera bat bidaltzen denean, sistemak kutxako liburuaren lerro bat sortzen du kostuetarako.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="ed5f7-144">Prezio lehenetsia</span><span class="sxs-lookup"><span data-stu-id="ed5f7-144">Default pricing</span></span>

<span data-ttu-id="ed5f7-145">Materialaren prezio lehenetsiak sartzeko logika produktuaren eta unitateen konbinazioan oinarritzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="ed5f7-146">Transakzioaren data, proiektua esleitu duen kontratuaren lerroa eta dibisaren emaitza prezio-zerrenda egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="ed5f7-147">Prezio lehenetsiei eragiten dieten eremuak, adibidez **Produktuaren IDa** eta **Unitatea**, kutxako liburuaren lerroko prezio egokia zehazteko erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="ed5f7-148">Hala ere, katalogoko produktuetarako bakarrik funtzionatzen du.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-148">However, this only works for catalog products.</span></span> <span data-ttu-id="ed5f7-149">Idatzi produktuetan, materialaren erabilera erregistroa sortzen denean sartutako prezioa aldizkari lerroetako kostu eta salmenta preziorako erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="ed5f7-150">**Materialaren erabilera-erregistroa** sarreran eremu pertsonalizatua gehi dezakezu.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="ed5f7-151">Eremuaren balioa benetakoetara hedatzea nahi baduzu, sortu eremua **Benetako datuak** eta **Kutxako liburuaren lerroa** taulak.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="ed5f7-152">Erabili kode pertsonalizatua hautatutako eremuaren balioa Denbora-sarreratik Eguneraino aldizkariaren lerroaren bidez transakzio-jatorriak erabiliz hedatzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="ed5f7-153">Transakzioen jatorriari eta konexioei buruzko informazio gehiago lortzeko, ikusi [Benetakoak jatorrizko erregistroekin lotzea](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="ed5f7-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="ed5f7-154">Erabili sarreren aldizkariak kostuak erregistratzeko</span><span class="sxs-lookup"><span data-stu-id="ed5f7-154">Use entry journals to record costs</span></span>

<span data-ttu-id="ed5f7-155">Aldizkariek kostua edo diru-sarrerak erregistratzen dizkizute material, kuota, denbora, gastu edo zerga transakzio klaseetan.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="ed5f7-156">Aldizkariak helburu hauetarako erabil daitezke:</span><span class="sxs-lookup"><span data-stu-id="ed5f7-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="ed5f7-157">Eraman transakzioen egitateak beste sistema batetik Microsoft Dynamics 365 Project Operations-era.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="ed5f7-158">Beste sistema batean gertatu diren kostuak erregistratu.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="ed5f7-159">Kostu horien artean kontratazio edo azpikontratazio kostuak sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ed5f7-160">Aplikazioak ez ditu aldizkari lerro mota edo aldizkari lerroan sartutako erlazionatutako prezioak balioztatzen.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="ed5f7-161">Hori dela eta, egiazkoek proiektuan duten kontabilitate-inpaktuaz guztiz jabetzen den erabiltzaileak soilik erabili beharko lituzke sarrera-aldizkariak egiazkoak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="ed5f7-162">Aldizkari mota honen eragina dela eta, arretaz aukeratu beharko zenuke nork duen sarbidea aldizkariak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="ed5f7-163">Erregistratu proiektuen gertaeretan oinarritutako benetako datuak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-163">Record actuals based on project events</span></span>

<span data-ttu-id="ed5f7-164">Project Operations-ek proiektu batean gertatzen diren finantza-transakzioak erregistratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="ed5f7-165">Transakzio hauek honela erregistratzen dira: unekoak.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="ed5f7-166">Hurrengo tauletan, sortzen diren errealitate mota desberdinak daude, proiektuaren denbora eta materialak, prezio finkoa edo barne proiektua den ala ez, edo aurrez aurreko fasean dagoen ala ez, edo barne-proiektua den.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="ed5f7-167">Baliabidea proiektuaren kontratazio unitateko antolakuntza unitate bera da</span><span class="sxs-lookup"><span data-stu-id="ed5f7-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ed5f7-168">Gertaera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ed5f7-169">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="ed5f7-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ed5f7-170">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="ed5f7-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ed5f7-171">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ed5f7-172">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ed5f7-173">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ed5f7-174">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-174">Actuals</span></span></th>
<th><span data-ttu-id="ed5f7-175">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="ed5f7-175">Transaction currency</span></span></th>
<th><span data-ttu-id="ed5f7-176">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-176">Fixed price</span></span></th>
<th><span data-ttu-id="ed5f7-177">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ed5f7-178">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ed5f7-179">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="ed5f7-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-180">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ed5f7-181">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="ed5f7-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ed5f7-182">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ed5f7-183">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-183">Cost actual</span></span></td>
<td><span data-ttu-id="ed5f7-184">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-185">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-186">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="ed5f7-187">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-188">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-189">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ed5f7-190">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ed5f7-191">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ed5f7-192">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-192">Cost actual</span></span></td>
<td><span data-ttu-id="ed5f7-193">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-194">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-195">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-196">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-197">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-198">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ed5f7-199">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-200">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ed5f7-201">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ed5f7-202">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ed5f7-203">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ed5f7-204">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-205">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-206">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-207">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-208">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-209">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-209">Billed sales</span></span></td>
<td><span data-ttu-id="ed5f7-210">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ed5f7-211">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ed5f7-212">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ed5f7-213">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-214">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-215">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-216">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-217">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-218">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ed5f7-219">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-220">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ed5f7-221">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ed5f7-222">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ed5f7-223">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ed5f7-224">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ed5f7-225">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ed5f7-226">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="ed5f7-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ed5f7-227">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-228">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-229">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-230">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-230">Billed sales</span></span></td>
<td><span data-ttu-id="ed5f7-231">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ed5f7-232">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ed5f7-233">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ed5f7-234">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-235">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ed5f7-236">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-237">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ed5f7-238">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="ed5f7-239">Baliabidea proiektuaren kontratazio unitateko antolakuntza ez da unitate bera da</span><span class="sxs-lookup"><span data-stu-id="ed5f7-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ed5f7-240">Gertaera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ed5f7-241">Proiektu fakultagarria edo saldu</span><span class="sxs-lookup"><span data-stu-id="ed5f7-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ed5f7-242">Proiektua presazko etapan</span><span class="sxs-lookup"><span data-stu-id="ed5f7-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ed5f7-243">Barne proiektua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ed5f7-244">Denbora eta materialak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ed5f7-245">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ed5f7-246">Benetakoak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-246">Actuals</span></span></th>
<th><span data-ttu-id="ed5f7-247">Transakzio-moneta</span><span class="sxs-lookup"><span data-stu-id="ed5f7-247">Transaction currency</span></span></th>
<th><span data-ttu-id="ed5f7-248">Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-248">Fixed price</span></span></th>
<th><span data-ttu-id="ed5f7-249">Transakzio-dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ed5f7-250">Denbora-sarrera bat sortu da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ed5f7-251">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="ed5f7-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-252">Denbora-sarrera bat bidali da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ed5f7-253">Ez dago jarduerarik Aktiboen entitatean</span><span class="sxs-lookup"><span data-stu-id="ed5f7-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="ed5f7-254">Ordua onartzen da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ed5f7-255">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-255">Cost actual</span></span></td>
<td><span data-ttu-id="ed5f7-256">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ed5f7-257">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ed5f7-258">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ed5f7-259">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ed5f7-260">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-261">Fakturatu gabeko salmenten benetako zenbatekoa - Kargagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ed5f7-262">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-263">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ed5f7-264">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-265">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ed5f7-266">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="ed5f7-267">Ordua onartzen da eta ez da igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ed5f7-268">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-268">Cost actual</span></span></td>
<td><span data-ttu-id="ed5f7-269">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-270">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-271">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-272">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-273">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-274">Baliabidearen unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="ed5f7-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ed5f7-275">Baliabidearen unitate-dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-276">Erakunde arteko salmentak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ed5f7-277">Kontratatzailearen unitatearen dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-278">Fakturatu gabeko salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ed5f7-279">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-280">Fakturatu gabeko salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ed5f7-281">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ed5f7-282">Faktura berresten da eta ez da aldaketarik edo igoerarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ed5f7-283">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ed5f7-284">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-285">Mugarriko salmenta fakturatuak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-286">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-287">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ed5f7-288">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-289">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-289">Billed sales</span></span></td>
<td><span data-ttu-id="ed5f7-290">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ed5f7-291">Faktura berresten da eta ez jeitsierarik fakturazio orduetan onartzen da.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ed5f7-292">Fakturatu gabeko salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ed5f7-293">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-294">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-295">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-296">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ed5f7-297">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-298">Fakturatutako salmenten benetako kopurua - Kargagarria kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ed5f7-299">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-300">Fakturatutako salmenten benetako kopurua: ez da kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ed5f7-301">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ed5f7-302">Faktura zuzentzen da kargatu beharreko kantitatea handitzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ed5f7-303">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ed5f7-304">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ed5f7-305">Mugarriko salmenta itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ed5f7-306">Mugarri-egoera aldatu da <strong>Fakturatutakoa</strong> egoeratik <strong>Faktura egiteko prest</strong> egoerara</span><span class="sxs-lookup"><span data-stu-id="ed5f7-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ed5f7-307">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-308">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ed5f7-309">Ez da aplikagarria</span><span class="sxs-lookup"><span data-stu-id="ed5f7-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-310">Fakturatutako salmentak</span><span class="sxs-lookup"><span data-stu-id="ed5f7-310">Billed sales</span></span></td>
<td><span data-ttu-id="ed5f7-311">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ed5f7-312">Faktura zuzentzen da kargatu beharreko kantitatea gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="ed5f7-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ed5f7-313">Fakturatutako salmenten itzulera</span><span class="sxs-lookup"><span data-stu-id="ed5f7-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ed5f7-314">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-315">Fakturatutako salmenten benetako kopurua: kantitate berri baterako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ed5f7-316">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ed5f7-317">Fakturatu gabeko salmenten benetako kopurua: kargagarria ezberdintasunerako</span><span class="sxs-lookup"><span data-stu-id="ed5f7-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ed5f7-318">Proiektu-kontratuaren dibisa</span><span class="sxs-lookup"><span data-stu-id="ed5f7-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
