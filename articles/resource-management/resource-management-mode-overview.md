---
title: Baliabide-kudeaketaren moduen informazio orokorra
description: Gai honek Baliabide-kudeaketaren funtzionalitateari buruzko informazioa ematen du Dynamics 365 Project Operations-en.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4d132bcbef5421202d2f4899091f0dc75166dd66
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949934"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="c3f30-103">Baliabideen kudeaketaren moduen informazio orokorra</span><span class="sxs-lookup"><span data-stu-id="c3f30-103">Resource management modes overview</span></span>

<span data-ttu-id="c3f30-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="c3f30-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c3f30-105">Dynamics 365 Project Operations-ek bi modu onartzen ditu erreserba-fluxu orokorra exekutatu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="c3f30-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="c3f30-106">Kudeaketa modua proiektuaren parametro gisa definitzen da eta zure negozioa aldatu behar bada alda daiteke.</span><span class="sxs-lookup"><span data-stu-id="c3f30-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="c3f30-107">Modu zentrala</span><span class="sxs-lookup"><span data-stu-id="c3f30-107">Central mode</span></span>
<span data-ttu-id="c3f30-108">Proiektuetarako baliabideen zuzkidura zentralizatzen duten erakundeentzat, Modu Zentralak proiektuaren kudeatzaileek proiektuaren mailan baliabideen eskakizunak definitu ahal izateko modua eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="c3f30-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="c3f30-109">Baliabideen eskakizunak betetzea Baliabideen kudeatzaileari eskuordetzen zaio.</span><span class="sxs-lookup"><span data-stu-id="c3f30-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="c3f30-110">Proiektuen kudeatzaileek baliabideen kudeatzaileak proposatutako baliabideak onartu edo baztertu ditzakete.</span><span class="sxs-lookup"><span data-stu-id="c3f30-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![Modu zentrala](./media/resource-management-central.png)

<span data-ttu-id="c3f30-112">Baliabideak Erdiko moduarekin kudeatzeko, ikusi:</span><span class="sxs-lookup"><span data-stu-id="c3f30-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="c3f30-113">Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak</span><span class="sxs-lookup"><span data-stu-id="c3f30-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="c3f30-114">Erreserbatu izena duten baliabideak baliabide-eskakizunetatik</span><span class="sxs-lookup"><span data-stu-id="c3f30-114">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="c3f30-115">Bidali baliabide-eskaera bat</span><span class="sxs-lookup"><span data-stu-id="c3f30-115">Submit a resource request</span></span>](/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="c3f30-116">Bete baliabide-eskaera</span><span class="sxs-lookup"><span data-stu-id="c3f30-116">Fulfill a resource request</span></span>](/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="c3f30-117">Onartu edo baztertu proposatutako proiektuaren baliabidea baliabide-eskaera batetik</span><span class="sxs-lookup"><span data-stu-id="c3f30-117">Accept or reject a proposed project resource from a resource request</span></span>](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="c3f30-118">Modu hibridoa</span><span class="sxs-lookup"><span data-stu-id="c3f30-118">Hybrid mode</span></span>
<span data-ttu-id="c3f30-119">Baliabideen banaketan malgutasuna behar duten erakundeentzat, modu hibridoak proiektuen kudeatzaileei eta baliabideen kudeatzaileei baliabideak erreserbatzeko aukera ematen die.</span><span class="sxs-lookup"><span data-stu-id="c3f30-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![Modu hibridoa](./media/resource-management-hybrid.png)

<span data-ttu-id="c3f30-121">Onartutako Erdiko moduaren prozesua ez ezik, ikusi gai hauek Hibrido moduan onartutako erreserba-fluxu guztiak kudeatzeko:</span><span class="sxs-lookup"><span data-stu-id="c3f30-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="c3f30-122">Erreserbatu baliabide bat zuzenean proiektu bati:</span><span class="sxs-lookup"><span data-stu-id="c3f30-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="c3f30-123">Erreserbatu baliabide erreserbagarriak proiektuko talde bati eta esleitu zereginak</span><span class="sxs-lookup"><span data-stu-id="c3f30-123">Book named bookable resources to a project team and assign tasks</span></span>](/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="c3f30-124">Erreserbatu baliabide bat baliabide-eskakizunetatik:</span><span class="sxs-lookup"><span data-stu-id="c3f30-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="c3f30-125">Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide-eskakizunak</span><span class="sxs-lookup"><span data-stu-id="c3f30-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="c3f30-126">Erreserbatu izena duten baliabideak baliabide-eskakizunetatik</span><span class="sxs-lookup"><span data-stu-id="c3f30-126">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]