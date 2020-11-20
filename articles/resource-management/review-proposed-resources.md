---
title: Berrikusi baliabide proposatuak
description: Gai honek proiektuaren baliabideak proposatzeari buruzko informazioa ematen du.
author: ruhercul
manager: AnnBe
ms.date: 11/05/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 54a0924da17eac86e2fa400540e629f6d803aa35
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401158"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="32f3c-103">Berrikusi baliabide proposatuak</span><span class="sxs-lookup"><span data-stu-id="32f3c-103">Review proposed resources</span></span>

<span data-ttu-id="32f3c-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="32f3c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="32f3c-105">Baliabide-kudeatzaileek baliabide bat proposatu diezaiokete proiektu-kudeatzaileari baliabide-eskaera erabiliz.</span><span class="sxs-lookup"><span data-stu-id="32f3c-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="32f3c-106">Eskaera saretan edo eskaeran bertan, hautatu **Bilatu baliabideak**.</span><span class="sxs-lookup"><span data-stu-id="32f3c-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="32f3c-107">**Antolaketa-laguntzailea** orrialdean, hautatu baliabidea eta, ondoren, **Sortu baliabideen erreserba** panelean, **Erreserbaren egoera** eremuan, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="32f3c-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="32f3c-108">Hurrengo egoeraren eguneratzeak gertatzen dira:</span><span class="sxs-lookup"><span data-stu-id="32f3c-108">The following status updates occur:</span></span>

- <span data-ttu-id="32f3c-109">**Antolaketa-laguntzailea** orrian, egoeraren adierazleak eguneratu egiten dira erreserba proposatu dela adierazteko, ez behin betiko erreserba.</span><span class="sxs-lookup"><span data-stu-id="32f3c-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="32f3c-110">Baliabide-eskaeran, egoera aldatu egingo da **Berrikusi behar da** egoerara.</span><span class="sxs-lookup"><span data-stu-id="32f3c-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="32f3c-111">Proiektuaren **Taldea** fitxan, taldeko kide orokorraren **Eskaeraren egoera** balioa **Berrikusi behar da** baliora aldatu da.</span><span class="sxs-lookup"><span data-stu-id="32f3c-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="32f3c-112">Proiektu-kudeatzaileak proposamena onartu edo baztertu dezake.</span><span class="sxs-lookup"><span data-stu-id="32f3c-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="32f3c-113">Baliabide-kudeatzaileek baliabide-eskaerak prozesatzen dituztenean, honako ikuspegi hauetakoren bat erabil dezakete:</span><span class="sxs-lookup"><span data-stu-id="32f3c-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="32f3c-114">Eskaria asetzeko hainbat baliabide proposatzea beharrezko orduak betetzeko baliabiderik ez badago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="32f3c-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="32f3c-115">Proposatutako orduak behar diren orduak asetzeko baliabide ugarien artean banatzen dira.</span><span class="sxs-lookup"><span data-stu-id="32f3c-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="32f3c-116">Egoera horretan, orduak ezin dira gainjarri.</span><span class="sxs-lookup"><span data-stu-id="32f3c-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="32f3c-117">Behar direnak baino baliabide gutxiago proposatzea.</span><span class="sxs-lookup"><span data-stu-id="32f3c-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="32f3c-118">Egoera horretan, proposatutako baliabideen ahalmena eskatzaileak zehaztutako beharrezko orduak baino txikiagoa da.</span><span class="sxs-lookup"><span data-stu-id="32f3c-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="32f3c-119">Beraz, eskatzaileak proposatutako baliabideak onartzen dituenean, bete gabeko baliabide-eskakizuna sortzen da geratzen den eskaria harrapatzeko.</span><span class="sxs-lookup"><span data-stu-id="32f3c-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="32f3c-120">Erreserbatu eskaria asetzeko hainbat baliabide lana osatzeko baliabiderik ez badago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="32f3c-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="32f3c-121">Behar direnak baino baliabide gutxiago erreserbatzea.</span><span class="sxs-lookup"><span data-stu-id="32f3c-121">Book fewer resources than are required.</span></span> <span data-ttu-id="32f3c-122">Egoera horretan, erreserbatutako orduak eskatutako orduak baino txikiagoak dira.</span><span class="sxs-lookup"><span data-stu-id="32f3c-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="32f3c-123">Sistemak erreserbatu beharrean baliabideak proposatzeko gidatzen zaitu, eskatzaileak gainerako eskaerak egiaztatu eta jarrai ditzan.</span><span class="sxs-lookup"><span data-stu-id="32f3c-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="32f3c-124">Baliabide-erabilgarritasuna</span><span class="sxs-lookup"><span data-stu-id="32f3c-124">Resource availability</span></span>

<span data-ttu-id="32f3c-125">Garrantzitsua da baliabide-kudeatzaileak baliabideen erabilgarritasuna eta erreserben eguneratzeak ikusteko gai izatea.</span><span class="sxs-lookup"><span data-stu-id="32f3c-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="32f3c-126">Zenbait kasutan, ez dago eskari formalik (baliabide-eskaera), baina baliabide-kudeatzaileak mezu elektronikoak, telefono-deiak edo berehalako mezuak bezalako kanalen bidez iristen den ezusteko eskaera bati erantzun behar dio.</span><span class="sxs-lookup"><span data-stu-id="32f3c-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="32f3c-127">Baliabide-kudeatzaileek antolaketa-panela erabiltzen dute baliabideak eta erreserbak eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="32f3c-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="32f3c-128">Baliabideen lan orduak baliabide baten erabilgarritasuna kalkulatzeko oinarri gisa erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="32f3c-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="32f3c-129">Baliabideen erreserbak baliabideen ahalmena kontsumitzen du.</span><span class="sxs-lookup"><span data-stu-id="32f3c-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="32f3c-130">Antolaketa-panelak koloreak eta itzalak erabiltzen ditu erreserbetarako, erabilgarritasunerako, gainditutako erreserbetarako eta erreserben egoerarako.</span><span class="sxs-lookup"><span data-stu-id="32f3c-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="32f3c-131">Antolaketa-paneleko ezarpenetako batek legenda erakusten du.</span><span class="sxs-lookup"><span data-stu-id="32f3c-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="32f3c-132">Eskuinera gezi bat agertzen bada erreserbatzeko baliabide indibidualaren ondoan antolaketa-panelean, baliabidea hedatu egin daiteke baliabidea erreserbatuta dagoen lanaren xehetasunak erakusteko.</span><span class="sxs-lookup"><span data-stu-id="32f3c-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="32f3c-133">Dynamics 365 Project Operations aplikazioak Universal Resource Scheduling motorra erabiltzen duenez, Dynamics 365 Field Service instalatuta baduzu, proiektu, lan-eskaera eta antolatzeko hedatu duzun beste edozein entitateren baliabideen erreserben xehetasunak ikus ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="32f3c-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="32f3c-134">Baliabide indibidualei buruzko xehetasun gehiago ikusteko, egin klik eskuineko botoiarekin gainean baliabide-txartela irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="32f3c-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>

