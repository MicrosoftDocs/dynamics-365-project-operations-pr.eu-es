---
title: Sortu lanorduen-txantiloia
description: Nola sortu lanorduen txantiloiak Project Service-n
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 1a519487-25f1-4e9d-b739-1c1becf1d649
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5e7ef4af5f22419cccd8f29ea2a0a0a21a75875a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748892"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="6572d-103">Sortu lanorduen txantiloiak (Project Service)</span><span class="sxs-lookup"><span data-stu-id="6572d-103">Create a work hours template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6572d-104">Proiektu-antolaketak sortu baino lehen, lan-orduak definitzen dituen proiektu-egutegia konfiguratu behar duzu, antolaketa egunero egokitzeko baita negozio-itxierak ere.</span><span class="sxs-lookup"><span data-stu-id="6572d-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="6572d-105">Lanorduen txantiloiekin egiten da hori. Egun bakoitzeko lanorduei, jaiegunei eta besteko negozio-itxierei buruzko informazioa baitute.</span><span class="sxs-lookup"><span data-stu-id="6572d-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="6572d-106">Proiektua bat sortzen ari zerenean, lan-txantiloi bat proiektu-egutegi batekin lotu dezakezu, proiektu horren antolaketa aplikatzeko.</span><span class="sxs-lookup"><span data-stu-id="6572d-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="6572d-107">Lanorduen txantiloia sortzeko bi modu daude:</span><span class="sxs-lookup"><span data-stu-id="6572d-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="6572d-108">Sortu lanorduen txantiloia baliabideen egutegian oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="6572d-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="6572d-109">Sortu lanorduen txantiloi berri bat.</span><span class="sxs-lookup"><span data-stu-id="6572d-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="6572d-110">Lanorduen txantiloia baliabideen egutegian oinarrituta sortzeko</span><span class="sxs-lookup"><span data-stu-id="6572d-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="6572d-111">Joan **Project Service > Baliabideak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="6572d-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="6572d-112">Hautatu lanorduen oinarri gisa hartu nahi duzun baliabidea.</span><span class="sxs-lookup"><span data-stu-id="6572d-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="6572d-113">Sakatu **Gorde egutegi gisa**, idatzi lanorduen txantiloiren izena eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="6572d-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="6572d-114">Aukerak aldatzen amaitutakoan, sakatu **Gorde eta itxi**.</span><span class="sxs-lookup"><span data-stu-id="6572d-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="6572d-115">Sakatu **Gorde** pantailaren behe-eskuineko izkineko botoia.</span><span class="sxs-lookup"><span data-stu-id="6572d-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="6572d-116">Lanorduen txantiloi berri bat sortzeko</span><span class="sxs-lookup"><span data-stu-id="6572d-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="6572d-117">Joan **Project Service > Lanorduen txantiloiak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="6572d-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="6572d-118">Sakatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="6572d-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="6572d-119">Idatzi lanorduen txantiloiaren izena.</span><span class="sxs-lookup"><span data-stu-id="6572d-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="6572d-120">Hautatu lanorduak oinarritzeko baliabidea eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="6572d-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="6572d-121">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="6572d-121">See Also</span></span>  
 [<span data-ttu-id="6572d-122">Baliabideak konfiguratu</span><span class="sxs-lookup"><span data-stu-id="6572d-122">Set up resources</span></span>](../project-service/set-up-resources.md)
