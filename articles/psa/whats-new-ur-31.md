---
title: Project Service Automation eguneratzearen 31, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 31. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: a595c0a129ac35d3416984e57908e73e1eaef2fd
ms.sourcegitcommit: 6e1498502461e86cff722ccaf8795ff11c7c47ad
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5945520"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="d8d45-103">Project Service Automation eguneratzearen 31, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="d8d45-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="d8d45-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="d8d45-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="d8d45-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="d8d45-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="d8d45-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="d8d45-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="d8d45-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="d8d45-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="d8d45-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="d8d45-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="d8d45-109">Gai honek Project Service Automation V3, 31. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="d8d45-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="d8d45-110">Bertsio honen konpilazio-zenbakia V3.10.52.77 da eta, oro har, 2021eko maiatzeko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="d8d45-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="d8d45-111">31. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="d8d45-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="d8d45-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="d8d45-112">Bug fixes</span></span>

<span data-ttu-id="d8d45-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="d8d45-113">**Time and Expense**</span></span>

<span data-ttu-id="d8d45-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="d8d45-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="d8d45-115">Denboraren sarrera kontrolatzeko komando botoiak **Erreserbatzeko Baliabidea** orrialdea nahasgarria zen.</span><span class="sxs-lookup"><span data-stu-id="d8d45-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="d8d45-116">Urtean erreferentziazko salbuespen nulua sortu zen **Project.SetTrackingFields** denbora sarrera onartzerakoan.</span><span class="sxs-lookup"><span data-stu-id="d8d45-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="d8d45-117">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="d8d45-117">**Resource Management**</span></span>

<span data-ttu-id="d8d45-118">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="d8d45-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="d8d45-119">**Sortu taldeko kidea** ez du behar bezala erakusten erreserbaren konfigurazioko metadatuen ezarpena **Erreserbaren lehenetsitako konpromiso egoera**.</span><span class="sxs-lookup"><span data-stu-id="d8d45-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="d8d45-120">PSA 1.X-tik 3.X-ra eguneratzean, eguneratze prozesuak huts egiten du **UpgradeResourceRequirements**.</span><span class="sxs-lookup"><span data-stu-id="d8d45-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="d8d45-121">**Salmentak**</span><span class="sxs-lookup"><span data-stu-id="d8d45-121">**Sales**</span></span>

<span data-ttu-id="d8d45-122">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="d8d45-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="d8d45-123">Benetako diru-sarrerek zenbatekoak proiektuaren monetara bihurtzen dituzte jarraipen-saretan.</span><span class="sxs-lookup"><span data-stu-id="d8d45-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="d8d45-124">Moneta lehenetsia ez da argia egunkari-lerroak, aurrekontu-lerroak eta kontratu-lerroak sortzerakoan erakunde baten oinarrizko moneta proiektuaren moneta desberdina den agertokietan.</span><span class="sxs-lookup"><span data-stu-id="d8d45-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="d8d45-125">**Aldizkariaren balioztapenaren zain** kontsultak ez du proiektuaren arabera iragazten.</span><span class="sxs-lookup"><span data-stu-id="d8d45-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="d8d45-126">Gainerako salmentak proiektu batean gaizki kalkulatzen dira.</span><span class="sxs-lookup"><span data-stu-id="d8d45-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="d8d45-127">Kontaktu batean oinarritutako aurrekontuek huts egiten dute prezio zerrendarik gabe sortzen direnean.</span><span class="sxs-lookup"><span data-stu-id="d8d45-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="d8d45-128">Hautatzen duzunean ez da prozesatzeko birarik erakusten **Berretsi faktura**.</span><span class="sxs-lookup"><span data-stu-id="d8d45-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="d8d45-129">Hautatzen duzunean ez da prozesatzeko birarik erakusten **Sortu faktura**.</span><span class="sxs-lookup"><span data-stu-id="d8d45-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="d8d45-130">Aurrekontua galdu ahala itxiz gero, ez dira erreserbak bertan behera geratuko.</span><span class="sxs-lookup"><span data-stu-id="d8d45-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







