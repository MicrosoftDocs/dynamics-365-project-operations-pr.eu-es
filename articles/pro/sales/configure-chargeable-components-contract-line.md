---
title: Konfiguratu proiektuetan oinarritutako kontratuaren lerro bateko kobra daitezkeen osagaiak
description: Gai honetan Project Operations-eko kontratuaren lerroetan osagai kargagarriak gehitzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ddada2cb412ba7370fb0a750325a84772937d8d0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858458"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="c1196-103">Konfiguratu proiektuetan oinarritutako kontratuaren lerro bateko kobra daitezkeen osagaiak</span><span class="sxs-lookup"><span data-stu-id="c1196-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="c1196-104">_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c1196-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c1196-105">Proiektuetan oinarritutako kontratuaren lerroak osagaiak eta osagai *kargagarriak* *ditu barne*.</span><span class="sxs-lookup"><span data-stu-id="c1196-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="c1196-106">Osagai hauek honako hauen menpeko osagaiak dira:</span><span class="sxs-lookup"><span data-stu-id="c1196-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="c1196-107">Fakturazio metodoa eta bezeroen banaketak</span><span class="sxs-lookup"><span data-stu-id="c1196-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="c1196-108">Ez gainditzeko mugak</span><span class="sxs-lookup"><span data-stu-id="c1196-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="c1196-109">Proiektuan oinarritutako kontratu lerroan zehaztutako fakturen maiztasun ezarpenak</span><span class="sxs-lookup"><span data-stu-id="c1196-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="c1196-110">Sartutako osagaien azpimultzoa kargagarria gisa markatu daiteke **Fakturazio mota** eremua.</span><span class="sxs-lookup"><span data-stu-id="c1196-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="c1196-111">**Fakturazio mota** eremua kontratu lerro baten testuinguruan balio hauek onartzen dituen aukera multzoa da:</span><span class="sxs-lookup"><span data-stu-id="c1196-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="c1196-112">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-112">Chargeable</span></span>
  - <span data-ttu-id="c1196-113">Ezin da kargatu</span><span class="sxs-lookup"><span data-stu-id="c1196-113">Non-chargeable</span></span>

