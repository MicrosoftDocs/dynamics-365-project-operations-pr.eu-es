---
title: Proposatu proiektuaren baliabideak
description: Gai honek proiektuaren baliabideak proposatzeari buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: bdb0dcb2-4421-4ee1-b97d-89a8cdefbd8d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3a7f7c15c3c7a3c39f2b7b9eeb88b9cf0cfdc220
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748943"
---
# <a name="propose-project-resources"></a><span data-ttu-id="0415f-103">Proposatu proiektuaren baliabideak</span><span class="sxs-lookup"><span data-stu-id="0415f-103">Propose project resources</span></span>

<span data-ttu-id="0415f-104">Baliabide-kudeatzaileek baliabide bat proposatu diezaiokete proiektu-kudeatzaileari baliabide-eskaera erabiliz.</span><span class="sxs-lookup"><span data-stu-id="0415f-104">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="0415f-105">Eskaera saretan edo eskaeran bertan, hautatu **Bilatu baliabideak**.</span><span class="sxs-lookup"><span data-stu-id="0415f-105">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="0415f-106">**Antolaketa-laguntzailea** orrialdean, hautatu baliabidea eta, ondoren, **Sortu baliabideen erreserba** panelean, **Erreserbaren egoera** eremuan, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="0415f-106">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

    ![Hautatutako proposatutako baliabideak](media/Resource-Management-image62.png)

<span data-ttu-id="0415f-108">Hurrengo egoeraren eguneratzeak gertatzen dira:</span><span class="sxs-lookup"><span data-stu-id="0415f-108">The following status updates occur:</span></span>

- <span data-ttu-id="0415f-109">**Antolaketa-laguntzailea** orrian, egoeraren adierazleak eguneratu egiten dira erreserba proposatu dela adierazteko, ez behin betiko erreserba.</span><span class="sxs-lookup"><span data-stu-id="0415f-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>

    ![Antolaketa-laguntzailearen orrian proposatutako erreserben egoeraren adierazleak](media/Resource-Management-image63.png)

- <span data-ttu-id="0415f-111">Baliabide-eskaeran, egoera aldatu egingo da **Berrikusi behar da** egoerara.</span><span class="sxs-lookup"><span data-stu-id="0415f-111">On the resource request, the status is changed to **Needs Review**.</span></span>

    ![Baliabide-eskaeraren egoera aldatu da "Berrikusi behar da" egoerara.](media/Resource-Management-image64.png)

- <span data-ttu-id="0415f-113">Proiektuaren **Taldea** fitxan, taldeko kide orokorraren **Eskaeraren egoera** balioa **Berrikusi behar da** baliora aldatu da.</span><span class="sxs-lookup"><span data-stu-id="0415f-113">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

    ![Proiektuko kide orokorraren eskaera-egoera aldatu egin da "Berrikusi behar da" baliora Taldea fitxan.](media/Resource-Management-image48.png)

<span data-ttu-id="0415f-115">Proiektu-kudeatzaileak proposamena onartu edo baztertu dezake.</span><span class="sxs-lookup"><span data-stu-id="0415f-115">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="0415f-116">Baliabide-kudeatzaileek baliabide-eskaerak prozesatzen dituztenean, honako ikuspegi hauetakoren bat erabil dezakete:</span><span class="sxs-lookup"><span data-stu-id="0415f-116">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="0415f-117">Eskaria asetzeko hainbat baliabide proposatzea beharrezko orduak betetzeko baliabiderik ez badago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="0415f-117">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="0415f-118">Proposatutako orduak behar diren orduak asetzeko baliabide ugarien artean banatzen dira.</span><span class="sxs-lookup"><span data-stu-id="0415f-118">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="0415f-119">Egoera horretan, orduak ezin dira gainjarri.</span><span class="sxs-lookup"><span data-stu-id="0415f-119">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="0415f-120">Behar direnak baino baliabide gutxiago proposatzea.</span><span class="sxs-lookup"><span data-stu-id="0415f-120">Propose fewer resources than are required.</span></span> <span data-ttu-id="0415f-121">Egoera horretan, proposatutako baliabideen ahalmena eskatzaileak zehaztutako beharrezko orduak baino txikiagoa da.</span><span class="sxs-lookup"><span data-stu-id="0415f-121">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="0415f-122">Beraz, eskatzaileak proposatutako baliabideak onartzen dituenean, bete gabeko baliabide-eskakizuna sortzen da geratzen den eskaria harrapatzeko.</span><span class="sxs-lookup"><span data-stu-id="0415f-122">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="0415f-123">Erreserbatu eskaria asetzeko hainbat baliabide lana osatzeko baliabiderik ez badago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="0415f-123">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="0415f-124">Behar direnak baino baliabide gutxiago erreserbatzea.</span><span class="sxs-lookup"><span data-stu-id="0415f-124">Book fewer resources than are required.</span></span> <span data-ttu-id="0415f-125">Egoera horretan, erreserbatutako orduak eskatutako orduak baino txikiagoak dira.</span><span class="sxs-lookup"><span data-stu-id="0415f-125">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="0415f-126">Sistemak erreserbatu beharrean baliabideak proposatzeko gidatzen zaitu, eskatzaileak gainerako eskaerak egiaztatu eta jarrai ditzan.</span><span class="sxs-lookup"><span data-stu-id="0415f-126">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="0415f-127">Erabilera fakturagarria</span><span class="sxs-lookup"><span data-stu-id="0415f-127">Billable utilization</span></span>

