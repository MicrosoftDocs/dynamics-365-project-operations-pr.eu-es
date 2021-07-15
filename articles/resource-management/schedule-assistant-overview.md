---
title: Antolaketa-laguntzailearen ikuspegi orokorra
description: Gai honek baliabideak erreserbatzeko Ordutegiaren laguntzailearekin lan egiteari buruzko informazioa eskaintzen du.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 83583c97e4ecb5f1fdc0d8d98098afe8e12d27e4
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368101"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="76d4d-103">Antolaketa-laguntzailearen ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="76d4d-103">Schedule assistant overview</span></span>

<span data-ttu-id="76d4d-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="76d4d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="76d4d-105">Ordutegiaren laguntzailea proiektuaren kudeatzaileak zehaztutako eskakizunen arabera baliabideak erreserbatzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="76d4d-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="76d4d-106">Ordutegiaren laguntzailea baliabidearen eskakizunean emandako parametroetan oinarritzen da, baliabidea aurkitzeko.</span><span class="sxs-lookup"><span data-stu-id="76d4d-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="76d4d-107">Ordutegien laguntzaileak eskakizun egokiekin bat datozen baliabideak gomendatzen ditu, hala nola, denbora leihoak edo beharrezkoak diren trebetasunak.</span><span class="sxs-lookup"><span data-stu-id="76d4d-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="76d4d-108">Baliabide egokiak identifikatu ondoren, Baliabideak edo Proiektuen kudeatzaileak baliabidea lanerako gorde dezake.</span><span class="sxs-lookup"><span data-stu-id="76d4d-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76d4d-109">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="76d4d-109">Prerequisites</span></span>

<span data-ttu-id="76d4d-110">Ordutegien laguntzailea Universal Resource Scheduling soluzioaren zati bat da.</span><span class="sxs-lookup"><span data-stu-id="76d4d-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="76d4d-111">Irtenbide hau instalatuta dago Dynamics 365 Project Operations, Dynamics 365 Field Service eta Dynamics 365 Customer Service-kin.</span><span class="sxs-lookup"><span data-stu-id="76d4d-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="76d4d-112">Bat egiten duten eskakizunak eta baliabideak</span><span class="sxs-lookup"><span data-stu-id="76d4d-112">Matching requirements and resources</span></span>

<span data-ttu-id="76d4d-113">Sortutako baliabideen eskakizunak honelako xehetasunetan oinarritzen dira:</span><span class="sxs-lookup"><span data-stu-id="76d4d-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="76d4d-114">Ezaugarriak</span><span class="sxs-lookup"><span data-stu-id="76d4d-114">Characteristics</span></span>
-   <span data-ttu-id="76d4d-115">Funtzioak</span><span class="sxs-lookup"><span data-stu-id="76d4d-115">Roles</span></span>
-   <span data-ttu-id="76d4d-116">Negozio-unitateak</span><span class="sxs-lookup"><span data-stu-id="76d4d-116">Business units</span></span>
-   <span data-ttu-id="76d4d-117">Baliabideen hobespenak</span><span class="sxs-lookup"><span data-stu-id="76d4d-117">Resource preferences</span></span>
-   <span data-ttu-id="76d4d-118">Esfortzu sestra</span><span class="sxs-lookup"><span data-stu-id="76d4d-118">Effort contours</span></span>
-   <span data-ttu-id="76d4d-119">Ordu-zona</span><span class="sxs-lookup"><span data-stu-id="76d4d-119">Time zone</span></span>

<span data-ttu-id="76d4d-120">Programazio laguntzaileak xehetasun hauek erabiltzen ditu baliabideak iragazteko.</span><span class="sxs-lookup"><span data-stu-id="76d4d-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="76d4d-121">Abiarazi Antolaketa-laguntzailea</span><span class="sxs-lookup"><span data-stu-id="76d4d-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="76d4d-122">Ordutegi laguntzailea abiarazteko bi modu daude.</span><span class="sxs-lookup"><span data-stu-id="76d4d-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="76d4d-123">Modu hibridoa erabiltzen ari bazara, taldekideen saretan, bete gabeko baliabide eskakizuna duen edozein taldekide hautatu dezakezu eta, ondoren, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="76d4d-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="76d4d-124">Modu zentrala erabiltzen ari bazara, Resource Manager baliabidea aurkitu eta hautatzen du.</span><span class="sxs-lookup"><span data-stu-id="76d4d-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="76d4d-125">Antolaketa-laguntzailearen iragazkiak</span><span class="sxs-lookup"><span data-stu-id="76d4d-125">Schedule assistant filters</span></span>

<span data-ttu-id="76d4d-126">Ordutegiaren laguntzailea exekutatu ondoren, baliabide eskakizunaren xehetasunak ezkerreko panelean iragazitako balio gisa bistaratuko dira.</span><span class="sxs-lookup"><span data-stu-id="76d4d-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="76d4d-127">Baliabideen kudeatzaileak edo Proiektuaren kudeatzaileak emaitzak zehatz ditzake, iragazkiak egokituz programazio beharrak asetzeko.</span><span class="sxs-lookup"><span data-stu-id="76d4d-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="76d4d-128">Iragazki-panelak lanarekin lotutako aukerak erakusten ditu, besteak beste:</span><span class="sxs-lookup"><span data-stu-id="76d4d-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="76d4d-129">Lanaren hasiera eta amaiera</span><span class="sxs-lookup"><span data-stu-id="76d4d-129">Work start and end</span></span>
-   <span data-ttu-id="76d4d-130">Ezaugarriak</span><span class="sxs-lookup"><span data-stu-id="76d4d-130">Characteristics</span></span>
-   <span data-ttu-id="76d4d-131">Funtzioak</span><span class="sxs-lookup"><span data-stu-id="76d4d-131">Roles</span></span>
-   <span data-ttu-id="76d4d-132">Erakundearen unitateak</span><span class="sxs-lookup"><span data-stu-id="76d4d-132">Organizational units</span></span>
-   <span data-ttu-id="76d4d-133">Baliabideen enpresa</span><span class="sxs-lookup"><span data-stu-id="76d4d-133">Resourcing company</span></span>
-   <span data-ttu-id="76d4d-134">Baliabide motak</span><span class="sxs-lookup"><span data-stu-id="76d4d-134">Resource types</span></span>
-   <span data-ttu-id="76d4d-135">Hobetsitako baliabideak</span><span class="sxs-lookup"><span data-stu-id="76d4d-135">Preferred resources</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]