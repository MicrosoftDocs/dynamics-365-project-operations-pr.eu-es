---
title: Utzi aurrez onartutako denbora- eta gastu-sarrerak
description: Gai honek aldez aurretik onartutako proiektu baten denbora- edo gastu-transakzioa uzteari buruzko informazioa eskaintzen du.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 2fc74aba2a837b7cdff55385ffa20d78c2678bb7
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748779"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="16b62-103">Utzi aurrez onartutako denbora- edo gastu-sarrerak</span><span class="sxs-lookup"><span data-stu-id="16b62-103">Cancel previously approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="16b62-104">Dynamics 365 Project Service Automation-en azken bertsioan, onuradunek aurretik onartu dituzten denbora- edo gastu-sarrerak utzi ditzakete.</span><span class="sxs-lookup"><span data-stu-id="16b62-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="16b62-105">Utzi aurrez onartutako denbora- edo gastu-sarrera</span><span class="sxs-lookup"><span data-stu-id="16b62-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="16b62-106">Jarraitu urrats hauei aurretik onartutako denbora- edo gastu-sarrera uzteko.</span><span class="sxs-lookup"><span data-stu-id="16b62-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="16b62-107">Joan **Proiektuak** \> **Nire lana** \> **Onartutakoak** atalera.</span><span class="sxs-lookup"><span data-stu-id="16b62-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="16b62-108">**Onartutakoak** zerrenda-orrian, aldatu ikuspegia **Nire iraganeko onespenak** egoerara.</span><span class="sxs-lookup"><span data-stu-id="16b62-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="16b62-109">Aurretik onartu zenituen denbora- eta gastu-sarreren zerrenda agertzen da.</span><span class="sxs-lookup"><span data-stu-id="16b62-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="16b62-110">Hautatu sarrera bat edo gehiago eta, ondoren, hautatu **Utzi onespena**.</span><span class="sxs-lookup"><span data-stu-id="16b62-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="16b62-111">Abisu mezu bat jasoko duzu.</span><span class="sxs-lookup"><span data-stu-id="16b62-111">You receive a warning message.</span></span>
4. <span data-ttu-id="16b62-112">Hautatu **Utzi** onarpena uzteko.</span><span class="sxs-lookup"><span data-stu-id="16b62-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="16b62-113">Denbora edo gastuak sartzeko baimena baliogabetzeak izan dezakeen eragina ulertu</span><span class="sxs-lookup"><span data-stu-id="16b62-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="16b62-114">Onarpena bertan behera uzten denean, bai eragiketa-eragina eta bai finantza-eragina daude.</span><span class="sxs-lookup"><span data-stu-id="16b62-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="16b62-115">Eragile operazionala</span><span class="sxs-lookup"><span data-stu-id="16b62-115">Operational impact</span></span>

