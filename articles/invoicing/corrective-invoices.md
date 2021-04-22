---
title: Sortu proiektuetan oinarritutako faktura zuzentzaileak
description: Gai honek faktura zuzentzailearen inguruko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 03/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32772d64b3fc77f0af9618edff40e3b295593454
ms.sourcegitcommit: 504c09365bf404c1f1aa9b5034c1e1e5bc9d0d54
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788828"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="70e9f-103">Sortu proiektuetan oinarritutako faktura zuzentzaileak</span><span class="sxs-lookup"><span data-stu-id="70e9f-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="70e9f-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="70e9f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="70e9f-105">Egiaztatutako proiektuaren faktura zuzendu daiteke bezeroarekin eta proiektuaren arduradunarekin negoziatutako aldaketak edo kredituak prozesatzeko.</span><span class="sxs-lookup"><span data-stu-id="70e9f-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="70e9f-106">Berretsitako faktura batean aldaketak egiteko, ireki berretsitako faktura eta hautatu **Zuzendu faktura hau**.</span><span class="sxs-lookup"><span data-stu-id="70e9f-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="70e9f-107">Aukeraketa hau ez dago erabilgarri proiektuaren faktura baieztatu ezean.</span><span class="sxs-lookup"><span data-stu-id="70e9f-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="70e9f-108">Berretsitako fakturatik faktura zirriborro berria sortzen da.</span><span class="sxs-lookup"><span data-stu-id="70e9f-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="70e9f-109">Aurretik baieztatutako fakturaren faktura-lerroaren xehetasun guztiak zirriborro berrira kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="70e9f-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="70e9f-110">Honako hauek dira faktura zuzendu berriaren lerroaren xehetasunak gehiago ulertzen laguntzeko funtsezko puntu batzuk:</span><span class="sxs-lookup"><span data-stu-id="70e9f-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="70e9f-111">Kopuru guztiak zero bihurtzen dira.</span><span class="sxs-lookup"><span data-stu-id="70e9f-111">All quantities are updated to zero.</span></span> <span data-ttu-id="70e9f-112">Fakturatutako elementu guztiak guztiz kreditatuta daudela suposatzen du.</span><span class="sxs-lookup"><span data-stu-id="70e9f-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="70e9f-113">Behar izanez gero, eskuz egunera ditzakezu kantitate horiek fakturatzen ari diren kopurua eta ez kreditatzen den kopurua.</span><span class="sxs-lookup"><span data-stu-id="70e9f-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="70e9f-114">Sartzen duzun kantitatearen arabera, aplikazioak kreditatutako kantitatea kalkulatzen du.</span><span class="sxs-lookup"><span data-stu-id="70e9f-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="70e9f-115">Zenbateko hori faktura zuzena baieztatzen denean sortzen diren errealetan islatzen da.</span><span class="sxs-lookup"><span data-stu-id="70e9f-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="70e9f-116">Zergaren zenbatekoan aldaketak egiten ari bazara, zergaren zenbateko zuzena sartu behar duzu eta ez kreditatzen den zergaren zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="70e9f-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="70e9f-117">Mugarrien zuzenketak kreditu oso gisa prozesatzen dira beti.</span><span class="sxs-lookup"><span data-stu-id="70e9f-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="70e9f-118">Atxikitako edo aurreratutako zenbatekoak zuzendu daitezke bezeroari zenbateko okerra fakturatzen bazaio.</span><span class="sxs-lookup"><span data-stu-id="70e9f-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="70e9f-119">Atxikitzaileen eta aurrerakinen bateragarritasuna zuzendu daiteke, aurrez baieztatutako faktura bateko kargekin bateratzeko zenbateko okerra erabili bada.</span><span class="sxs-lookup"><span data-stu-id="70e9f-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="70e9f-120">Dagoeneko fakturatutako beste karga batzuen zuzenketak diren faktura lerroaren xehetasunek **Zuzenketa** eremua ezarrita dute **Bai**.</span><span class="sxs-lookup"><span data-stu-id="70e9f-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="70e9f-121">Faktura lerroaren xehetasunak zuzendu dituzten fakturek izeneko eremua dute **Zuzenketak ditu** hori ere ezarrita dago **Bai**.</span><span class="sxs-lookup"><span data-stu-id="70e9f-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="70e9f-122">Faktura zuzentzailea berrestean sortutako datuak</span><span class="sxs-lookup"><span data-stu-id="70e9f-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="70e9f-123">Hurrengo taulan faktura zuzentzailea baieztatzen denean sortzen diren errealitateak agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="70e9f-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="70e9f-124">
                    <strong>Egoera</strong>
                </span><span class="sxs-lookup"><span data-stu-id="70e9f-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="70e9f-125">
                    <strong>Berrespenean sortutako datuak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="70e9f-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="70e9f-126">Berretsi fakturatutako aurrerakinaren edo atxikipenaren zuzenketa.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="70e9f-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-127">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="70e9f-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="70e9f-128">Zenbateko hori positiboa da, atxikipena edo aurrerakina fakturatu zenean sortutako negatiboa bertan behera uzteko pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="70e9f-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-129">Fakturatutako salmenten berraztertzea jatorrizko fakturatutako salmentak alderantzikatzeko atxikipena edo aurrerakinaren zenbatekoa sortzen da.</span><span class="sxs-lookup"><span data-stu-id="70e9f-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-130">Fakturatutako salmenta berria atxikipeneko zuzendutako zenbatekoarekin edo aurrerakinean oinarritutako zuzendutako kontratuaren lerroarekin sortzen da.</span><span class="sxs-lookup"><span data-stu-id="70e9f-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-131">Adiskidetzerako erabili beharreko atxikipenaren edo aurrerakinean oinarritutako zuzendutako fakturaren lerroaren zenbateko negatiboaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="70e9f-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="70e9f-132">Aurretik bateratutako atxikipen edo aurrerakinaren zuzenketaren berrespena.</span><span class="sxs-lookup"><span data-stu-id="70e9f-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-133">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="70e9f-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="70e9f-134">Zenbateko hori positiboa da eta atxikipena edo aurrerakina fakturatu zenean kontziliazioa geratu zenerako pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="70e9f-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-135">Aurreko fakturako zenbatekoaren fakturatutako alderantzikako salmentak.</span><span class="sxs-lookup"><span data-stu-id="70e9f-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-136">Fakturatutako salmenta berria atxikipeneko zuzendutako zenbatekoarekin zuzendutako kontratuaren lerroarekin sortzen da.</span><span class="sxs-lookup"><span data-stu-id="70e9f-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-137">Adiskidetzerako erabili beharreko atxikipenaren lerroaren zenbateko negatiboaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="70e9f-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="70e9f-138">Aurretik fakturatutako denbora transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-139">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-140">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="70e9f-141">Kreditu partziala fakturatzea denborako transakzio batean.</span><span class="sxs-lookup"><span data-stu-id="70e9f-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-142">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-143">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-144">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako orduetan eta zenbatekoan kobratuko dena.</span><span class="sxs-lookup"><span data-stu-id="70e9f-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="70e9f-145">Aurretik fakturatutako gastua transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-146">Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-147">Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="70e9f-148">Aurretik fakturatutako gastua transakzio baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-149">Gastuaren jatorrizko fakturatutako lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-150">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-151">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako kopuruan eta zenbatekoan kobratuko dena</span><span class="sxs-lookup"><span data-stu-id="70e9f-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="70e9f-152">Aurretik fakturatutako zerga transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-153">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-154">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="70e9f-155">Aurretik fakturatutako zerga transakzio baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-156">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-157">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokidea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="70e9f-158">Aurretik fakturatutako mugarri baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-159">Mugarriaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="70e9f-160">Mugarriaren fakturaren egoera eguneratzen da <b>Bezeroaren faktura argitaratua</b> <b>Fakturatzeko prest</b>.</span><span class="sxs-lookup"><span data-stu-id="70e9f-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="70e9f-161">Aurretik fakturatutako mugarri baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="70e9f-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="70e9f-162">Ez dira onartzen</span><span class="sxs-lookup"><span data-stu-id="70e9f-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
