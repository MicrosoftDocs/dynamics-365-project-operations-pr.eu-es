---
title: Antolaketa moduak
description: Gai honek antolaketa moduei buruzko informazioa ematen du.
author: ruhercul
manager: AnnBe
ms.date: 05/04/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fe54944999617b248ff925148a78601dd4be7aca
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981420"
---
# <a name="scheduling-modes"></a><span data-ttu-id="9b916-103">Antolaketa moduak</span><span class="sxs-lookup"><span data-stu-id="9b916-103">Scheduling modes</span></span>

<span data-ttu-id="9b916-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="9b916-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="9b916-105">Dynamics 365 Project Operations gaitasuna ematen die erakundeei lanaren banakako egituraren zereginetan aldagai gakoen aldaketak nola kudeatzen dituzten definitzeko.</span><span class="sxs-lookup"><span data-stu-id="9b916-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="9b916-106">Erakundearen behar espezifikoetan oinarrituta, proiektuen arduradunek planifikazio moduan aldaketak egin ditzakete proiektu bat sortzen denean.</span><span class="sxs-lookup"><span data-stu-id="9b916-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="9b916-107">Project Operations-en hiru programazio modu daude eskuragarri:</span><span class="sxs-lookup"><span data-stu-id="9b916-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="9b916-108">Iraupen finkoa (modu lehenetsia da)</span><span class="sxs-lookup"><span data-stu-id="9b916-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="9b916-109">Lan finkoa</span><span class="sxs-lookup"><span data-stu-id="9b916-109">Fixed work</span></span>
  - <span data-ttu-id="9b916-110">Unitate finkoak</span><span class="sxs-lookup"><span data-stu-id="9b916-110">Fixed units</span></span>

<span data-ttu-id="9b916-111">Programazio modu zehatz baten definizioak eragindako balioak honako formula honen bidez zehazten dira:</span><span class="sxs-lookup"><span data-stu-id="9b916-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="9b916-112">Esfortzua (*Lana*) = Iraupena x Unitateak</span><span class="sxs-lookup"><span data-stu-id="9b916-112">Effort (*Work*) = Duration x Units</span></span>

<span data-ttu-id="9b916-113">Proiektu baten antolaketa modua definitzen duzunean, balio horietako bat ezartzen ari zara, gero aldatu ezin direnak.</span><span class="sxs-lookup"><span data-stu-id="9b916-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="9b916-114">Balio hori konstante gisa mantentzeak lehentasuna ematen dio balio horri, eta horrek sistemari beste bi balioak aldatzen direnean ez aldatzeko jakinarazten dio.</span><span class="sxs-lookup"><span data-stu-id="9b916-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="9b916-115">Ondorengo taulan modu zehatz bat hautatzearen eraginari buruzko informazioa ematen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="9b916-116">**Zereginean**</span><span class="sxs-lookup"><span data-stu-id="9b916-116">**In this task**</span></span>             | <span data-ttu-id="9b916-117">**Unitateak berrikusten badituzu**</span><span class="sxs-lookup"><span data-stu-id="9b916-117">**If you revise units**</span></span>   | <span data-ttu-id="9b916-118">**Iraupena berrikusten baduzu**</span><span class="sxs-lookup"><span data-stu-id="9b916-118">**If you revise duration**</span></span> | <span data-ttu-id="9b916-119">**Esfortzua berrikusten baduzu**</span><span class="sxs-lookup"><span data-stu-id="9b916-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="9b916-120">Unitate-zeregin finkoak</span><span class="sxs-lookup"><span data-stu-id="9b916-120">Fixed units task</span></span>     | <span data-ttu-id="9b916-121">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-121">Duration is recalculated.</span></span> | <span data-ttu-id="9b916-122">Ahalegina berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-122">Effort is recalculated.</span></span>    | <span data-ttu-id="9b916-123">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="9b916-124">Ahalegin finkoaren zeregina</span><span class="sxs-lookup"><span data-stu-id="9b916-124">Fixed effort task</span></span>    | <span data-ttu-id="9b916-125">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-125">Duration is recalculated.</span></span> | <span data-ttu-id="9b916-126">Unitateak berriro kalkulatzen dira.</span><span class="sxs-lookup"><span data-stu-id="9b916-126">Units are recalculated.</span></span>    | <span data-ttu-id="9b916-127">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="9b916-128">Iraupen finkoko zeregina</span><span class="sxs-lookup"><span data-stu-id="9b916-128">Fixed duration task</span></span>  | <span data-ttu-id="9b916-129">Ahalegina berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-129">Effort is recalculated.</span></span>   | <span data-ttu-id="9b916-130">Ahalegina berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="9b916-130">Effort is recalculated.</span></span>    | <span data-ttu-id="9b916-131">Unitateak berriro kalkulatzen dira.</span><span class="sxs-lookup"><span data-stu-id="9b916-131">Units are recalculated.</span></span>   |

