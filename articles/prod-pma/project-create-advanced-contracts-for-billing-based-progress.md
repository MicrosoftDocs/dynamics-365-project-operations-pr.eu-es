---
title: Sortu fakturazioaren araberako aurrerapenerako kontratu aurreratuak
description: Gai honetan proiektuen kontratuak nola sortu azaltzen da, bezeroentzako fakturak sortu ahal izateko, egindako lanaren ehunekoan oinarrituta.
author: RadhikaRS
ms.date: 03/26/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 3b445488100e0a8335a05505405953b173ff836c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999656"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="7e589-103">Sortu fakturazioaren araberako aurrerapenerako kontratu aurreratuak</span><span class="sxs-lookup"><span data-stu-id="7e589-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="7e589-104">Gai honetan proiektuen kontratuak nola sortu azaltzen da, bezeroentzako fakturak sortu ahal izateko, egindako lanaren ehunekoan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="7e589-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="7e589-105">Fakturen zenbatekoak automatikoki kalkulatzen dira proiektu baterako konfiguratutako aurrekontu lanen kategorietarako.</span><span class="sxs-lookup"><span data-stu-id="7e589-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="7e589-106">Fakturaren denbora ezartzen da bezeroarekin proiektuaren kontratua negoziatzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="7e589-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="7e589-107">Erabili gai honetako prozedurak kontratua, lotutako proiektu bat eta proiektuarentzako konfiguratu dituzun aurrekontuen lan-kategorien fakturen zenbatekoak kalkulatzen dituzten fakturazio-arauak ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="7e589-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="7e589-108">Kontratua eta proiektua sortu ondoren, proiektuaren xehetasunak konfigura ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="7e589-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="7e589-109">Adibidez, jarduerak definitu eta langileak proiektuan esleitu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="7e589-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="7e589-110">Adibidez</span><span class="sxs-lookup"><span data-stu-id="7e589-110">Example</span></span>

<span data-ttu-id="7e589-111">Zure erakundea softwarea garatzeko enpresa da.</span><span class="sxs-lookup"><span data-stu-id="7e589-111">Your organization is a software development firm.</span></span> <span data-ttu-id="7e589-112">Onartzen duzu bezeroarentzako nominaren kontabilitate paketea garatzea, guztira 20.000 dolar (USD) kuotaren truke.</span><span class="sxs-lookup"><span data-stu-id="7e589-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="7e589-113">Zure erakundeak ados dago bezeroari fakturatzea proiektuaren ehuneko zehatzak burutu ahala.</span><span class="sxs-lookup"><span data-stu-id="7e589-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="7e589-114">Proiektuen kategoria hauek konfiguratzen dituzu lanerako, fakturazio prozesuan erabil ditzazun:</span><span class="sxs-lookup"><span data-stu-id="7e589-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="7e589-115">Aholkularitza</span><span class="sxs-lookup"><span data-stu-id="7e589-115">Consulting</span></span>
- <span data-ttu-id="7e589-116">Diseinua</span><span class="sxs-lookup"><span data-stu-id="7e589-116">Design</span></span>
- <span data-ttu-id="7e589-117">Instalazioa</span><span class="sxs-lookup"><span data-stu-id="7e589-117">Installation</span></span>

<span data-ttu-id="7e589-118">Fakturazio-arauak konfiguratzen dituzu kategoria bakoitzerako egindako proiektuaren lan portzentajearen fakturen zenbatekoak automatikoki kalkulatzen dituztenak.</span><span class="sxs-lookup"><span data-stu-id="7e589-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="7e589-119">Aurrekontu kudeatzaileak proiektuen kategorietarako aurrekontua sortzen du.</span><span class="sxs-lookup"><span data-stu-id="7e589-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="7e589-120">Egindako lanaren zenbatekoa automatikoki kalkulatzen da benetako lanaren ehuneko gisa, aurrekontuekin alderatuta.</span><span class="sxs-lookup"><span data-stu-id="7e589-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e589-121">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="7e589-121">Prerequisites</span></span>

