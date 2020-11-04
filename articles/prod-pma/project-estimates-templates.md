---
title: Sinkronizatu proiektuaren kalkuluak zuzenean Project Service Automation-etik Finance and Operations
description: Gai honek proiektuaren orduen kalkuluak eta proiektuaren gastuen kalkuluak Microsoft-etik zuzenean sinkronizatzeko erabiltzen diren txantiloiak eta azpiko atazak deskribatzen ditu Microsoft Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.
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
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 336de474c859d30d1ec07ae34bf0c3d578faeef1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071164"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="1e78b-103">Sinkronizatu proiektuaren kalkuluak zuzenean Project Service Automation-etik Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="1e78b-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="1e78b-104">Gai honek proiektuaren orduen kalkuluak eta proiektuaren gastuen kalkuluak zuzenean sinkronizatzeko erabiltzen diren txantiloiak eta azpiko atazak deskribatzen ditu Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="1e78b-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="1e78b-105">Proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa eskuragarri daude 8.0 bertsioan.</span><span class="sxs-lookup"><span data-stu-id="1e78b-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="1e78b-106">Datu bateratuen integrazioa eskuragarri dago 8.0.1 bertsioan edo hurrengoan.</span><span class="sxs-lookup"><span data-stu-id="1e78b-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="1e78b-107">Project Service Automation Finantzararen datu-fluxua</span><span class="sxs-lookup"><span data-stu-id="1e78b-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="1e78b-108">Project Service Automation to Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko.</span><span class="sxs-lookup"><span data-stu-id="1e78b-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="1e78b-109">Datuak integratzeko funtzioarekin eskuragarri dauden integrazio txantiloiek proiektuaren orduen kalkuluen eta proiektuaren gastuen kalkuluen inguruko datuen fluxua ahalbidetzen dute Project Service Automation-etik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="1e78b-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="1e78b-110">Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.</span><span class="sxs-lookup"><span data-stu-id="1e78b-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="1e78b-111">[![Project Service Automation Finantzarekin integratzeko datuen fluxua](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="1e78b-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="1e78b-112">Proiektuaren orduaren aurreikuspenak</span><span class="sxs-lookup"><span data-stu-id="1e78b-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="1e78b-113">Txantiloia eta zereginak</span><span class="sxs-lookup"><span data-stu-id="1e78b-113">Template and tasks</span></span>

<span data-ttu-id="1e78b-114">Eskuragarri dauden txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.</span><span class="sxs-lookup"><span data-stu-id="1e78b-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects** , and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="1e78b-115">Ondorengo txantiloia eta azpiko zereginak proiektuaren orduen kalkuluak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="1e78b-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="1e78b-116">**Datuen integrazioko txantiloiaren izena:** Proiektuaren orduen kalkuluak (PSA Fin eta Ops)</span><span class="sxs-lookup"><span data-stu-id="1e78b-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="1e78b-117">**Proiektuko zereginaren izena:**</span><span class="sxs-lookup"><span data-stu-id="1e78b-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="1e78b-118">Transakzio-harremanak</span><span class="sxs-lookup"><span data-stu-id="1e78b-118">Transaction relationships</span></span>
    - <span data-ttu-id="1e78b-119">Expense estimates</span><span class="sxs-lookup"><span data-stu-id="1e78b-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="1e78b-120">Entitate multzoaren</span><span class="sxs-lookup"><span data-stu-id="1e78b-120">Entity set</span></span>

| <span data-ttu-id="1e78b-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="1e78b-121">Project Service Automation</span></span> | <span data-ttu-id="1e78b-122">Finantzak</span><span class="sxs-lookup"><span data-stu-id="1e78b-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="1e78b-123">Proiektuen zereginak</span><span class="sxs-lookup"><span data-stu-id="1e78b-123">Project tasks</span></span>              | <span data-ttu-id="1e78b-124">Integrazio entitatea proiektuaren orduen kalkuluen arabera</span><span class="sxs-lookup"><span data-stu-id="1e78b-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="1e78b-125">Entitate fluxua</span><span class="sxs-lookup"><span data-stu-id="1e78b-125">Entity flow</span></span>

