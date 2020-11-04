---
title: Zehaztu proiektuen egutegiak
description: Gai honek proiektuaren egutegia proiektuaren egutegia jarraitzeko erabiltzeari buruzko informazioa eskaintzen du.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 774399f2c02d8434c9c042c3a9f995792893bfce
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071210"
---
# <a name="define-project-calendars"></a><span data-ttu-id="d67ad-103">Zehaztu proiektuen egutegiak</span><span class="sxs-lookup"><span data-stu-id="d67ad-103">Define project calendars</span></span>

<span data-ttu-id="d67ad-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="d67ad-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d67ad-105">Proiektuaren antolaketa sortzeko, sortu eguneko lan-orduak definitzen dituen proiektu-egutegia eta baita negozio-itxierak ere.</span><span class="sxs-lookup"><span data-stu-id="d67ad-105">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="d67ad-106">Proiektu-egutegiaren txantiloia sortzeko, lotu laneko txantiloi bat **Egutegiaren txantiloia** eremuarekin proiekturako.</span><span class="sxs-lookup"><span data-stu-id="d67ad-106">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="d67ad-107">Jarraitu urrats hauei lan-txantiloia sortzeko.</span><span class="sxs-lookup"><span data-stu-id="d67ad-107">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="d67ad-108">Ezkerreko nabigazio-panelean, hautatu **Baliabideak**.</span><span class="sxs-lookup"><span data-stu-id="d67ad-108">In the left navigation pane, select **Resources**.</span></span> 
2. <span data-ttu-id="d67ad-109">**Baliabideak** zerrenda-orrian, ireki erabiltzaileen erregistroa eta hautatu hautatu **Erakutsi lanorduak**.</span><span class="sxs-lookup"><span data-stu-id="d67ad-109">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="d67ad-110">Ziurtatu arakatzailearen orrian leiho gainerakorrak onartzen dituzula.</span><span class="sxs-lookup"><span data-stu-id="d67ad-110">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="d67ad-111">Horrek baliabiderako ezarritako lanorduak ikusteko aukera ematen du.</span><span class="sxs-lookup"><span data-stu-id="d67ad-111">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="d67ad-112">**Hileroko ikuspegia** fitxan, hautatu **Konfiguratu** aukeran.</span><span class="sxs-lookup"><span data-stu-id="d67ad-112">On the **Monthly View** tab, select **Set Up**.</span></span> <span data-ttu-id="d67ad-113">Hiru aukeradun zerrenda bat agertzen da:</span><span class="sxs-lookup"><span data-stu-id="d67ad-113">A list of three options appears:</span></span> 

  - <span data-ttu-id="d67ad-114">Asteko antolaketa berria</span><span class="sxs-lookup"><span data-stu-id="d67ad-114">New Weekly Schedule</span></span>
  - <span data-ttu-id="d67ad-115">Egun baterako lan-antolaketa</span><span class="sxs-lookup"><span data-stu-id="d67ad-115">Work Schedule for One Day</span></span>
  - <span data-ttu-id="d67ad-116">Astialdia</span><span class="sxs-lookup"><span data-stu-id="d67ad-116">Time Off</span></span>

4. <span data-ttu-id="d67ad-117">Hautatu **Asteko antolaketa berria** eta, ondoren, ezarri baliabideen antolaketa horretarako aukerak.</span><span class="sxs-lookup"><span data-stu-id="d67ad-117">Select **New Weekly Schedule** , and then set the options for this resource schedule.</span></span> <span data-ttu-id="d67ad-118">Asteroko ordutegi errepikakorra, eguneroko ordu-parametroak, negozioen itxiera eta beste batzuk ezar ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="d67ad-118">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="d67ad-119">Ezarri data-tartea, hautatu **Gorde** eta, ondoren, hautatu **Itxi** aukeran.</span><span class="sxs-lookup"><span data-stu-id="d67ad-119">Set the date range, select **Save** , and then select **Close**.</span></span> 
6. <span data-ttu-id="d67ad-120">Itzuli berriro **Baliabideak** zerrenda-orrira eta hautatu lanorduak zehaztu dituzun baliabidea.</span><span class="sxs-lookup"><span data-stu-id="d67ad-120">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="d67ad-121">Hautatu **Ezarri egutegia honela** lan txantiloia ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="d67ad-121">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="d67ad-122">**Lan-txantiloia** elkarrizketa-koadroan, idatzi lan-txantiloiaren izena eta hautatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="d67ad-122">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="d67ad-123">Orain lan-txantiloia proiektuaren egutegi txantiloiarekin lotu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="d67ad-123">You can now associate the work template with a project calendar template.</span></span>
