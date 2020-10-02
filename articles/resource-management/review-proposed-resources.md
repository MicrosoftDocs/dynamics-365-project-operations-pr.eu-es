---
title: Berrikusi baliabide proposatuak
description: Gai honek proiektuaren baliabideak proposatzeari buruzko informazioa ematen du.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 212b80a7fde8368eedd7572dd5f9278cc53fae98
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897346"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="cec41-103">Berrikusi baliabide proposatuak</span><span class="sxs-lookup"><span data-stu-id="cec41-103">Review proposed resources</span></span>

<span data-ttu-id="cec41-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="cec41-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cec41-105">Baliabide-kudeatzaileek baliabide bat proposatu diezaiokete proiektu-kudeatzaileari baliabide-eskaera erabiliz.</span><span class="sxs-lookup"><span data-stu-id="cec41-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="cec41-106">Eskaera saretan edo eskaeran bertan, hautatu **Bilatu baliabideak**.</span><span class="sxs-lookup"><span data-stu-id="cec41-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="cec41-107">**Antolaketa-laguntzailea** orrialdean, hautatu baliabidea eta, ondoren, **Sortu baliabideen erreserba** panelean, **Erreserbaren egoera** eremuan, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="cec41-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="cec41-108">Hurrengo egoeraren eguneratzeak gertatzen dira:</span><span class="sxs-lookup"><span data-stu-id="cec41-108">The following status updates occur:</span></span>

- <span data-ttu-id="cec41-109">**Antolaketa-laguntzailea** orrian, egoeraren adierazleak eguneratu egiten dira erreserba proposatu dela adierazteko, ez behin betiko erreserba.</span><span class="sxs-lookup"><span data-stu-id="cec41-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="cec41-110">Baliabide-eskaeran, egoera aldatu egingo da **Berrikusi behar da** egoerara.</span><span class="sxs-lookup"><span data-stu-id="cec41-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="cec41-111">Proiektuaren **Taldea** fitxan, taldeko kide orokorraren **Eskaeraren egoera** balioa **Berrikusi behar da** baliora aldatu da.</span><span class="sxs-lookup"><span data-stu-id="cec41-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="cec41-112">Proiektu-kudeatzaileak proposamena onartu edo baztertu dezake.</span><span class="sxs-lookup"><span data-stu-id="cec41-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="cec41-113">Baliabide-kudeatzaileek baliabide-eskaerak prozesatzen dituztenean, honako ikuspegi hauetakoren bat erabil dezakete:</span><span class="sxs-lookup"><span data-stu-id="cec41-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="cec41-114">Eskaria asetzeko hainbat baliabide proposatzea beharrezko orduak betetzeko baliabiderik ez badago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="cec41-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="cec41-115">Proposatutako orduak behar diren orduak asetzeko baliabide ugarien artean banatzen dira.</span><span class="sxs-lookup"><span data-stu-id="cec41-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="cec41-116">Egoera horretan, orduak ezin dira gainjarri.</span><span class="sxs-lookup"><span data-stu-id="cec41-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="cec41-117">Behar direnak baino baliabide gutxiago proposatzea.</span><span class="sxs-lookup"><span data-stu-id="cec41-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="cec41-118">Egoera horretan, proposatutako baliabideen ahalmena eskatzaileak zehaztutako beharrezko orduak baino txikiagoa da.</span><span class="sxs-lookup"><span data-stu-id="cec41-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="cec41-119">Beraz, eskatzaileak proposatutako baliabideak onartzen dituenean, bete gabeko baliabide-eskakizuna sortzen da geratzen den eskaria harrapatzeko.</span><span class="sxs-lookup"><span data-stu-id="cec41-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="cec41-120">Erreserbatu eskaria asetzeko hainbat baliabide lana osatzeko baliabiderik ez badago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="cec41-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="cec41-121">Behar direnak baino baliabide gutxiago erreserbatzea.</span><span class="sxs-lookup"><span data-stu-id="cec41-121">Book fewer resources than are required.</span></span> <span data-ttu-id="cec41-122">Egoera horretan, erreserbatutako orduak eskatutako orduak baino txikiagoak dira.</span><span class="sxs-lookup"><span data-stu-id="cec41-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="cec41-123">Sistemak erreserbatu beharrean baliabideak proposatzeko gidatzen zaitu, eskatzaileak gainerako eskaerak egiaztatu eta jarrai ditzan.</span><span class="sxs-lookup"><span data-stu-id="cec41-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="cec41-124">Erabilera fakturagarria</span><span class="sxs-lookup"><span data-stu-id="cec41-124">Billable utilization</span></span>