<span data-ttu-id="9b916-132">Modu jakin baten inplikazioei buruzko informazio gehiago lortzeko, ikusi [Aldatu zeregin mota programazio zehatzagoa lortzeko](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="9b916-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="9b916-133">Gaian, terminoa **Lana** ordez erabiltzen da **Esfortzua**.</span><span class="sxs-lookup"><span data-stu-id="9b916-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="9b916-134">Aldatu erakundearen programazio modua</span><span class="sxs-lookup"><span data-stu-id="9b916-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="9b916-135">Osatu urrats hauek erakunde baten antolaketa modua definitzeko.</span><span class="sxs-lookup"><span data-stu-id="9b916-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="9b916-136">Joan **Ezarpenak**\> **Orokorra** \> **Parametroak** aukerara, eta hautatu proiektuaren parametroa.</span><span class="sxs-lookup"><span data-stu-id="9b916-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="9b916-137">**Proiektuaren parametroak** orrialdean, hautatu antolaketarako antolaketa modu lehenetsia eta, ondoren, proiektuaren kudeatzaileak proiektu berria sortzerakoan ezarpena gainidazteko duen gaitasuna definitu.</span><span class="sxs-lookup"><span data-stu-id="9b916-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="9b916-138">Aldatu proiektu baten antolaketa moduaren ezarpena</span><span class="sxs-lookup"><span data-stu-id="9b916-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="9b916-139">Erakunde batek proiektuaren kudeatzaileari antolaketa modu lehenetsia gainbideratzen uzten badio, proiektuaren kudeatzaileak proiektu hori sortzen duenean aldaketa hori egin dezake.</span><span class="sxs-lookup"><span data-stu-id="9b916-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="9b916-140">Hala ere, proiektua gorde eta gero, ezin da planifikazio modua aldatu.</span><span class="sxs-lookup"><span data-stu-id="9b916-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="9b916-141">Kopiatutako proiektuak</span><span class="sxs-lookup"><span data-stu-id="9b916-141">Copied projects</span></span>

<span data-ttu-id="9b916-142">Kopiatu proiektuaren ekintza egiten denean proiektu bat sortzen denez, Proiektu kudeatzaileak ezin du planifikazio modua ezarri.</span><span class="sxs-lookup"><span data-stu-id="9b916-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="9b916-143">Helmugako proiektuak beti antolaketa mailan definitutako modua lehenetsiko du.</span><span class="sxs-lookup"><span data-stu-id="9b916-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="9b916-144">Kopiatutako zereginak</span><span class="sxs-lookup"><span data-stu-id="9b916-144">Copied tasks</span></span>

<span data-ttu-id="9b916-145">Zeregin bat proiektu batetik bestera kopiatzen denean, zereginak helmugako proiektuaren antolaketa modua heredatzen du.</span><span class="sxs-lookup"><span data-stu-id="9b916-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
