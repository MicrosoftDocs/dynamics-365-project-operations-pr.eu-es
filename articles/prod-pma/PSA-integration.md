---
title: Project Service Automation-en ikuspegi orokorra
description: Gai honek informazioari buruzko informazioa eskaintzen du Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance integrazio irtenbidea.
author: ruhercul
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5ca459b99881b612e4656be112c8a2e420b4196e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005866"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="0095f-103">Project Service Automation-en ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="0095f-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="0095f-104">Project Service Automation hurrengora Finantza integrazioaren soluzioak erabiltzen du Datu integrazioaren eginbidea sinkronizatzeko datuak instantzien artean Dynamics 365 Finance eta Dynamics 365 Project Service Automation bidez Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="0095f-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="0095f-105">Integrazio-txantiloiak eskuragarri daudenak Datu-integrazioaren eginbidearekin gaitzen du proiektuen fluxua, proiektu-kontratuak, proiektu-kontratu lerroak, proiektu-kontratu lerroen mugarriak, proiektu-zereginak, gastuen transakzio kategoriak, aurreikusitako orduak, eta gastu-aurreikusiak Project Service Automation Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="0095f-106">Bertsioa 7.3.0 erabiltzen ari bazara, KB 4074835 instalatu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="0095f-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="0095f-107">Orduan, prezio finkoaren proiektuak integratu ahal izango dituzu.</span><span class="sxs-lookup"><span data-stu-id="0095f-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="0095f-108">7.3.0 bertsioa erabiltzen ari bazara eta Project Service Automation-etik kuoten transakzioak ekartzen badituzu, KB 4345320 instalatu behar duzu tasak proiektuaren fakturan sartzeko.</span><span class="sxs-lookup"><span data-stu-id="0095f-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="0095f-109">8.0 bertsioa erabiltzen ari bazara, gai izango zara erabiltzeko proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa.</span><span class="sxs-lookup"><span data-stu-id="0095f-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="0095f-110">8.0.1 bertsioa edo berriagoa erabiltzen baduzu, benetakoak sinkronizatu ahal izango dituzu.</span><span class="sxs-lookup"><span data-stu-id="0095f-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="0095f-111">Project Service Automation Finance integratu aurretik, Project Service Automation integrazio parametroak konfiguratu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="0095f-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="0095f-112">Informazio gehiagorako, ikusi [Project Service Automation integrazio-parametroak](PSA-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="0095f-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="0095f-113">Integrazio irtenbide honek zuzeneko sinkronizazioa ahalbidetzen du agertoki hauetan:</span><span class="sxs-lookup"><span data-stu-id="0095f-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="0095f-114">Mantendu proiektuen kontratuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0095f-115">Sortu proiektuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0095f-116">Mantendu proiektuen kontratu-lerroak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0095f-117">Mantendu proiektuen kontratu-lerroen mugarriak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0095f-118">Mantendu proiektuen zereginak kontratuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0095f-119">Mantendu gastuen transakzio-kategoriak Finantzan, eta sinkronizatu horiek zuzenean Finantzatik Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="0095f-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="0095f-120">Sortu proiektuak aurreikusitako orduak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0095f-121">Sortu proiektuak aurreikusitako gastuak Project Service Automation zerbitzuan eta sinkronizatu zuzenean Project Service Automationetik Finantzara.</span><span class="sxs-lookup"><span data-stu-id="0095f-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0095f-122">Sortu proiektuaren denbora, gastua eta kuoten errealitatea Project Service Automation-en eta sortu proiektuaren transakzioak Project Service Automation integrazio aldizkarian, Finantzan argitaratu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="0095f-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="0095f-123">Datuen sinkronizazioa</span><span class="sxs-lookup"><span data-stu-id="0095f-123">Data synchronization</span></span>

<span data-ttu-id="0095f-124">Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak integrazioaren parte gisa Project Service Automation eta Finance artean.</span><span class="sxs-lookup"><span data-stu-id="0095f-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="0095f-125">Txantiloi guztiak ez daude unean eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="0095f-125">Not all templates are currently available.</span></span> <span data-ttu-id="0095f-126">Txantiloiak amaitu ahala kaleratuko dira.</span><span class="sxs-lookup"><span data-stu-id="0095f-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="0095f-127">[![Project Service Automation Finantzarekin integratzeko](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="0095f-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="0095f-128">Finantzetarako sistemaren eskakizunak</span><span class="sxs-lookup"><span data-stu-id="0095f-128">System requirements for Finance</span></span>

<span data-ttu-id="0095f-129">Project Service Automation to Finance integrazio konponbidea erabiltzeko, Enterprise edition 7.3 instalatu behar duzu Plataforma 12 bertsio berriagoa edo berriagoarekin.</span><span class="sxs-lookup"><span data-stu-id="0095f-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="0095f-130">Sistemaren eskakizunak Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="0095f-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="0095f-131">Project Service Automation to Finance integrazio irtenbidea erabiltzeko, osagai hauek instalatu behar dituzu:</span><span class="sxs-lookup"><span data-stu-id="0095f-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="0095f-132">Dynamics 365 Project Service Automation 9.0.0.0 bertsioa edo berriagoa</span><span class="sxs-lookup"><span data-stu-id="0095f-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="0095f-133">Dynamics 365 Sales-erako dirua ateratzeko irtenbidea, 1.14.0.0 (v14) bertsioa edo berriagoa</span><span class="sxs-lookup"><span data-stu-id="0095f-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="0095f-134">Project Service Automation to Finance irtenbidea Dynamics 365 Project Service Automation 1.0.0.0 bertsioa edo berriagoa</span><span class="sxs-lookup"><span data-stu-id="0095f-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="0095f-135">Instalatu Project Service Automation to Finance integrazio konponbidea zure Project Service Automation instantzia</span><span class="sxs-lookup"><span data-stu-id="0095f-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="0095f-136">Deskargatu Project Service Automation to Finance integrazio irtenbidea [Microsoft Deskarga Zentroa](https://www.microsoft.com/download/details.aspx?id=57016), eta jarraitu irtenbidearekin bat datozen argibideak.</span><span class="sxs-lookup"><span data-stu-id="0095f-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]