---
title: Sinkronizatu proiektuaren zereginak zuzenean Project Service Automation-etik Finance and Operations
description: Gai honek deskribatzen du txantiloiak eta azpiko zeregina erabiliak direnak sinkronizatzeko zereginen proiektuak zuzenean Microsoft Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 16cd38f2f190414d7be9c93e8ab90d55006f47e1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009961"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="493e8-103">Sinkronizatu proiektuaren zereginak zuzenean Project Service Automation-etik Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="493e8-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="493e8-104">Gai honek deskribatzen du txantiloiak eta azpiko zeregina erabiliak direnak sinkronizatzeko zereginen proiektuak zuzenean Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="493e8-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="493e8-105">Proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa eskuragarri daude 8.0 bertsioan.</span><span class="sxs-lookup"><span data-stu-id="493e8-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="493e8-106">KB 4132657 eta KB 4132660 instalatu ondoren Enterprise edition 7.3.0 erabiltzen ari bazara, txantiloiak erabil ditzakezu proiektuaren zereginak, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta benetakoak konfiguratzeko eta konfiguratzeko funtzionalitate blokeoa.</span><span class="sxs-lookup"><span data-stu-id="493e8-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="493e8-107">Kontabilitate banaketak berrezarri behar badituzu, KB 4131710 ere instalatzea gomendatzen dizugu.</span><span class="sxs-lookup"><span data-stu-id="493e8-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="493e8-108">Datu bateratuen integrazioa eskuragarri dago 8.0.1 bertsioan edo hurrengoan.</span><span class="sxs-lookup"><span data-stu-id="493e8-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="493e8-109">Project Service Automation Finantzararen datu-fluxua</span><span class="sxs-lookup"><span data-stu-id="493e8-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="493e8-110">Project Service Automation to Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko.</span><span class="sxs-lookup"><span data-stu-id="493e8-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="493e8-111">Datuak integratzeko funtzioarekin eskuragarri dauden integrazio txantiloiek proiektuaren zereginen inguruko datuen fluxua ahalbidetzen dute Project Service Automation-etik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="493e8-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="493e8-112">Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.</span><span class="sxs-lookup"><span data-stu-id="493e8-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="493e8-113">[![Project Service Automation Finantzarekin integratzeko datuen fluxua](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="493e8-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="493e8-114">Txantiloia eta zeregina</span><span class="sxs-lookup"><span data-stu-id="493e8-114">Template and task</span></span>

<span data-ttu-id="493e8-115">Txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.</span><span class="sxs-lookup"><span data-stu-id="493e8-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="493e8-116">Ondorengo txantiloia eta azpiko zereginaren proiektuaren zereginen Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="493e8-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="493e8-117">**Datuen integrazioko txantiloiaren izena:** Proiektuaren zereginak (PSA Fin eta Ops)</span><span class="sxs-lookup"><span data-stu-id="493e8-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="493e8-118">**Proiektuko zereginen izena:** Proiektuaren zereginak</span><span class="sxs-lookup"><span data-stu-id="493e8-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="493e8-119">Proiektuen zereginen sinkronizazioa gertatu aurretik, kontuak sinkronizatu proiektuaren kontratuak eta proiektuak behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="493e8-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="493e8-120">Entitate multzoaren</span><span class="sxs-lookup"><span data-stu-id="493e8-120">Entity set</span></span>

| <span data-ttu-id="493e8-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="493e8-121">Project Service Automation</span></span> | <span data-ttu-id="493e8-122">Finantzak</span><span class="sxs-lookup"><span data-stu-id="493e8-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="493e8-123">Proiektuen zereginak</span><span class="sxs-lookup"><span data-stu-id="493e8-123">Project Tasks</span></span>              | <span data-ttu-id="493e8-124">Proiektuaren zeregina datu-bateratuak integrazio entitatea</span><span class="sxs-lookup"><span data-stu-id="493e8-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="493e8-125">Entitate fluxua</span><span class="sxs-lookup"><span data-stu-id="493e8-125">Entity flow</span></span>

<span data-ttu-id="493e8-126">Proiektuaren zereginak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren jarduerak gisa.</span><span class="sxs-lookup"><span data-stu-id="493e8-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="493e8-127">Aurrebaldintzak eta mapen konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="493e8-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="493e8-128">Proiektuen zereginen sinkronizazioa gertatu aurretik, kontuak sinkronizatu proiektuaren kontratuak eta proiektuak behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="493e8-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="493e8-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="493e8-129">Power Query</span></span>

<span data-ttu-id="493e8-130">Microsoft Power Query Excel-era erabili behar duzu datuak iragazteko baldintza hori gertatzean:</span><span class="sxs-lookup"><span data-stu-id="493e8-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="493e8-131">Baliabideen araberako erregistroak dituzu proiektuko zeregin batean.</span><span class="sxs-lookup"><span data-stu-id="493e8-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="493e8-132">Power Query erabili behar baduzu, jarraitu jarraibide hori:</span><span class="sxs-lookup"><span data-stu-id="493e8-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="493e8-133">Project tasks (PSA to Fin and Ops) txantiloiak iragazki lehenetsia du, baliabide espezifikoak erregistroak proiektuko zereginetik kanpo uzten dituena iragazkia ezarriz **IsLineTask** hurrengora **Gezurra**.</span><span class="sxs-lookup"><span data-stu-id="493e8-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="493e8-134">Zure txantiloia sortzen baduzu, iragazki hau gehitu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="493e8-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="493e8-135">Datuen integrazioan txantiloien mapaketa</span><span class="sxs-lookup"><span data-stu-id="493e8-135">Template mapping in Data integration</span></span>

<span data-ttu-id="493e8-136">Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen mapen adibide bat erakusten du.</span><span class="sxs-lookup"><span data-stu-id="493e8-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="493e8-137">Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="493e8-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="493e8-138">[![Txantiloien mapaketa](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="493e8-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]