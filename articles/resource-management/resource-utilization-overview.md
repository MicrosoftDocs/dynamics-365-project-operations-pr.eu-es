---
title: Baliabide-erabileraren informazio orokorra
description: Gai honek baliabideen erabilerari buruzko informazioa eskaintzen du Project Operations-en.
author: ruhercul
ms.date: 11/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: c9464b1de87211f8317a39a1d749e619769309ae
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/07/2021
ms.locfileid: "6367921"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="f80ab-103">Baliabide-erabileraren informazio orokorra</span><span class="sxs-lookup"><span data-stu-id="f80ab-103">Resource utilization overview</span></span>

<span data-ttu-id="f80ab-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="f80ab-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f80ab-105">Baliabideek xede erabilera fakturagarria izan dezakete.</span><span class="sxs-lookup"><span data-stu-id="f80ab-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="f80ab-106">Xede-erabilera hori baliabidearen funtzio lehenetsiko atributu gisa definitzen da edo erreserbatu daitekeen baliabide indibidualaren erregistroan ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="f80ab-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="f80ab-107">Erabileraren kalkuluak baliabideek onartutako denbora-sarrerak erabilita jakinarazi dituzten orduetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="f80ab-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="f80ab-108">Erabilera kalkulatzeko honako formula hauek erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="f80ab-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="f80ab-109">Erabilera fakturagarria = Kobratu daitezkeen benetako orduak ÷ Baliabidearen ahalmena</span><span class="sxs-lookup"><span data-stu-id="f80ab-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="f80ab-110">Erabilera ez fakturagarria = ID motako fakturaziodun denbora erreala = Kobratu ezin dena, osagarria edo eskuragarri ez dagoena ÷ Baliabidearen ahalmena</span><span class="sxs-lookup"><span data-stu-id="f80ab-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="f80ab-111">Barnekoa = Salmenta kontraturik gabeko denbora erreala ÷ Baliabideen ahalmena</span><span class="sxs-lookup"><span data-stu-id="f80ab-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="f80ab-112">Baliabideen ahalmena = Baliabideen lan orduak – Bulegotik kanpo – Lanik gabeko egunak</span><span class="sxs-lookup"><span data-stu-id="f80ab-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="f80ab-113">**Baliabideen erabilera** ikuspegia **Baliabideak** panelean aurkituko duzu.</span><span class="sxs-lookup"><span data-stu-id="f80ab-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="f80ab-114">Saretako gelaxka bakoitzak baliabidearen erabilera fakturagarriaren ehunekoa adierazten du aldi batean, hala nola, egun batean, astean edo hilean.</span><span class="sxs-lookup"><span data-stu-id="f80ab-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="f80ab-115">Gelaxkei kolorea emateko honako formula hauek erabiltzen dira:</span><span class="sxs-lookup"><span data-stu-id="f80ab-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="f80ab-116">**Berdea**: Fakturazioaren erabilera >= Baliabidearen helburuko erabilera</span><span class="sxs-lookup"><span data-stu-id="f80ab-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="f80ab-117">**Horia**: Helburuaren erabilera – 20 < Fakturazioaren erabilera = < Helburuko erabilera</span><span class="sxs-lookup"><span data-stu-id="f80ab-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="f80ab-118">**Gorria**: Erabilera fakturagarria < Helburuko erabilera - 20</span><span class="sxs-lookup"><span data-stu-id="f80ab-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="f80ab-119">**Baliabide-erabilera** ikuspegia antolaketa-panelean oinarrituta dagoenez, antolaketa paneleko iragazkien ahalmenak erabil ditzakezu emaitzak iragazteko.</span><span class="sxs-lookup"><span data-stu-id="f80ab-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="f80ab-120">Saretak helburuko erabilera ezartzea eskatzen du, bai funtzioan, bai baliabide indibidualean.</span><span class="sxs-lookup"><span data-stu-id="f80ab-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="f80ab-121">Konfigurazio hori egiteko, joan **Baliabideak** > **Baliabideen funtzioak** atalera.</span><span class="sxs-lookup"><span data-stu-id="f80ab-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="f80ab-122">Gainera, eginkizun lehenetsi bat esleitu behar zaio erreserbatu daitekeen baliabide bakoitzari.</span><span class="sxs-lookup"><span data-stu-id="f80ab-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="f80ab-123">Joan **Baliabideak** > **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="f80ab-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="f80ab-124">**Project Service** fitxan, egiaztatu baliabide funtzioa definituta dagoela, eta **Lehenetsia da** eremua **Bai** gisa ezarrita dagoela.</span><span class="sxs-lookup"><span data-stu-id="f80ab-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="f80ab-125">Funtzio osagarriak gehi ditzakezu **Lehenetsia da** = **Ez** den tokian.</span><span class="sxs-lookup"><span data-stu-id="f80ab-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="f80ab-126">**Lehenetsia da** = **Bai** aukeran erabiltzen den funtzioa baliabidearen erabilera ebaluatzeko erabiltzen da funtzioaren helburuarekin alderatuz.</span><span class="sxs-lookup"><span data-stu-id="f80ab-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="f80ab-127">**Project Service** fitxan, helburuko erabilera indibiduala ere ezar dezakezu baliabiderako.</span><span class="sxs-lookup"><span data-stu-id="f80ab-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="f80ab-128">Ondoren, erabileraren kalkuluak helburuko erabilera hori erabiltzen du baliabidearen helburua ebaluatzeko, baliabidearen funtzio lehenetsiaren helburua ebaluatu beharrean.</span><span class="sxs-lookup"><span data-stu-id="f80ab-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="f80ab-129">Erabilera baliabide gisa erakusten da baliabideak saretan agertzen den aldian kobratu daitekeen denbora onartu badu soilik.</span><span class="sxs-lookup"><span data-stu-id="f80ab-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]