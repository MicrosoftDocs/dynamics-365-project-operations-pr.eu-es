---
title: Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak
description: Gai honek proiektuan oinarritutako aurrekontu lerro batean kargagarriak eta kargagarriak ez diren osagaiak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858278"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="e1ec6-103">Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak</span><span class="sxs-lookup"><span data-stu-id="e1ec6-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="e1ec6-104">_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_</span><span class="sxs-lookup"><span data-stu-id="e1ec6-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e1ec6-105">Proiektuetan oinarritutako eskaintzaren lerroak *barne* osagaiak eta *kargagarriak* osagaiak kontzeptuak ditu.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="e1ec6-106">Sartutako osagaien menpe daude:</span><span class="sxs-lookup"><span data-stu-id="e1ec6-106">Included components are subject to:</span></span>

  - <span data-ttu-id="e1ec6-107">Fakturazio metodoa eta bezeroen banaketak</span><span class="sxs-lookup"><span data-stu-id="e1ec6-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="e1ec6-108">Ez gainditzeko mugak</span><span class="sxs-lookup"><span data-stu-id="e1ec6-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="e1ec6-109">Proiektuan oinarritutako eskaintzaren lerroan zehaztutako fakturen maiztasun ezarpenak</span><span class="sxs-lookup"><span data-stu-id="e1ec6-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="e1ec6-110">Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="e1ec6-111">**Fakturazio mota** eremua eskaintzaren lerro baten testuinguruan balio hauek onartzen dituen aukera multzoa da:</span><span class="sxs-lookup"><span data-stu-id="e1ec6-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="e1ec6-112">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-112">Chargeable</span></span>
  - <span data-ttu-id="e1ec6-113">Ezin da kargatu</span><span class="sxs-lookup"><span data-stu-id="e1ec6-113">Non-chargeable</span></span>