<span data-ttu-id="1e78b-126">Proiektuaren orduen kalkuluak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren orduen iragarpen gisa.</span><span class="sxs-lookup"><span data-stu-id="1e78b-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="1e78b-127">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="1e78b-127">Prerequisites</span></span>

<span data-ttu-id="1e78b-128">Proiektuaren orduen kalkuluen sinkronizazioa gertatu aurretik, proiektuak, proiektuaren zereginak eta proiektuaren gastuen transakzio kategoriak sinkronizatu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="1e78b-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="1e78b-129">Power Query</span></span>

<span data-ttu-id="1e78b-130">Proiektuaren orduen kalkuluen txantiloian, Microsoft Power Query Excel erabili behar duzu zeregin hauek burutzeko:</span><span class="sxs-lookup"><span data-stu-id="1e78b-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="1e78b-131">Ezarri integrazioak ordu iragarpen berriak sortzen dituenean erabiliko den iragarpen eredu lehenetsia.</span><span class="sxs-lookup"><span data-stu-id="1e78b-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="1e78b-132">Ordu iragarpenetan integrazioa huts egingo duen atazan baliabide espezifikoen erregistroak iragazi.</span><span class="sxs-lookup"><span data-stu-id="1e78b-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="1e78b-133">Iragazi transakzio kategoriako errenkada hutsak.</span><span class="sxs-lookup"><span data-stu-id="1e78b-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="1e78b-134">Zeregin hori ez betetzeak ordu iragarpen okerrak sor ditzake.</span><span class="sxs-lookup"><span data-stu-id="1e78b-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="1e78b-135">Ezarri iragarpen eredu lehenetsiaren IDa</span><span class="sxs-lookup"><span data-stu-id="1e78b-135">Set the default forecast model ID</span></span>

<span data-ttu-id="1e78b-136">Txantiloian aurreikusitako modeloaren ID lehenetsia eguneratzeko, egin klik **Mapa** gezia mapa irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="1e78b-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="1e78b-137">Ondoren, hautatu **Kontsulta eta iragazki aurreratuak** esteka.</span><span class="sxs-lookup"><span data-stu-id="1e78b-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="1e78b-138">Proiektuaren ordu-estimazio lehenetsiak (PSA to Fin eta Ops) txantiloia erabiltzen ari bazara, hautatu **Txertatutako baldintza** zerrendan **Urrats Aplikatuak**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="1e78b-139">**Funtzioa** sarrera, ordeztu **O\_iragarpena** integrazioarekin batera erabili behar den aurreikuspen ereduaren IDaren izenarekin.</span><span class="sxs-lookup"><span data-stu-id="1e78b-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="1e78b-140">Txantiloi lehenetsiak iragarpen eredu IDa du demo datuetatik.</span><span class="sxs-lookup"><span data-stu-id="1e78b-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="1e78b-141">Txantiloi berria sortzen ari bazara, zutabe hau gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="1e78b-142">Power Query atalean, hautatu **Gehitu baldintzazko zutabea** , eta idatzi zutabe berriaren izena, adibidez **ID eredua**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-142">In Power Query, select **Add Conditional Column** , and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="1e78b-143">Idatzi zutabearen baldintza. Proiektuaren zeregina nulua ez bada, orduan \<enter the forecast model ID\>; bestela nulua.</span><span class="sxs-lookup"><span data-stu-id="1e78b-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="1e78b-144">Iragazi baliabide espezifikoen erregistroak</span><span class="sxs-lookup"><span data-stu-id="1e78b-144">Filter out resource-specific records</span></span>

