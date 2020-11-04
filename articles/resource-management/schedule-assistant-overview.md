---
title: Antolaketa-laguntzailearen ikuspegi orokorra
description: Gai honek baliabideak erreserbatzeko Ordutegiaren laguntzailearekin lan egiteari buruzko informazioa eskaintzen du.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: da551e805f395e466952df1dbb7d193bdddba358
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070892"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="8e08f-103">Antolaketa-laguntzailearen ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="8e08f-103">Schedule assistant overview</span></span>

<span data-ttu-id="8e08f-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="8e08f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8e08f-105">Ordutegiaren laguntzailea proiektuaren kudeatzaileak zehaztutako eskakizunen arabera baliabideak erreserbatzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="8e08f-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="8e08f-106">Ordutegiaren laguntzailea baliabidearen eskakizunean emandako parametroetan oinarritzen da, baliabidea aurkitzeko.</span><span class="sxs-lookup"><span data-stu-id="8e08f-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="8e08f-107">Ordutegien laguntzaileak eskakizun egokiekin bat datozen baliabideak gomendatzen ditu, hala nola, denbora leihoak edo beharrezkoak diren trebetasunak.</span><span class="sxs-lookup"><span data-stu-id="8e08f-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="8e08f-108">Baliabide egokiak identifikatu ondoren, Baliabideak edo Proiektuen kudeatzaileak baliabidea lanerako gorde dezake.</span><span class="sxs-lookup"><span data-stu-id="8e08f-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e08f-109">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="8e08f-109">Prerequisites</span></span>

<span data-ttu-id="8e08f-110">Ordutegien laguntzailea Universal Resource Scheduling soluzioaren zati bat da.</span><span class="sxs-lookup"><span data-stu-id="8e08f-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="8e08f-111">Soluzio hau Dynamics 365 Project Operations, Dynamics 365 Field Service eta Dynamics 365 Customer Service zerbitzuen barne eta instalatuta dago.</span><span class="sxs-lookup"><span data-stu-id="8e08f-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="8e08f-112">Bat egiten duten eskakizunak eta baliabideak</span><span class="sxs-lookup"><span data-stu-id="8e08f-112">Matching requirements and resources</span></span>

<span data-ttu-id="8e08f-113">Sortutako baliabideen eskakizunak honelako xehetasunetan oinarritzen dira:</span><span class="sxs-lookup"><span data-stu-id="8e08f-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="8e08f-114">Ezaugarriak</span><span class="sxs-lookup"><span data-stu-id="8e08f-114">Characteristics</span></span>
-   <span data-ttu-id="8e08f-115">Funtzioak</span><span class="sxs-lookup"><span data-stu-id="8e08f-115">Roles</span></span>
-   <span data-ttu-id="8e08f-116">Negozio-unitateak</span><span class="sxs-lookup"><span data-stu-id="8e08f-116">Business units</span></span>
-   <span data-ttu-id="8e08f-117">Baliabideen hobespenak</span><span class="sxs-lookup"><span data-stu-id="8e08f-117">Resource preferences</span></span>
-   <span data-ttu-id="8e08f-118">Esfortzu sestra</span><span class="sxs-lookup"><span data-stu-id="8e08f-118">Effort contours</span></span>
-   <span data-ttu-id="8e08f-119">Ordu-zona</span><span class="sxs-lookup"><span data-stu-id="8e08f-119">Time zone</span></span>

<span data-ttu-id="8e08f-120">Programazio laguntzaileak xehetasun hauek erabiltzen ditu baliabideak iragazteko.</span><span class="sxs-lookup"><span data-stu-id="8e08f-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="8e08f-121">Abiarazi Antolaketa-laguntzailea</span><span class="sxs-lookup"><span data-stu-id="8e08f-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="8e08f-122">Ordutegi laguntzailea abiarazteko bi modu daude.</span><span class="sxs-lookup"><span data-stu-id="8e08f-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="8e08f-123">Modu hibridoa erabiltzen ari bazara, taldekideen saretan, bete gabeko baliabide eskakizuna duen edozein taldekide hautatu dezakezu eta, ondoren, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="8e08f-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="8e08f-124">Modu zentrala erabiltzen ari bazara, Resource Manager baliabidea aurkitu eta hautatzen du.</span><span class="sxs-lookup"><span data-stu-id="8e08f-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="8e08f-125">Antolaketa-laguntzailearen iragazkiak</span><span class="sxs-lookup"><span data-stu-id="8e08f-125">Schedule assistant filters</span></span>

<span data-ttu-id="8e08f-126">Ordutegiaren laguntzailea exekutatu ondoren, baliabide eskakizunaren xehetasunak ezkerreko panelean iragazitako balio gisa bistaratuko dira.</span><span class="sxs-lookup"><span data-stu-id="8e08f-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="8e08f-127">Baliabideen kudeatzaileak edo Proiektuaren kudeatzaileak emaitzak zehatz ditzake, iragazkiak egokituz programazio beharrak asetzeko.</span><span class="sxs-lookup"><span data-stu-id="8e08f-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="8e08f-128">Iragazki-panelak lanarekin lotutako aukerak erakusten ditu, besteak beste:</span><span class="sxs-lookup"><span data-stu-id="8e08f-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="8e08f-129">Lanaren hasiera eta amaiera</span><span class="sxs-lookup"><span data-stu-id="8e08f-129">Work start and end</span></span>
-   <span data-ttu-id="8e08f-130">Ezaugarriak</span><span class="sxs-lookup"><span data-stu-id="8e08f-130">Characteristics</span></span>
-   <span data-ttu-id="8e08f-131">Funtzioak</span><span class="sxs-lookup"><span data-stu-id="8e08f-131">Roles</span></span>
-   <span data-ttu-id="8e08f-132">Erakundearen unitateak</span><span class="sxs-lookup"><span data-stu-id="8e08f-132">Organizational units</span></span>
-   <span data-ttu-id="8e08f-133">Baliabideen enpresa</span><span class="sxs-lookup"><span data-stu-id="8e08f-133">Resourcing company</span></span>
-   <span data-ttu-id="8e08f-134">Baliabide motak</span><span class="sxs-lookup"><span data-stu-id="8e08f-134">Resource types</span></span>
-   <span data-ttu-id="8e08f-135">Hobetsitako baliabideak</span><span class="sxs-lookup"><span data-stu-id="8e08f-135">Preferred resources</span></span>
