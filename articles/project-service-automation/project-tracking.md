---
title: Proiektuen garapena eta kostuen kontsumoa
description: Gai honek proiektuaren garapenaren eta kostuen kontsumoaren jarraipena egiteari buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748923"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="69325-103">Proiektuen garapena eta kostuen kontsumoa</span><span class="sxs-lookup"><span data-stu-id="69325-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="69325-104">Antolaketa eta garapena jarraitzeko beharra aldatu egiten da industriaren arabera.</span><span class="sxs-lookup"><span data-stu-id="69325-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="69325-105">Zenbait industriak jarraipen zehatza egiten du; beste batzuek, aldiz, jarraipen orokorragoa egiten dute.</span><span class="sxs-lookup"><span data-stu-id="69325-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="69325-106">Gai honek erakundearen eskakizunak betetzeko nola antolatu behar den erakusten du.</span><span class="sxs-lookup"><span data-stu-id="69325-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="69325-107">Ahaleginen segimenduaren ikuspegia</span><span class="sxs-lookup"><span data-stu-id="69325-107">Effort tracking view</span></span>

<span data-ttu-id="69325-108">**Ahaleginen jarraipena** ikuspegiak antolaketako zereginen garapenaren jarraipena egiten du.</span><span class="sxs-lookup"><span data-stu-id="69325-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="69325-109">Zeregin batean egin diren uneko ahalegin orduak eta zereginerako aurreikusitako esfortzu orduak konparatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="69325-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="69325-110">PSA-k honako formula hauek erabiltzen ditu jarraipen-neurriak kalkulatzeko:</span><span class="sxs-lookup"><span data-stu-id="69325-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="69325-111">Garapenaren ehunekoa = Orain arte egindako egiazko ahalegina ÷ Zereginerako aurreikusitako ahalegina</span><span class="sxs-lookup"><span data-stu-id="69325-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="69325-112">Burutzeko estimazioa (ETC) = Aurreikusitako ahalegina - Orain arte egindako ahalegina</span><span class="sxs-lookup"><span data-stu-id="69325-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="69325-113">Burutzean egindako estimazioa (EAC) = Geratzen den ahalegina + Orain arte egindako ahalegina</span><span class="sxs-lookup"><span data-stu-id="69325-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="69325-114">Proiektatutako ahaleginaren bariantza = Aurreikusitako ahalegina - EAC</span><span class="sxs-lookup"><span data-stu-id="69325-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="69325-115">PSA-k zereginen bariantzaren bistaratzea erakusten du.</span><span class="sxs-lookup"><span data-stu-id="69325-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="69325-116">EAC aurreikusitako ahalegina baino handiagoa bada, zereginak hasieran aurreikusitakoa baino denbora gehiago beharko duela aurreikusten da.</span><span class="sxs-lookup"><span data-stu-id="69325-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="69325-117">Hori dela eta, atzeratuta dago.</span><span class="sxs-lookup"><span data-stu-id="69325-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="69325-118">EAC aurreikusitako ahalegina baino txikiagoa bada, zereginak hasieran aurreikusitakoa baino denbora gutxiago beharko duela aurreikusten da.</span><span class="sxs-lookup"><span data-stu-id="69325-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="69325-119">Hori dela eta, aurreratuta dago.</span><span class="sxs-lookup"><span data-stu-id="69325-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="69325-120">Berriro proiektatzeko ahalegina</span><span class="sxs-lookup"><span data-stu-id="69325-120">Re-projecting effort</span></span>

