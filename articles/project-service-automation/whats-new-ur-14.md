---
title: Project Service Automation eguneratzea 14, V3 bertsioari buruzko berritasunak
description: Gai honek Project Service Automation eguneratzea 14, V3 bertsioko berritasunei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c69eab3b-0bb9-4b52-b606-e8a96e893471
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 31134756a5f4bff3022fca7df8364c49217b9b55
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748863"
---
# <a name="project-service-automation-v3-update-release-14"></a><span data-ttu-id="932b2-103">Project Service Automation V3, eguneratzea 14</span><span class="sxs-lookup"><span data-stu-id="932b2-103">Project Service Automation V3, Update Release 14</span></span>
<span data-ttu-id="932b2-104">Atsegin handiz adierazten dugu Dynamics 365 Project Service Automation (PSA) aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="932b2-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="932b2-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="932b2-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="932b2-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="932b2-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="932b2-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroa eta joan soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="932b2-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="932b2-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="932b2-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="932b2-109">Gai honek PSA V3, 14. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="932b2-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="932b2-110">Bertsio honek V3.10.4.21 konpilazio-zenbakia du eta antolaketa honetan dago erabilgarri:</span><span class="sxs-lookup"><span data-stu-id="932b2-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="932b2-111">**Erabilgarritasun orokorra (auto-eguneratzea):** 2020ko urtarrila</span><span class="sxs-lookup"><span data-stu-id="932b2-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="932b2-112">**Auto eguneratzea:** 2020ko otsaila</span><span class="sxs-lookup"><span data-stu-id="932b2-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="932b2-113">14. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="932b2-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="932b2-114">Hobekuntzak</span><span class="sxs-lookup"><span data-stu-id="932b2-114">Enhancements</span></span>

- <span data-ttu-id="932b2-115">Sales</span><span class="sxs-lookup"><span data-stu-id="932b2-115">Sales</span></span>

     - <span data-ttu-id="932b2-116">**Eskaintza-lerroaren xehetasunak** eremuko eremu-balio pertsonalizatuak **Proiektuaren kontratuaren lerroaren xehetasunak** eremuan kopiatzen dira eskaintza bat **Irabazitako moduan itxia** egoerara eguneratzean.</span><span class="sxs-lookup"><span data-stu-id="932b2-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="932b2-117">Berretsitako proiektuak **Galdutako moduan itxia** gisa ezar daitezke.</span><span class="sxs-lookup"><span data-stu-id="932b2-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="932b2-118">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="932b2-118">Resource Management</span></span>

     - <span data-ttu-id="932b2-119">Erreserbak luzatzean, erabiltzaileei berresteko elkarrizketa-koadroa agertuko zaie erreserba-emaitzak laburbiltzeko eta Erreserbak mantentzeko esteka bat emateko.</span><span class="sxs-lookup"><span data-stu-id="932b2-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="932b2-120">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="932b2-120">Bug fixes</span></span>

- <span data-ttu-id="932b2-121">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="932b2-121">Time and Expense</span></span>

     - <span data-ttu-id="932b2-122">Konponduta: erabiltzailearen esperientzia hobetu da erabiltzaileak ez duelako hautatu zuzentzeko sarrerarik.</span><span class="sxs-lookup"><span data-stu-id="932b2-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="932b2-123">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="932b2-123">Resource Management</span></span>

     - <span data-ttu-id="932b2-124">Konponduta: Baliabide bat behin baino gehiagotan erreserbatzean, erreserba daitekeen baliabidearen izena gainjartzen da.</span><span class="sxs-lookup"><span data-stu-id="932b2-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="932b2-125">Sales</span><span class="sxs-lookup"><span data-stu-id="932b2-125">Sales</span></span>

     - <span data-ttu-id="932b2-126">Konponduta: Salmenta-prezio totala ez da kalkulatzen erabiltzaileak proiektu bateko gutxi gorabeherako kostuaren prezioak ere idatzi arte.</span><span class="sxs-lookup"><span data-stu-id="932b2-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="932b2-127">Konponduta: Eskaintza bat **Irabazita** gisa ixteak huts egiten du, lotutako proiektuaren kontratua ez badago **Zirriborroa** egoeran.</span><span class="sxs-lookup"><span data-stu-id="932b2-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>

