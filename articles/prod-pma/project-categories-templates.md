---
title: Sinkronizatu proiektuaren gastuen kategoriak Finance and Operations eta Project Service Automation
description: Gai honek deskribatzen du txantiloiak eta azpiko zereginak erabiliak direnak sinkronizatzeko proiektuaren gastuaren kategoriak Microsoft Dynamics 365 Finance eta Dynamics 365 Project Service Automation artean.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: ed7ca3c85d3f99b7eefe10f4ddec822b9aeb1684
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071175"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="56214-103">Sinkronizatu proiektuaren gastuen kategoriak Finance and Operations eta Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="56214-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="56214-104">Gai honek deskribatzen du txantiloiak eta azpiko zereginak erabiliak direnak sinkronizatzeko proiektuaren gastuaren kategoriak Dynamics 365 Finance eta Dynamics 365 Project Service Automation artean.</span><span class="sxs-lookup"><span data-stu-id="56214-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="56214-105">Proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa eskuragarri daude 8.0 bertsioan.</span><span class="sxs-lookup"><span data-stu-id="56214-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="56214-106">Datu bateratuen integrazioa eskuragarri dago 8.0.1 bertsioan edo hurrengoan.</span><span class="sxs-lookup"><span data-stu-id="56214-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="56214-107">KB 4132657 eta KB 4132660 instalatu ondoren Enterprise edition 7.3.0 erabiltzen ari bazara, txantiloiak erabil ditzakezu proiektuaren zereginak, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta benetakoak konfiguratzeko eta konfiguratzeko funtzionalitate blokeoa.</span><span class="sxs-lookup"><span data-stu-id="56214-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="56214-108">Kontabilitate banaketak berrezarri behar badituzu, KB 4131710 ere instalatzea gomendatzen dizugu.</span><span class="sxs-lookup"><span data-stu-id="56214-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="56214-109">Project Service Automation eta Finantzararen datu-fluxua</span><span class="sxs-lookup"><span data-stu-id="56214-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="56214-110">Project Service Automation eta Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko.</span><span class="sxs-lookup"><span data-stu-id="56214-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="56214-111">Integrazio txantiloiak eskuragarri daude Datu-integrazio eginbidearekin gaitzen du fluxuaren datuak proiektuaren gastuari buruz transakzio-kategoriak artean Finantza eta Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="56214-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="56214-112">Proiektuaren gastuen kategoriak Finantzan menderatzen badira, integrazio-fluxua lehenik Finantzetatik Project Service Automation-era da.</span><span class="sxs-lookup"><span data-stu-id="56214-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="56214-113">Proiektuaren gastuen kategorien integrazio IDak eguneratzen dira sinkronizazioaren bidez, Project Service Automation-etik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="56214-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="56214-114">Proiektuaren gastuen kategoriak Project Service Automation menderatzen badira, integrazio-fluxua lehenik Finantzetatik Project Service Automation-era Finantza da.</span><span class="sxs-lookup"><span data-stu-id="56214-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="56214-115">Proiektuen kategoriak dagoeneko Finantzan konfiguratuta egon behar dira Project Service Automation-etik sinkronizatu aurretik.</span><span class="sxs-lookup"><span data-stu-id="56214-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="56214-116">Ondoren, sinkronizatu Finantzatik Project Service Automation-era eta, ondoren, Project Service Automation-etik Finance-ra berriro.</span><span class="sxs-lookup"><span data-stu-id="56214-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="56214-117">Horrela, kategoriak lotuta daudela eta bikoizturik sortuko ez dela bermatzen lagunduko duzu.</span><span class="sxs-lookup"><span data-stu-id="56214-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="56214-118">Normalean, proiektuaren gastuen kategoriak Finantzan menderatzen dira.</span><span class="sxs-lookup"><span data-stu-id="56214-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="56214-119">Hala ere, hala ez bada edo Project Service Automation dagoeneko gastuen kategoriak sortu badira, lehenengo sinkronizatu behar duzu Proiektuaren gastuen transakzioen kategoriak (PSA Fin eta Ops) txantiloia erabiliz.</span><span class="sxs-lookup"><span data-stu-id="56214-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="56214-120">Ondoren, sinkronizatu Proiektuaren gastuen transakzio kategoriak (Fin eta Ops PSA) txantiloia erabiliz.</span><span class="sxs-lookup"><span data-stu-id="56214-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="56214-121">Project Service Automation Finantzara sinkronizazioa beste behin exekutatu beharko zenuke.</span><span class="sxs-lookup"><span data-stu-id="56214-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="56214-122">Project Service Automation-etik lehen sinkronizatzen baduzu, baldintza hauek bete beharko dira Finantzan sinkronizazioa exekutatu aurretik:</span><span class="sxs-lookup"><span data-stu-id="56214-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="56214-123">Project Service Automation-en konfiguratutako proiektuaren kategoriarekin bat datorren kategoria partekatua existitu behar da eta bietarako gaituta egon behar du **Proiektua** eta **Gastua**.</span><span class="sxs-lookup"><span data-stu-id="56214-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="56214-124">Horrekin batera integratu behar den Finantza entitate juridiko bakoitzerako proiektuen kategoria hauek egon behar dira:</span><span class="sxs-lookup"><span data-stu-id="56214-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="56214-125">**Proiektuaren kategoria** existitzen da.</span><span class="sxs-lookup"><span data-stu-id="56214-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="56214-126">**Erabilera Gastuan** gaituta dago.</span><span class="sxs-lookup"><span data-stu-id="56214-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="56214-127">**Aktibo egunkarian** gaituta dago.</span><span class="sxs-lookup"><span data-stu-id="56214-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="56214-128">**Transakzio mota** ezarrita dago **Gastua**.</span><span class="sxs-lookup"><span data-stu-id="56214-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="56214-129">Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.</span><span class="sxs-lookup"><span data-stu-id="56214-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="56214-130">[![Project Service Automation Finantzarekin integratzeko datuen fluxua](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="56214-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="56214-131">Proiektuaren gastuaren kategoriaren sinkronizazioa hurrengotik Finantza hurrengora Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="56214-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="56214-132">Txantiloia eta zeregina</span><span class="sxs-lookup"><span data-stu-id="56214-132">Template and task</span></span>

<span data-ttu-id="56214-133">Txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.</span><span class="sxs-lookup"><span data-stu-id="56214-133">To access the template, in the Microsoft Power Apps admin center, select **Projects** , and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="56214-134">Ondorengo txantiloia eta azpiko zeregina proiektuaren gastuen kategoriak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="56214-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="56214-135">**Datuen integrazioko txantiloiaren izena:** Proiektuaren gastuen transakzioaren kategoriak (PSA Fin eta Ops)</span><span class="sxs-lookup"><span data-stu-id="56214-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="56214-136">**Zereginaren izena proiektuan:** Sinkronizatu kategoriak PSArekin</span><span class="sxs-lookup"><span data-stu-id="56214-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="56214-137">Entitate multzoaren</span><span class="sxs-lookup"><span data-stu-id="56214-137">Entity set</span></span>

| <span data-ttu-id="56214-138">Finantzak</span><span class="sxs-lookup"><span data-stu-id="56214-138">Finance</span></span>                           | <span data-ttu-id="56214-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="56214-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="56214-140">Kategoriak datu-bateratuak integrazio entitatea</span><span class="sxs-lookup"><span data-stu-id="56214-140">Integration entity for categories</span></span> | <span data-ttu-id="56214-141">Transakzio-kategoriak</span><span class="sxs-lookup"><span data-stu-id="56214-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="56214-142">Entitate fluxua</span><span class="sxs-lookup"><span data-stu-id="56214-142">Entity flow</span></span>

<span data-ttu-id="56214-143">Proiektuaren gastuen kategoriak Finantza-ren kudeatzen dira eta Project Service Automation sinkronizatzen dira transakzio-kategoriak gisa.</span><span class="sxs-lookup"><span data-stu-id="56214-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="56214-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="56214-144">Power Query</span></span>

<span data-ttu-id="56214-145">Project Service Automation-ekin sinkronizatzen ari zarenean, Microsoft Power Query erabili behar duzu Excel-erako fakturazio transakzio kategorian ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="56214-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="56214-146">Proiektuaren gastuen transakzioen kategoriak (Fin eta Ops PSA) txantiloiak zutabe eta mapaketa lehenetsiak eskaintzen ditu.</span><span class="sxs-lookup"><span data-stu-id="56214-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="56214-147">Zure txantiloia sortzen baduzu, baldintzazko zutabearen hau gehitu behar duzu Power Query.</span><span class="sxs-lookup"><span data-stu-id="56214-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="56214-148">Jarraitu urrats hauei.</span><span class="sxs-lookup"><span data-stu-id="56214-148">Follow these steps.</span></span>

1. <span data-ttu-id="56214-149">Egin klik gezian proiektuaren gastuen kategorien zereginaren mapaketa irekitzeko, Proiektuaren gastuen transakzioen kategoriak (Fin eta Ops to PSA) txantiloian.</span><span class="sxs-lookup"><span data-stu-id="56214-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="56214-150">Klik egin **Kontsulta eta iragazki aurreratuak** esteka irekitzeko Power Query.</span><span class="sxs-lookup"><span data-stu-id="56214-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="56214-151">Aukeratu **Gehitu baldintzazko zutabea**.</span><span class="sxs-lookup"><span data-stu-id="56214-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="56214-152">Idatzi zutabe berriaren izena, adibidez **Fakturazio mota**.</span><span class="sxs-lookup"><span data-stu-id="56214-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="56214-153">Idatzi baldintza hau: **CATEGORYID ez bada nulua bezainbeste 19235001, Bestela nulua**.</span><span class="sxs-lookup"><span data-stu-id="56214-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="56214-154">Klik egin **Ados** zutabean.</span><span class="sxs-lookup"><span data-stu-id="56214-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="56214-155">Ziurtatu mapen orrian zutabe berri hau mapeatzen.</span><span class="sxs-lookup"><span data-stu-id="56214-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="56214-156">Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du.</span><span class="sxs-lookup"><span data-stu-id="56214-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="56214-157">Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="56214-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="56214-158">[![Proiektuaren gastuaren kategoria Project Service Automation txantiloiei esleitzea](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="56214-158">[![Project expense category to Project Service Automation template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="56214-159">Proiektuaren gastuaren kategoriaren sinkronizazioa hurrengotik Finantza hurrengora Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="56214-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="56214-160">Txantiloia eta zeregina</span><span class="sxs-lookup"><span data-stu-id="56214-160">Template and task</span></span>

<span data-ttu-id="56214-161">Ondorengo txantiloia eta azpiko zeregina proiektuaren gastuen kategoriak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="56214-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="56214-162">**Datuen integrazioko txantiloiaren izena:** Proiektuaren gastuen transakzioaren kategoriak (PSA Fin eta Ops)</span><span class="sxs-lookup"><span data-stu-id="56214-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="56214-163">**Zereginaren izena proiektuan:** Sinkronizatu kategoriak Fin Ops</span><span class="sxs-lookup"><span data-stu-id="56214-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="56214-164">Entitate multzoaren</span><span class="sxs-lookup"><span data-stu-id="56214-164">Entity set</span></span>

| <span data-ttu-id="56214-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="56214-165">Project Service Automation</span></span> | <span data-ttu-id="56214-166">Finantzak</span><span class="sxs-lookup"><span data-stu-id="56214-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="56214-167">Transakzio-kategoriak</span><span class="sxs-lookup"><span data-stu-id="56214-167">Transaction categories</span></span>     | <span data-ttu-id="56214-168">Kategoriak datu-bateratuak integrazio entitatea</span><span class="sxs-lookup"><span data-stu-id="56214-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="56214-169">Entitate fluxua</span><span class="sxs-lookup"><span data-stu-id="56214-169">Entity flow</span></span>

<span data-ttu-id="56214-170">Proiektuaren gastuen kategoriak Finantza-ren kudeatzen dira eta Project Service Automation sinkronizatzen dira transakzio-kategoriak gisa.</span><span class="sxs-lookup"><span data-stu-id="56214-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="56214-171">Sinkronizazioaren atzeko Finantza eguneratzeak proiektuaren kategoria Finantzan integrazioarekin ID-a hurrengoarekin Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="56214-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="56214-172">Datuen integrazioan txantiloien mapaketa</span><span class="sxs-lookup"><span data-stu-id="56214-172">Template mapping in Data integration</span></span>

<span data-ttu-id="56214-173">Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du.</span><span class="sxs-lookup"><span data-stu-id="56214-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="56214-174">Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="56214-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="56214-175">[![Project Service Automation Finance txantiloiei esleitzea](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="56214-175">[![Project Service Automation to Finance template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>