<span data-ttu-id="69325-121">Ohikoa da proiektu-kudeatzaile batek zereginen jatorrizko kalkuluak berrikustea.</span><span class="sxs-lookup"><span data-stu-id="69325-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="69325-122">Proiektuaren birproiekzioak proiektu-kudeatzaileak proiektuaren egungo egoera ikusita duen kalkuluen pertzepzioa da.</span><span class="sxs-lookup"><span data-stu-id="69325-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="69325-123">Hala ere, ez dugu gomendatzen proiektu-kudeatzaileak oinarrizko zenbakiak aldatzea, proiektuaren oinarria baita proiektuaren antolaketaren eta kostuen ezarritako benetako jatorria eta proiektuko interes-talde guztiek onartu dute hori.</span><span class="sxs-lookup"><span data-stu-id="69325-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="69325-124">Proiektu-kudeatzaileak bi modutara birproiektatu ditzake zereginetako ahaleginak:</span><span class="sxs-lookup"><span data-stu-id="69325-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="69325-125">Gainidatzi ETC lehenetsia zereginen benetako ahaleginaren beste kalkulu batekin.</span><span class="sxs-lookup"><span data-stu-id="69325-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="69325-126">Gainidatzi garapenaren ehuneko lehenetsia zereginen benetako garapenaren beste kalkulu batekin.</span><span class="sxs-lookup"><span data-stu-id="69325-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="69325-127">Planteamendu horietako bakoitzak zereginaren ETC, EAC eta garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du.</span><span class="sxs-lookup"><span data-stu-id="69325-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="69325-128">Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa ere berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.</span><span class="sxs-lookup"><span data-stu-id="69325-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="69325-129">Laburpen-zereginetan ahalegina berriro proiektatzea</span><span class="sxs-lookup"><span data-stu-id="69325-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="69325-130">Laburpen-zereginetan edo edukitzaile-zereginetan ahalegina berriro proiektatu daiteke.</span><span class="sxs-lookup"><span data-stu-id="69325-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="69325-131">Erabiltzaileak laburpen-zereginetan gelditzen den ahalegina edo garapenaren ehunekoa erabiliz birproiektatzen duen kontuan izan gabe, honako kalkulu multzoa hasten da:</span><span class="sxs-lookup"><span data-stu-id="69325-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="69325-132">Zeregineko EAC, ETC eta garapenaren ehunekoa kalkulatzen dira.</span><span class="sxs-lookup"><span data-stu-id="69325-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="69325-133">EAC berria bigarren mailako zereginetan banatzen da jatorrizko zereginean zegoen EAC proportzio berean.</span><span class="sxs-lookup"><span data-stu-id="69325-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="69325-134">Hosto-nodoen zereginetara jaitsitako zeregin indibidualetako EAC berria kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="69325-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="69325-135">Berriro kalkulatzen dira hosto-nodoetan kaltetutako bigarren mailako zereginen ETC balioa eta garapenaren portzentajea EAC balioaren arabera.</span><span class="sxs-lookup"><span data-stu-id="69325-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="69325-136">Horrek zereginaren ahaleginaren bariantzarako beste proiekzio bat sortzen du.</span><span class="sxs-lookup"><span data-stu-id="69325-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="69325-137">Erro-nodora bideratutako laburpen-zereginen EAC-ak berriro kalkulatzen dira.</span><span class="sxs-lookup"><span data-stu-id="69325-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="69325-138">Kostuen jarraipenaren ikuspegia</span><span class="sxs-lookup"><span data-stu-id="69325-138">Cost tracking view</span></span> 

