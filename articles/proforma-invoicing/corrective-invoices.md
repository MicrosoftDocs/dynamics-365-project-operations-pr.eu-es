---
title: Proiektuetan oinarritutako faktura zuzentzaileak
description: Gai honek proiektuan oinarritutako faktura zuzentzaileak sortu eta berresteko Project Operations-en informazioa ematen du.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6b6670f823577bf7f784443f97f0b77e1e9a6aa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012256"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="fd1a9-103">Proiektuetan oinarritutako faktura zuzentzaileak</span><span class="sxs-lookup"><span data-stu-id="fd1a9-103">Corrective project-based invoices</span></span>

<span data-ttu-id="fd1a9-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="fd1a9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="fd1a9-105">Egiaztatutako proiektuaren faktura zuzendu daiteke bezeroarekin eta proiektuaren arduradunarekin negoziatutako aldaketak edo kredituak prozesatzeko.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="fd1a9-106">Berretsitako faktura batean aldaketak egiteko, ireki berretsitako faktura eta hautatu **Zuzendu faktura hau**.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="fd1a9-107">Aukeraketa hau ez dago erabilgarri proiektuaren faktura baieztatzen ez bada edo proiektuan oinarritutako fakturak aurrerakinak edo atxikipenak edo aurrerakinen edo atxikipenak bateratzeko.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="fd1a9-108">Berretsitako fakturatik faktura zirriborro berria sortzen da.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="fd1a9-109">Aurretik baieztatutako fakturaren faktura-lerroaren xehetasun guztiak zirriborro berrira kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="fd1a9-110">Honako hauek dira faktura zuzendu berriaren lerroaren xehetasunak ulertzeko gakoetako batzuk:</span><span class="sxs-lookup"><span data-stu-id="fd1a9-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="fd1a9-111">Kopuru guztiak zero bihurtzen dira.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-111">All quantities are updated to zero.</span></span> <span data-ttu-id="fd1a9-112">Dynamics 365 Project Operations fakturatutako elementu guztiak guztiz kreditatuta daudela suposatzen du.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="fd1a9-113">Behar izanez gero, eskuz egunera ditzakezu kantitate horiek fakturatzen ari diren kopurua eta ez kreditatzen den kopurua.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="fd1a9-114">Sartzen duzun kantitatearen arabera, aplikazioak kreditatutako kantitatea kalkulatzen du.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="fd1a9-115">Zenbateko hori faktura zuzena baieztatzen denean sortzen diren errealetan islatzen da.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="fd1a9-116">Zergaren zenbatekoan aldaketak egiten ari bazara, zergaren zenbateko zuzena sartu behar duzu eta ez kreditatzen den zergaren zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="fd1a9-117">Mugarrien zuzenketak kreditu oso gisa prozesatzen dira beti.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="fd1a9-118">Dagoeneko fakturatutako beste karga batzuen zuzenketak diren faktura lerroaren xehetasunetarako **Zuzenketa** eremua ezarrita dago **Bai**.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="fd1a9-119">Zuzendutako fakturaren lerroak dituzten fakturen xehetasunak, **Zuzenketak ditu** eremua ezarrita dago **Bai**.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="fd1a9-120">Faktura zuzentzailea baieztatzean sortutako datuak</span><span class="sxs-lookup"><span data-stu-id="fd1a9-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="fd1a9-121">Hurrengo taulan faktura zuzentzailea baieztatzen denean sortzen diren errealitateak agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="fd1a9-122">
                    <strong>Egoera</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fd1a9-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="fd1a9-123">
                    <strong>Berrespenean sortutako datuak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="fd1a9-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fd1a9-124">Aurretik fakturatutako denbora transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-125">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-126">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="fd1a9-127">Kreditu partziala fakturatzea denborako transakzio batean.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-128">Denboraren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-129">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-130">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako orduetan eta zenbatekoan kobratuko dena.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fd1a9-131">Aurretik fakturatutako gastua transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-132">Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-133">Gastuaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="fd1a9-134">Aurretik fakturatutako gastua transakzio baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-135">Gastuaren jatorrizko fakturatutako lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-136">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-137">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako kopuruan eta zenbatekoan kobratuko dena</span><span class="sxs-lookup"><span data-stu-id="fd1a9-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fd1a9-138">Aurretik fakturatutako transakzio material baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-139">Fakturatutako salmenten itzulketa materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-140">Fakturatu gabeko salmenten benetako datuak materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="fd1a9-141">Transakzio material baten kreditu partziala fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-142">Fakturatutako salmenten itzulketa materialaren jatorrizko fakturaren lerroaren xehetasunean dagoen fakturatutako kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-143">Editatutako fakturaren lerroaren xehetasunean zenbatekoaren eta zenbatekoaren kargura dagoen fakturaziorik gabeko salmenta berri bat, honen itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-144">Fakturarik gabeko salmenten faktura berri bat, fakturazio lerroaren xehetasunean zuzendu diren zifrak kendu ondorengo gainerako kopuruan eta zenbatekoan kobratuko dena</span><span class="sxs-lookup"><span data-stu-id="fd1a9-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fd1a9-145">Aurretik fakturatutako zerga transakzio baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-146">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-147">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatu gabeko zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="fd1a9-148">Aurretik fakturatutako zerga transakzio baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-149">Zergaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako zenbatekoaren alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-150">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, horien itzulketa eta fakturatutako salmenten baliokidea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="fd1a9-151">Aurretik fakturatutako mugarri baten kreditu osoa fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-152">Mugarriaren jatorrizko fakturaren lerroko xehetasunen eta zenbatekoaren fakturatutako salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="fd1a9-153">Mugarriaren fakturaren egoera eguneratzen da <b>Bezeroaren faktura argitaratua</b> <b>Fakturatzeko prest</b>.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="fd1a9-154">Aurretik fakturatutako mugarri baten kredituaren zati bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="fd1a9-155">Egoera hau ez da onartzen.</span><span class="sxs-lookup"><span data-stu-id="fd1a9-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
