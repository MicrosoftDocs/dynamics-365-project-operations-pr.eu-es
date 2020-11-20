---
title: Berretsi proformako faktura
description: Gai honek proforma faktura berresteari buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fa1e6c17fbda76a283c2ec68760a00e846decf83
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128088"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="dc857-103">Berretsi proformako faktura</span><span class="sxs-lookup"><span data-stu-id="dc857-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="dc857-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="dc857-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="dc857-105">Proforma faktura baieztatu ondoren, proiektuaren fakturaren egoera eguneratu egingo da **Baieztatuta**.</span><span class="sxs-lookup"><span data-stu-id="dc857-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="dc857-106">Faktura bat baieztatzen denean, irakurtzeko soilik bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="dc857-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="dc857-107">Aurrerantzean, faktura bezeroak hasitako zuzenketak edo kredituak badaude bakarrik zuzendu ahal izango da, edo ordainduta dagoela markatuta badago.</span><span class="sxs-lookup"><span data-stu-id="dc857-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="dc857-108">Hurrengo taulan sistemak sortutako errealitateak zerrendatzen dira.</span><span class="sxs-lookup"><span data-stu-id="dc857-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="dc857-109">Egitate horiek proiektuaren fakturaren zirriborroan eragiketa batzuk egiten direnean sortzen dira, hori baieztatu aurretik.</span><span class="sxs-lookup"><span data-stu-id="dc857-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="dc857-110">
                    <strong>Egoera</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dc857-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="dc857-111">
                    <strong>Berrespenean sortutako datuak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dc857-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dc857-112">Denbora-transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.</span><span class="sxs-lookup"><span data-stu-id="dc857-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-113">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-114">Orduen eta zenbatekoaren fakturatutako salmentak jatorrizko denboraren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="dc857-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="dc857-115">Kopurua murrizteko editatu den denbora-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-116">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-117">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="dc857-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-118">Editatutako fakturaren lerroaren xehetasunean geratzen diren orduak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatu gabeko salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="dc857-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dc857-119">Kopurua areagotzeko editatu den denbora-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-120">Jatorrizko denbora-onespen bateko orduen eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-121">Editatutako fakturaren lerroaren xehetasunean orduak eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="dc857-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dc857-122">Gastu transakzio bat fakturatzea zirriborroaren fakturan aldaketarik egin gabe.</span><span class="sxs-lookup"><span data-stu-id="dc857-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-123">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="dc857-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-124">Zenbatekoaren eta zenbatekoaren fakturatutako salmentak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="dc857-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="dc857-125">Kopurua murrizteko editatu den gastu-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-126">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="dc857-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-127">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="dc857-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-128">Editatutako fakturaren lerroaren xehetasunean geratzen diren kopuruak eta zuzendutako zenbakiak kendu eta gero zenbatekoa kobratzen ez duen fakturaziorik gabeko salmenta berria, fakturatutako salmenten itzulketa eta fakturatu gabeko salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="dc857-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dc857-129">Kopurua areagotzeko editatu den gastu-transakzio bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-130">Zenbatekoaren eta zenbatekoaren fakturatu gabeko salmenten alderantzikatzeak jatorrizko gastuaren onarpenean.</span><span class="sxs-lookup"><span data-stu-id="dc857-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-131">Editatutako fakturaren lerroaren xehetasunean kopurua eta zenbatekoa kobratzen duen fakturaziorik gabeko salmenta berria, fakturatu gabeko salmenten itzulketa eta fakturatutako salmenten baliokide baliokidea.</span><span class="sxs-lookup"><span data-stu-id="dc857-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dc857-132">Kuota fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-133">Jatorrizko kutxako liburuaren lerroko zerga-zenbatekoaren fakturatu gabeko salmenten alderantzikatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-134">Zenbatekoaren eta zenbatekoaren fakturatutako salmentak zergen kutxako liburuaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="dc857-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="dc857-135">Mugarri bat fakturatzea.</span><span class="sxs-lookup"><span data-stu-id="dc857-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dc857-136">Proiektuaren kontratu linearen jatorrizko mugarriaren zenbatekoaren fakturatutako salmentak.</span><span class="sxs-lookup"><span data-stu-id="dc857-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