<span data-ttu-id="e1ec6-114">Osagai kargagarriak zereginetan, roletan eta transakzio kategorietan defini daitezke.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="e1ec6-115">Kargagarritasuna eskaintzaren kontratu lerro bateko zereginetan definitzen da eta lerroan sartutako transakzio klase guztiei aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="e1ec6-116">**Gehitu zereginak** eremua **Proiektu osoa** bada edo hutsik badago, **Kobratzeko zereginak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="e1ec6-117">Eskaintzaren lerro bateko roletan definitutako kargagarritasuna **Denbora** transakzio klasea.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="e1ec6-118">Eremuan, **Gehitu denbora** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="e1ec6-119">Eskaintzaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="e1ec6-120">Eremuan, **Gehitu gastuak** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="e1ec6-121">Eguneratu proiektuaren zeregina kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="e1ec6-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="e1ec6-122">Proiektuaren zeregina proiektuetan oinarritutako eskaintzaren lerro zehatz baten testuinguruan kargagarria edo ez kargagarria izan daiteke eta horrek konfigurazio hau posible egiten du.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="e1ec6-123">Proiektuan oinarritutako aurrekontu lerroak biltzen badu **Denbora** eta zeregina **T1**, zeregina aurrekontu lerroarekin lotzen da kobratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="e1ec6-124">Horrek barne hartzen duen bigarren eskaintzaren lerro bat badago **Gastuak**, **T1** zeregina eskaintzaren lerroan lotu dezakezu kobratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="e1ec6-125">Emaitza da zereginean grabatutako denbora guztia kargagarria dela eta kargagarriak ez diren zereginetako gastu guztiak ez direla erregistratzen.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="e1ec6-126">Ataza baten fakturazio mota konfiguratu daiteke **Zeregin kargagarriak** proiektuan oinarritutako eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Kontratu lerroaren atazak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="e1ec6-127">Bestela, eguneratu dezakezu **Fakturazio mota** eremuko proiektu-zereginaren fakturazio motaren azpisarea eremuan, zeregin bati lotutako kontratu lerroak erakusten dituen proiektu baten fakturazio konfigurazioa.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="e1ec6-128">Eguneratu funtzioa kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="e1ec6-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="e1ec6-129">Eginkizun bat kargagarria edo ez kargagarria izan daiteke proiektuan oinarritutako aurrekontu lerro jakin baten testuinguruan.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="e1ec6-130">Funtzioa baten fakturazio mota konfiguratu daiteke **Funtzio kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Funtzio kargagarriak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="e1ec6-131">Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="e1ec6-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="e1ec6-132">Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke eskaintzaren lerro jakin batean.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="e1ec6-133">Transakzioaren fakturazio mota konfiguratu daiteke **Kategoria kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Kategoria kargagarriak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="e1ec6-134">Kargagarritasuna ebatzi</span><span class="sxs-lookup"><span data-stu-id="e1ec6-134">Resolve chargeability</span></span>
<span data-ttu-id="e1ec6-135">Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="e1ec6-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="e1ec6-136">**Denbora** eskaintza-lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="e1ec6-137">**Rola** eskaintza-linean kargatzeko moduan konfiguratuta dago.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="e1ec6-138">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="e1ec6-139">Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="e1ec6-140">Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="e1ec6-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="e1ec6-141">**Gastua** eskaintza-lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="e1ec6-142">**Transakzioaren kategoria** eskaintza-linean kargatzeko moduan konfiguratuta dago.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="e1ec6-143">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="e1ec6-144">Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="e1ec6-145">Materialerako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="e1ec6-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="e1ec6-146">**Materialak** eskaintza-lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="e1ec6-147">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="e1ec6-148">Bi gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="e1ec6-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-149">
                    <strong>Denbora barne</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="e1ec6-150">
                    <strong>Gastua barne</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="e1ec6-151">
                    <strong>Materialak barne</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="e1ec6-152">
                    <strong>Gehitutako zereginak</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-153">
                    <strong>Funtzioa</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-154">
                    <strong>Kategoria</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-155">
                    <strong>Ataza</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="e1ec6-156">
                    <strong>Kargagarritasunaren eragina</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-157">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-158">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-159">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-160">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="e1ec6-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-161">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-162">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-163">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-164">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-165">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-166">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-167">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-168">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-169">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-170">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="e1ec6-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-171">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-172">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-173">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-174">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-175">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-176">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-177">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-178">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-179">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-180">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="e1ec6-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-181">
                    <strong>Ezin da kargatu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-182">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-183">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-184">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-185">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-186">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-187">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-188">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-189">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-190">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="e1ec6-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-191">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-192">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-193">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-194">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-195">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-196">Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-197">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-198">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-199">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-200">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="e1ec6-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-201">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-202">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-203">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-204">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-205">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-206">Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-207">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-208">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-209">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-210">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="e1ec6-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-211">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-212">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-213">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-214">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-215">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-216">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-218">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-219">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-220">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="e1ec6-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-221">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-222">
                    <strong>Kobra daiteke</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-223">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-224">Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-225">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-226">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-228">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-229">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-230">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="e1ec6-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-231">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-232">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-233">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-234">Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-235">Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-236">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-237">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="e1ec6-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-239">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-240">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="e1ec6-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-241">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-242">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-243">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-244">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-245">Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-246">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-247">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="e1ec6-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="e1ec6-249">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-250">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="e1ec6-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-251">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-252">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-253">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-254">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-255">Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-256">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-257">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-258">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="e1ec6-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-260">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="e1ec6-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-261">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-262">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="e1ec6-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-263">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-264">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-265">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="e1ec6-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="e1ec6-266">Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="e1ec6-267">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="e1ec6-268">Yes</span><span class="sxs-lookup"><span data-stu-id="e1ec6-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="e1ec6-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="e1ec6-270">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="e1ec6-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="e1ec6-271">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="e1ec6-272">
                    <strong>Ezin da kargatu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="e1ec6-273">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="e1ec6-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="e1ec6-274">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-275">Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="e1ec6-276">Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e1ec6-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
