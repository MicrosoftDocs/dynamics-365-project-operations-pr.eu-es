---
title: Eguneratu aurreikusitako kostua osatzen denerako
description: Gai honek proiektu baten ahaleginaren proiekzioa eguneratzeari buruzko informazioa eskaintzen du.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 16393133a5de17308caceb069d7bca670caa04c8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071219"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="ba923-103">Eguneratu aurreikusitako kostua osatzen denerako</span><span class="sxs-lookup"><span data-stu-id="ba923-103">Update estimate at completion</span></span>

<span data-ttu-id="ba923-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="ba923-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ba923-105">Ohikoa da proiektu-kudeatzaile batek zereginen jatorrizko kalkuluak berrikustea.</span><span class="sxs-lookup"><span data-stu-id="ba923-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="ba923-106">Proiektuaren birproiekzioak proiektu-kudeatzaileak proiektuaren egungo egoera ikusita duen kalkuluen pertzepzioa da.</span><span class="sxs-lookup"><span data-stu-id="ba923-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="ba923-107">Hala ere, ez dugu gomendatzen proiektu-kudeatzaileak oinarrizko zenbakiak aldatzea, proiektuaren oinarria baita proiektuaren antolaketaren eta kostuen ezarritako benetako jatorria eta proiektuko interes-talde guztiek onartu dute hori.</span><span class="sxs-lookup"><span data-stu-id="ba923-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="ba923-108">Proiektu-kudeatzaileak bi modutara birproiektatu ditzake zereginetako ahaleginak:</span><span class="sxs-lookup"><span data-stu-id="ba923-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="ba923-109">Gainidatzi osatzeko aurreikuspena (ETC) lehenetsia zereginen benetako ahaleginaren beste kalkulu batekin.</span><span class="sxs-lookup"><span data-stu-id="ba923-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="ba923-110">Gainidatzi garapenaren ehuneko lehenetsia zereginen benetako garapenaren beste kalkulu batekin.</span><span class="sxs-lookup"><span data-stu-id="ba923-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="ba923-111">Planteamendu horietako bakoitzak zereginaren ETC, osatzeko aurreikuspena (EAC) eta garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du.</span><span class="sxs-lookup"><span data-stu-id="ba923-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="ba923-112">Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa berriro kalkulatzen dira eta ahaleginaren bariantzaren proiekzio berri bat sortzen dute.</span><span class="sxs-lookup"><span data-stu-id="ba923-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
