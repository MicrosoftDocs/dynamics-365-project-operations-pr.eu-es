---
title: Antolaketa moduak
description: Gai honek antolaketa moduei buruzko informazioa ematen du.
author: ruhercul
ms.date: 05/28/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 508ff1df8f7e31066712fab6f8871dfdb107a43b
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116692"
---
# <a name="scheduling-modes"></a><span data-ttu-id="a9e3c-103">Antolaketa moduak</span><span class="sxs-lookup"><span data-stu-id="a9e3c-103">Scheduling modes</span></span>

<span data-ttu-id="a9e3c-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="a9e3c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="a9e3c-105">Dynamics 365 Project Operations gaitasuna ematen die erakundeei lanaren banakako egituraren zereginetan aldagai gakoen aldaketak nola kudeatzen dituzten definitzeko.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="a9e3c-106">Erakundearen behar espezifikoetan oinarrituta, proiektuen arduradunek planifikazio moduan aldaketak egin ditzakete proiektu bat sortzen denean.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="a9e3c-107">Project Operations-en hiru programazio modu daude eskuragarri:</span><span class="sxs-lookup"><span data-stu-id="a9e3c-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="a9e3c-108">Iraupen finkoa (modu lehenetsia da)</span><span class="sxs-lookup"><span data-stu-id="a9e3c-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="a9e3c-109">Ahalegin finkoa (*Lana*)</span><span class="sxs-lookup"><span data-stu-id="a9e3c-109">Fixed effort (*Work*)</span></span>
  - <span data-ttu-id="a9e3c-110">Unitate finkoak</span><span class="sxs-lookup"><span data-stu-id="a9e3c-110">Fixed units</span></span>

<span data-ttu-id="a9e3c-111">Programazio modu zehatz baten definizioak eragindako balioak honako formula honen bidez zehazten dira:</span><span class="sxs-lookup"><span data-stu-id="a9e3c-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="a9e3c-112">Esfortzua = Iraupena x Unitateak</span><span class="sxs-lookup"><span data-stu-id="a9e3c-112">Effort  = Duration x Units</span></span>

<span data-ttu-id="a9e3c-113">Proiektu baten antolaketa modua definitzen duzunean, balio horietako bat ezartzen ari zara, gero aldatu ezin direnak.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="a9e3c-114">Balio hori konstante gisa mantentzeak lehentasuna ematen dio balio horri, eta horrek sistemari beste bi balioak aldatzen direnean ez aldatzeko jakinarazten dio.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="a9e3c-115">Ondorengo taulan modu zehatz bat hautatzearen eraginari buruzko informazioa ematen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="a9e3c-116">**Zereginean**</span><span class="sxs-lookup"><span data-stu-id="a9e3c-116">**In this task**</span></span>             | <span data-ttu-id="a9e3c-117">**Unitateak berrikusten badituzu**</span><span class="sxs-lookup"><span data-stu-id="a9e3c-117">**If you revise units**</span></span>   | <span data-ttu-id="a9e3c-118">**Iraupena berrikusten baduzu**</span><span class="sxs-lookup"><span data-stu-id="a9e3c-118">**If you revise duration**</span></span> | <span data-ttu-id="a9e3c-119">**Esfortzua berrikusten baduzu**</span><span class="sxs-lookup"><span data-stu-id="a9e3c-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="a9e3c-120">Unitate-zeregin finkoak</span><span class="sxs-lookup"><span data-stu-id="a9e3c-120">Fixed units task</span></span>     | <span data-ttu-id="a9e3c-121">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-121">Duration is recalculated.</span></span> | <span data-ttu-id="a9e3c-122">Ahalegina berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-122">Effort is recalculated.</span></span>    | <span data-ttu-id="a9e3c-123">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="a9e3c-124">Ahalegin finkoaren zeregina</span><span class="sxs-lookup"><span data-stu-id="a9e3c-124">Fixed effort task</span></span>    | <span data-ttu-id="a9e3c-125">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-125">Duration is recalculated.</span></span> | <span data-ttu-id="a9e3c-126">Unitateak berriro kalkulatzen dira.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-126">Units are recalculated.</span></span>    | <span data-ttu-id="a9e3c-127">Iraupena berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="a9e3c-128">Iraupen finkoko zeregina</span><span class="sxs-lookup"><span data-stu-id="a9e3c-128">Fixed duration task</span></span>  | <span data-ttu-id="a9e3c-129">Ahalegina berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-129">Effort is recalculated.</span></span>   | <span data-ttu-id="a9e3c-130">Ahalegina berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-130">Effort is recalculated.</span></span>    | <span data-ttu-id="a9e3c-131">Unitateak berriro kalkulatzen dira.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-131">Units are recalculated.</span></span>   |

<span data-ttu-id="a9e3c-132">Modu jakin baten inplikazioei buruzko informazio gehiago lortzeko, ikusi [Aldatu zeregin mota programazio zehatzagoa lortzeko](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="a9e3c-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="a9e3c-133">Gaian, terminoa **Lana** ordez erabiltzen da **Esfortzua**.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="a9e3c-134">Aldatu erakundearen programazio modua</span><span class="sxs-lookup"><span data-stu-id="a9e3c-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="a9e3c-135">Osatu urrats hauek erakunde baten antolaketa modua definitzeko.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="a9e3c-136">Joan **Ezarpenak**\> **Orokorra** \> **Parametroak** aukerara, eta hautatu proiektuaren parametroa.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="a9e3c-137">**Proiektuaren parametroak** orrialdean, hautatu antolaketarako antolaketa modu lehenetsia eta, ondoren, proiektuaren kudeatzaileak proiektu berria sortzerakoan ezarpena gainidazteko duen gaitasuna definitu.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="a9e3c-138">Aldatu proiektu baten antolaketa moduaren ezarpena</span><span class="sxs-lookup"><span data-stu-id="a9e3c-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="a9e3c-139">Erakunde batek proiektuaren kudeatzaileari antolaketa modu lehenetsia gainbideratzen uzten badio, proiektuaren kudeatzaileak proiektu hori sortzen duenean aldaketa hori egin dezake.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="a9e3c-140">Hala ere, proiektua gorde eta gero, ezin da planifikazio modua aldatu.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="a9e3c-141">Kopiatutako proiektuak</span><span class="sxs-lookup"><span data-stu-id="a9e3c-141">Copied projects</span></span>

<span data-ttu-id="a9e3c-142">Kopiatu proiektuaren ekintza egiten denean proiektu bat sortzen denez, Proiektu kudeatzaileak ezin du planifikazio modua ezarri.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="a9e3c-143">Helmugako proiektuak beti antolaketa mailan definitutako modua lehenetsiko du.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="a9e3c-144">Kopiatutako zereginak</span><span class="sxs-lookup"><span data-stu-id="a9e3c-144">Copied tasks</span></span>

<span data-ttu-id="a9e3c-145">Zeregin bat proiektu batetik bestera kopiatzen denean, zereginak helmugako proiektuaren antolaketa modua heredatzen du.</span><span class="sxs-lookup"><span data-stu-id="a9e3c-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