<span data-ttu-id="0415f-128">Baliabideek xede erabilera fakturagarria izan dezakete.</span><span class="sxs-lookup"><span data-stu-id="0415f-128">Resources can have a target billable utilization.</span></span> <span data-ttu-id="0415f-129">Xede-erabilera hori baliabidearen funtzio lehenetsiko atributu gisa definitzen da edo erreserbatu daitekeen baliabide indibidualaren erregistroan ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="0415f-129">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="0415f-130">Erabileraren kalkuluak baliabideek onartutako denbora-sarrerak erabilita jakinarazi dituzten orduetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="0415f-130">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="0415f-131">Erabilera kalkulatzeko honako formula hauek erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="0415f-131">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="0415f-132">Erabilera fakturagarria = Kobratu daitezkeen benetako orduak ÷ Baliabidearen ahalmena</span><span class="sxs-lookup"><span data-stu-id="0415f-132">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="0415f-133">Erabilera ez fakturagarria = ID motako fakturaziodun denbora erreala = Kobratu ezin dena, osagarria edo eskuragarri ez dagoena ÷ Baliabidearen ahalmena</span><span class="sxs-lookup"><span data-stu-id="0415f-133">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="0415f-134">Barnekoa = Salmenta kontraturik gabeko denbora erreala ÷ Baliabideen ahalmena</span><span class="sxs-lookup"><span data-stu-id="0415f-134">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="0415f-135">Baliabideen ahalmena = Baliabideen lan orduak – Bulegotik kanpo – Lanik gabeko egunak</span><span class="sxs-lookup"><span data-stu-id="0415f-135">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="0415f-136">**Baliabideen erabilera** ikuspegia **Baliabideak** panelean aurkituko duzu.</span><span class="sxs-lookup"><span data-stu-id="0415f-136">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

![Baliabide-erabileraren ikuspegia](media/Resource-Management-image65.png)

<span data-ttu-id="0415f-138">Saretako gelaxka bakoitzak baliabidearen erabilera fakturagarriaren ehunekoa adierazten du aldi batean, hala nola, egun batean, astean edo hilean.</span><span class="sxs-lookup"><span data-stu-id="0415f-138">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="0415f-139">Gelaxkei kolorea emateko honako formula hauek erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="0415f-139">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="0415f-140">**Berdea:** Erabilera fakturagarria \>= Baliabidearen helburuko erabilera</span><span class="sxs-lookup"><span data-stu-id="0415f-140">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="0415f-141">**Horia:** Helburuko erabilera – 20 \<= Erabilera fakturagarria \< Helburuko erabilera</span><span class="sxs-lookup"><span data-stu-id="0415f-141">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="0415f-142">**Gorria:** Erabilera fakturagarria \< Helburuko erabilera – 20</span><span class="sxs-lookup"><span data-stu-id="0415f-142">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="0415f-143">**Baliabide-erabilera** ikuspegia antolaketa-panelean oinarrituta dagoenez, antolaketa paneleko iragazkien ahalmenak erabil ditzakezu emaitzak iragazteko.</span><span class="sxs-lookup"><span data-stu-id="0415f-143">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="0415f-144">Saretak helburuko erabilera ezartzea eskatzen du, bai funtzioan, bai baliabide indibidualean.</span><span class="sxs-lookup"><span data-stu-id="0415f-144">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="0415f-145">Konfigurazio hori egiteko, joan **Baliabideak** \> **Baliabideen funtzioak** atalera.</span><span class="sxs-lookup"><span data-stu-id="0415f-145">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="0415f-146">Gainera, eginkizun lehenetsi bat esleitu behar zaio erreserbatu daitekeen baliabide bakoitzari.</span><span class="sxs-lookup"><span data-stu-id="0415f-146">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="0415f-147">Joan **Baliabideak** \> **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="0415f-147">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="0415f-148">**Project Service** fitxan, egiaztatu baliabide funtzioa definituta dagoela, eta **Lehenetsia da** eremua **Bai** gisa ezarrita dagoela.</span><span class="sxs-lookup"><span data-stu-id="0415f-148">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="0415f-149">Funtzio osagarriak gehi ditzakezu **Lehenetsia da = Ez** den tokian.</span><span class="sxs-lookup"><span data-stu-id="0415f-149">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="0415f-150">**Lehenetsia da = Bai** aukeran erabiltzen den funtzioa baliabidearen erabilera ebaluatzeko erabiltzen da funtzioaren helburuarekin alderatuz.</span><span class="sxs-lookup"><span data-stu-id="0415f-150">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