<span data-ttu-id="cec41-125">Baliabideek xede erabilera fakturagarria izan dezakete.</span><span class="sxs-lookup"><span data-stu-id="cec41-125">Resources can have a target billable utilization.</span></span> <span data-ttu-id="cec41-126">Xede-erabilera hori baliabidearen funtzio lehenetsiko atributu gisa definitzen da edo erreserbatu daitekeen baliabide indibidualaren erregistroan ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="cec41-126">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="cec41-127">Erabileraren kalkuluak baliabideek onartutako denbora-sarrerak erabilita jakinarazi dituzten orduetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="cec41-127">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="cec41-128">Erabilera kalkulatzeko honako formula hauek erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="cec41-128">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="cec41-129">Erabilera fakturagarria = Kobratu daitezkeen benetako orduak ÷ Baliabidearen ahalmena</span><span class="sxs-lookup"><span data-stu-id="cec41-129">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="cec41-130">Erabilera ez fakturagarria = ID motako fakturaziodun denbora erreala = Kobratu ezin dena, osagarria edo eskuragarri ez dagoena ÷ Baliabidearen ahalmena</span><span class="sxs-lookup"><span data-stu-id="cec41-130">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="cec41-131">Barnekoa = Salmenta kontraturik gabeko denbora erreala ÷ Baliabideen ahalmena</span><span class="sxs-lookup"><span data-stu-id="cec41-131">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="cec41-132">Baliabideen ahalmena = Baliabideen lan orduak – Bulegotik kanpo – Lanik gabeko egunak</span><span class="sxs-lookup"><span data-stu-id="cec41-132">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="cec41-133">**Baliabideen erabilera** ikuspegia **Baliabideak** panelean aurkituko duzu.</span><span class="sxs-lookup"><span data-stu-id="cec41-133">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="cec41-134">Saretako gelaxka bakoitzak baliabidearen erabilera fakturagarriaren ehunekoa adierazten du aldi batean, hala nola, egun batean, astean edo hilean.</span><span class="sxs-lookup"><span data-stu-id="cec41-134">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="cec41-135">Gelaxkei kolorea emateko honako formula hauek erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="cec41-135">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="cec41-136">**Berdea:** Erabilera fakturagarria \>= Baliabidearen helburuko erabilera</span><span class="sxs-lookup"><span data-stu-id="cec41-136">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="cec41-137">**Horia:** Helburuko erabilera – 20 \<= Erabilera fakturagarria \< Helburuko erabilera</span><span class="sxs-lookup"><span data-stu-id="cec41-137">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="cec41-138">**Gorria:** Erabilera fakturagarria \< Helburuko erabilera – 20</span><span class="sxs-lookup"><span data-stu-id="cec41-138">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="cec41-139">**Baliabide-erabilera** ikuspegia antolaketa-panelean oinarrituta dagoenez, antolaketa paneleko iragazkien ahalmenak erabil ditzakezu emaitzak iragazteko.</span><span class="sxs-lookup"><span data-stu-id="cec41-139">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="cec41-140">Saretak helburuko erabilera ezartzea eskatzen du, bai funtzioan, bai baliabide indibidualean.</span><span class="sxs-lookup"><span data-stu-id="cec41-140">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="cec41-141">Konfigurazio hori egiteko, joan **Baliabideak** \> **Baliabideen funtzioak** atalera.</span><span class="sxs-lookup"><span data-stu-id="cec41-141">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="cec41-142">Gainera, eginkizun lehenetsi bat esleitu behar zaio erreserbatu daitekeen baliabide bakoitzari.</span><span class="sxs-lookup"><span data-stu-id="cec41-142">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="cec41-143">Joan **Baliabideak** \> **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="cec41-143">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="cec41-144">**Project Service** fitxan, egiaztatu baliabide funtzioa definituta dagoela, eta **Lehenetsia da** eremua **Bai** gisa ezarrita dagoela.</span><span class="sxs-lookup"><span data-stu-id="cec41-144">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="cec41-145">Funtzio osagarriak gehi ditzakezu **Lehenetsia da = Ez** den tokian.</span><span class="sxs-lookup"><span data-stu-id="cec41-145">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="cec41-146">**Lehenetsia da = Bai** aukeran erabiltzen den funtzioa baliabidearen erabilera ebaluatzeko erabiltzen da funtzioaren helburuarekin alderatuz.</span><span class="sxs-lookup"><span data-stu-id="cec41-146">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="cec41-147">**Project Service** fitxan, helburuko erabilera indibiduala ere ezar dezakezu baliabiderako.</span><span class="sxs-lookup"><span data-stu-id="cec41-147">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="cec41-148">Ondoren, erabileraren kalkuluak helburuko erabilera hori erabiltzen du baliabidearen helburua ebaluatzeko, baliabidearen funtzio lehenetsiaren helburua ebaluatu beharrean.</span><span class="sxs-lookup"><span data-stu-id="cec41-148">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="cec41-149">Erabilera baliabide gisa erakusten da baliabideak saretan agertzen den aldian kobratu daitekeen denbora onartu badu soilik.</span><span class="sxs-lookup"><span data-stu-id="cec41-149">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="cec41-150">Baliabide-erabilgarritasuna</span><span class="sxs-lookup"><span data-stu-id="cec41-150">Resource availability</span></span>

