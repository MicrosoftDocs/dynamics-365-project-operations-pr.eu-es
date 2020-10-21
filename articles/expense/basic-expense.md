---
title: Oinarrizko gastuen sarrera (arina)
description: Gai honek lite inplementazio batean gastuen sarrerarekin lan egiteko moduari buruzko informazioa eskaintzen du.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 746d5d9ff56222e7d6b9b6e264db75d5814365c7
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965718"
---
# <a name="expense-entry-lite"></a><span data-ttu-id="6410b-103">Oinarrizko gastuen sarrera (arina)</span><span class="sxs-lookup"><span data-stu-id="6410b-103">Expense entry (lite)</span></span>

<span data-ttu-id="6410b-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="6410b-104">_**Applies to:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6410b-105">Oinarrizko edo oinarrizko gastuen kudeaketa gastu sinpleak erregistratzeko gaitasuna da.</span><span class="sxs-lookup"><span data-stu-id="6410b-105">Basic, or lite, expense management is the capability to record simple expenses.</span></span> <span data-ttu-id="6410b-106">Proiektu baten kontrako gastuak erregistratu ditzakezu eta, ondoren, proiektuaren onartzaileak berrikusi eta onartuko ditu.</span><span class="sxs-lookup"><span data-stu-id="6410b-106">You can record expenses against a project, and then the project approver will review and approve them.</span></span>

<span data-ttu-id="6410b-107">Dynamics 365 Project Operations-en gastuen gaitasunei buruzko informazio gehiago lortzeko, ikusi [Gastuen ikuspegi orokorra](expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="6410b-107">For more information about expense capabilities in Dynamics 365 Project Operations, see [Expense overview](expense-overview.md).</span></span>

## <a name="capture-a-basic-expense"></a><span data-ttu-id="6410b-108">Hartu oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="6410b-108">Capture a basic expense</span></span>

<span data-ttu-id="6410b-109">Zure gastuak har ditzakezu, homologatzaileari bidali ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="6410b-109">You can capture your expenses so that you can submit them to the approver.</span></span>

1. <span data-ttu-id="6410b-110">Joan **Gastuak**, eta hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="6410b-110">Go to **Expenses**, and select **New**.</span></span>
2. <span data-ttu-id="6410b-111">**Gastu berria** orrian, sartu beharrezko gastuen informazioa eta hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="6410b-111">On the **New Expense** page, enter the required expense information, and then select **Save**.</span></span>

## <a name="submit-a-basic-expense"></a><span data-ttu-id="6410b-112">Bidali oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="6410b-112">Submit a basic expense</span></span>

<span data-ttu-id="6410b-113">Zure gastu guztiak jasotzen amaitu ondoren, eta horiek onartzeko prest zaudenean, bidali egin beharko dituzu.</span><span class="sxs-lookup"><span data-stu-id="6410b-113">After you've finished capturing all your expenses, and you're ready to have them approved, you must submit them.</span></span>

1. <span data-ttu-id="6410b-114">Joan **Gastuak**, eta hautatu gastu bat.</span><span class="sxs-lookup"><span data-stu-id="6410b-114">Go to **Expenses**, and select an expense.</span></span> <span data-ttu-id="6410b-115">Edo hautatu gastu guztiak goiburuko kontrol-laukia erabiliz.</span><span class="sxs-lookup"><span data-stu-id="6410b-115">Or, select all the expenses by using the check box on the header.</span></span>
2. <span data-ttu-id="6410b-116">Hautatu **Bidali**.</span><span class="sxs-lookup"><span data-stu-id="6410b-116">Select **Submit**.</span></span> <span data-ttu-id="6410b-117">Sistemak hautatutako sarrerak prozesatzen ditu eta gero gastuak onartzeko eskaerak sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="6410b-117">The system processes the selected entries and then creates expense approval requests.</span></span>

## <a name="recall-a-basic-expense"></a><span data-ttu-id="6410b-118">Berreskuratu oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="6410b-118">Recall a basic expense</span></span>

<span data-ttu-id="6410b-119">Gastu bat akatsen bidez bidaltzen duzunean, gogora dezakezu.</span><span class="sxs-lookup"><span data-stu-id="6410b-119">When you submit an expense by mistake, you can recall it.</span></span> <span data-ttu-id="6410b-120">Gastu sarrera bat berreskuratzeko behar den denbora onarpen fasearen araberakoa da.</span><span class="sxs-lookup"><span data-stu-id="6410b-120">The time that is required to recall an expense entry depends on its approval stage.</span></span>  <span data-ttu-id="6410b-121">Onartzaileak oraindik sarrera onartu ez badu, gogora ekartzea berehala gerta daiteke.</span><span class="sxs-lookup"><span data-stu-id="6410b-121">If the approver hasn't yet approved the entry, the recall can occur immediately.</span></span> <span data-ttu-id="6410b-122">Hala ere, sarrera dagoeneko onartuta badago, onartzaileari berreskurapena onartzea eta transakzioak atzeratzea eskatzen zaio.</span><span class="sxs-lookup"><span data-stu-id="6410b-122">However, if the entry has already been approved, the approver is asked to approve the recall and reverse the transactions.</span></span>

1. <span data-ttu-id="6410b-123">Joan **Gastuak** aukerara eta, ondoren, gastuen zerrendan, hautatu gogora ekarri beharreko gastua.</span><span class="sxs-lookup"><span data-stu-id="6410b-123">Go to **Expenses**, and then, in the list of expenses, select the expense to recall.</span></span>
2. <span data-ttu-id="6410b-124">Hautatu **Berreskuratu**.</span><span class="sxs-lookup"><span data-stu-id="6410b-124">Select **Recall**.</span></span> <span data-ttu-id="6410b-125">Gastu sarrera oraindik onartu ez bada, sistemak berehala gogorarazten du.</span><span class="sxs-lookup"><span data-stu-id="6410b-125">If the expense entry hasn't yet been approved, the system immediately recalls it.</span></span> <span data-ttu-id="6410b-126">Gastu sarrera dagoeneko onartuta badago, berreskuratzeko eskaera sortzen da onartzaileari gastua alderantzikatu nahi duzula jakinarazteko.</span><span class="sxs-lookup"><span data-stu-id="6410b-126">If the expense entry has already been approved, a recall request is created to notify the approver that you want to reverse the expense.</span></span> <span data-ttu-id="6410b-127">Onartzaileak gero atzerapena egin daitekeela baieztatuko du eta sarrera itzuliko da.</span><span class="sxs-lookup"><span data-stu-id="6410b-127">The approver will then confirm that the reversal can be done, and the entry will be returned.</span></span>

## <a name="delete-a-basic-expense"></a><span data-ttu-id="6410b-128">Ezabatu oinarrizko gastua</span><span class="sxs-lookup"><span data-stu-id="6410b-128">Delete a basic expense</span></span>

<span data-ttu-id="6410b-129">Oraindik bidali ez diren gastuak ezabatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="6410b-129">Expenses that haven't yet been submitted can be deleted.</span></span> <span data-ttu-id="6410b-130">Lehendik bidalitako gastua ezabatzeko, lehenik eta behin gogoratu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="6410b-130">To delete an expense that has already been submitted, you must first recall it.</span></span>

## <a name="see-also"></a><span data-ttu-id="6410b-131">Ikus baita ere</span><span class="sxs-lookup"><span data-stu-id="6410b-131">See also</span></span>

- [<span data-ttu-id="6410b-132">Onespenen ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="6410b-132">Approvals overview</span></span>](../approvals/approvals-overview.md)
