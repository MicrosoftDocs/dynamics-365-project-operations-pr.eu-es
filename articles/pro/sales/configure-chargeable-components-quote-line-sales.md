---
title: Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak
description: Gai honek proiektuan oinarritutako aurrekontu lerro batean kargagarriak eta kargagarriak ez diren osagaiak konfiguratzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c933a3800aae72624dbcbe3f06df20e5981d74d4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003751"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="c817e-103">Konfiguratu eskaintzaren lerro bateko kobra daitezkeen osagaiak</span><span class="sxs-lookup"><span data-stu-id="c817e-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="c817e-104">_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c817e-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c817e-105">Proiektuetan oinarritutako eskaintzaren lerroak *barne* osagaiak eta *kargagarriak* osagaiak kontzeptuak ditu.</span><span class="sxs-lookup"><span data-stu-id="c817e-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="c817e-106">Sartutako osagaien menpe daude:</span><span class="sxs-lookup"><span data-stu-id="c817e-106">Included components are subject to:</span></span>

  - <span data-ttu-id="c817e-107">Fakturazio metodoa eta bezeroen banaketak</span><span class="sxs-lookup"><span data-stu-id="c817e-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="c817e-108">Ez gainditzeko mugak</span><span class="sxs-lookup"><span data-stu-id="c817e-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="c817e-109">Proiektuan oinarritutako eskaintzaren lerroan zehaztutako fakturen maiztasun ezarpenak</span><span class="sxs-lookup"><span data-stu-id="c817e-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="c817e-110">Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua.</span><span class="sxs-lookup"><span data-stu-id="c817e-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="c817e-111">**Fakturazio mota** eremua eskaintzaren lerro baten testuinguruan balio hauek onartzen dituen aukera multzoa da:</span><span class="sxs-lookup"><span data-stu-id="c817e-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="c817e-112">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-112">Chargeable</span></span>
  - <span data-ttu-id="c817e-113">Ezin da kargatu</span><span class="sxs-lookup"><span data-stu-id="c817e-113">Non-chargeable</span></span>

