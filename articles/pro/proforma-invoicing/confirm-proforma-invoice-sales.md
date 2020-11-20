---
title: Berretsi proformako faktura - arina
description: Gai honetan Project Operations-eko proformako fakturak berresteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 02b671e4ad327b2448529d7119211613f3a9cb27
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176506"
---
# <a name="confirm-a-proforma-invoice---lite"></a><span data-ttu-id="0070f-103">Berretsi proformako faktura - arina</span><span class="sxs-lookup"><span data-stu-id="0070f-103">Confirm a proforma invoice - lite</span></span>

<span data-ttu-id="0070f-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="0070f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="0070f-105">Proforma faktura baieztatu ondoren, proiektuaren fakturaren egoera eguneratu egingo da **Baieztatuta**.</span><span class="sxs-lookup"><span data-stu-id="0070f-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="0070f-106">Faktura bat baieztatzen denean, irakurtzeko soilik bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="0070f-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="0070f-107">Aurrerantzean, faktura bezeroak hasitako zuzenketak edo kredituak badaude bakarrik zuzendu ahal izango da, faktura ordainduta dagoela markatuta badago.</span><span class="sxs-lookup"><span data-stu-id="0070f-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, of if the invoice is marked as paid.</span></span>

<span data-ttu-id="0070f-108">Hurrengo taulan sistemak sortutako errealitateak zerrendatzen dira.</span><span class="sxs-lookup"><span data-stu-id="0070f-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="0070f-109">Egitate horiek proiektuaren fakturaren zirriborroan eragiketa batzuk egiten direnean sortzen dira, hori baieztatu aurretik.</span><span class="sxs-lookup"><span data-stu-id="0070f-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="0070f-110">
                    <strong>Egoera</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0070f-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="0070f-111">
                    <strong>Berrespenean sortutako datuak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0070f-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0070f-112">Atxikipen edo aurrerakin bat fakturatzea</span><span class="sxs-lookup"><span data-stu-id="0070f-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-113">Mota bateko fakturatutako salmentak, <strong>Atxikitzailea</strong> aurrerakinaren edo atxikipenaren zenbatekoarengatik sortzen da.</span><span class="sxs-lookup"><span data-stu-id="0070f-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-114">Adiskidetzerako erabili beharreko atxikipenaren edo aurrerakinaren zenbateko negatiboaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="0070f-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0070f-115">Atxikimendu bat edo faktura baten aurrerapena guztiz bateratu ondoren.</span><span class="sxs-lookup"><span data-stu-id="0070f-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-116">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="0070f-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="0070f-117">Zenbateko hori positiboa da, atxikipena edo aurrerakina fakturatu zenean sortutako negatiboa bertan behera uzteko pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="0070f-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-118">Faktura honetako zenbatekoaren fakturatutako salmentak.</span><span class="sxs-lookup"><span data-stu-id="0070f-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0070f-119">Atxikimendu bat edo faktura baten aurrerapena zati batean bateratu ondoren.</span><span class="sxs-lookup"><span data-stu-id="0070f-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-120">Adiskidetzerako sortu zen atxikipenaren edo aurrerakinaren fakturaziorik gabeko salmentak.</span><span class="sxs-lookup"><span data-stu-id="0070f-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="0070f-121">Zenbateko hori positiboa da, atxikipena edo aurrerakina fakturatu zenean sortutako negatiboa bertan behera uzteko pentsatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="0070f-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-122">Faktura honetako zenbatekoaren fakturatutako salmentak.</span><span class="sxs-lookup"><span data-stu-id="0070f-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-123">Etorkizuneko fakturetan adiskidetzerako erabili beharreko geratzen den atxikipenaren edo aurrerakinaren fakturatu gabeko salmenta negatiboak.</span><span class="sxs-lookup"><span data-stu-id="0070f-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0070f-124">Denbora-transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.</span><span class="sxs-lookup"><span data-stu-id="0070f-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-125">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-126">Orduen eta zenbatekoaren fakturatutako salmentak jatorrizko denboraren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0070f-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0070f-127">Kopurua murrizteko editatu den denbora-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-128">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-129">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0070f-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-130">Editatutako fakturaren lerroaren xehetasunean geratzen diren orduak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0070f-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0070f-131">Kopurua areagotzeko editatu den denbora-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-132">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-133">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0070f-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0070f-134">Gastu transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.</span><span class="sxs-lookup"><span data-stu-id="0070f-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-135">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0070f-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-136">Zenbatekoaren eta zenbatekoaren fakturatutako salmentak jatorrizko gastuaren onarpenean</span><span class="sxs-lookup"><span data-stu-id="0070f-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="0070f-137">Kopurua murrizteko editatu den gastu-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-138">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0070f-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-139">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0070f-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-140">Editatutako fakturaren lerroaren xehetasunean geratzen diren kopuruak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatu gabeko salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0070f-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0070f-141">Kopurua areagotzeko editatu den gastu-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-142">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="0070f-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-143">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="0070f-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0070f-144">Kuota fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-144">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-145">Jatorrizko kutxako liburuaren lerroko zerga-zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-145">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-146">Zenbatekoaren eta zenbatekoaren fakturatutako salmentak zergen kutxako liburuaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0070f-146">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="0070f-147">Mugarri bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="0070f-147">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-148">Proiektuaren kontratu linearen jatorrizko mugarriaren zenbatekoaren fakturatutako salmentak.</span><span class="sxs-lookup"><span data-stu-id="0070f-148">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="0070f-149">Produktuetan oinarritutako kontratuaren lerroaren fakturazioa.</span><span class="sxs-lookup"><span data-stu-id="0070f-149">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="0070f-150">Produktu-lerroaren fakturatutako salmentak, produktuan oinarritutako kontratu-lerroaren zenbatekoarekin eta zenbatekoarekin.</span><span class="sxs-lookup"><span data-stu-id="0070f-150">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
