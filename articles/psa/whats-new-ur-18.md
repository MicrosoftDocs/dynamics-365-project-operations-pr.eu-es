---
title: Project Service Automation eguneratzearen 18, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 18. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: f7def50e77a83fd790b81b1b4fd36008ce293b0c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006631"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="b0269-103">Project Service Automation 18, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="b0269-103">Project Service Automation Update Release 18, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b0269-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="b0269-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b0269-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="b0269-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b0269-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="b0269-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b0269-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="b0269-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="b0269-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="b0269-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b0269-109">Gai honek Project Service Automation V3, 18. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="b0269-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="b0269-110">Bertsio honen konpilazio-zenbakia V3.10.8.12 da eta, oro har, 2020ko apirileko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="b0269-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="b0269-111">18. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="b0269-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b0269-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="b0269-112">Bug fixes</span></span>

<span data-ttu-id="b0269-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="b0269-113">**Time and Expense**</span></span>

- <span data-ttu-id="b0269-114">Konponduta: **Berreskuratu**, **Eskatu** eta **Utzi onespena** fluxuek salbuespenak botatzen dituzte errore-mezu ilunekin.</span><span class="sxs-lookup"><span data-stu-id="b0269-114">Fixed: **Recall**, **Request**, and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="b0269-115">Konponduta: **Utzi onespena** aukerak huts egiten duenean gastu batean, dagokion salbuespen-errorea ez da erakusten.</span><span class="sxs-lookup"><span data-stu-id="b0269-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="b0269-116">Konponduta: Orduaren sarrera saretak oker kudeatzen ditu lanegunak ez diren egunak Australian, neguko ordutegira (DST) aldatzean urrian.</span><span class="sxs-lookup"><span data-stu-id="b0269-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="b0269-117">Konponduta: Lehenesteko logika okerrak ez du uzten gastuak bidaltzen.</span><span class="sxs-lookup"><span data-stu-id="b0269-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="b0269-118">Konponduta: Orduaren sarrera onesteak huts egiten duenean, onespena **Zain** egoeran geratzen da.</span><span class="sxs-lookup"><span data-stu-id="b0269-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="b0269-119">Konponduta: SQL erroreak onespen masiboetan (blokeoa/denbora-muga).</span><span class="sxs-lookup"><span data-stu-id="b0269-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="b0269-120">Konponduta: Errendimendu-arazo nabarmenak erabiltzaile-esperientzian denbora-sarrerak onesten diren bitartean taldeko kideak eguneratzeak eragindakoa.</span><span class="sxs-lookup"><span data-stu-id="b0269-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="b0269-121">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="b0269-121">**Project Management**</span></span>

- <span data-ttu-id="b0269-122">Konponduta: Ordu-zonaren jakinarazpena **Adiskidetzea** ikuspegitik **Proiektua** inprimaki nagusira aldatu da.</span><span class="sxs-lookup"><span data-stu-id="b0269-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="b0269-123">Konponduta: Egutegiko txantiloia ez da behar bezala lehenesten proiektuaren inprimaki berri bat irekitzean.</span><span class="sxs-lookup"><span data-stu-id="b0269-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="b0269-124">Konponduta: Chromium-en oinarritutako arakatzaileetan, erabiltzaileek ezin dute erraz hautatu aurrekoaren zereginak ezabatzeko.</span><span class="sxs-lookup"><span data-stu-id="b0269-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="b0269-125">Konponduta: **Txantiloia hutsetako proiektua** sortzean edo kopiatzean, loturarik gabeko zereginak eskuratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="b0269-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="b0269-126">Konponduta: Edge kasu zehatzetan, zereginen saretatik zeregin berri bat sortzean erregistro bikoiztuak sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="b0269-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="b0269-127">Konponduta: Eskuzko moduan, erabiltzaileek ezin dituzte eguneratu zereginen hasiera-datak gordetako uneko data baino geroago.</span><span class="sxs-lookup"><span data-stu-id="b0269-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="b0269-128">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="b0269-128">**Resource Management**</span></span>

- <span data-ttu-id="b0269-129">Konponduta: **Adiskidetzea** ikuspegiko subtotalen errenkadak oker kalkulatzen ditu erreserben aldaera erreserbak luzatu ondoren.</span><span class="sxs-lookup"><span data-stu-id="b0269-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="b0269-130">Konponduta: **Adiskidetzea** ikuspegiak oker bistaratzen ditu baliabideen esleipenak baliabide erreserbagarriak proiektuaren egutegiarekin bat ez datorren egutegia duenean.</span><span class="sxs-lookup"><span data-stu-id="b0269-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="b0269-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="b0269-131">**Sales**</span></span>

- <span data-ttu-id="b0269-132">Konponduta: Denbora-sarrerak berriro onartzen direnean (**Onartu > Utzi >** onartu berriro), kargatu ezin daitekeen benetako datuen kopia bat sortzen da.</span><span class="sxs-lookup"><span data-stu-id="b0269-132">Fixed: When time entries are re-approved (**Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]