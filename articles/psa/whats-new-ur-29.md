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
ms.openlocfilehash: 0e1ff0db42adb8b991b26dca1585bd603b2e2276
ms.sourcegitcommit: f57408d6637f670b920d7ce95f8ace8eb1963093
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/17/2021
ms.locfileid: "5664628"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="9ab62-103">Project Service Automation eguneratzearen 29, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="9ab62-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="9ab62-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="9ab62-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="9ab62-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="9ab62-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="9ab62-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="9ab62-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="9ab62-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="9ab62-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="9ab62-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="9ab62-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="9ab62-109">Gai honek Project Service Automation V3, 29. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="9ab62-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="9ab62-110">Bertsio honek V3.10.47.7 konpilazio-zenbakia du eta, oro har, 2021eko otsailean jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="9ab62-110">This version has a build number of V3.10.47.7 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="9ab62-111">29. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="9ab62-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="9ab62-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="9ab62-112">Bug fixes</span></span>

<span data-ttu-id="9ab62-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="9ab62-113">**Time and Expense**</span></span>

<span data-ttu-id="9ab62-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="9ab62-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="9ab62-115">Erabiltzaileek ezin dituzte lanorduak egun baliodunetan erregistratuta ikusi denbora sartzeko saretan.</span><span class="sxs-lookup"><span data-stu-id="9ab62-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="9ab62-116">Onartutako gastuen sarrerak saretan editatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="9ab62-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="9ab62-117">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="9ab62-117">**Project Management**</span></span>

<span data-ttu-id="9ab62-118">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="9ab62-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="9ab62-119">Baliabideak esleitzeko esfortzuaren orduak ziurtatzeko balioztatzeko logika ezin da negatiboa izan.</span><span class="sxs-lookup"><span data-stu-id="9ab62-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="9ab62-120">Pertsonalizatutako ekintza, **AssignResourcesForTask** eremu guztiak eguneratzen ditu aldatutako eremuen ordez.</span><span class="sxs-lookup"><span data-stu-id="9ab62-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="9ab62-121">Fitxategian erregistratuta dauden plug-inekin edo lan-fluxuekin ingurune batean proiektu bat kopiatzean **CreateProject** gertaera, **msdyn_bulkgenerationstatus** atributua ez da eguneratu **CopyWBSToProject** huts egiten du.</span><span class="sxs-lookup"><span data-stu-id="9ab62-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="9ab62-122">Proiektuaren egutegia zabaltzen duzunean, lanegunak ez dira ordenan gorantz ordenatzen proiektuaren zereginen eguneratze batzuek huts egin dezaten.</span><span class="sxs-lookup"><span data-stu-id="9ab62-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="9ab62-123">Lehendik dagoen proiektu batean Proiektuen Kudeatzailea aldatzeak antolaketa-unitate lehenetsitako logika abiarazten du.</span><span class="sxs-lookup"><span data-stu-id="9ab62-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="9ab62-124">**Salmentak**</span><span class="sxs-lookup"><span data-stu-id="9ab62-124">**Sales**</span></span>

<span data-ttu-id="9ab62-125">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="9ab62-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="9ab62-126">**Kontratua gauzatzea** fitxan **Kontratua** orrialdeak isilean huts egiten du hasierakoan, kontratu lerroak ez daudenean.</span><span class="sxs-lookup"><span data-stu-id="9ab62-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>
