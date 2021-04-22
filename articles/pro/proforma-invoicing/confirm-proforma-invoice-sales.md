---
title: Berretsi proformako proiektuaren faktura
description: Gai honek Proforma proiektuaren fakturak berrestearen inguruko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 04/05/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 144c1b6a49951af8be0c619f41808e7617e59c92
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/07/2021
ms.locfileid: "5867071"
---
# <a name="confirm-a-proforma-project-invoice"></a><span data-ttu-id="0eefd-103">Berretsi proformako proiektuaren faktura</span><span class="sxs-lookup"><span data-stu-id="0eefd-103">Confirm a proforma project invoice</span></span> 

<span data-ttu-id="0eefd-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="0eefd-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="0eefd-105">Proforma faktura baieztatu ondoren, proiektuaren fakturaren egoera eguneratu egingo da **Baieztatuta**.</span><span class="sxs-lookup"><span data-stu-id="0eefd-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="0eefd-106">Faktura bat baieztatzen denean, irakurtzeko soilik bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="0eefd-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="0eefd-107">Aurrerantzean, fakturak bezeroak hasitako zuzenketak edo kredituak baldin badaude bakarrik konpondu ahal izango dira.</span><span class="sxs-lookup"><span data-stu-id="0eefd-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits.</span></span>

<span data-ttu-id="0eefd-108">Hurrengo taulan sistemak sortutako errealitateak zerrendatzen dira.</span><span class="sxs-lookup"><span data-stu-id="0eefd-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="0eefd-109">Egitate horiek proiektuaren fakturaren zirriborroan eragiketa batzuk egiten direnean sortzen dira, hori baieztatu aurretik.</span><span class="sxs-lookup"><span data-stu-id="0eefd-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="0eefd-110">
                    <strong>Egoera</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0eefd-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="0eefd-111">
                    <strong>Berrespenean sortutako datuak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0eefd-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-112">Atxikipen edo aurrerakin bat fakturatzea</span><span class="sxs-lookup"><span data-stu-id="0eefd-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-113">Mota bateko fakturatutako salmentak, <strong>Atxikitzailea</strong> aurrerakinaren edo atxikipenaren zenbatekoarengatik sortzen da.</span><span class="sxs-lookup"><span data-stu-id="0eefd-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-114">Adiskidetzerako erabili beharreko atxikipenaren edo aurrerakinaren zenbateko negatiboaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="0eefd-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-115">Atxikimendu bat edo faktura baten aurrerapena guztiz bateratu ondoren.</span><span class="sxs-lookup"><span data-stu-id="0eefd-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-116">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="0eefd-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="0eefd-117">Zenbateko hori positiboa da, atxikipena edo aurrerakina fakturatu zenean sortutako negatiboa bertan behera uzteko pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="0eefd-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-118">Faktura honetako zenbatekoaren fakturatutako salmentak.</span><span class="sxs-lookup"><span data-stu-id="0eefd-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0eefd-119">Atxikimendu bat edo faktura baten aurrerapena zati batean bateratu ondoren.</span><span class="sxs-lookup"><span data-stu-id="0eefd-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-120">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="0eefd-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="0eefd-121">Zenbateko hori positiboa da, atxikipena edo aurrerakina fakturatu zenean sortutako negatiboa bertan behera uzteko pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="0eefd-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-122">Faktura honetako zenbatekoaren fakturatutako salmentak.</span><span class="sxs-lookup"><span data-stu-id="0eefd-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-123">Etorkizuneko fakturetan adiskidetzerako erabili beharreko geratzen den atxikipenaren edo aurrerakinaren fakturatu gabeko salmenta negatiboak.</span><span class="sxs-lookup"><span data-stu-id="0eefd-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-124">Denbora-transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.</span><span class="sxs-lookup"><span data-stu-id="0eefd-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-125">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-126">Orduen eta zenbatekoaren fakturatutako salmentak jatorrizko denboraren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0eefd-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0eefd-127">Kopurua murrizteko editatu den denbora-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-128">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-129">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-130">Editatutako fakturaren lerroaren xehetasunean geratzen diren orduak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-131">Kopurua areagotzeko editatu den denbora-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-132">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-133">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-134">Gastu transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.</span><span class="sxs-lookup"><span data-stu-id="0eefd-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-135">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0eefd-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-136">Zenbatekoaren eta zenbatekoaren fakturatutako salmentak jatorrizko gastuaren onarpenean</span><span class="sxs-lookup"><span data-stu-id="0eefd-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0eefd-137">Kopurua murrizteko editatu den gastu-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-138">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0eefd-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-139">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-140">Editatutako fakturaren lerroaren xehetasunean geratzen diren kopuruak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatu gabeko salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-141">Kopurua areagotzeko editatu den gastu-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-142">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0eefd-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-143">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-144">Transakzio materiala fakturatzea zirriborroaren fakturan aldaketarik egin gabe.</span><span class="sxs-lookup"><span data-stu-id="0eefd-144">Invoicing a material transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-145">Fakturatu gabeko salmenten itzulketa materialaren jatorrizko erabilera-onespenean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="0eefd-145">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-146">Fakturatutako benetako salmentak materialaren jatorrizko erabilera-onespenean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="0eefd-146">A billed sales actual for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0eefd-147">Kopurua murrizteko editatu den transakzio materiala fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-147">Invoicing a material transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-148">Fakturatu gabeko salmenten itzulketa materialaren jatorrizko denbora-onespenean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="0eefd-148">An unbilled sales reversal for the quantity and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-149">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-149">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-150">Editatutako fakturaren lerroaren xehetasunean geratzen diren kopuruak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatu gabeko salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-150">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-151">Kopurua areagotzeko editatu den transakzio materiala fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-151">Invoicing a material transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-152">Fakturatu gabeko salmenten itzulketa materialaren jatorrizko erabilera-onespenean dagoen kantitatea eta zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="0eefd-152">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-153">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-153">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0eefd-154">Kuota fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-154">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-155">Jatorrizko kutxako liburuaren lerroko zerga-zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-155">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-156">Zenbatekoaren eta zenbatekoaren fakturatutako salmentak zergen kutxako liburuaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0eefd-156">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="0eefd-157">Mugarri bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0eefd-157">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-158">Proiektuaren kontratu linearen jatorrizko mugarriaren zenbatekoaren fakturatutako salmentak.</span><span class="sxs-lookup"><span data-stu-id="0eefd-158">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="0eefd-159">Produktuetan oinarritutako kontratuaren lerroaren fakturazioa.</span><span class="sxs-lookup"><span data-stu-id="0eefd-159">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0eefd-160">Produktu-lerroaren fakturatutako salmentak, produktuan oinarritutako kontratu-lerroaren zenbatekoarekin eta zenbatekoarekin.</span><span class="sxs-lookup"><span data-stu-id="0eefd-160">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