<span data-ttu-id="7e589-122">Fakturazio arauak erabiltzen dituen proiektua sortu aurretik, fakturazio arauen zenbaki sekuentziak eta aurrerapen fakturazioak argitaratzeko erabiltzen den kuota egunkaria ezarri behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="7e589-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="7e589-123">Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Proiektuen kudeaketa eta kontabilitate parametroak**.</span><span class="sxs-lookup"><span data-stu-id="7e589-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="7e589-124">**Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, **Zenbaki sekuentziak** fitxa, konfiguratu fakturazio arauak sortzen direnean erabili nahi duzun zenbaki sekuentzia.</span><span class="sxs-lookup"><span data-stu-id="7e589-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="7e589-125">Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Egunkariak** \> **Kostua**.</span><span class="sxs-lookup"><span data-stu-id="7e589-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="7e589-126">**Tasen aldizkaria** orrialdean, hautatu **Berria**, eta idatzi aldizkariaren izena.</span><span class="sxs-lookup"><span data-stu-id="7e589-126">On the **Fee journal** page, select **New**, and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="7e589-127">Sortu aurrerapen fakturazioetarako kontratua</span><span class="sxs-lookup"><span data-stu-id="7e589-127">Create a contract for progress billings</span></span>

<span data-ttu-id="7e589-128">Erabili prozedura hau prezio finko baterako proiektuaren kontratua sortzeko.</span><span class="sxs-lookup"><span data-stu-id="7e589-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="7e589-129">Proiektuaren faktura sortzen duzu proiektuan amaitutako lana ehuneko jakin batera iristen denean.</span><span class="sxs-lookup"><span data-stu-id="7e589-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="7e589-130">Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu-kontratuak**.</span><span class="sxs-lookup"><span data-stu-id="7e589-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="7e589-131">**Proiektuaren kontratuak** orrian, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="7e589-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="7e589-132">**Proiektuaren kontratu berria** elkarrizketa-koadroan, ezarri eremu hauek:</span><span class="sxs-lookup"><span data-stu-id="7e589-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="7e589-133">**Izena**</span><span class="sxs-lookup"><span data-stu-id="7e589-133">**Name**</span></span>
    - <span data-ttu-id="7e589-134">**Funts mota**</span><span class="sxs-lookup"><span data-stu-id="7e589-134">**Funding type**</span></span>
    - <span data-ttu-id="7e589-135">**Finantzaketa iturria**</span><span class="sxs-lookup"><span data-stu-id="7e589-135">**Funding source**</span></span>
    - <span data-ttu-id="7e589-136">**Salmenten moneta** - Lehenespenez, moneta hau proiektuaren kontratuarekin lotutako bezeroen fakturetarako erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="7e589-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="7e589-137">Hala ere, salmenten moneta alda dezakezu bezeroaren faktura jakin batean.</span><span class="sxs-lookup"><span data-stu-id="7e589-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="7e589-138">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="7e589-138">Select **OK**.</span></span> <span data-ttu-id="7e589-139">Informazioa fitxategiaren goiburuan kopiatzen da **Proiektuen kontratuak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="7e589-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="7e589-140">**Proiektuen kontratuak** orrialdean, bete proiektuarentzako beharrezko gainerako informazioa.</span><span class="sxs-lookup"><span data-stu-id="7e589-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="7e589-141">Sortu aurrerapen fakturazioetarako proiektua</span><span class="sxs-lookup"><span data-stu-id="7e589-141">Create a project for progress billings</span></span>

<span data-ttu-id="7e589-142">Jarraitu urrats hauek proiektu bat eta proiektuaren kontratuarekin lotura duten azpiproiektuak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="7e589-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="7e589-143">Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="7e589-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="7e589-144">**Proiektu denak** orrian, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="7e589-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="7e589-145">**Proiektu berria** elkarrizketa-koadroan, **Proiektu mota** eremuan, hautatu **Denbora eta materiala**.</span><span class="sxs-lookup"><span data-stu-id="7e589-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="7e589-146">Hautatu proiektu-taldea.</span><span class="sxs-lookup"><span data-stu-id="7e589-146">Select a project group.</span></span> <span data-ttu-id="7e589-147">Proiektu talde batek taldeari esleitutako proiektuen argitaratze informazioa definitzen du.</span><span class="sxs-lookup"><span data-stu-id="7e589-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="7e589-148">Hautatu **Sortu proiektua**.</span><span class="sxs-lookup"><span data-stu-id="7e589-148">Select **Create project**.</span></span>
6. <span data-ttu-id="7e589-149">Proiektua sortu ondoren, ezarri proiektuaren etapa **Prozesuan**.</span><span class="sxs-lookup"><span data-stu-id="7e589-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="7e589-150">Sortu proiektu baten aurrekontua</span><span class="sxs-lookup"><span data-stu-id="7e589-150">Create a budget for a project</span></span>

