---
title: Proiektuen denbora eta material proiektuen salmenta aginduak
description: Gai honetan proiektuetan oinarritutako salmenta aginduak nola sortu azaltzen da denbora eta proiektu materialetarako.
author: Yowelle
manager: AnnBe
ms.date: 04/05/2019
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
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 3653a6869dab323be88f1fd0f9fd0f2cb35c456f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071021"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="e19ba-103">Proiektuen denbora eta material proiektuen salmenta aginduak</span><span class="sxs-lookup"><span data-stu-id="e19ba-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="e19ba-104">Gai honetan proiektu baten salmenta eskaera nola sortu azaltzen da.</span><span class="sxs-lookup"><span data-stu-id="e19ba-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="e19ba-105">Salmenta aginduak motako proiektuetarako bakarrik sor daitezke **denbora eta materiala**.</span><span class="sxs-lookup"><span data-stu-id="e19ba-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="e19ba-106">Denbora eta material proiektu batek proiektuaren kontratuan finantzaketa iturri ugari baditu, gaitu behar duzu **Baimendu diru iturri anitz dituzten proiektuen salmenta aginduak** parametroa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="e19ba-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="e19ba-107">Finantzaketa iturri anitz dituzten proiektuen salmenta eskaerei buruzko laguntza eskuragarri dago 10.0.2 aplikazioaren bertsio berritik hasita.</span><span class="sxs-lookup"><span data-stu-id="e19ba-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="e19ba-108">Finantzaketa iturri anitz dituzten proiektuen salmenta aginduen laguntza gaitzeko parametroa kenduko da 2020ko apirileko bertsio uhinean, eta ondoren funtzionaltasuna beti gaituko da.</span><span class="sxs-lookup"><span data-stu-id="e19ba-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="e19ba-109">Proiektuetan oinarritutako salmenta aginduak bi modutan sor ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="e19ba-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="e19ba-110">Joan proiektura bertara.</span><span class="sxs-lookup"><span data-stu-id="e19ba-110">Go to the project itself.</span></span> <span data-ttu-id="e19ba-111">Ekintza panelean, hautatu **Kudeatu > Elementuen zereginak > Salmenta agindua**.</span><span class="sxs-lookup"><span data-stu-id="e19ba-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="e19ba-112">Proiektuaren informazioa proiektuaren salmenta eskaera lehenetsiko da.</span><span class="sxs-lookup"><span data-stu-id="e19ba-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="e19ba-113">Proiektuaren kontratuak finantzaketa iturri bat baino gehiago baditu, finantzaketa iturria hautatu beharko duzu bezeroa salmenta eskaerarako ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="e19ba-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="e19ba-114">Proiektua finantzatzeko iturri bakarra baldin badago, bezeroa automatikoki konfiguratuko da.</span><span class="sxs-lookup"><span data-stu-id="e19ba-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="e19ba-115">Joan **Salmenta eskaera guztiak** zerrendaren orria eta salmenta eskaera berria sortu.</span><span class="sxs-lookup"><span data-stu-id="e19ba-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="e19ba-116">Salmenta eskaeraren proiektua hautatu beharko duzu.</span><span class="sxs-lookup"><span data-stu-id="e19ba-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="e19ba-117">Proiektua hautatu ondoren, bezeroa finantziazio iturritik ezarriko da edo finantzaketa iturria hautatu beharko duzu proiektuaren kontratuak finantzazio iturri anitz baditu.</span><span class="sxs-lookup"><span data-stu-id="e19ba-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>

