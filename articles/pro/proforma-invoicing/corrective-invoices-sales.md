---
title: Proiektuaren faktura zuzentzaileak
description: Gai honek faktura zuzentzaileak sortu eta berresteko Project Operations-en informazioa ematen du.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: dfa5535597ee6e144259c9246b33075f3492285e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004066"
---
# <a name="corrective-project-invoices"></a><span data-ttu-id="33a12-103">Proiektuaren faktura zuzentzaileak</span><span class="sxs-lookup"><span data-stu-id="33a12-103">Corrective project invoices</span></span>

<span data-ttu-id="33a12-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="33a12-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="33a12-105">Egiaztatutako proiektuaren faktura zuzendu daiteke bezeroarekin eta proiektuaren arduradunarekin negoziatutako aldaketak edo kredituak prozesatzeko.</span><span class="sxs-lookup"><span data-stu-id="33a12-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="33a12-106">Berretsitako faktura batean aldaketak egiteko, ireki berretsitako faktura eta hautatu **Zuzendu faktura hau**.</span><span class="sxs-lookup"><span data-stu-id="33a12-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="33a12-107">Aukeraketa hau ez dago erabilgarri proiektuaren faktura baieztatu ezean.</span><span class="sxs-lookup"><span data-stu-id="33a12-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="33a12-108">Berretsitako fakturatik faktura zirriborro berria sortzen da.</span><span class="sxs-lookup"><span data-stu-id="33a12-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="33a12-109">Aurretik baieztatutako fakturaren faktura-lerroaren xehetasun guztiak zirriborro berrira kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="33a12-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="33a12-110">Honako hauek dira faktura zuzendu berriaren lerroaren xehetasunak ulertzeko gakoetako batzuk:</span><span class="sxs-lookup"><span data-stu-id="33a12-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="33a12-111">Kopuru guztiak zero bihurtzen dira.</span><span class="sxs-lookup"><span data-stu-id="33a12-111">All quantities are updated to zero.</span></span> <span data-ttu-id="33a12-112">Aplikazioak fakturatutako elementu guztiak guztiz kreditatuta daudela suposatzen du.</span><span class="sxs-lookup"><span data-stu-id="33a12-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="33a12-113">Behar izanez gero, eskuz egunera ditzakezu kantitate horiek fakturatzen ari diren kopurua eta ez kreditatzen den kopurua.</span><span class="sxs-lookup"><span data-stu-id="33a12-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="33a12-114">Sartzen duzun kantitatearen arabera, aplikazioak kreditatutako kantitatea kalkulatzen du.</span><span class="sxs-lookup"><span data-stu-id="33a12-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="33a12-115">Zenbateko hori faktura zuzena baieztatzen denean sortzen diren errealetan islatzen da.</span><span class="sxs-lookup"><span data-stu-id="33a12-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="33a12-116">Zergaren zenbatekoan aldaketak egiten ari bazara, zergaren zenbateko zuzena sartu behar duzu eta ez kreditatzen den zergaren zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="33a12-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="33a12-117">Aurretik baieztatutako produktuetan oinarritutako kontratu lerroak ez dira kopiatzen.</span><span class="sxs-lookup"><span data-stu-id="33a12-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="33a12-118">Ez da onartzen produktuan oinarritutako proiektuaren fakturan zuzenketak prozesatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="33a12-119">Mugarrien zuzenketak kreditu oso gisa prozesatzen dira beti.</span><span class="sxs-lookup"><span data-stu-id="33a12-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="33a12-120">Atxikitako edo aurreratutako zenbatekoak zuzendu daitezke bezeroari zenbateko okerra fakturatzen bazaio.</span><span class="sxs-lookup"><span data-stu-id="33a12-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="33a12-121">Atxikitzaileen eta aurrerakinen bateragarritasuna zuzendu daiteke, aurrez baieztatutako faktura bateko kargekin bateratzeko zenbateko okerra erabili bada.</span><span class="sxs-lookup"><span data-stu-id="33a12-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="33a12-122">Jada fakturatutako beste karga batzuen zuzenketen faktura-lerroaren xehetasunak daude **Zuzenketa** ezarri **Bai**.</span><span class="sxs-lookup"><span data-stu-id="33a12-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="33a12-123">Faktura lerroaren xehetasunak zuzendu dituzten fakturek izeneko eremua dute **Zuzenketak ditu** hori ere ezarrita dago **Bai**.</span><span class="sxs-lookup"><span data-stu-id="33a12-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="33a12-124">Faktura zuzentzailea baieztatzean sortutako datuak</span><span class="sxs-lookup"><span data-stu-id="33a12-124">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="33a12-125">Hurrengo taulan faktura zuzentzailea baieztatzen denean sortzen diren errealitateak agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="33a12-125">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="33a12-126">
                    <strong>Egoera</strong>
                </span><span class="sxs-lookup"><span data-stu-id="33a12-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="33a12-127">
                    <strong>Berrespenean sortutako datuak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="33a12-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="33a12-128">Berretsi fakturatutako aurrerakinaren edo atxikipenaren zuzenketa.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="33a12-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-129">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="33a12-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="33a12-130">Zenbateko hori positiboa da, atxikipena edo aurrerakina fakturatu zenean sortutako negatiboa bertan behera uzteko pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="33a12-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-131">Fakturatutako salmenten berraztertzea jatorrizko fakturatutako salmentak alderantzikatzeko atxikipena edo aurrerakinaren zenbatekoa sortzen da.</span><span class="sxs-lookup"><span data-stu-id="33a12-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-132">Fakturatutako salmenta berria atxikipeneko zuzendutako zenbatekoarekin edo aurrerakinean oinarritutako zuzendutako kontratuaren lerroarekin sortzen da.</span><span class="sxs-lookup"><span data-stu-id="33a12-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-133">Adiskidetzerako erabili beharreko atxikipenaren edo aurrerakinean oinarritutako zuzendutako fakturaren lerroaren zenbateko negatiboaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="33a12-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="33a12-134">Aurretik bateratutako atxikipen edo aurrerakinaren zuzenketaren berrespena.</span><span class="sxs-lookup"><span data-stu-id="33a12-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-135">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="33a12-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="33a12-136">Zenbateko hori positiboa da eta atxikipena edo aurrerakina fakturatu zenean kontziliazioa geratu zenerako pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="33a12-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-137">Aurreko fakturako zenbatekoaren fakturatutako alderantzikako salmentak.</span><span class="sxs-lookup"><span data-stu-id="33a12-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-138">Fakturatutako salmenta berria atxikipeneko zuzendutako zenbatekoarekin zuzendutako kontratuaren lerroarekin sortzen da.</span><span class="sxs-lookup"><span data-stu-id="33a12-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-139">Adiskidetzerako erabili beharreko atxikipenaren lerroaren zenbateko negatiboaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="33a12-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="33a12-140">Aurretik fakturatutako denbora transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-141">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-142">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="33a12-143">Kreditu partziala fakturatzea denborako transakzio batean.</span><span class="sxs-lookup"><span data-stu-id="33a12-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-144">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-145">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="33a12-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-146">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako orduetan eta zenbatekoan kobratuko dena.</span><span class="sxs-lookup"><span data-stu-id="33a12-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="33a12-147">Aurretik fakturatutako gastua transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-148">Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-149">Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="33a12-150">Aurretik fakturatutako gastua transakzio baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-151">Gastuaren jatorrizko fakturatutako lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-152">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="33a12-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-153">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako kopuruan eta zenbatekoan kobratuko dena</span><span class="sxs-lookup"><span data-stu-id="33a12-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="33a12-154">Aurretik fakturatutako transakzio material baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-154">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-155">Fakturatutako salmenten itzulketa materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="33a12-155">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-156">Fakturatu gabeko salmenten benetako datuak materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="33a12-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="33a12-157">Transakzio material baten kreditu partziala fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-157">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-158">Fakturatutako salmenten itzulketa materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen fakturatutako kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="33a12-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-159">Editatutako fakturaren lerroaren xehetasunean zenbatekoaren eta zenbatekoaren kargura dagoen fakturaziorik gabeko salmenta berri bat, honen itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="33a12-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-160">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako kopuruan eta zenbatekoan kobratuko dena</span><span class="sxs-lookup"><span data-stu-id="33a12-160">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="33a12-161">Aurretik fakturatutako zerga transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-161">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-162">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-162">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-163">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-163">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="33a12-164">Aurretik fakturatutako zerga transakzio baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-164">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-165">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-165">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-166">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokidea.</span><span class="sxs-lookup"><span data-stu-id="33a12-166">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="33a12-167">Aurretik fakturatutako mugarri baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-167">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-168">Mugarriaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-168">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="33a12-169">Mugarriaren fakturaren egoera eguneratzen da <b>Bezeroaren faktura argitaratua</b> <b>Fakturatzeko prest</b>.</span><span class="sxs-lookup"><span data-stu-id="33a12-169">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="33a12-170">Aurretik fakturatutako mugarri baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="33a12-170">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-171">Ez dira onartzen</span><span class="sxs-lookup"><span data-stu-id="33a12-171">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="33a12-172">Aurretik fakturatutako produktuan oinarritutako kontratu lerro baten kredituak eta zuzenketak.</span><span class="sxs-lookup"><span data-stu-id="33a12-172">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="33a12-173">Ez dira onartzen</span><span class="sxs-lookup"><span data-stu-id="33a12-173">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