<span data-ttu-id="c817e-114">Osagai kargagarriak zereginetan, roletan eta transakzio kategorietan defini daitezke.</span><span class="sxs-lookup"><span data-stu-id="c817e-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="c817e-115">Kargagarritasuna eskaintzaren kontratu lerro bateko zereginetan definitzen da eta lerroan sartutako transakzio klase guztiei aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="c817e-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="c817e-116">**Gehitu zereginak** eremua **Proiektu osoa** bada edo hutsik badago, **Kobratzeko zereginak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="c817e-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="c817e-117">Eskaintzaren lerro bateko roletan definitutako kargagarritasuna **Denbora** transakzio klasea.</span><span class="sxs-lookup"><span data-stu-id="c817e-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="c817e-118">Eremuan, **Gehitu denbora** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="c817e-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="c817e-119">Eskaintzaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea.</span><span class="sxs-lookup"><span data-stu-id="c817e-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="c817e-120">Eremuan, **Gehitu gastuak** eremua **Ez** gisa ezarrita badago proiektuaren kuota lerroan, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="c817e-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="c817e-121">Eguneratu proiektuaren zeregina kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="c817e-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="c817e-122">Proiektuaren zeregina proiektuetan oinarritutako eskaintzaren lerro zehatz baten testuinguruan kargagarria edo ez kargagarria izan daiteke eta horrek konfigurazio hau posible egiten du.</span><span class="sxs-lookup"><span data-stu-id="c817e-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="c817e-123">Proiektuan oinarritutako aurrekontu lerroak biltzen badu **Denbora** eta zeregina **T1**, zeregina aurrekontu lerroarekin lotzen da kobratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="c817e-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="c817e-124">Horrek barne hartzen duen bigarren eskaintzaren lerro bat badago **Gastuak**, **T1** zeregina eskaintzaren lerroan lotu dezakezu kobratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="c817e-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="c817e-125">Emaitza da zereginean grabatutako denbora guztia kargagarria dela eta kargagarriak ez diren zereginetako gastu guztiak ez direla erregistratzen.</span><span class="sxs-lookup"><span data-stu-id="c817e-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="c817e-126">Ataza baten fakturazio mota konfiguratu daiteke **Zeregin kargagarriak** proiektuan oinarritutako eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Kontratu lerroaren atazak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="c817e-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="c817e-127">Bestela, eguneratu dezakezu **Fakturazio mota** eremuko proiektu-zereginaren fakturazio motaren azpisarea eremuan, zeregin bati lotutako kontratu lerroak erakusten dituen proiektu baten fakturazio konfigurazioa.</span><span class="sxs-lookup"><span data-stu-id="c817e-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="c817e-128">Eguneratu funtzioa kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="c817e-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="c817e-129">Eginkizun bat kargagarria edo ez kargagarria izan daiteke proiektuan oinarritutako aurrekontu lerro jakin baten testuinguruan.</span><span class="sxs-lookup"><span data-stu-id="c817e-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="c817e-130">Funtzioa baten fakturazio mota konfiguratu daiteke **Funtzio kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Funtzio kargagarriak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="c817e-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="c817e-131">Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="c817e-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="c817e-132">Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke eskaintzaren lerro jakin batean.</span><span class="sxs-lookup"><span data-stu-id="c817e-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="c817e-133">Transakzioaren fakturazio mota konfiguratu daiteke **Kategoria kargagarriak** eskaintzaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua **Kategoria kargagarriak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="c817e-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="c817e-134">Kargagarritasuna ebatzi</span><span class="sxs-lookup"><span data-stu-id="c817e-134">Resolve chargeability</span></span>
<span data-ttu-id="c817e-135">Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="c817e-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="c817e-136">**Denbora** eskaintza-lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="c817e-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="c817e-137">**Rola** eskaintza-linean kargatzeko moduan konfiguratuta dago.</span><span class="sxs-lookup"><span data-stu-id="c817e-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="c817e-138">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.</span><span class="sxs-lookup"><span data-stu-id="c817e-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="c817e-139">Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="c817e-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="c817e-140">Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="c817e-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="c817e-141">**Gastua** eskaintza-lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="c817e-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="c817e-142">**Transakzioaren kategoria** eskaintza-linean kargatzeko moduan konfiguratuta dago.</span><span class="sxs-lookup"><span data-stu-id="c817e-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="c817e-143">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.</span><span class="sxs-lookup"><span data-stu-id="c817e-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="c817e-144">Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="c817e-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="c817e-145">Materialerako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="c817e-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="c817e-146">**Materialak** eskaintza-lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="c817e-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="c817e-147">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** eskaintza-lerroan.</span><span class="sxs-lookup"><span data-stu-id="c817e-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="c817e-148">Bi gauza hauek egia badira, **Zeregina** kargatzeko moduan ere konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="c817e-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-149">
                    <strong>Denbora barne</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c817e-150">
                    <strong>Gastua barne</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c817e-151">
                    <strong>Materialak barne</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="c817e-152">
                    <strong>Gehitutako zereginak</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-153">
                    <strong>Funtzioa</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-154">
                    <strong>Kategoria</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-155">
                    <strong>Ataza</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="c817e-156">
                    <strong>Kargagarritasunaren eragina</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-157">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-158">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-159">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-160">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c817e-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-161">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-162">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-163">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-164">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-165">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-166">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-167">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-168">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-169">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-170">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c817e-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-171">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-172">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-173">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-174">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-175">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-176">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-177">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-178">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-179">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-180">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c817e-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-181">
                    <strong>Ezin da kargatu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-182">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-183">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-184">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-185">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-186">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-187">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-188">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-189">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-190">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c817e-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-191">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-192">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-193">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-194">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-195">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-196">Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-197">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-198">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-199">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-200">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c817e-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-201">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-202">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-203">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-204">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-205">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-206">Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-207">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-208">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-209">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-210">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c817e-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-211">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-212">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-213">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-214">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-215">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-216">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-218">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-219">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-220">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c817e-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-221">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-222">
                    <strong>Kobra daiteke</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-223">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-224">Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-225">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-226">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-228">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-229">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-230">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c817e-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-231">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-232">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-233">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-234">Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-235">Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-236">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-237">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c817e-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-239">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-240">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c817e-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-241">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-242">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-243">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-244">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-245">Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-246">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-247">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c817e-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c817e-249">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-250">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c817e-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-251">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-252">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-253">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-254">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-255">Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-256">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-257">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-258">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c817e-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-260">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c817e-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-261">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-262">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c817e-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-263">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-264">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-265">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c817e-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c817e-266">Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c817e-267">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c817e-268">Yes</span><span class="sxs-lookup"><span data-stu-id="c817e-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c817e-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c817e-270">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c817e-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c817e-271">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c817e-272">
                    <strong>Ezin da kargatu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c817e-273">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c817e-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c817e-274">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-275">Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c817e-276">Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c817e-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
