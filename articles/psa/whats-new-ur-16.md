---
title: Project Service Automation eguneratzearen 16, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 16. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
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
ms.openlocfilehash: 2c93d34b61001b7755d426539ac384641a7bc9da
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121563"
---
# <a name="project-service-automation-update-release-16-v3"></a><span data-ttu-id="2f353-103">Project Service Automation 16, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="2f353-103">Project Service Automation Update Release 16, V3</span></span>

<span data-ttu-id="2f353-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="2f353-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="2f353-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="2f353-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="2f353-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="2f353-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="2f353-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f353-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="2f353-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu soluzio hobetsi bat](https://docs.microsoft.com/dynamics365/project-service/upgrade-psa-home-page).</span><span class="sxs-lookup"><span data-stu-id="2f353-108">For more information, see [Install, Update a Preferred Solution](https://docs.microsoft.com/dynamics365/project-service/upgrade-psa-home-page).</span></span>
<span data-ttu-id="2f353-109">Gai honek PSA V3, 16. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="2f353-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 16.</span></span> <span data-ttu-id="2f353-110">Bertsio honek V3.10.6.34 konpilazio-zenbakia du eta, oro har, 2020ko urtarrilean jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="2f353-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in January 2020.</span></span>


## <a name="update-release-16"></a><span data-ttu-id="2f353-111">16. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="2f353-111">Update Release 16</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="2f353-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="2f353-112">Bug fixes</span></span>

-   <span data-ttu-id="2f353-113">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="2f353-113">Time and Expense</span></span>

    -   <span data-ttu-id="2f353-114">Konponduta: ezabatutako denboraren eta gastuen sarrerak onartzeko bidaltzen saiatzen diren erabiltzaileek errore-mezuak jasoko dituzte.</span><span class="sxs-lookup"><span data-stu-id="2f353-114">Fixed: Users attempting to submit deleted time and expense entries for approvals will now receive relevant error messages.</span></span>

-   <span data-ttu-id="2f353-115">Proiektuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="2f353-115">Project Management</span></span>

    -   <span data-ttu-id="2f353-116">Konponduta: txantiloietan taldekideek zehaztutako resourcing unitateak txantiloiak proiektu berri bati aplikatzen zaizkio.</span><span class="sxs-lookup"><span data-stu-id="2f353-116">Fixed: The resourcing units defined for team members in templates are respected with the templates are applied to a new project.</span></span>

    -   <span data-ttu-id="2f353-117">Konponduta: Erregistroen jabetza berriro esleitzea hobeto kudeatzea.</span><span class="sxs-lookup"><span data-stu-id="2f353-117">Fixed: Improved handling of the re-assignment of record ownership.</span></span>

    -   <span data-ttu-id="2f353-118">Konponduta: kopia prozesuan dauden proiektuei ezin zaie kopiatu baimendu operazio guztiak amaitu arte.</span><span class="sxs-lookup"><span data-stu-id="2f353-118">Fixed: Projects that are in the process of being copied will not be permitted to copied until all copy operations are complete.</span></span>

-   <span data-ttu-id="2f353-119">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="2f353-119">Resource Management</span></span>

    -   <span data-ttu-id="2f353-120">Konponduta: Luzatu erreserbak orain arteko iraupen laburrak behar bezala kudeatzen ditu eta ez du zero ordu sortzen erreserba luzatuetarako.</span><span class="sxs-lookup"><span data-stu-id="2f353-120">Fixed: Extend bookings now handles short durations correctly and no longer creates zero hours for extended bookings.</span></span>

    -   <span data-ttu-id="2f353-121">Konponduta: bateratze ikuspegia proiektuaren ordu-eremua +5:30 GMT denean eta erabiltzailearen denbora bakar bat desberdina denean ematen da.</span><span class="sxs-lookup"><span data-stu-id="2f353-121">Fixed: The reconciliation view now renders when the project time zone is +5:30 GMT and the user’s time aone is different.</span></span>

-   <span data-ttu-id="2f353-122">Sales</span><span class="sxs-lookup"><span data-stu-id="2f353-122">Sales</span></span>

    -   <span data-ttu-id="2f353-123">Konponduta: proiektu bat kontratatu lerrora kendutakoan eta proiektu berri bat mapatzen denean, proiektu berriaren benetako erregistroak ez ziren berriro ebaluatu kontratuaren lerroan zehaztutako fakturazio- eta prezio-arauen arabera.</span><span class="sxs-lookup"><span data-stu-id="2f353-123">Fixed: When a project mapped to a contract line is removed and a new project is mapped, the actual records on the new project were not getting re-evaluated based on the billing and pricing rules defined on the contract line.</span></span> <span data-ttu-id="2f353-124">Hori konpondu da bertsio honetan.</span><span class="sxs-lookup"><span data-stu-id="2f353-124">This has been fixed in this release.</span></span> <span data-ttu-id="2f353-125">Mapatu berri den proiektuaren prezioak eta benetako erregistroak behar bezala berraztertu eta berriro sortuko dira, kontratuaren lerroko prezio eta fakturazio arauetan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="2f353-125">Pricing and actual records on the newly mapped project will get reversed and re-created correctly based on the pricing and billing rules of the contract line.</span></span> <span data-ttu-id="2f353-126">Mapatu gabeko proiektuaren benetako erregistroak berriro ebaluatu eta berriro sortuko dira.</span><span class="sxs-lookup"><span data-stu-id="2f353-126">The actual records of the un-mapped project will also get re-evaluated and re-created as a consequence.</span></span>

    -   <span data-ttu-id="2f353-127">Konponduta: balioztapen gehigarria gehitu zaio estimazio lerroari **Zenbatekoa** eremua balio nuluak ez direla irauten ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="2f353-127">Fixed: Additional validation has been added to an estimate line’s **Amount** field to ensure that null values are not persisted.</span></span>

    -   <span data-ttu-id="2f353-128">Konponduta: proiektuak eguneratu direnean, freskatze botoia gehitu da proiektuaren formulario nagusian, erabiltzaileak berriak sinkronizatu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="2f353-128">Fixed: When actuals have been updated on a project, a refresh button has been added to the project main form to allow users to re-sync the actuals.</span></span>

    -   <span data-ttu-id="2f353-129">Konponduta: erabiltzaileak 2.X bertsiotik 3.X bertsiora berritzen dutenean, proiektuaren NULL balioa duten proiektuak baimenduko dira.</span><span class="sxs-lookup"><span data-stu-id="2f353-129">Fixed: When users upgrade from 2.X to 3.X, projects with a NULL value for project name will be permitted.</span></span>

