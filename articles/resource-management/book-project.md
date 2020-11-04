---
title: Erreserbatu proiektu bat
description: Gai honek proiektu baterako baliabideak erreserbatzeari buruzko informazioa ematen du.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 19128264ed3db7efeeba948155f0ddbdc806c2a0
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070888"
---
# <a name="book-to-a-project"></a><span data-ttu-id="76fdd-103">Erreserbatu proiektu bat</span><span class="sxs-lookup"><span data-stu-id="76fdd-103">Book to a project</span></span>

<span data-ttu-id="76fdd-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="76fdd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="76fdd-105">Batzuetan, Proiektu kudeatzaile batek edo Baliabide kudeatzaile batek baliabide bat esleitu beharko du proiektura taldekide generiko batek eskatzen duen baldintza zehatzik zehaztu gabe.</span><span class="sxs-lookup"><span data-stu-id="76fdd-105">There are times where a Project manager or Resource manager will need to allocate a resource to project without a specific requirement being defined from a generic team member.</span></span> <span data-ttu-id="76fdd-106">Hori hiru eratara lor daiteke.</span><span class="sxs-lookup"><span data-stu-id="76fdd-106">This can be achieved in one of three ways.</span></span>

- <span data-ttu-id="76fdd-107">Erreserbatu taldearen kide saretatik</span><span class="sxs-lookup"><span data-stu-id="76fdd-107">Book from the team member grid</span></span>
- <span data-ttu-id="76fdd-108">Erreserbatu antolaketa-paneletik</span><span class="sxs-lookup"><span data-stu-id="76fdd-108">Book from the schedule board</span></span>
- <span data-ttu-id="76fdd-109">Erreserbat **Proiektua** inprimakitik</span><span class="sxs-lookup"><span data-stu-id="76fdd-109">Book from the **Project** form</span></span>

## <a name="book-from-the-team-member-grid"></a><span data-ttu-id="76fdd-110">Erreserbatu taldearen kide saretatik</span><span class="sxs-lookup"><span data-stu-id="76fdd-110">Book from the team member grid</span></span>

<span data-ttu-id="76fdd-111">Zure erakundea Baliabideen esleipen modu hibridoan funtzionatzen badu, proiektuaren kudeatzaileak baliabide bat zuzenean proiektuan erreserbatu dezake, urrats hauek emanez.</span><span class="sxs-lookup"><span data-stu-id="76fdd-111">If your organization is operating in hybrid Resource allocation mode, the Project manager can book a resource directly to the project by completing the following steps.</span></span>

1. <span data-ttu-id="76fdd-112">Proiektuan, joan taldekideen sarera eta hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="76fdd-112">From the project, go to the team member grid and select **New**.</span></span>
2. <span data-ttu-id="76fdd-113">Definitu posizioaren izena eta baliabidearen rola.</span><span class="sxs-lookup"><span data-stu-id="76fdd-113">Define the position name and the role of the resource.</span></span>
3. <span data-ttu-id="76fdd-114">Hautatu baliabide erreserbagarria bilaketa erabilgarritik.</span><span class="sxs-lookup"><span data-stu-id="76fdd-114">Select the bookable resource from the available lookup.</span></span>
4. <span data-ttu-id="76fdd-115">Baliabidea hautatu ondoren, definitu eremuko informazio hau baliabidea erreserbatzeko:</span><span class="sxs-lookup"><span data-stu-id="76fdd-115">After you select the resource, define the following field information to book the resource:</span></span>

    - <span data-ttu-id="76fdd-116">Hasiera-data</span><span class="sxs-lookup"><span data-stu-id="76fdd-116">Start date</span></span>
    - <span data-ttu-id="76fdd-117">Amaieraren data</span><span class="sxs-lookup"><span data-stu-id="76fdd-117">Finish date</span></span>
    - <span data-ttu-id="76fdd-118">Esleipen-metodoa</span><span class="sxs-lookup"><span data-stu-id="76fdd-118">Allocation method</span></span>
    - <span data-ttu-id="76fdd-119">Ordutegia, hala badagokio</span><span class="sxs-lookup"><span data-stu-id="76fdd-119">Hours, if applicable</span></span>
    - <span data-ttu-id="76fdd-120">Proiektuaren onartzailea</span><span class="sxs-lookup"><span data-stu-id="76fdd-120">Project approver</span></span>

6. <span data-ttu-id="76fdd-121">Hautatu **Gorde eta itxi**</span><span class="sxs-lookup"><span data-stu-id="76fdd-121">Select **Save and Close**</span></span>

## <a name="book-from-the-schedule-board"></a><span data-ttu-id="76fdd-122">Erreserbatu antolaketa-paneletik</span><span class="sxs-lookup"><span data-stu-id="76fdd-122">Book from the schedule board</span></span>

