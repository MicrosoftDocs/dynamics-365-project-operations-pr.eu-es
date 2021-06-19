---
title: Jarraitu proiektu-egoerari
description: Nola jarraitu proiektu-egoerari Project Service-n
author: ruhercul
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
ms.openlocfilehash: 2385f7e52f3b5051b76daa9169f98bd73487e22d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014371"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="f0b4a-103">Jarraitu proiektu-egoerari (Project Service)</span><span class="sxs-lookup"><span data-stu-id="f0b4a-103">Track a project’s status (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="f0b4a-104">Erabili [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] bezeroaren proiektuaren progresioari jarraipena egiteko.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="f0b4a-105">Konpromiso-progresio gisa, proiektu-faseak eguneratzen dira, konpromisoaren fasea islatzeko:</span><span class="sxs-lookup"><span data-stu-id="f0b4a-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="f0b4a-106">**Berria**</span><span class="sxs-lookup"><span data-stu-id="f0b4a-106">**New**</span></span>    | <span data-ttu-id="f0b4a-107">Proiektua sortzen duzunean, fasea **Berria** gisa ezartzen da.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="f0b4a-108">Proiektua txantiloi batetik sortu baduzu, proiektuaren fasean antolaketa, estimazioak eta taldea datuak izan ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="f0b4a-109">Bestela, proiektuaren ingerada izango da eta eskuz sartu beharko dituzu gainerako osagai guztiak.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="f0b4a-110">**Eskaintza**</span><span class="sxs-lookup"><span data-stu-id="f0b4a-110">**Quote**</span></span>   |      <span data-ttu-id="f0b4a-111">Erlazionatu eskaintza proiektua edo eskaintza bateko sortu proiektua fasea gisa ezarrita badago, **Eskaintza**, eta, estimatutako hasiera eta amaiera-datak ere eguneratzen dira.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="f0b4a-112">Eskaintzaren xehetasunak bistaratu proiektuan eskaintza fase dagoenean, **Salmentak** atalean fitxan, **Proiektua** orria.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="f0b4a-113">**Plana**</span><span class="sxs-lookup"><span data-stu-id="f0b4a-113">**Plan**</span></span>   |                                     <span data-ttu-id="f0b4a-114">Proiektua fasea eguneratzen denean proiektua bat batekin erlazionatutako eskaintza irabazi eta konpromiso, bilakatzen da kontratua fasera duzunean, **Antolatu**.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="f0b4a-115">Kontratu-xehetasunak **Salmentak** fitxan agertzen da, **Proiektua** orrian.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="f0b4a-116">**Osatuta**</span><span class="sxs-lookup"><span data-stu-id="f0b4a-116">**Complete**</span></span> |                    <span data-ttu-id="f0b4a-117">Proiektuaren lana osatutakoan, fasea **Osatuta** gisa ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="f0b4a-118">Proiektua fasea osatzeko egoeran daudenean, lana % 100 osatu da baina zain ordua edo expense sarrerak erregistratzen dira ireki sinkronizatzen proiektuan understood da hori.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="f0b4a-119">**Itxi**</span><span class="sxs-lookup"><span data-stu-id="f0b4a-119">**Close**</span></span>   |           <span data-ttu-id="f0b4a-120">Transakzio guztiak proiektuan erregistratu ostean eta beste ezer erregistratzea espero ez duzunean, eskuz alda dezakezu fasea **Itxi** egoerara.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="f0b4a-121">Proiektuan **Itxi** gisa dagoenean, ezin duzu transakzio gehiago gehitu proiektuan eta proiektua irakurtzeko soilik izango da.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="f0b4a-122">Proiektu-egoerari jarraitzeko</span><span class="sxs-lookup"><span data-stu-id="f0b4a-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="f0b4a-123">Joan **Project Service > Proiektuak**.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="f0b4a-124">Sakatu landu nahi duzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="f0b4a-125">Pantailaren goialdean dagoen barran, hautatu proiektuaren izenaren alboan dagoen beherako gezia eta sakatu **Proiektuaren jarraipena**.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="f0b4a-126">Hautatu **Ahaleginen jarraipena** edo **Kostuen jarraipena** zeregin-zerrendaren goiko goitibeherako zerrendan.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="f0b4a-127">Egin klik bikoitza editatu nahi duzun edozein zereginetan.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-127">Double-click any task to edit it.</span></span> <span data-ttu-id="f0b4a-128">Gainera, Gantt diagramako barrak mugitu edo tamainaz alda ditzakezu, zereginaren ordua eta progresioa aldatzeko.</span><span class="sxs-lookup"><span data-stu-id="f0b4a-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="f0b4a-129">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="f0b4a-129">See Also</span></span>  
 [<span data-ttu-id="f0b4a-130">Proiektu-kudeatzailearen gida</span><span class="sxs-lookup"><span data-stu-id="f0b4a-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]