<span data-ttu-id="7e589-151">Aurrekontu kategoriak kategoria bakoitzerako egindako lan portzentajearen fakturen zenbatekoak automatikoki kalkulatzeko erabiltzen dituztenak.</span><span class="sxs-lookup"><span data-stu-id="7e589-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="7e589-152">Jarraitu urrats hauei aurrekontu-kategoriak sortzeko kalkulatutako kostuetarako.</span><span class="sxs-lookup"><span data-stu-id="7e589-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="7e589-153">Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="7e589-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="7e589-154">**Proiektu guztiak** orrian, hautatu eta ireki nahi duzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="7e589-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="7e589-155">**Proiektuak** orrialdeko Ekintza panelean, **Plana** fitxan, **Aurrekontua** taldean, hautatu **Proiektuaren aurrekontua**.</span><span class="sxs-lookup"><span data-stu-id="7e589-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="7e589-156">**Proiektuaren aurrekontua** orrian, sartu proiektuaren kategoria bakoitzaren kostu estimatua.</span><span class="sxs-lookup"><span data-stu-id="7e589-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="7e589-157">Sortu fakturazio arauak aurrerapen fakturazioetarako</span><span class="sxs-lookup"><span data-stu-id="7e589-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="7e589-158">Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Proiektuak** \> **Proiektu-kontratuak**.</span><span class="sxs-lookup"><span data-stu-id="7e589-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="7e589-159">**Proiektuen kontratuak** orrian, hautatu eta ireki proiektu-kontratua.</span><span class="sxs-lookup"><span data-stu-id="7e589-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="7e589-160">Proiektuaren kontratuaren orrian, **Fakturazio arauak** FastTab-en, hautatu **Gehitu**.</span><span class="sxs-lookup"><span data-stu-id="7e589-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="7e589-161">**Fakturazio araua** orrialdean, **Lerro mota** eremua, hautatu **Aurrerapena**.</span><span class="sxs-lookup"><span data-stu-id="7e589-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="7e589-162">**Fakturazio arauaren lerroaren xehetasunak** FastTab fitxategian **Kontratuaren balioa** eremuan, sartu kontratuaren balio osoa.</span><span class="sxs-lookup"><span data-stu-id="7e589-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="7e589-163">**Kategoria** eremuan, hautatu kuota transakzioa bidaltzeko kategoria.</span><span class="sxs-lookup"><span data-stu-id="7e589-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="7e589-164">**Proiektua** eremuan, hautatu fakturazio arau hau erabiltzen duen proiektua.</span><span class="sxs-lookup"><span data-stu-id="7e589-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="7e589-165">Aukerakoa: esleitu fakturazio araua proiektu osagarriei.</span><span class="sxs-lookup"><span data-stu-id="7e589-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="7e589-166">**Proiektua** FastTab fitxategian **Eskuragarri dauden proiektuak** atalean, hautatu proiektu bat eta, ondoren, hautatu eskuineko geziaren botoia proiektua gehitzeko **Aukeratutako proiektuak** atala.</span><span class="sxs-lookup"><span data-stu-id="7e589-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="7e589-167">Aukerakoa: kalkulatu fakturak fakturatutako ordainketetan bezeroak gordetzen duen ehuneko kopurua.</span><span class="sxs-lookup"><span data-stu-id="7e589-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="7e589-168">**Ordainketak atxikitzeko baldintzak** FastTab-en, hautatu finantzaketa iturria eta, ondoren, **Atxikipen portzentajea** eremuan, sartu atxikipen ehunekoa.</span><span class="sxs-lookup"><span data-stu-id="7e589-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="7e589-169">Errepikatu urrats hauek proiektuaren kontratuaren fakturazio arau osagarriak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="7e589-169">Repeat these steps to create additional billing rules for the project contract.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]