<span data-ttu-id="c1196-114">Osagai kargagarriak zereginetan, roletan eta transakzio kategorietan defini daitezke.</span><span class="sxs-lookup"><span data-stu-id="c1196-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="c1196-115">Kargagarritasuna proiektuko kontratu lerro bateko zereginetan definitzen da eta lerroan sartutako transakzio klase guztiei aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="c1196-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="c1196-116">Kontratuaren lerroko **Gehitu zereginak** eremua hutsik badago edo **Proiektu osoa** gisa ezarrita badago, **Kobratzeko zereginak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="c1196-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="c1196-117">Proiektuaren kontratu lerro bateko roletan definitutako kargagarritasuna **Denbora** transakzio klasea.</span><span class="sxs-lookup"><span data-stu-id="c1196-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="c1196-118">Kontratuaren lerroko **Gehitu denbora** eremua **Ez** gisa ezarrita badago, **Kobratzeko funtzioak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="c1196-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="c1196-119">Proiektuaren kontratuaren lerro bateko transakzio-kategorietan definitutako kobragarritasuna **Gastuak** transakzio klasea.</span><span class="sxs-lookup"><span data-stu-id="c1196-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="c1196-120">Kontratuaren lerroko **Gehitu gastuak** eremua **Ez** gisa ezarrita badago, **Kobratzeko kategoriak** fitxa ez da erabilgarri egongo.</span><span class="sxs-lookup"><span data-stu-id="c1196-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="c1196-121">Eguneratu proiektuaren zeregina kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="c1196-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="c1196-122">Proiektuaren zeregina kontratu-lerro zehatz batean kargagarria edo ez kargagarria izan daiteke eta horrek konfigurazio hau posible egiten du:</span><span class="sxs-lookup"><span data-stu-id="c1196-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="c1196-123">Proiektuetan oinarritutako kontratu lerroak barne hartzen badu **Denbora** eta zeregin jakin bat, **T1** kargagarri gisa lotzen zaio.</span><span class="sxs-lookup"><span data-stu-id="c1196-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="c1196-124">Horrek barne hartzen duen bigarren kontratu linea bat badago **Gastua**, T1 zeregina kontratu-lerroan lotu dezakezu kobratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="c1196-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="c1196-125">Emaitza da zereginean grabatutako denbora guztia kargagarria dela eta gastu guztiak ez direla kobratzen.</span><span class="sxs-lookup"><span data-stu-id="c1196-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="c1196-126">Ataza baten fakturazio mota konfiguratu daiteke **Zeregin kargagarriak** kontratuaren lerroaren fitxa eguneratuz **Fakturazio mota** eremua kontratu lerroaren atazen azpisarea.</span><span class="sxs-lookup"><span data-stu-id="c1196-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="c1196-127">Bestela, eguneratu dezakezu **Fakturazio mota** ataza azpisarea eremuan, zeregin bati lotutako kontratu lerroak erakusten dituen proiektu baten fakturazio konfigurazioa.</span><span class="sxs-lookup"><span data-stu-id="c1196-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="c1196-128">Eguneratu funtzioa kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="c1196-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="c1196-129">Eginkizun bat kargagarria edo ez kargagarria izan daiteke kontratu-lerro jakin batean.</span><span class="sxs-lookup"><span data-stu-id="c1196-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="c1196-130">Rol baten fakturazio mota konfiguratu daiteke **Kargatzeko rolak** kontratu lerro baten fitxa.</span><span class="sxs-lookup"><span data-stu-id="c1196-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="c1196-131">Horretarako, eguneratu **Fakturazio mota** eremuan **Kargatzeko rolak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="c1196-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="c1196-132">Eguneratu transakzio-kategoria kargagarria edo kargagarria ez den moduan</span><span class="sxs-lookup"><span data-stu-id="c1196-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="c1196-133">Transakzio-kategoria bat kargagarria edo ez kargagarria izan daiteke kontratu-lerro jakin batean.</span><span class="sxs-lookup"><span data-stu-id="c1196-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="c1196-134">Transakzio baten fakturazio mota konfiguratu daiteke **Kargatzeko kategoriak** kontratuaren lerro batean oinarritutako proiektatearen fitxa.</span><span class="sxs-lookup"><span data-stu-id="c1196-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="c1196-135">Horretarako, eguneratu **Fakturazio mota** eremuan **Kargatzeko kategoriak** azpisarea.</span><span class="sxs-lookup"><span data-stu-id="c1196-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="c1196-136">Kargagarritasuna ebatzi</span><span class="sxs-lookup"><span data-stu-id="c1196-136">Resolve chargeability</span></span>

