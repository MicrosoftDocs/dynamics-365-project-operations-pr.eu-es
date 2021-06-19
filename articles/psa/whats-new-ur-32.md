---
title: Project Service Automation eguneratzearen 32, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 32. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 11bf451ef4f24e2301ffde4f86a556a8a4fe30b0
ms.sourcegitcommit: 886102894244887d72e5a6213071e8d8a52c9d48
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/01/2021
ms.locfileid: "6129651"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a><span data-ttu-id="711a5-103">Project Service Automation eguneratzearen 32, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="711a5-103">What's new or changed in Project Service Automation Update Release 32, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="711a5-104">Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa.</span><span class="sxs-lookup"><span data-stu-id="711a5-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="711a5-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="711a5-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="711a5-106">Dynamics 365 9.x-rekin bateragarria da.</span><span class="sxs-lookup"><span data-stu-id="711a5-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="711a5-107">Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="711a5-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="711a5-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="711a5-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="711a5-109">Gai honek Project Service Automation V3, 32. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="711a5-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 32.</span></span> <span data-ttu-id="711a5-110">Bertsio honen konpilazio-zenbakia V3.10.53.108 da eta, oro har, 2021eko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="711a5-110">This version has a build number of V3.10.53.108 and is generally available through a self-update in June 2021.</span></span>

## <a name="update-release-32"></a><span data-ttu-id="711a5-111">32. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="711a5-111">Update Release 32</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="711a5-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="711a5-112">Bug fixes</span></span>

#### <a name="general"></a><span data-ttu-id="711a5-113">Orokorrak</span><span class="sxs-lookup"><span data-stu-id="711a5-113">General</span></span>

- <span data-ttu-id="711a5-114">Berritze garrantzitsu batek huts egiten duenean, aplikazioaren sarrera puntu nagusiak soilik blokeatu beharko lirateke, partekatutako entitateak oraindik eskuragarriak direla ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="711a5-114">When a major upgrade fails, only the main application entry points should be blocked, to ensure that shared entities are still accessible.</span></span>

#### <a name="time-and-expense"></a><span data-ttu-id="711a5-115">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="711a5-115">Time and Expense</span></span>

<span data-ttu-id="711a5-116">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="711a5-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="711a5-117">**TimeEntriesImportFromResourceAssignment** ez ditu baliabideak esleitzeko sestra zatiaren hasiera eta amaiera orduak mantentzen.</span><span class="sxs-lookup"><span data-stu-id="711a5-117">**TimeEntriesImportFromResourceAssignment** doesn't maintain the start and end times of the resource assignment contour slice.</span></span>
- <span data-ttu-id="711a5-118">Hautatzen duzunean **Sarrera irekia** **Denbora-sarrera** saretan, baliteke beste inprimaki batzuk hautatzea eragotzi.</span><span class="sxs-lookup"><span data-stu-id="711a5-118">When you select **Open Entry** on the **Time Entry** grid, you might be prevented from selecting other forms.</span></span>
- <span data-ttu-id="711a5-119">Zereginak denbora sarreretara inportatzen dituzunean, bezeroaren kodearen kontsultak kontsultak huts egiten duen URL luzea sor dezake.</span><span class="sxs-lookup"><span data-stu-id="711a5-119">While you import assignments to time entries, the client code query could generate a long URL that fails the query.</span></span>
- <span data-ttu-id="711a5-120">**Denbora-sarrera** saretan, gelaxka batetik balioa ezabatu ondoren, fokua ez da saretan geratzen.</span><span class="sxs-lookup"><span data-stu-id="711a5-120">In the **Time Entry** grid, after a value is deleted from a cell, the focus doesn't remain in the grid.</span></span>
- <span data-ttu-id="711a5-121">**Baztertu** botoia kendu da **Onarpenak tramitatzea** onarpen modernoetarako ikuspegia.</span><span class="sxs-lookup"><span data-stu-id="711a5-121">The **Reject** button has been removed from the **Processing approvals** view for modern approvals.</span></span>
- <span data-ttu-id="711a5-122">Denbora sartzeko ontziratutako onarpenaren egonkortasuna eta errendimendua blokeoek eragiten dute eta pertsonalizazioarekin erlazionatutako pertsonalizazioak modu egokian kudeatzen ez badute **Denbora-sarrera** entitatearekin.</span><span class="sxs-lookup"><span data-stu-id="711a5-122">The stability and performance of time entry bulk approval are affected by deadlocks and a failure to appropriately handle customizations that are related to the **Time Entry** entity.</span></span>