<span data-ttu-id="69325-139">**Kostuen jarraipena** ikuspegiak zeregin batean gastatu diren kostu errealak zeregin batean aurreikusitako kostuekin alderatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="69325-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="69325-140">Ikuspegi honek lan-kostuak bakarrik erakusten ditu eta ez ditu gastuen kalkuluko gastuak barne hartzen.</span><span class="sxs-lookup"><span data-stu-id="69325-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="69325-141">PSA-k honako formula hauek erabiltzen ditu jarraipen-neurriak kalkulatzeko:</span><span class="sxs-lookup"><span data-stu-id="69325-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="69325-142">Kontsumitutako kostuaren ehunekoa = Orain arte gastatutako kostua ÷ Zereginerako aurreikusitako kostua</span><span class="sxs-lookup"><span data-stu-id="69325-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="69325-143">Burutzeko kostua (CTC) = Aurreikusitako kostua - Orain arte egindako kostua</span><span class="sxs-lookup"><span data-stu-id="69325-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="69325-144">EAC = CTC + Orain arte gastatutako benetako kostua</span><span class="sxs-lookup"><span data-stu-id="69325-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="69325-145">Proiektatutako kostuaren bariantza = Aurreikusitako kostua - EAC</span><span class="sxs-lookup"><span data-stu-id="69325-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="69325-146">Kostuaren bariantzaren proiekzioa erakusten da zereginean.</span><span class="sxs-lookup"><span data-stu-id="69325-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="69325-147">EAC aurreikusitako kostua baino handiagoa bada, zereginak hasieran aurreikusitakoa baino kostu handiagoa beharko duela aurreikusten da.</span><span class="sxs-lookup"><span data-stu-id="69325-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="69325-148">Beraz, aurrekontu gainditzeko joera erakusten du.</span><span class="sxs-lookup"><span data-stu-id="69325-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="69325-149">EAC aurreikusitako kostua baino txikiagoa bada, zereginak hasieran aurreikusitakoa baino kostu txikiagoa beharko duela aurreikusten da.</span><span class="sxs-lookup"><span data-stu-id="69325-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="69325-150">Beraz, aurrekontuaren azpitik gelditzeko joera erakusten du.</span><span class="sxs-lookup"><span data-stu-id="69325-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="69325-151">Proiektu-kudeatzaileak egindako kostuaren birproiekzioa</span><span class="sxs-lookup"><span data-stu-id="69325-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="69325-152">Esfortzua berriro proiektatzen denean, CTC, EAC, kontsumitutako kostuaren ehunekoa eta proiektatutako kostuen bariantza berriro kalkulatuko dira **Kostuen jarraipena** ikuspegian.</span><span class="sxs-lookup"><span data-stu-id="69325-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="69325-153">Proiektuaren egoeraren laburpena</span><span class="sxs-lookup"><span data-stu-id="69325-153">Project status summary</span></span>

<span data-ttu-id="69325-154">**Ahaleginen jarraipena** eta **Kostuen jarraipena** ikuspegietako datuen jarraipenak proiektuaren erro-nodoaren, laburpen-zereginaren eta hosto-nodoaren zereginen mailan egondako garapena eta kostuen kontsumoa erakusten dute.</span><span class="sxs-lookup"><span data-stu-id="69325-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="69325-155">**Egoera** atalak, **Proiektuaren entitatea** orrialdeakoak, proiektu-mailaren egoeraren laburpena erakusten du.</span><span class="sxs-lookup"><span data-stu-id="69325-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="69325-156">Egoeraren laburpen-eremuak</span><span class="sxs-lookup"><span data-stu-id="69325-156">Status summary fields</span></span>

<span data-ttu-id="69325-157">**Proiektuaren egoera orokorra** eremua editagarria den eremua da, eta proiektuaren egoera orokorra erakusten du.</span><span class="sxs-lookup"><span data-stu-id="69325-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="69325-158">Kolore bidezko kodeketa erabiltzen du, hala nola berdea, horia eta gorria, arriskua handitzen dela adierazteko.</span><span class="sxs-lookup"><span data-stu-id="69325-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="69325-159">**Oharrak** eremuak proiektu-kudeatzaileari egoerari buruzko iruzkin zehatzak sartzen uzten dio.</span><span class="sxs-lookup"><span data-stu-id="69325-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="69325-160">**Egoera eguneratu da** eremua ez da editagarria eta balioa egoera azkenekoz noiz eguneratu zen adierazten duen denbora-zigilua da.</span><span class="sxs-lookup"><span data-stu-id="69325-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="69325-161">**Antolaketaren errendimendua** eta **Kostuen errendimendua** eremuak jarraipen-datatik ezartzen dira.</span><span class="sxs-lookup"><span data-stu-id="69325-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="69325-162">Erro-nodoaren antolaketa eta kostuaren bariantza positiboak direnean **Ahaleginaren jarraipena** ikuspegian, eremu horiek **Aurreratua** gisa ezar ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="69325-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="69325-163">Erro-nukleoaren antolaketa eta kostuaren bariantza negatiboak direnean, **Atzeratuta** gisa ezar ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="69325-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