<span data-ttu-id="c1196-137">Denborarako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="c1196-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="c1196-138">**Denbora** kontratu-lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="c1196-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="c1196-139">**Rola** kontratu-linean kargatzeko moduan konfiguratuta dago.</span><span class="sxs-lookup"><span data-stu-id="c1196-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="c1196-140">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** kontratu lerroan.</span><span class="sxs-lookup"><span data-stu-id="c1196-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="c1196-141">Hiru gauza hauek egia badira, zeregina kargatzeko moduan konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="c1196-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="c1196-142">Gasturako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="c1196-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="c1196-143">**Gastua** kontratu-lerroan sartzen da</span><span class="sxs-lookup"><span data-stu-id="c1196-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="c1196-144">**Transakzioaren kategoria** kontratu-linean kargatzeko moduan konfiguratuta dago</span><span class="sxs-lookup"><span data-stu-id="c1196-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="c1196-145">**Zereginak barne** ezarrita dago **Aukeratutako zeregina** kontratu lerroan</span><span class="sxs-lookup"><span data-stu-id="c1196-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="c1196-146">Hiru gauza hauek egia badira, **Zeregina** kargatzeko moduan konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="c1196-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="c1196-147">Materialerako sortutako aurrekontua edo benetakoa soilik kobratuko da:</span><span class="sxs-lookup"><span data-stu-id="c1196-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="c1196-148">**Materialak** kontratu-lerroan sartzen da</span><span class="sxs-lookup"><span data-stu-id="c1196-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="c1196-149">**Zereginak barne** ezarrita dago **Aukeratutako zereginak** kontratu lerroan</span><span class="sxs-lookup"><span data-stu-id="c1196-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="c1196-150">Bi gauza hauek egia badira, **Zeregina** kargatzeko moduan konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="c1196-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-151">
                    <strong>Denbora barne</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c1196-152">
                    <strong>Gastua barne</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c1196-153">
                    <strong>Materialak barne</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="c1196-154">
                    <strong>Gehitutako zereginak</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-155">
                    <strong>Funtzioa</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-156">
                    <strong>Kategoria</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-157">
                    <strong>Ataza</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="c1196-158">
                    <strong>Kargagarritasunaren eragina</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-159">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-160">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-161">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-162">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c1196-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-163">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-164">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-165">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-166">Fakturazioa denbora errealean: <strong>Kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-167">Fakturazio mota benetako gastuan: <strong>Kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-168">Fakturazio mota benetako materialean: <strong>Kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-169">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-170">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-171">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-172">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c1196-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-173">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-174">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-175">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-176">Fakturazioa denbora errealean: <strong>Kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-177">Fakturazio mota benetako gastuan: <strong>Kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-178">Fakturazio mota benetako materialean: <strong>Kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-179">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-180">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-181">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-182">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c1196-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-183">
                    <strong>Ezin da kargatu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-184">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-185">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-186">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-187">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c1196-188">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-189">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-190">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-191">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-192">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c1196-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-193">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-194">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-195">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-196">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-197">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-198">Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-199">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-200">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-201">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-202">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c1196-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-203">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-204">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-205">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-206">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-207">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-208">Fakturazio mota benetako materialean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-209">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-210">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-211">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-212">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="c1196-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-213">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-214">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-215">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-216">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-217">Fakturazio mota benetako gastuan: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-218">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-219">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-220">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-221">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-222">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c1196-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-223">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-224">
                    <strong>Kobra daiteke</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-225">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-226">Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-227">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c1196-228">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-229">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-230">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-231">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-232">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c1196-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-233">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-234">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-235">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-236">Fakturazioa denbora errealean: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-237">Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-238">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-239">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c1196-240">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-241">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-242">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c1196-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-243">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-244">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-245">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-246">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c1196-247">Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-248">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-249">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="c1196-250">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="c1196-251">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-252">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c1196-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-253">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-254">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-255">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-256">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-257">Fakturazio mota benetako gastuan: <strong>Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-258">Fakturazio mota benetako materialean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-259">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-260">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c1196-261">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-262">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c1196-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-263">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-264">Kobra daiteke</span><span class="sxs-lookup"><span data-stu-id="c1196-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-265">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-266">Fakturazioa denbora errealean: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c1196-267">Fakturazio mota benetako gastuan: Kargagarria</span><span class="sxs-lookup"><span data-stu-id="c1196-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="c1196-268">Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="c1196-269">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="c1196-270">Yes</span><span class="sxs-lookup"><span data-stu-id="c1196-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="c1196-271">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="c1196-272">Proiektu osoa</span><span class="sxs-lookup"><span data-stu-id="c1196-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="c1196-273">
                    <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="c1196-274">
                    <strong>Ezin da kargatu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="c1196-275">Ezin da ezarri</span><span class="sxs-lookup"><span data-stu-id="c1196-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="c1196-276">Fakturazioa denbora errealean: <strong>Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-277">Fakturazio mota benetako gastuan: <strong> Ez-kargagarria</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="c1196-278">Fakturazio mota benetako materialean: <strong> Ez dago erabilgarri</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c1196-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