#### <a name="project-planning"></a><span data-ttu-id="711a5-123">Proiektuaren antolaketa</span><span class="sxs-lookup"><span data-stu-id="711a5-123">Project Planning</span></span>

- <span data-ttu-id="711a5-124">Erreferentzia baliogabeko salbuespena sortzen da fitxategian balio baliogabea duen proiektu bat eguneratzen duzunean **Kontratazio-unitatea** eremuan.</span><span class="sxs-lookup"><span data-stu-id="711a5-124">A null reference exception is generated when you update a project that has a null value in the **Contracting Unit** field.</span></span>
- <span data-ttu-id="711a5-125">**Freskatu proiektuaren guztirakoak** proiektu baten gainerako kostua eta gainerako salmentak gaizki kalkulatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="711a5-125">**Refresh Project Totals** incorrectly calculates the remaining cost and remaining sales on a project.</span></span>
- <span data-ttu-id="711a5-126">Prezioen kalkulu erredundanteak eragina dute baliabideak esleitzeko inguruneen eguneratzeekin erlazionatutako errendimenduan.</span><span class="sxs-lookup"><span data-stu-id="711a5-126">Redundant pricing calculations affect performance that is related to updates on resource assignment contours.</span></span>

#### <a name="resource-management"></a><span data-ttu-id="711a5-127">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="711a5-127">Resource Management</span></span>

<span data-ttu-id="711a5-128">Arazo hau konpondu da:</span><span class="sxs-lookup"><span data-stu-id="711a5-128">The following issue has been fixed:</span></span>

- <span data-ttu-id="711a5-129">Erreserbatzeko baliabideen egutegiaren edukiera 1 baino handiagoa denean, Project Service Automation-ek gaitasuna 0 (zero) gisa gaizki aitortzen du.</span><span class="sxs-lookup"><span data-stu-id="711a5-129">When a bookable resource's calendar capacity is more than 1, Project Service Automation incorrectly recognizes the capacity as 0 (zero).</span></span> <span data-ttu-id="711a5-130">Hori dela eta, begizta infinitua gertatzen da programazio ikuspegian.</span><span class="sxs-lookup"><span data-stu-id="711a5-130">Therefore, an infinite loop occurs in the schedule view.</span></span>

#### <a name="sales"></a><span data-ttu-id="711a5-131">Salmentak</span><span class="sxs-lookup"><span data-stu-id="711a5-131">Sales</span></span>

<span data-ttu-id="711a5-132">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="711a5-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="711a5-133">Transakzio mota pertsonalizatua duen aldizkari lerroa sortzen denean, erreferentzia nuluko salbuespen hau gertatzen da: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span><span class="sxs-lookup"><span data-stu-id="711a5-133">When a journal line is created that has a custom transaction type, the following null reference exception occurs: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span></span>
- <span data-ttu-id="711a5-134">Eskaintza baino lehenago inaktibo dauden funtzioak eta kategoriak kopiatzen dira eta ez dira gehitu behar sortu berri den aipamenaren kobra daitezkeen rolak eta kategoriak.</span><span class="sxs-lookup"><span data-stu-id="711a5-134">Roles and categories that are inactivated before a quotation is copied should not be added to chargeable roles and categories of the newly copied quotation.</span></span>
- <span data-ttu-id="711a5-135">Dokumentuen data eta kontabilitate data ez daude bat eginda faktura zirriborroan zuzenean sortzen den faktura lerroaren xehetasunean ematen den hasierako datarekin.</span><span class="sxs-lookup"><span data-stu-id="711a5-135">The document date and accounting date aren't aligned with the start date that is provided on an invoice line detail that is created directly on a draft invoice.</span></span>
- <span data-ttu-id="711a5-136">Aipamen bat kopiatu baino lehen rol eta kategorien desaktibazioarekin lotutako eszenatokietan erreferentzia nuluen salbuespenak sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="711a5-136">Null reference exceptions are generated in scenarios that are related to inactivation of roles and categories before a quotation is copied.</span></span>
- <span data-ttu-id="711a5-137">**Eguneratu Prezioak** ekintza **Proiektuak** orrialdeak ez ditu gastuen kalkuluak eta estimazio materialak eguneratzen.</span><span class="sxs-lookup"><span data-stu-id="711a5-137">The **Update Prices** action on the **Projects** page doesn't update expense estimates and material estimates.</span></span>
