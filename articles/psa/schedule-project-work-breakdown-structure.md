---
title: Antolaketa proiektua atazen xehapenaren egiturarekin
description: Nola antolatu proiektua zereginen xehetasunen egiturarekin Project Service-n
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a00e39f78890426721a49cd569ba8ce4accb30a9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282678"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="7cd9f-103">Antolaketa proiektua zereginen xehetasunen egiturarekin (Project Service)</span><span class="sxs-lookup"><span data-stu-id="7cd9f-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="7cd9f-104">Proiektu-antolaketak zein lan egin behar den komunikatzen du, zein baliabidek gauzatuko duen lana eta zein denbora-tartetan egingo den lana.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="7cd9f-105">Proiektu-antolaketak proiektua garaiz entregatzearekin lotutako lan guztia islatzen du.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="7cd9f-106">Proiektuaren hasierako faseko lehen urratsetako bat proiektuaren antolaketa izatea da.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="7cd9f-107">Proiektu-antolaketa zehazteko, atazen xehapenaren egitura sortu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="7cd9f-108">Sortu proiektu-egitura atazen xehapenaren egiturarekin, eta honetan lagunduko dizu:</span><span class="sxs-lookup"><span data-stu-id="7cd9f-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="7cd9f-109">Lana zeregin kudeagarritan zatitzen</span><span class="sxs-lookup"><span data-stu-id="7cd9f-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="7cd9f-110">Zeregina osatzeko beharrezko denbora kalkulatzen</span><span class="sxs-lookup"><span data-stu-id="7cd9f-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="7cd9f-111">Mendeko zereginak eta zereginen iraupena ezartzen</span><span class="sxs-lookup"><span data-stu-id="7cd9f-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="7cd9f-112">Zeregin bakoitza gauzatzeko beharrezko funtzioak zehazten</span><span class="sxs-lookup"><span data-stu-id="7cd9f-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="7cd9f-113">Atazen xehapenaren egiturako proiektu-antolaketak itxura ezaguna du, Gantt taula interaktibo batekin lagunduta.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="7cd9f-114">Sortu proiektuaren atazen xehapenaren egitura</span><span class="sxs-lookup"><span data-stu-id="7cd9f-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="7cd9f-115">Sortu proiektuan zereginen sekuentzia adierazten duen atazen xehapenaren egitura.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="7cd9f-116">Atazen xehapenaren egiturak zereginak, zeregin bakoitzerako eskakizunak eta irabaziei eta kostuei buruzko informazioa ditu.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="7cd9f-117">Atazen xehapenaren egituran gehi ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="7cd9f-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="7cd9f-118">Hierarkiako zereginen sekuentzia</span><span class="sxs-lookup"><span data-stu-id="7cd9f-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="7cd9f-119">Zeregina hasi ahal izateko, egin behar diren beste zeregin batzuk, baldin badaude</span><span class="sxs-lookup"><span data-stu-id="7cd9f-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="7cd9f-120">Hasiera-data, amaiera-data eta zereginaren iraupena</span><span class="sxs-lookup"><span data-stu-id="7cd9f-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="7cd9f-121">Zeregina egiteko behar den ordu kopurua</span><span class="sxs-lookup"><span data-stu-id="7cd9f-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="7cd9f-122">Langileek behar dituzten trebakuntzak eta heziketa</span><span class="sxs-lookup"><span data-stu-id="7cd9f-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="7cd9f-123">Zereginera esleitutako langileak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="7cd9f-124">Gutxi gorabeherako diru-sarrerak eta kostuak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="7cd9f-125">Zeregin motak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-125">Task types</span></span>  
<span data-ttu-id="7cd9f-126">Zeregin mota hauek erabiliko dituzu atazen xehapenaren egitura sortzean:</span><span class="sxs-lookup"><span data-stu-id="7cd9f-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="7cd9f-127">**Proiektuaren erroko nodoa**</span><span class="sxs-lookup"><span data-stu-id="7cd9f-127">**Project root node**</span></span> | <span data-ttu-id="7cd9f-128">Proiektuaren goi-mailako laburpen-zeregina.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-128">The top-level summary task for the project.</span></span> <span data-ttu-id="7cd9f-129">Gainerako proiektu-zereginak bere barnean sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-129">All other project tasks are created under it.</span></span> <span data-ttu-id="7cd9f-130">Erroko zereginaren izena proiektuaren izena da.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-130">The name of the root task is the project name.</span></span> <span data-ttu-id="7cd9f-131">Erroko nodoaren ahalegina, datak eta iraupena bere azpiko hierarkiako balioetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="7cd9f-132">Ezin duzu erroko nodoaren propietaterik editatu edo erroko nodoa ezabatu.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="7cd9f-133">**Laburpena edo edukiontzi-zereginak**</span><span class="sxs-lookup"><span data-stu-id="7cd9f-133">**Summary or container tasks**</span></span> | <span data-ttu-id="7cd9f-134">Zeregin-laburpena azpizereginak konbinatzeko zeregina da.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="7cd9f-135">Zeregin-laburpenak ez di lan-ahaleginik edo kosturik.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="7cd9f-136">Lan-ahalegina eta kostua azpizereginetan bateratzen dira.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="7cd9f-137">Laburpen-zereginaren izena alda dezakezu, baina ezin duzu aldatu ahalegina, datak edo iraupena, automatikoki kalkulatzen baitira.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="7cd9f-138">Laburpen-zeregin bat ezabatzen baduzu, zereginak eta azpizeregin guztiak ezabatuko dituzu.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="7cd9f-139">**Hosto-nodoaren zereginak**</span><span class="sxs-lookup"><span data-stu-id="7cd9f-139">**Leaf node tasks**</span></span> | <span data-ttu-id="7cd9f-140">Hosto-nodoaren zereginak proiektuaren lan xehatuena adierazten du.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="7cd9f-141">Estimatutako ahalegina, antolatutako baliabide kopurua, antolatutako hasiera- eta amaiera-datak eta iraupena ditu.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="7cd9f-142">Zeregin-hierarkia</span><span class="sxs-lookup"><span data-stu-id="7cd9f-142">Task hierarchy</span></span>  
 <span data-ttu-id="7cd9f-143">Aukera hauek dituzu zeregin-hierarkia sortzeko:</span><span class="sxs-lookup"><span data-stu-id="7cd9f-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="7cd9f-144">**Gehitu zeregina**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-144">**Add task**.</span></span>   <span data-ttu-id="7cd9f-145">Zeregin bat gehi dezakezu zeregin-hierarkian aukeratu duzun posizioan.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="7cd9f-146">Ez baduzu posiziorik hautatzen, zeregin berria amaieran agertuko da.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="7cd9f-147">**Jarri koska zereginari**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-147">**Indent task**.</span></span>   <span data-ttu-id="7cd9f-148">Jarri koska zeregin bati, zereginaren bigarren mailako bat sortzeko bere gainean.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="7cd9f-149">**Kendu koska zereginari**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-149">**Outdent task**.</span></span>   <span data-ttu-id="7cd9f-150">Kendu koska zereginari zeregin nagusiaren azpizeregina izateari utz diezaion.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="7cd9f-151">**Eraman gora eta behera**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-151">**Move up and Move down**.</span></span>   <span data-ttu-id="7cd9f-152">Eraman zereginak gora eta behera zeregin nagusiaren hierarkian.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="7cd9f-153">Zereginak gora edo behera eramateak ez du eragiten ahaleginean, kostuan, datetan edo iraupenean.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="7cd9f-154">Zeregin-atributuak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-154">Task attributes</span></span>  
 <span data-ttu-id="7cd9f-155">Zeregin-izenak egin beha den lana deskribatzen du.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="7cd9f-156">Erabili hainbat zeregin-atributu antolaketa azaltzeko eta zereginaren eskakizunak gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="7cd9f-157">Antolaketa-atributuak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-157">Schedule attributes</span></span>

 - <span data-ttu-id="7cd9f-158">Esleitu balioak **Ahalegin-orduak**, **Baliabide kopurua**, **Hasiera-data**, **Amaiera-data** eta **Iraupena** aukerei, zereginaren antolaketa zehazteko.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-158">Assign values to **Effort hours**, **Number of resources**, **Start date**, **End date**, and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="7cd9f-159">**Ahalegina** zeregina egiteko behar den orduen estimazioa da.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="7cd9f-160">**Baliabide kopurua** ahalik eta antolaketa onena lortzen laguntzeko proiektu-kudeatzaileak jartzen duen estimazioa da.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="7cd9f-161">**Iraupena** (egunetan), zeregina egiteko behar diren egun kopurua adierazten du.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="7cd9f-162">Betetze-atributuak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-162">Staffing attributes</span></span>

 - <span data-ttu-id="7cd9f-163">**Funtzioa**, **Baliabideen antolakuntza-unitatea**, **Baliabide kopurua** eta **Baliabideak** aukerek zereginaren betetze-eskakizunak deskribatzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-163">**Role**, **Resource organizational unit**, **Number of resources**, and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="7cd9f-164">**Funtzioa**, zeregina egiteko behar den baliabide mota azaltzen du.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="7cd9f-165">**Baliabideen antolakuntza-unitatea** aukerak zeregina egiteko baliabideak hartu behar diren erakunde-unitatea adierazten du; zereginaren kostuari eta salmentei ere eragiten die, baliabidearen unitatearen salmenta-prezioa zehaztean kontatzen baita.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="7cd9f-166">**Baliabideak** baliabide orokorra adierazten du edo bat izendatzen du aurkitzen duenean.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="7cd9f-167">Zeregin-mendekotasunak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-167">Task dependencies</span></span>  
 <span data-ttu-id="7cd9f-168">Aurrekoen harremanak sor ditzakezu atazen xehapenaren egiturako zeregin baten edo gehiagoren artean.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="7cd9f-169">Zereginen aurrekari-eremuan balio bat edo gehiago ezar ditzakezu mendeko izango zaren zereginak adierazteko.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="7cd9f-170">Aurreko balio bat esleitzen duzunean, zeregina hasteko aurreko zeregin guztiak osatu direnean abiaraziko dira.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="7cd9f-171">Zereginean mendekotasun hori ezarrita, zereginaren planeatutako hasiera-data berriro kalkulatuko da aurreko zereginen azken amaiera gisa.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="7cd9f-172">Antolaketako aurrekoekin lotutako inpaktu guztiak ez daude zeregin bidez mugatuta.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="7cd9f-173">Zeregin modua</span><span class="sxs-lookup"><span data-stu-id="7cd9f-173">Task mode</span></span>  
 <span data-ttu-id="7cd9f-174">Zeregin modua antolaketako hosto-nodoaren zereginak zehazten dituen faktore garrantzitsuetako bat da.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="7cd9f-175">Zeregin bakoitzak bi zeregin modu ditu: automatikoki antolatzeko modua eta eskuz antolatzeko modua.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="7cd9f-176">**Antolaketa automatikoa**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-176">**Auto scheduling**.</span></span>   <span data-ttu-id="7cd9f-177">Automatikoki antolatzea Zeregin modua Automatikoki antolatuta gisa ezartzen duzunean, zeregina antolatzeko motorrak antolaketa-arauak erabiltzen ditu zeregin-atributu hauetan, zereginaren antolaketa zehazteko:</span><span class="sxs-lookup"><span data-stu-id="7cd9f-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="7cd9f-178">Aurrekoak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="7cd9f-179">Ahalegina</span><span class="sxs-lookup"><span data-stu-id="7cd9f-179">Effort</span></span>  
  
    -   <span data-ttu-id="7cd9f-180">Baliabide kopurua</span><span class="sxs-lookup"><span data-stu-id="7cd9f-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="7cd9f-181">Hasiera- eta amaiera-datak</span><span class="sxs-lookup"><span data-stu-id="7cd9f-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="7cd9f-182">**Nire antolaketa-arauak**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-182">**Scheduling rules**.</span></span>   <span data-ttu-id="7cd9f-183">Arauen antolaketa Hosto-nodoaren hasiera-data, aurrekaririk ez duten lehenetsiak proiektuaren antolatzeko hasiera-data.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="7cd9f-184">Hosto-nodoaren zereginaren iraupena hasiera- eta amaiera-datuen arteko lan-egun kopuru gisa kalkulatzen da beti.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="7cd9f-185">Zeregina automatikoki antolatzen denean, antolaketa-motorrak arau hauei jarraitzen die:</span><span class="sxs-lookup"><span data-stu-id="7cd9f-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="7cd9f-186">Zereginen hasiera- eta amaiera-datek lanegunak izan behar dute, proiektuaren antolaketa-egutegiaren arabera</span><span class="sxs-lookup"><span data-stu-id="7cd9f-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="7cd9f-187">Bere aurrekarien azken amaiera-dataren aurrekariak dituzten zereginen hasiera-data</span><span class="sxs-lookup"><span data-stu-id="7cd9f-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="7cd9f-188">Ahalegina = pertsona kopurua \* Iraupena \* orduak proiektu-egutegiaren lanegun estandarrean</span><span class="sxs-lookup"><span data-stu-id="7cd9f-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="7cd9f-189">**Eskuzko antolaketa**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-189">**Manual scheduling**.</span></span>   <span data-ttu-id="7cd9f-190">Zenbait kasutan, baliteke arau horiek desbideratu behar izatea.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="7cd9f-191">Kasu horietan, eskuz antolatzeko zereginen zeregin modua ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="7cd9f-192">Beste antolaketa-atributu batzuek balioak kalkulatzea eragozten dio antolaketa-motorrari.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="7cd9f-193">Zereginetan aurrekariak ezartzeak mendeko zereginen hasiera-datari eragiten die.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="7cd9f-194">Sortu atazen xehapenaren egitura</span><span class="sxs-lookup"><span data-stu-id="7cd9f-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="7cd9f-195">Joan **Project Service > Proiektuak**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="7cd9f-196">Sakatu landu nahi duzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="7cd9f-197">Pantailaren goialdean dagoen barran, hautatu proiektuaren izenaren alboan dagoen beherako gezia eta sakatu Atazen xehapenaren egitura.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="7cd9f-198">Zeregina gehitzeko, sakatu **Gehitu zeregina**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="7cd9f-199">Bete zereginaren eremuak eta, ondoren, klikatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="7cd9f-200">Jarraitu zereginak gehitzen, atazen xehapenaren egitura bete arte.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="7cd9f-201">Atazen xehapenaren egitura sortzen ari zaren bitartean, zera egin dezakezu zereginak antolatzeko:</span><span class="sxs-lookup"><span data-stu-id="7cd9f-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="7cd9f-202">Hautatu zeregin bat eta sakatu **Ezarri koska** beste zeregin baten mende jartzeko edo sakatu Kendu koska mailaz igotzeko.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="7cd9f-203">Hautatu zeregina eta sakatu **Eraman gora** edo **Eraman behera** zerrendan gora edo behera eramateko.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="7cd9f-204">Sakatu **Ezkutatu Gantt** Gantt diagrama ezkutatzeko eta sakatu **Erakutsi Gantt** berriro bistaratzeko.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="7cd9f-205">Hautatu beste denbora-tarte bat Gantt diagraman, **Ordu-eskala** aukeran.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="7cd9f-206">Atazen xehapenaren egituran zehaztu dituzun funtzioak gehitzeko proiektuaren taldekideetan, sakatu **Sortu proiektu-taldea**.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="7cd9f-207">Aldaketak egiten amaitzean, sakatu **Gorde** pantailaren behe-eskuineko izkinan.</span><span class="sxs-lookup"><span data-stu-id="7cd9f-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="7cd9f-208">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="7cd9f-208">See Also</span></span>  
 [<span data-ttu-id="7cd9f-209">Proiektu-kudeatzailearen gida</span><span class="sxs-lookup"><span data-stu-id="7cd9f-209">Project manager guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]