<span data-ttu-id="1e78b-145">Project hour estimations (PSA to Fin and Ops) txantiloiak iragazki lehenetsia du, baliabide espezifikoen erregistroak ezabatzen dituena.</span><span class="sxs-lookup"><span data-stu-id="1e78b-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="1e78b-146">Zure txantiloia sortzen baduzu, iragazki hau gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="1e78b-147">Aukeratu **Kontsulta eta iragazki aurreratuak** fitxategian iragazteko esteka **msdyn\_islinetask** zutabea soilik beraz **Gezurra** erregistroak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="1e78b-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="1e78b-148">Iragazi transakzio kategoriako errenkada hutsak</span><span class="sxs-lookup"><span data-stu-id="1e78b-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="1e78b-149">Iragazki bat gehitu behar duzu transakzio kategoria hutsak dituzten errenkadak ezabatzeko.</span><span class="sxs-lookup"><span data-stu-id="1e78b-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="1e78b-150">Zeregin hori beharrezkoa da, txantiloi lehenetsia erabiltzen ari zaren edo zeure txantiloia sortzen ari zaren kontuan hartu gabe.</span><span class="sxs-lookup"><span data-stu-id="1e78b-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="1e78b-151">Iragazki honek Project Service Automation-en laburpen-errenkadak kentzen ditu Finantzako orduen iragarpenak okerrak izan daitezkeen.</span><span class="sxs-lookup"><span data-stu-id="1e78b-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="1e78b-152">Aukeratu **Kontsulta eta iragazki aurreratuak** esteka erregistro nuluak iragazteko **msdyn\_transakziokategoria\_balioa** zutabea.</span><span class="sxs-lookup"><span data-stu-id="1e78b-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="1e78b-153">Datuen integrazioan txantiloien mapaketa</span><span class="sxs-lookup"><span data-stu-id="1e78b-153">Template mapping in Data integration</span></span>