<span data-ttu-id="cec41-151">Garrantzitsua da baliabide-kudeatzaileak baliabideen erabilgarritasuna eta erreserben eguneratzeak ikusteko gai izatea.</span><span class="sxs-lookup"><span data-stu-id="cec41-151">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="cec41-152">Zenbait kasutan, ez dago eskari formalik (baliabide-eskaera), baina baliabide-kudeatzaileak mezu elektronikoak, telefono-deiak edo berehalako mezuak bezalako kanalen bidez iristen den ezusteko eskaera bati erantzun behar dio.</span><span class="sxs-lookup"><span data-stu-id="cec41-152">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="cec41-153">Baliabide-kudeatzaileek antolaketa-panela erabiltzen dute baliabideak eta erreserbak eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="cec41-153">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="cec41-154">Baliabideen lan orduak baliabide baten erabilgarritasuna kalkulatzeko oinarri gisa erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="cec41-154">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="cec41-155">Baliabideen erreserbak baliabideen ahalmena kontsumitzen du.</span><span class="sxs-lookup"><span data-stu-id="cec41-155">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="cec41-156">Antolaketa-panelak koloreak eta itzalak erabiltzen ditu erreserbetarako, erabilgarritasunerako, gainditutako erreserbetarako eta erreserben egoerarako.</span><span class="sxs-lookup"><span data-stu-id="cec41-156">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="cec41-157">Antolaketa-paneleko ezarpenetako batek legenda erakusten du.</span><span class="sxs-lookup"><span data-stu-id="cec41-157">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="cec41-158">Eskuinera gezi bat agertzen bada erreserbatzeko baliabide indibidualaren ondoan antolaketa-panelean, baliabidea hedatu egin daiteke baliabidea erreserbatuta dagoen lanaren xehetasunak erakusteko.</span><span class="sxs-lookup"><span data-stu-id="cec41-158">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="cec41-159">Dynamics 365 Project Operations aplikazioak Universal Resource Scheduling motorra erabiltzen duenez, Dynamics 365 Field Service instalatuta baduzu, proiektu, lan-eskaera eta antolatzeko hedatu duzun beste edozein entitateren baliabideen erreserben xehetasunak ikus ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="cec41-159">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="cec41-160">Baliabide indibidualei buruzko xehetasun gehiago ikusteko, egin klik eskuineko botoiarekin gainean baliabide-txartela irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="cec41-160">To view more details about an individual resource, right-click it to open the resource card.</span></span>

