---
title: Oinarrizko gastuen sarrera (arina)
description: Gai honek lite inplementazio batean gastuen sarrerarekin lan egiteko moduari buruzko informazioa eskaintzen du.
author: stsporen
manager: AnnBe
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 539d0ba6be6f49a6f0509595a0776ef67135496d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276738"
---
# <a name="expense-entry-lite"></a><span data-ttu-id="9beff-103">Oinarrizko gastuen sarrera (arina)</span><span class="sxs-lookup"><span data-stu-id="9beff-103">Expense entry (lite)</span></span>

<span data-ttu-id="9beff-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="9beff-104">_**Applies to:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9beff-105">Oinarrizko edo oinarrizko gastuen kudeaketa gastu sinpleak erregistratzeko gaitasuna da.</span><span class="sxs-lookup"><span data-stu-id="9beff-105">Basic, or lite, expense management is the capability to record simple expenses.</span></span> <span data-ttu-id="9beff-106">Proiektu baten kontrako gastuak erregistratu ditzakezu eta, ondoren, proiektuaren onartzaileak berrikusi eta onartuko ditu.</span><span class="sxs-lookup"><span data-stu-id="9beff-106">You can record expenses against a project, and then the project approver will review and approve them.</span></span>

<span data-ttu-id="9beff-107">Dynamics 365 Project Operations-eko gastuen gaitasunen inguruko informazio gehiago lortzeko, ikusi [Gastuen ikuspegi orokorra](expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9beff-107">For more information about expense capabilities in Dynamics 365 Project Operations, see [Expense overview](expense-overview.md).</span></span>

## <a name="capture-a-basic-expense"></a><span data-ttu-id="9beff-108">Hartu oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="9beff-108">Capture a basic expense</span></span>

<span data-ttu-id="9beff-109">Zure gastuak har ditzakezu, homologatzaileari bidali ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="9beff-109">You can capture your expenses so that you can submit them to the approver.</span></span>

1. <span data-ttu-id="9beff-110">Joan **Gastuak**, eta hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="9beff-110">Go to **Expenses**, and select **New**.</span></span>
2. <span data-ttu-id="9beff-111">**Gastu berria** orrian, sartu beharrezko gastuen informazioa eta hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="9beff-111">On the **New Expense** page, enter the required expense information, and then select **Save**.</span></span>

## <a name="submit-a-basic-expense"></a><span data-ttu-id="9beff-112">Bidali oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="9beff-112">Submit a basic expense</span></span>

<span data-ttu-id="9beff-113">Zure gastu guztiak jasotzen amaitu ondoren, eta horiek onartzeko prest zaudenean, bidali egin beharko dituzu.</span><span class="sxs-lookup"><span data-stu-id="9beff-113">After you've finished capturing all your expenses, and you're ready to have them approved, you must submit them.</span></span>

1. <span data-ttu-id="9beff-114">Joan **Gastuak**, eta hautatu gastu bat.</span><span class="sxs-lookup"><span data-stu-id="9beff-114">Go to **Expenses**, and select an expense.</span></span> <span data-ttu-id="9beff-115">Edo hautatu gastu guztiak goiburuko kontrol-laukia erabiliz.</span><span class="sxs-lookup"><span data-stu-id="9beff-115">Or, select all the expenses by using the check box on the header.</span></span>
2. <span data-ttu-id="9beff-116">Hautatu **Bidali**.</span><span class="sxs-lookup"><span data-stu-id="9beff-116">Select **Submit**.</span></span> <span data-ttu-id="9beff-117">Sistemak hautatutako sarrerak prozesatzen ditu eta gero gastuak onartzeko eskaerak sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="9beff-117">The system processes the selected entries and then creates expense approval requests.</span></span>

## <a name="add-an-attachment"></a><span data-ttu-id="9beff-118">Gehitu eranskin bat</span><span class="sxs-lookup"><span data-stu-id="9beff-118">Add an attachment</span></span>

<span data-ttu-id="9beff-119">Baliteke homologatzaileari zure gastuari buruzko dokumentazio osagarria eman behar izatea.</span><span class="sxs-lookup"><span data-stu-id="9beff-119">You may have to provide the approver with additional documentation about your expense.</span></span> <span data-ttu-id="9beff-120">Ordainagiria erants dezakezu gastuaren sarreraren kronograman.</span><span class="sxs-lookup"><span data-stu-id="9beff-120">You can attach a receipt in the timeline of the expense entry.</span></span> <span data-ttu-id="9beff-121">Aukeratu **Editatu** eta **Denbora-lerroa** atalean, hautatu papertxoaren ikonoa ordainagiria erantsi ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="9beff-121">Select **Edit** and in the **Timeline** section, and then select the paperclip icon to attach your receipt.</span></span>

## <a name="recall-a-basic-expense"></a><span data-ttu-id="9beff-122">Berreskuratu oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="9beff-122">Recall a basic expense</span></span>

<span data-ttu-id="9beff-123">Gastu bat akatsen bidez bidaltzen duzunean, gogora dezakezu.</span><span class="sxs-lookup"><span data-stu-id="9beff-123">When you submit an expense by mistake, you can recall it.</span></span> <span data-ttu-id="9beff-124">Gastu sarrera bat berreskuratzeko behar den denbora onarpen fasearen araberakoa da.</span><span class="sxs-lookup"><span data-stu-id="9beff-124">The time that is required to recall an expense entry depends on its approval stage.</span></span>  <span data-ttu-id="9beff-125">Onartzaileak oraindik sarrera onartu ez badu, gogora ekartzea berehala gerta daiteke.</span><span class="sxs-lookup"><span data-stu-id="9beff-125">If the approver hasn't yet approved the entry, the recall can occur immediately.</span></span> <span data-ttu-id="9beff-126">Hala ere, sarrera dagoeneko onartuta badago, onartzaileari berreskurapena onartzea eta transakzioak atzeratzea eskatzen zaio.</span><span class="sxs-lookup"><span data-stu-id="9beff-126">However, if the entry has already been approved, the approver is asked to approve the recall and reverse the transactions.</span></span>

1. <span data-ttu-id="9beff-127">Joan **Gastuak** aukerara eta, ondoren, gastuen zerrendan, hautatu gogora ekarri beharreko gastua.</span><span class="sxs-lookup"><span data-stu-id="9beff-127">Go to **Expenses**, and then, in the list of expenses, select the expense to recall.</span></span>
2. <span data-ttu-id="9beff-128">Hautatu **Berreskuratu**.</span><span class="sxs-lookup"><span data-stu-id="9beff-128">Select **Recall**.</span></span> <span data-ttu-id="9beff-129">Gastu sarrera oraindik onartu ez bada, sistemak berehala gogorarazten du.</span><span class="sxs-lookup"><span data-stu-id="9beff-129">If the expense entry hasn't yet been approved, the system immediately recalls it.</span></span> <span data-ttu-id="9beff-130">Gastu sarrera dagoeneko onartuta badago, berreskuratzeko eskaera sortzen da onartzaileari gastua alderantzikatu nahi duzula jakinarazteko.</span><span class="sxs-lookup"><span data-stu-id="9beff-130">If the expense entry has already been approved, a recall request is created to notify the approver that you want to reverse the expense.</span></span> <span data-ttu-id="9beff-131">Onartzaileak gero atzerapena egin daitekeela baieztatuko du eta sarrera itzuliko da.</span><span class="sxs-lookup"><span data-stu-id="9beff-131">The approver will then confirm that the reversal can be done, and the entry will be returned.</span></span>

## <a name="delete-a-basic-expense"></a><span data-ttu-id="9beff-132">Ezabatu oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="9beff-132">Delete a basic expense</span></span>

<span data-ttu-id="9beff-133">Oraindik bidali ez diren gastuak ezabatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="9beff-133">Expenses that haven't yet been submitted can be deleted.</span></span> <span data-ttu-id="9beff-134">Lehendik bidalitako gastua ezabatzeko, lehenik eta behin gogoratu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="9beff-134">To delete an expense that has already been submitted, you must first recall it.</span></span>

## <a name="see-also"></a><span data-ttu-id="9beff-135">Ikus baita ere</span><span class="sxs-lookup"><span data-stu-id="9beff-135">See also</span></span>

- [<span data-ttu-id="9beff-136">Onespenen ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="9beff-136">Approvals overview</span></span>](../approvals/approvals-overview.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]