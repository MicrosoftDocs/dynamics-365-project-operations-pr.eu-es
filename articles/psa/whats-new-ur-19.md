---
title: Project Service Automation eguneratzearen 19, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 19. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: ecc923cccfad21985025ab9d8006aaff16afc25f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070989"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="b7c58-103">Project Service Automation 19, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="b7c58-103">Project Service Automation Update Release 19, V3</span></span>

<span data-ttu-id="b7c58-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="b7c58-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b7c58-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="b7c58-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b7c58-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="b7c58-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b7c58-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="b7c58-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="b7c58-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="b7c58-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b7c58-109">Gai honek PSA V3, 19. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="b7c58-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="b7c58-110">Bertsio honen konpilazio-zenbakia V3.10.30.41 da eta, oro har, 2020ko maiatzeko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="b7c58-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="b7c58-111">19. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="b7c58-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b7c58-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="b7c58-112">Bug fixes</span></span>

<span data-ttu-id="b7c58-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="b7c58-113">**Time and Expense**</span></span>

<span data-ttu-id="b7c58-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="b7c58-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="b7c58-115">Denbora-sarrerak ongi ez agertzetik eratorritako akatsak.</span><span class="sxs-lookup"><span data-stu-id="b7c58-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="b7c58-116">Denbora-sarreren saretak ez du onartzen **Data soilik** eremuko portaera.</span><span class="sxs-lookup"><span data-stu-id="b7c58-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="b7c58-117">Project Resources ez dago erabilgarri, proiektu baten gastua sortzeko.</span><span class="sxs-lookup"><span data-stu-id="b7c58-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="b7c58-118">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="b7c58-118">**Project Management**</span></span>

<span data-ttu-id="b7c58-119">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="b7c58-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="b7c58-120">Hirugarren mailako zereginek gutxi gorabeherako ahalegin okerra eragiten du Osatzea (EAC) kalkulatzeko garaian.</span><span class="sxs-lookup"><span data-stu-id="b7c58-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="b7c58-121">**Sales**</span><span class="sxs-lookup"><span data-stu-id="b7c58-121">**Sales**</span></span>

<span data-ttu-id="b7c58-122">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="b7c58-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="b7c58-123">**Birkalkulatu** ekintzak ez du funtzionatzen gastuen kontratuaren lerroko xehetasunekin edo eskaintzaren lerroko xehetasunekin.</span><span class="sxs-lookup"><span data-stu-id="b7c58-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="b7c58-124">**Eguneratu prezioak** falta da gutxi gorabeherako gastuetan.</span><span class="sxs-lookup"><span data-stu-id="b7c58-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="b7c58-125">Bezeroek ezin dute hautatu kontratuaren egoeraren arrazoi pertsonalizatua **Proiektuaren kontratua** orrian.</span><span class="sxs-lookup"><span data-stu-id="b7c58-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="b7c58-126">Bezeroek errendimendu degradatua izaten dute eskaintza batetik prezio-zerrenda pertsonalizatua sortzean.</span><span class="sxs-lookup"><span data-stu-id="b7c58-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="b7c58-127">Bezeroek inkoherentziak dituzte lehenetsitako **unitateekin** **Eskaintzaren lerroko xehetasunak** eta **Kontratuaren lerroko xehetasunak** orrietan.</span><span class="sxs-lookup"><span data-stu-id="b7c58-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="b7c58-128">Egotz ezin daitekeen transakzioen kategoriako elementuak egotz daitekeen kontratuaren lerro batean gehitzeak ez du errespetatuko transakzio kategoriako **Egotz ezin daitekeena** fakturazio mota.</span><span class="sxs-lookup"><span data-stu-id="b7c58-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="b7c58-129">Bezeroek ezin dituzte erabili gehitu berri diren funtzioak eta kategoriak aurrez sortutako kontratuetan.</span><span class="sxs-lookup"><span data-stu-id="b7c58-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="b7c58-130">Bezeroek errendimendu degradatua izaten dute Ezinbesteko berreskuratzea PreValidateProjectTeamMemberUpdate.cs-en</span><span class="sxs-lookup"><span data-stu-id="b7c58-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="b7c58-131">**Baliabideen kategoriak** zerrendan egotz ezin daitezkeen funtzio gisa konfiguratutako funtzioak **Funtzio egozgarriak** fitxan gehituko dira **Egotz ezin daitezkeenak** gisa proiektuaren kontratuaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="b7c58-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="b7c58-132">Bezeroek errendimendu degradatua izan dezakete proiektu bat sortzerakoan **GetBookableResourceIdFromUser** parametroak baliabide erreserbagarrien zutabe guztiak berreskuratzen dituelako ID nagusia bakarrik berreskuratu beharrean.</span><span class="sxs-lookup"><span data-stu-id="b7c58-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="b7c58-133">**TransactionType** entitateari aurre-balioztatzea eguneratzeko plugina falta zaio, erabiltzaileak transakzio motetarako baliozkoak ez diren **Unitateak** eta **UnitGroups** transakzio motetan ez sartzeko.</span><span class="sxs-lookup"><span data-stu-id="b7c58-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="b7c58-134">**Kendu** urratsak ez du funtzionatzen denbora-sarreren inportaziorako.</span><span class="sxs-lookup"><span data-stu-id="b7c58-134">The **Remove** step does not work for time entry import.</span></span>
