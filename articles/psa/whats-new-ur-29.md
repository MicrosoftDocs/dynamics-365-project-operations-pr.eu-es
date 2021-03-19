---
title: Project Service Automation eguneratzearen 29, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 29. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 711255ab66f84fe46d0f16fa72e5a10fe0360394
ms.sourcegitcommit: f78087174a8512199a1bcbd7e8610bbc80e64801
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "5499656"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="59927-103">Project Service Automation eguneratzearen 29, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="59927-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="59927-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="59927-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="59927-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="59927-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="59927-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="59927-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="59927-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="59927-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="59927-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="59927-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="59927-109">Gai honek Project Service Automation V3, 29. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="59927-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="59927-110">Bertsio honek V3.10.45.98 konpilazio-zenbakia du eta, oro har, 2021eko otsailean jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="59927-110">This version has a build number of V3.10.45.98 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="59927-111">29. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="59927-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="59927-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="59927-112">Bug fixes</span></span>

<span data-ttu-id="59927-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="59927-113">**Time and Expense**</span></span>

<span data-ttu-id="59927-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="59927-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="59927-115">Erabiltzaileek ezin dituzte lanorduak egun baliodunetan erregistratuta ikusi denbora sartzeko saretan.</span><span class="sxs-lookup"><span data-stu-id="59927-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="59927-116">Onartutako gastuen sarrerak saretan editatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="59927-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="59927-117">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="59927-117">**Project Management**</span></span>

<span data-ttu-id="59927-118">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="59927-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="59927-119">Baliabideak esleitzeko esfortzuaren orduak ziurtatzeko balioztatzeko logika ezin da negatiboa izan.</span><span class="sxs-lookup"><span data-stu-id="59927-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="59927-120">Pertsonalizatutako ekintza, **AssignResourcesForTask** eremu guztiak eguneratzen ditu aldatutako eremuen ordez.</span><span class="sxs-lookup"><span data-stu-id="59927-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="59927-121">Fitxategian erregistratuta dauden plug-inekin edo lan-fluxuekin ingurune batean proiektu bat kopiatzean **CreateProject** gertaera, **msdyn_bulkgenerationstatus** atributua ez da eguneratu **CopyWBSToProject** huts egiten du.</span><span class="sxs-lookup"><span data-stu-id="59927-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="59927-122">Proiektuaren egutegia zabaltzen duzunean, lanegunak ez dira ordenan gorantz ordenatzen proiektuaren zereginen eguneratze batzuek huts egin dezaten.</span><span class="sxs-lookup"><span data-stu-id="59927-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="59927-123">Lehendik dagoen proiektu batean Proiektuen Kudeatzailea aldatzeak antolaketa-unitate lehenetsitako logika abiarazten du.</span><span class="sxs-lookup"><span data-stu-id="59927-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="59927-124">**Salmentak**</span><span class="sxs-lookup"><span data-stu-id="59927-124">**Sales**</span></span>

<span data-ttu-id="59927-125">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="59927-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="59927-126">**Kontratua gauzatzea** fitxan **Kontratua** orrialdeak isilean huts egiten du hasierakoan, kontratu lerroak ez daudenean.</span><span class="sxs-lookup"><span data-stu-id="59927-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>