<span data-ttu-id="16b62-116">Eragiketen aldean, onespena uzten denean, erregistroaren egoera berrezarri da **Zirriborroa** egoeran, eta onarpena ez da agertzen **Nire iraganeko onespenak** ikuspegian</span><span class="sxs-lookup"><span data-stu-id="16b62-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft**, and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="16b62-117">Horren ordez, utzitako onarpena agertzen da **Onarpena emateko denbora-sarrerak** ikuspegian edo **Onarpena emateko gastu-sarrerak** ikuspegian, denbora- edo gastu-sarrera izan den ala ez kontuan hartuta.</span><span class="sxs-lookup"><span data-stu-id="16b62-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="16b62-118">Gainera, erlazionatutako denbora- edo gastu-sarreren egoera aldatu egiten da **Bidalita** egoerara, eta, beraz, lotura dagokion egoera **Zirriborroa** egoera duten onarpenekin bat etorriko da.</span><span class="sxs-lookup"><span data-stu-id="16b62-118">Additionally, the status of the related time or expense entry is changed to **Submitted**, so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="16b62-119">Onartzaile gisa, **Zirriborroa** egoera duten onarpen eremu batzuk editatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="16b62-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="16b62-120">Eremu horien artean daude **Fakturazio mota** eta **Denbora-sarrerarako fakturatu daitezkeen orduak**.</span><span class="sxs-lookup"><span data-stu-id="16b62-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="16b62-121">Aldaketak egin ondoren, berriro onartu dezakezu erregistroa.</span><span class="sxs-lookup"><span data-stu-id="16b62-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="16b62-122">Bestela, sarrera ukatu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="16b62-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="16b62-123">Denbora-sarrera baten onespena ukatzen baduzu, sarreraren egoera aldatu egingo da **Itzulia** egoerara.</span><span class="sxs-lookup"><span data-stu-id="16b62-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="16b62-124">Gastu-sarrera baten onespena ukatzen baduzu, sarreraren egoera aldatu egingo da **Ukatuta** egoerara.</span><span class="sxs-lookup"><span data-stu-id="16b62-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="16b62-125">Funtzionalki, itzultutako eta ukatutako sarrerek **Zirriborroa** egoeraren bat duen sarreren antzera funtzionatuko dute.</span><span class="sxs-lookup"><span data-stu-id="16b62-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="16b62-126">Proiektuko taldekide batek sarrerako beharrezko aldaketak egin ditzake eta, ondoren, berriro bidali, onartzeko edo, bestela, ezabatu egin dezake.</span><span class="sxs-lookup"><span data-stu-id="16b62-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="16b62-127">Eragin ekonomikoa</span><span class="sxs-lookup"><span data-stu-id="16b62-127">Financial impact</span></span>

<span data-ttu-id="16b62-128">Proiektu bat ere ekonomikoki kaltetuta dago onespen bat uzten denean.</span><span class="sxs-lookup"><span data-stu-id="16b62-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="16b62-129">Lehenik eta behin, kostuari eta salmentei dagozkien datu errealak era honetara eguneratzen dira:</span><span class="sxs-lookup"><span data-stu-id="16b62-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="16b62-130">Doikuntzaren egoera ezarrita dago **Doituta** egoerara.</span><span class="sxs-lookup"><span data-stu-id="16b62-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="16b62-131">Fakturazioaren egoera ezarrita dago **Utzita** egoerara.</span><span class="sxs-lookup"><span data-stu-id="16b62-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="16b62-132">Ondoren, itzulera-sarrerak Datu errealak taulan sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="16b62-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="16b62-133">Itzulera-sarrerak sortzeko, sistemak eremuko balioak baino gehiago kopiatzen ditu jatorrizko datu errealetatik.</span><span class="sxs-lookup"><span data-stu-id="16b62-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="16b62-134">Kopiatzen ez diren balio bakarrak kantitatearen balioak dira.</span><span class="sxs-lookup"><span data-stu-id="16b62-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="16b62-135">Horren ordez itzuli egiten dira balio horiek.</span><span class="sxs-lookup"><span data-stu-id="16b62-135">These values are reversed instead.</span></span> <span data-ttu-id="16b62-136">Itzulitako datu errealak hauetarako sortzen dira: **Kostua** eta **Fakturatu gabeko salmentak**.</span><span class="sxs-lookup"><span data-stu-id="16b62-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="16b62-137">**Egokitzearen egoera** eremua, itzulitako datu errealetan, **Egokiezina** eremuan ezarrita dago eta fakturazio-egoera ezarrita dago **Utzita** egoeran.</span><span class="sxs-lookup"><span data-stu-id="16b62-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="16b62-138">Aldaketa horiek egin ondoren, proiektuan gastatu bezala erregistratzen diren diru-sarrerak eta proiektuan egindako sarreren atzerapenak denbora gehiago izango dute gertaera horiek ordezkatzen dituzten kontuak baino.</span><span class="sxs-lookup"><span data-stu-id="16b62-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>
