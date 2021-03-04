---
title: Esleitu erreserbatzeko baliabide generikoak zeregin eta proiektu talde bati
description: Gai honek zereginetara eta proiektu taldeetara baliabide generikoak erreserbatzeko informazioa eskaintzen du.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: 684167f0a68872ef871fbaa06c5161e78045c9a5
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145388"
---
# <a name="assign-generic-bookable-resources-to-a-task-and-generate-resource-requirements"></a><span data-ttu-id="fa8da-103">Esleitu baliabide erreserbagarri generikoak zeregin bati eta sortu baliabide eskakizunak</span><span class="sxs-lookup"><span data-stu-id="fa8da-103">Assign generic bookable resources to a task and generate resource requirements</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="fa8da-104">Proiektuari izen edo benetako baliabideak erreserbatzeaz eta esleitzeaz gain, baliabide generikoak proiektuaren zereginei eslei diezaiezkezu.</span><span class="sxs-lookup"><span data-stu-id="fa8da-104">In addition to booking and assigning named or real resources to your project, you can assign generic resources to project tasks.</span></span> <span data-ttu-id="fa8da-105">Baliabide hauek leku-marketarako izendatutako baliabide gisa erabil daitezke, proiektuari baliabide izendatuak gehitu arte.</span><span class="sxs-lookup"><span data-stu-id="fa8da-105">These resources can serve as placeholders for named resources until you are ready to staff your project with named resources.</span></span> 

1. <span data-ttu-id="fa8da-106">Project Service Automation (PSA) atalean, ireki **Proiektua** orrialdea eta **Ordutegiak** fitxan, sartu baliabide generikoaren izenaren posizioa ordutegiko **Baliabideak** gelaxkan.</span><span class="sxs-lookup"><span data-stu-id="fa8da-106">In Project Service Automation (PSA), open the **Project** page and on the **Schedule** tab, enter the position name of the generic resource in the **Resource** cell of the schedule.</span></span> <span data-ttu-id="fa8da-107">Edo egin klik **Baliabideak** ikonoa gelaxkan, baliabide hautatzailea irekitzeko eta ondoren sortu nahi duzun baliabide generikoaren izena.</span><span class="sxs-lookup"><span data-stu-id="fa8da-107">Or, click the **Resource** icon in the cell to open the resource picker and then enter the name of the generic resource that you want to create.</span></span>

![Taldekide generiko bat sortzea eta esleitzea](media/RM-how-to-9.png)

<span data-ttu-id="fa8da-109">Honek irekiko du **Sorrera bizkorra: proiektuko taldekidea** panela.</span><span class="sxs-lookup"><span data-stu-id="fa8da-109">This will open the **Quick Create: Project Team Member** panel.</span></span> 

2. <span data-ttu-id="fa8da-110">Sartu baliabide generikoen taldeko kidearen rola eta antolaketa unitatea eta egin klik **Gorde** botoian.</span><span class="sxs-lookup"><span data-stu-id="fa8da-110">Enter the role and organization unit of the generic resource team member and then click **Save**.</span></span>

![Taldekide generikoko kideak azkar sortu](media/RM-how-to-10.png)

3. <span data-ttu-id="fa8da-112">Baliabide generikoen taldeko kide berria sortu ondoren, zereginari esleitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="fa8da-112">After you have created the new generic resource team member, it is assigned to the task.</span></span> <span data-ttu-id="fa8da-113">Baliabide generikoa zereginen egutegiko beste zeregin batzuei esleitzen jarraitu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="fa8da-113">You can continue to assign that generic resource to other tasks in the task schedule.</span></span>

![Dauden taldekide generikoak zereginetara esleitzea](media/RM-how-to-11.png)

4. <span data-ttu-id="fa8da-115">Baliabide generikoa esleitu ondoren, baliabide eskakizuna sor dezakezu eta bete baliabideen kudeatzaileari zuzenean erreserbatuz edo bidaliz.</span><span class="sxs-lookup"><span data-stu-id="fa8da-115">After you have assigned the generic resource, you can generate a resource requirement and fulfill it by directly booking or submitting a resource request to a resource manager.</span></span>

![Taldekide generikorako baldintza bat sortzea](media/RM-how-to-12.png)

<span data-ttu-id="fa8da-117">Taldekideen sarean, lehenago aipatu bezala baliabide hautatzailea erabiltzeaz gain, baliabide generikoak zuzenean gehi ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="fa8da-117">On the team member grid, in addition to being able to use the resource picker as mentioned above, you can add generic resources directly.</span></span> <span data-ttu-id="fa8da-118">Baliabideak fitxategian zehaztutako hasiera/amaiera datetan eta esleipen metodoan oinarritutako baliabide eskakizunarekin gehitzen dira **Sorrera bizkorra: proiektuko taldekidea** panelean.</span><span class="sxs-lookup"><span data-stu-id="fa8da-118">The resources are added with a resource requirement that is based on the start/end dates and allocation method specified in the **Quick Create: Project Team Member** panel.</span></span>

<span data-ttu-id="fa8da-119">Desberdintasun bat ikus dezakezu talde generikoko kidea zuzenean gehitzen baduzu eta gero zeregin gehiago esleitzen badizkiozu baliabideei generikoa estaltzeko behar izan dituzten orduak baino.</span><span class="sxs-lookup"><span data-stu-id="fa8da-119">You can see a difference if you add the generic team member directly and then assign more tasks to the generic resource than they have required hours to cover.</span></span> <span data-ttu-id="fa8da-120">Egin klik **Sortu eskakizuna** aukeran zereginen aurrean behar diren orduak orekatzeko eskakizuna birsortzeko.</span><span class="sxs-lookup"><span data-stu-id="fa8da-120">Click **Generate Requirement** to regenerate the requirement to balance the required hours against assignments.</span></span>

<span data-ttu-id="fa8da-121">Gainera, **baliabide eskakizuna** atalean ere klik egin dezakezu taldeko sarean eskakizuna irekitzeko eta trebetasunak, baliabide hobetsiak eta abar gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="fa8da-121">You can also click the **Resource requirement** link in the team grid to open the requirement and add skills, preferred resources, etc.</span></span>

![Baliabideen eskakizuna](media/RM-how-to-13.png)

