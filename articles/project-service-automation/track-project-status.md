---
title: Jarraitu proiektu-egoerari
description: Nola jarraitu proiektu-egoerari Project Service-n
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 7610aecb-318c-422b-b626-9106b0736b5f
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: e4d53b6235c3b941bce525dca09ee3d647c3d242
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748936"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="4c44a-103">Jarraitu proiektu-egoerari (Project Service)</span><span class="sxs-lookup"><span data-stu-id="4c44a-103">Track a project’s status (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="4c44a-104">Erabili [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] bezeroaren proiektuaren progresioari jarraipena egiteko.</span><span class="sxs-lookup"><span data-stu-id="4c44a-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="4c44a-105">Konpromiso-progresio gisa, proiektu-faseak eguneratzen dira, konpromisoaren fasea islatzeko:</span><span class="sxs-lookup"><span data-stu-id="4c44a-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="4c44a-106">**Berria**</span><span class="sxs-lookup"><span data-stu-id="4c44a-106">**New**</span></span>    | <span data-ttu-id="4c44a-107">Proiektua sortzen duzunean, fasea **Berria** gisa ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="4c44a-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="4c44a-108">Proiektua txantiloi batetik sortu baduzu, proiektuaren fasean antolaketa, estimazioak eta taldea datuak izan ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="4c44a-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="4c44a-109">Bestela, proiektuaren ingerada izango da eta eskuz sartu beharko dituzu gainerako osagai guztiak.</span><span class="sxs-lookup"><span data-stu-id="4c44a-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="4c44a-110">**Eskaintza**</span><span class="sxs-lookup"><span data-stu-id="4c44a-110">**Quote**</span></span>   |      <span data-ttu-id="4c44a-111">Erlazionatu eskaintza proiektua edo eskaintza bateko sortu proiektua fasea gisa ezarrita badago, **Eskaintza**, eta, estimatutako hasiera eta amaiera-datak ere eguneratzen dira.</span><span class="sxs-lookup"><span data-stu-id="4c44a-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="4c44a-112">Eskaintzaren xehetasunak bistaratu proiektuan eskaintza fase dagoenean, **Salmentak** atalean fitxan, **Proiektua** orria.</span><span class="sxs-lookup"><span data-stu-id="4c44a-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="4c44a-113">**Plana**</span><span class="sxs-lookup"><span data-stu-id="4c44a-113">**Plan**</span></span>   |                                     <span data-ttu-id="4c44a-114">Proiektua fasea eguneratzen denean proiektua bat batekin erlazionatutako eskaintza irabazi eta konpromiso, bilakatzen da kontratua fasera duzunean, **Antolatu**.</span><span class="sxs-lookup"><span data-stu-id="4c44a-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="4c44a-115">Kontratu-xehetasunak **Salmentak**fitxan agertzen da, **Proiektua** orrian.</span><span class="sxs-lookup"><span data-stu-id="4c44a-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="4c44a-116">**Osatuta**</span><span class="sxs-lookup"><span data-stu-id="4c44a-116">**Complete**</span></span> |                    <span data-ttu-id="4c44a-117">Proiektuaren lana osatutakoan, fasea **Osatuta** gisa ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="4c44a-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="4c44a-118">Proiektua fasea osatzeko egoeran daudenean, lana % 100 osatu da baina zain ordua edo expense sarrerak erregistratzen dira ireki sinkronizatzen proiektuan understood da hori.</span><span class="sxs-lookup"><span data-stu-id="4c44a-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="4c44a-119">**Itxi**</span><span class="sxs-lookup"><span data-stu-id="4c44a-119">**Close**</span></span>   |           <span data-ttu-id="4c44a-120">Transakzio guztiak proiektuan erregistratu ostean eta beste ezer erregistratzea espero ez duzunean, eskuz alda dezakezu fasea **Itxi** egoerara.</span><span class="sxs-lookup"><span data-stu-id="4c44a-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="4c44a-121">Proiektuan **Itxi** gisa dagoenean, ezin duzu transakzio gehiago gehitu proiektuan eta proiektua irakurtzeko soilik izango da.</span><span class="sxs-lookup"><span data-stu-id="4c44a-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="4c44a-122">Proiektu-egoerari jarraitzeko</span><span class="sxs-lookup"><span data-stu-id="4c44a-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="4c44a-123">Joan **Project Service > Proiektuak**.</span><span class="sxs-lookup"><span data-stu-id="4c44a-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="4c44a-124">Sakatu landu nahi duzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="4c44a-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="4c44a-125">Pantailaren goialdean dagoen barran, hautatu proiektuaren izenaren alboan dagoen beherako gezia eta sakatu **Proiektuaren jarraipena**.</span><span class="sxs-lookup"><span data-stu-id="4c44a-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="4c44a-126">Hautatu **Ahaleginen jarraipena** edo **Kostuen jarraipena** zeregin-zerrendaren goiko goitibeherako zerrendan.</span><span class="sxs-lookup"><span data-stu-id="4c44a-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="4c44a-127">Egin klik bikoitza editatu nahi duzun edozein zereginetan.</span><span class="sxs-lookup"><span data-stu-id="4c44a-127">Double-click any task to edit it.</span></span> <span data-ttu-id="4c44a-128">Gainera, Gantt diagramako barrak mugitu edo tamainaz alda ditzakezu, zereginaren ordua eta progresioa aldatzeko.</span><span class="sxs-lookup"><span data-stu-id="4c44a-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="4c44a-129">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="4c44a-129">See Also</span></span>  
 [<span data-ttu-id="4c44a-130">Proiektu-kudeatzailearen gida</span><span class="sxs-lookup"><span data-stu-id="4c44a-130">Project Manager Guide</span></span>](../project-service/project-manager-guide.md)
