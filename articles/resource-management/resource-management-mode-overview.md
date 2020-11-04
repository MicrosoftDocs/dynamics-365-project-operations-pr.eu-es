---
title: Baliabide-kudeaketaren moduen informazio orokorra
description: Gai honek Baliabide kudeaketa funtzioari buruzko informazioa eskaintzen du Dynamics 365 Project Operations-en.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4a8e605109e48b50da68abeee989f8ac8d3d659c
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070924"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="40d16-103">Baliabide-kudeaketaren moduen informazio orokorra</span><span class="sxs-lookup"><span data-stu-id="40d16-103">Resource management modes overview</span></span>

<span data-ttu-id="40d16-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="40d16-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="40d16-105">Dynamics 365 Project Operations-ek bi modu onartzen ditu erreserba-fluxu orokorra exekutatu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="40d16-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="40d16-106">Kudeaketa modua proiektuaren parametro gisa definitzen da eta zure negozioa aldatu behar bada alda daiteke.</span><span class="sxs-lookup"><span data-stu-id="40d16-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="40d16-107">Modu zentrala</span><span class="sxs-lookup"><span data-stu-id="40d16-107">Central mode</span></span>
<span data-ttu-id="40d16-108">Proiektuetarako baliabideen zuzkidura zentralizatzen duten erakundeentzat, Modu Zentralak proiektuaren kudeatzaileek proiektuaren mailan baliabideen eskakizunak definitu ahal izateko modua eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="40d16-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="40d16-109">Baliabideen eskakizunak betetzea Baliabideen kudeatzaileari eskuordetzen zaio.</span><span class="sxs-lookup"><span data-stu-id="40d16-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="40d16-110">Proiektuen kudeatzaileek baliabideen kudeatzaileak proposatutako baliabideak onartu edo baztertu ditzakete.</span><span class="sxs-lookup"><span data-stu-id="40d16-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Modu zentrala](./media/resource-management-central.png)

<span data-ttu-id="40d16-112">Baliabideak Erdiko moduarekin kudeatzeko, ikusi:</span><span class="sxs-lookup"><span data-stu-id="40d16-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="40d16-113">Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak</span><span class="sxs-lookup"><span data-stu-id="40d16-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="40d16-114">Erreserbatu izena duten baliabideak baliabide-eskakizunetatik</span><span class="sxs-lookup"><span data-stu-id="40d16-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="40d16-115">Bidali baliabide-eskaera bat</span><span class="sxs-lookup"><span data-stu-id="40d16-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="40d16-116">Bete baliabide-eskaera</span><span class="sxs-lookup"><span data-stu-id="40d16-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="40d16-117">Onartu edo baztertu proposatutako proiektuaren baliabidea baliabide-eskaera batetik</span><span class="sxs-lookup"><span data-stu-id="40d16-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="40d16-118">Modu hibridoa</span><span class="sxs-lookup"><span data-stu-id="40d16-118">Hybrid mode</span></span>
<span data-ttu-id="40d16-119">Baliabideen banaketan malgutasuna behar duten erakundeentzat, modu hibridoak proiektuen kudeatzaileei eta baliabideen kudeatzaileei baliabideak erreserbatzeko aukera ematen die.</span><span class="sxs-lookup"><span data-stu-id="40d16-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Modu hibridoa](./media/resource-management-hybrid.png)

<span data-ttu-id="40d16-121">Onartutako Erdiko moduaren prozesua ez ezik, ikusi gai hauek Hibrido moduan onartutako erreserba-fluxu guztiak kudeatzeko:</span><span class="sxs-lookup"><span data-stu-id="40d16-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="40d16-122">Erreserbatu baliabide bat zuzenean proiektu bati:</span><span class="sxs-lookup"><span data-stu-id="40d16-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="40d16-123">Erreserbatu baliabide erreserbagarriak proiektuko talde bati eta esleitu zereginak</span><span class="sxs-lookup"><span data-stu-id="40d16-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="40d16-124">Erreserbatu baliabide bat baliabide-eskakizunetatik:</span><span class="sxs-lookup"><span data-stu-id="40d16-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="40d16-125">Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak</span><span class="sxs-lookup"><span data-stu-id="40d16-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="40d16-126">Erreserbatu izena duten baliabideak baliabide-eskakizunetatik</span><span class="sxs-lookup"><span data-stu-id="40d16-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