![Funtzio lehenetsien multzoa](media/Resource-Management-image67.png)

<span data-ttu-id="0415f-152">**Project Service** fitxan, helburuko erabilera indibiduala ere ezar dezakezu baliabiderako.</span><span class="sxs-lookup"><span data-stu-id="0415f-152">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="0415f-153">Ondoren, erabileraren kalkuluak helburuko erabilera hori erabiltzen du baliabidearen helburua ebaluatzeko, baliabidearen funtzio lehenetsiaren helburua ebaluatu beharrean.</span><span class="sxs-lookup"><span data-stu-id="0415f-153">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="0415f-154">Erabilera baliabide gisa erakusten da baliabideak saretan agertzen den aldian kobratu daitekeen denbora onartu badu soilik.</span><span class="sxs-lookup"><span data-stu-id="0415f-154">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="0415f-155">Baliabide-erabilgarritasuna</span><span class="sxs-lookup"><span data-stu-id="0415f-155">Resource availability</span></span>

<span data-ttu-id="0415f-156">Garrantzitsua da baliabide-kudeatzaileak baliabideen erabilgarritasuna eta erreserben eguneratzeak ikusteko gai izatea.</span><span class="sxs-lookup"><span data-stu-id="0415f-156">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="0415f-157">Zenbait kasutan, ez dago eskari formalik (baliabide-eskaera), baina baliabide-kudeatzaileak mezu elektronikoak, telefono-deiak edo berehalako mezuak bezalako kanalen bidez iristen den ezusteko eskaera bati erantzun behar dio.</span><span class="sxs-lookup"><span data-stu-id="0415f-157">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="0415f-158">Baliabide-kudeatzaileek antolaketa-panela erabiltzen dute baliabideak eta erreserbak eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="0415f-158">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="0415f-159">Baliabideen lan orduak baliabide baten erabilgarritasuna kalkulatzeko oinarri gisa erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="0415f-159">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="0415f-160">Baliabideen erreserbak baliabideen ahalmena kontsumitzen du.</span><span class="sxs-lookup"><span data-stu-id="0415f-160">Resource bookings consume the capacity of the resources.</span></span>

![Programatu taula](media/Resource-Management-image68.png)

<span data-ttu-id="0415f-162">Antolaketa-panelak koloreak eta itzalak erabiltzen ditu erreserbetarako, erabilgarritasunerako, gainditutako erreserbetarako eta erreserben egoerarako.</span><span class="sxs-lookup"><span data-stu-id="0415f-162">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="0415f-163">Antolaketa-paneleko ezarpenetako batek legenda erakusten du.</span><span class="sxs-lookup"><span data-stu-id="0415f-163">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="0415f-164">Eskuinera gezi bat agertzen bada erreserbatzeko baliabide indibidualaren ondoan antolaketa-panelean, baliabidea hedatu egin daiteke baliabidea erreserbatuta dagoen lanaren xehetasunak erakusteko.</span><span class="sxs-lookup"><span data-stu-id="0415f-164">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

![Antolaketa-panelean hedatuta dagoen baliabide erreserbagarria](media/Resource-Management-image69.png)

<span data-ttu-id="0415f-166">Dynamics 365 Project Service Automation aplikazioak Universal Resource Scheduling motorra erabiltzen duenez, Dynamics 365 Field Service instalatuta baduzu, proiektu, lan-eskaera eta antolatzeko hedatu duzun beste edozein entitateren baliabideen erreserben xehetasunak ikus ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="0415f-166">Because Dynamics 365 Project Service Automation uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

![Proiektuetarako eta lan-eskaeretarako baliabideen erreserbaren xehetasunak](media/Resource-Management-image70.png)

<span data-ttu-id="0415f-168">Baliabide indibidualei buruzko xehetasun gehiago ikusteko, egin klik eskuineko botoiarekin gainean baliabide-txartela irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="0415f-168">To view more details about an individual resource, right-click it to open the resource card.</span></span>

![Baliabide-txartela](media/Resource-Management-image71.png)
