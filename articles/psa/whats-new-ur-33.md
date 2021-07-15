---
title: Project Service Automation eguneratzearen 33, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 33. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334497"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="aa010-103">Project Service Automation eguneratzearen 33, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="aa010-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="aa010-104">Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa.</span><span class="sxs-lookup"><span data-stu-id="aa010-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="aa010-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="aa010-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="aa010-106">Dynamics 365 9.x-rekin bateragarria da.</span><span class="sxs-lookup"><span data-stu-id="aa010-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="aa010-107">Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="aa010-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="aa010-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="aa010-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="aa010-109">Gai honek Project Service Automation V3, 33. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="aa010-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="aa010-110">Bertsio honek V3.10.54.98 sorrera-zenbakia du eta orokorrean 2021eko uztailean auto-eguneratze baten bidez eskuragarri dago.</span><span class="sxs-lookup"><span data-stu-id="aa010-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="aa010-111">33. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="aa010-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="aa010-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="aa010-112">Bug fixes</span></span>

<span data-ttu-id="aa010-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="aa010-113">**Time and Expense**</span></span>

<span data-ttu-id="aa010-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="aa010-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="aa010-115">Bi blokeatutako eremuak, **msdyn_description** eta **msdyn_externaldescription** bidali ondoren editatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="aa010-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="aa010-116">Errore-mezu bat gertatzen da proiektu batekin zerikusia ez duen gastua sortzen bada.</span><span class="sxs-lookup"><span data-stu-id="aa010-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="aa010-117">Denbora sarrera bat sortzen denean, baliabide rolak rol inaktibo bihurtzen du lehenespenez.</span><span class="sxs-lookup"><span data-stu-id="aa010-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="aa010-118">Gogoratutako eta ezabatutako gastuarekin lotutako egunkari lerroak ez dira ezabatzen.</span><span class="sxs-lookup"><span data-stu-id="aa010-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="aa010-119">**Denbora sarreraren sorrera azkarreko inprimakian**, eguneratu **Proiektuaren ataza zerrenda** ikuspegia lehenespenez bistaratutako data ataza hasierako datara aldatzeko.</span><span class="sxs-lookup"><span data-stu-id="aa010-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="aa010-120">Fitxategiaren denbora sarrera bat sortzen duzunean baliabide erreserbagarriaren **Erlazionatuta** fitxategik, denbora sarrera gaizki sortu da saioa hasita duen erabiltzailearen baliabide erreserbagarri nagusiaren ordez.</span><span class="sxs-lookup"><span data-stu-id="aa010-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="aa010-121">Eremu berriak gehitzen dira **MDD homologazio masiboa** elkarrizketa-koadroan.</span><span class="sxs-lookup"><span data-stu-id="aa010-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="aa010-122">**Proiektuaren antolaketa**</span><span class="sxs-lookup"><span data-stu-id="aa010-122">**Project planning**</span></span>

<span data-ttu-id="aa010-123">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="aa010-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="aa010-124">Proiektuaren sorrera motela proiektuko lan orduen txantiloiak egutegi konplexuekin aplikatzen direnean.</span><span class="sxs-lookup"><span data-stu-id="aa010-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="aa010-125">Hasiera-data amaiera-data baino handiagoa denean, errore bat agertzen da kopiatzeko proiektuaren txantiloian, eremu bakoitzeko denbora-osagaian desberdintasunak daudelako.</span><span class="sxs-lookup"><span data-stu-id="aa010-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="aa010-126">**Baliabide-kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="aa010-126">**Resource management**</span></span>

<span data-ttu-id="aa010-127">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="aa010-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="aa010-128">Parametro oker bat erabiltzen da baliabideak erabiltzeko kontsultan eta XML-k iragazkiaren emaitza okerrak ekartzen ditu **Baliabideen erabilera** saretan.</span><span class="sxs-lookup"><span data-stu-id="aa010-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="aa010-129">**Luzatu Erreserbak** baieztapenean erreserbak amaitzeko data okerra da.</span><span class="sxs-lookup"><span data-stu-id="aa010-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="aa010-130">**Salmentak**</span><span class="sxs-lookup"><span data-stu-id="aa010-130">**Sales**</span></span>

<span data-ttu-id="aa010-131">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="aa010-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="aa010-132">Errore mezu bat gertatzen da kategoriako prezioa falta den balioekin sortzen bada.</span><span class="sxs-lookup"><span data-stu-id="aa010-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="aa010-133">Errore mezu bat gertatzen da kontratu lerroaren mugarri bat eskaera lerro gabe sortzen bada.</span><span class="sxs-lookup"><span data-stu-id="aa010-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