<span data-ttu-id="76fdd-123">Baliabide kudeatzaile batek baliabide bat zuzenean proiektu batera erreserbatu behar duenean, ordutegi taula eta proiektuaren eskakizuna erabil ditzake.</span><span class="sxs-lookup"><span data-stu-id="76fdd-123">When a Resource manager needs to book a resource directly to a project, they can use the schedule board and the project requirement.</span></span> <span data-ttu-id="76fdd-124">Proiektuaren eskakizuna beti erreserbatzeko eskuragarri dagoen baliabide-eskakizuna da.</span><span class="sxs-lookup"><span data-stu-id="76fdd-124">The project requirement is a resource requirement that is always available to be booked against.</span></span> <span data-ttu-id="76fdd-125">Antolaketa-paneletik proiektu inprimaki bat zuzenean erreserbatzeko, egin urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="76fdd-125">To book directly to a project form the schedule board, complete the following steps.</span></span>

1. <span data-ttu-id="76fdd-126">Joan ordutegira eta ezkerreko orrian, iragazi eskakizunerako kontuan hartzen ari zaren baliabideak.</span><span class="sxs-lookup"><span data-stu-id="76fdd-126">Navigate to the schedule board and on the left page, filter for the resources you are considering for the requirement.</span></span>
2. <span data-ttu-id="76fdd-127">Beheko panelean, hautatu **Proiektua** fitxa proiektuaren eskakizunen zerrenda ikusteko.</span><span class="sxs-lookup"><span data-stu-id="76fdd-127">In the bottom pane, select the **Project** tab to view a list of project requirements.</span></span>
3. <span data-ttu-id="76fdd-128">Arrastatu eskakizuna baliabide batera eta definitu informazio hau:</span><span class="sxs-lookup"><span data-stu-id="76fdd-128">Drag the requirement onto a resource and define the following information:</span></span>

    - <span data-ttu-id="76fdd-129">Hasiera-data</span><span class="sxs-lookup"><span data-stu-id="76fdd-129">Start date</span></span>
    - <span data-ttu-id="76fdd-130">Amaieraren data</span><span class="sxs-lookup"><span data-stu-id="76fdd-130">Finish date</span></span>
    - <span data-ttu-id="76fdd-131">Erreserba-egoera</span><span class="sxs-lookup"><span data-stu-id="76fdd-131">Booking status</span></span>
    - <span data-ttu-id="76fdd-132">Erreserba-metodoa</span><span class="sxs-lookup"><span data-stu-id="76fdd-132">Booking method</span></span>
    - <span data-ttu-id="76fdd-133">Iraupena</span><span class="sxs-lookup"><span data-stu-id="76fdd-133">Duration</span></span>

## <a name="book-from-the-project-form"></a><span data-ttu-id="76fdd-134">Erreserbat Proiektua inprimakitik</span><span class="sxs-lookup"><span data-stu-id="76fdd-134">Book from the Project form</span></span>

<span data-ttu-id="76fdd-135">Proiektu kudeatzailea zarenez, baliteke proiektu baterako baliabide bat erreserbatu behar izatea, baina baliabidearen izena baino irizpideak bakarrik ezagutu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="76fdd-135">As a Project manager, you might need to book a resource to a project, but only know the criteria rather than the name of the resource.</span></span> <span data-ttu-id="76fdd-136">Osatu urrats hauek programazio laguntzailea baliabidearen eskuragarri dauden atributuetan oinarritutako baliabide bat aurkitzeko.</span><span class="sxs-lookup"><span data-stu-id="76fdd-136">Complete the following steps to use the schedule assistant to find a resource based on any available attributes of the resource.</span></span> 

1. <span data-ttu-id="76fdd-137">Joan proiektura eta hautatu **Erreserbatu** Antolaketa laguntzailea irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="76fdd-137">Navigate to the project and select **Book** to open the Schedule Assistant.</span></span>
2. <span data-ttu-id="76fdd-138">Ordutegi Laguntzailearen ezkerraldeko iragazkiak erabiliz, irizpideak murriztu eta hautatu **Bilatu**.</span><span class="sxs-lookup"><span data-stu-id="76fdd-138">Using the filters on the left side of the Schedule Assistant, narrow the criteria and select **Search.**</span></span>
3. <span data-ttu-id="76fdd-139">Emaitzetan itzulitako baliabideetan oinarrituta, baliabide bat erreserbatu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="76fdd-139">Based on resources returned in the results, you can book a resource.</span></span>

> [!NOTE]
> <span data-ttu-id="76fdd-140">Metodo honek ez du baliabiderako erreserbarik sortzen.</span><span class="sxs-lookup"><span data-stu-id="76fdd-140">This method doesn't create any bookings for the resource.</span></span> <span data-ttu-id="76fdd-141">Edo, baliabidea gehitzen du taldean.</span><span class="sxs-lookup"><span data-stu-id="76fdd-141">Instead, it adds the resource to the team.</span></span> <span data-ttu-id="76fdd-142">Taldekidea proiektuan gehitu ondoren, proiektuaren zuzendariak erreserbak mantendu edo erreserbak luzatu ahal izango ditu baliabidean beharrezko erreserbak gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="76fdd-142">After the team member has been added to the project, the project manager can use maintain bookings or extend bookings to add the required bookings to the resource.</span></span>