<span data-ttu-id="1e78b-154">Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du.</span><span class="sxs-lookup"><span data-stu-id="1e78b-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="1e78b-155">Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="1e78b-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="1e78b-156">[![Datuen integrazioko txantiloien zeregin-esleipena](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="1e78b-156">[![Template task mapping in data integration](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="1e78b-157">Proiektuaren gastuen aurreikuspenak</span><span class="sxs-lookup"><span data-stu-id="1e78b-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="1e78b-158">Txantiloia eta zereginak</span><span class="sxs-lookup"><span data-stu-id="1e78b-158">Template and tasks</span></span>

<span data-ttu-id="1e78b-159">Ondorengo txantiloia eta azpiko zereginak proiektuaren gastuen kalkuluak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="1e78b-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="1e78b-160">**Datuen integrazioko txantiloiaren izena:** Proiektuaren gastuen kalkuluak (PSA Fin eta Ops)</span><span class="sxs-lookup"><span data-stu-id="1e78b-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="1e78b-161">**Proiektuko zereginaren izena:**</span><span class="sxs-lookup"><span data-stu-id="1e78b-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="1e78b-162">Transakzio-harremanak</span><span class="sxs-lookup"><span data-stu-id="1e78b-162">Transaction relationships</span></span> 
    - <span data-ttu-id="1e78b-163">Expense estimates</span><span class="sxs-lookup"><span data-stu-id="1e78b-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="1e78b-164">Entitate multzoaren</span><span class="sxs-lookup"><span data-stu-id="1e78b-164">Entity set</span></span>

| <span data-ttu-id="1e78b-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="1e78b-165">Project Service Automation</span></span> | <span data-ttu-id="1e78b-166">Finantzak</span><span class="sxs-lookup"><span data-stu-id="1e78b-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="1e78b-167">Transakzio-konexioak</span><span class="sxs-lookup"><span data-stu-id="1e78b-167">Transaction Connections</span></span>    | <span data-ttu-id="1e78b-168">Proiektuen transakzio harremanetarako integrazio entitatea</span><span class="sxs-lookup"><span data-stu-id="1e78b-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="1e78b-169">Aurreikuspenen lerroak</span><span class="sxs-lookup"><span data-stu-id="1e78b-169">Estimate Lines</span></span>             | <span data-ttu-id="1e78b-170">Integrazio entitatea proiektuaren gastuen kalkuluen arabera</span><span class="sxs-lookup"><span data-stu-id="1e78b-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="1e78b-171">Entitate fluxua</span><span class="sxs-lookup"><span data-stu-id="1e78b-171">Entity flow</span></span>

<span data-ttu-id="1e78b-172">Proiektuaren gastuen kalkuluak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren gastuen iragarpen gisa.</span><span class="sxs-lookup"><span data-stu-id="1e78b-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="1e78b-173">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="1e78b-173">Prerequisites</span></span>

<span data-ttu-id="1e78b-174">Proiektuaren gastuen kalkuluen sinkronizazioa gertatu aurretik, proiektuak, proiektuaren zereginak eta proiektuaren gastuen transakzio kategoriak sinkronizatu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="1e78b-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="1e78b-175">Power Query</span></span>

<span data-ttu-id="1e78b-176">Proiektuaren gastuen kalkuluen txantiloian, Power Query erabili behar duzu hurrengo zeregin hauek burutzeko:</span><span class="sxs-lookup"><span data-stu-id="1e78b-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="1e78b-177">Iragazi gastuen kalkuluen lerro erregistroak soilik sartzeko.</span><span class="sxs-lookup"><span data-stu-id="1e78b-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="1e78b-178">Ezarri integrazioak ordu iragarpen berriak sortzen dituenean erabiliko den iragarpen eredu lehenetsia.</span><span class="sxs-lookup"><span data-stu-id="1e78b-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="1e78b-179">Eraldatu fakturazio motak.</span><span class="sxs-lookup"><span data-stu-id="1e78b-179">Transform the billing types.</span></span>
- <span data-ttu-id="1e78b-180">Eraldatu transakzio motak.</span><span class="sxs-lookup"><span data-stu-id="1e78b-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="1e78b-181">Iragazi gastuen kalkuluen lerroak soilik sartzeko</span><span class="sxs-lookup"><span data-stu-id="1e78b-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="1e78b-182">Proiektuaren gastuen kalkuluak (PSA to Fin eta Ops) txantiloiak iragazki lehenetsia du, eta integrazioan gastu lerroak bakarrik biltzen ditu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="1e78b-183">Zure txantiloia sortzen baduzu, iragazki hau gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="1e78b-184">Aukeratu **Transakzio harremanak** zereginaren gainean eta egin klik **Mapa** gezia mapa irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="1e78b-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="1e78b-185">Hautatu **Kontsulta eta iragazki aurreratuak** esteka.</span><span class="sxs-lookup"><span data-stu-id="1e78b-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="1e78b-186">Iragazi **msdyn\_transakzio mota1** zutabea soilik barne izan dezan **msdyn\_estimateline**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="1e78b-187">Ezarri iragarpen eredu lehenetsiaren IDa</span><span class="sxs-lookup"><span data-stu-id="1e78b-187">Set the default forecast model ID</span></span>

<span data-ttu-id="1e78b-188">Eguneratu lehenetsitako iragarritako ereduaren ID txantiloian, hautatu **Gastuaren balioztatzea** zeregina, eta gero klik egin **Mapa** gezitu irekiz jarraipena.</span><span class="sxs-lookup"><span data-stu-id="1e78b-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="1e78b-189">Hautatu **Kontsulta eta iragazki aurreratuak** esteka.</span><span class="sxs-lookup"><span data-stu-id="1e78b-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="1e78b-190">Proiektuaren gastu-estimazio lehenetsiak (PSA to Fin eta Ops) txantiloia erabiltzen ari bazara Power Query-n, hautatu lehen **Txertatutako baldintza** hurrengotik **Urrats Aplikatuak** sekzioa.</span><span class="sxs-lookup"><span data-stu-id="1e78b-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="1e78b-191">**Funtzioa** sarrera, ordeztu **O\_iragarpena** integrazioarekin batera erabili behar den aurreikuspen ereduaren IDaren izenarekin.</span><span class="sxs-lookup"><span data-stu-id="1e78b-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="1e78b-192">Txantiloi lehenetsiak iragarpen eredu IDa du demo datuetatik.</span><span class="sxs-lookup"><span data-stu-id="1e78b-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="1e78b-193">Txantiloi berria sortzen ari bazara, zutabe hau gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="1e78b-194">Power Query atalean, hautatu **Gehitu baldintzazko zutabea** , eta idatzi zutabe berriaren izena, adibidez **ID eredua**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-194">In Power Query, select **Add Conditional Column** , and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="1e78b-195">Idatzi zutabearen baldintza. Aurreikusitako lerroaren IDa nulua ez bada, orduan \<enter the forecast model ID\>; bestela nulua.</span><span class="sxs-lookup"><span data-stu-id="1e78b-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="1e78b-196">Eraldatu fakturazio motak</span><span class="sxs-lookup"><span data-stu-id="1e78b-196">Transform the billing types</span></span>

<span data-ttu-id="1e78b-197">Proiektuaren gastuen kalkuluak (PSA to Fin eta Ops) txantiloiak integrazio garaian Project Service Automation-etik jasotzen diren fakturazio motak eraldatzeko erabiltzen den baldintzazko zutabe bat dauka.</span><span class="sxs-lookup"><span data-stu-id="1e78b-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="1e78b-198">Zure txantiloia sortzen baduzu, baldintzazko zutabearen hau gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="1e78b-199">Aukeratu **Kontsulta eta iragazki aurreratuak** estekatu eta hautatu **Gehitu baldintzazko zutabea**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="1e78b-200">Idatzi zutabe berriaren izena, adibidez **Fakturazio mota**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="1e78b-201">Orduan idatzi hurrengo baldintza:</span><span class="sxs-lookup"><span data-stu-id="1e78b-201">Then enter the following condition:</span></span>

<span data-ttu-id="1e78b-202">Bada **msdyn\_fakturazio mota** = 192350000, orduan **Kargagabea**</span><span class="sxs-lookup"><span data-stu-id="1e78b-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="1e78b-203">Edozer gauza bada **msdyn\_fakturazio mota** = 192350001, orduan **Kargagarria**</span><span class="sxs-lookup"><span data-stu-id="1e78b-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="1e78b-204">Edozer gauza bada **msdyn\_fakturazio mota** = 192350002, orduan **Osagarria**</span><span class="sxs-lookup"><span data-stu-id="1e78b-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="1e78b-205">Bestela **Ez dago erabilgarri**</span><span class="sxs-lookup"><span data-stu-id="1e78b-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="1e78b-206">Eraldatu transakzio motak</span><span class="sxs-lookup"><span data-stu-id="1e78b-206">Transform the transaction types</span></span>

<span data-ttu-id="1e78b-207">Proiektuaren gastuen kalkuluak (PSA to Fin eta Ops) txantiloiak integrazio garaian Project Service Automation-etik jasotzen diren transakzio motak eraldatzeko erabiltzen den baldintzazko zutabe bat dauka.</span><span class="sxs-lookup"><span data-stu-id="1e78b-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="1e78b-208">Zure txantiloia sortzen baduzu, baldintzazko zutabearen hau gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="1e78b-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="1e78b-209">Aukeratu **Kontsulta eta iragazki aurreratuak** estekatu eta hautatu **Gehitu baldintzazko zutabea**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="1e78b-210">Idatzi zutabe berriaren izena, adibidez **TransakzioMota**.</span><span class="sxs-lookup"><span data-stu-id="1e78b-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="1e78b-211">Orduan idatzi hurrengo baldintza:</span><span class="sxs-lookup"><span data-stu-id="1e78b-211">Then enter the following condition:</span></span>

<span data-ttu-id="1e78b-212">Bada **msdyn\_transakzio mota** = 192350000, orduan **Kostua**</span><span class="sxs-lookup"><span data-stu-id="1e78b-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="1e78b-213">Beste edozein bada **msdyn\_transakzio mota** = 192350005, orduan **Salmentak**</span><span class="sxs-lookup"><span data-stu-id="1e78b-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="1e78b-214">Bestela **nulua**</span><span class="sxs-lookup"><span data-stu-id="1e78b-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="1e78b-215">Datuen integrazioan txantiloien mapaketa</span><span class="sxs-lookup"><span data-stu-id="1e78b-215">Template mapping in Data integration</span></span>

<span data-ttu-id="1e78b-216">Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du.</span><span class="sxs-lookup"><span data-stu-id="1e78b-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="1e78b-217">Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="1e78b-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="1e78b-218">[![Gastuen aurreikusitako transakzioen txantiloien mapaketa](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="1e78b-218">[![Template mapping of expense estimate transactions](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="1e78b-219">[![Gastuen aurreikuspenen txantiloien mapaketa](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="1e78b-219">[![Template mapping of expense estimates](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>
