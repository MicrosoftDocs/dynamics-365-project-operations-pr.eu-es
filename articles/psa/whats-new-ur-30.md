---
title: Project Service Automation eguneratzearen 30, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 30. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 3b6b7dba9c2a22587d27006b9972c950fbb454f2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010411"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="1edef-103">Project Service Automation eguneratzearen 30, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="1edef-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="1edef-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="1edef-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="1edef-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="1edef-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="1edef-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="1edef-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="1edef-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="1edef-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="1edef-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution.md).</span><span class="sxs-lookup"><span data-stu-id="1edef-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="1edef-109">Gai honek Project Service Automation V3, 30. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="1edef-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="1edef-110">Bertsio honen konpilazio-zenbakia V3.10.51.61 da eta, oro har, 2021eko apirileko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="1edef-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="1edef-111">30. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="1edef-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="1edef-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="1edef-112">Bug fixes</span></span>

<span data-ttu-id="1edef-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="1edef-113">**Time and Expense**</span></span>

<span data-ttu-id="1edef-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="1edef-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="1edef-115">Errorea gertatzen da denbora - sarrera sortu eta gordetzen duzunean **Sortu bizkor** orrialdea bada **Rola** eremua kendu da.</span><span class="sxs-lookup"><span data-stu-id="1edef-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="1edef-116">Denbora sartzeko iragazkiak iragazki eragile okerra aplikatzen du.</span><span class="sxs-lookup"><span data-stu-id="1edef-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="1edef-117">Kopiatutako denbora-orriak ez dira automatikoki bistaratzen hautatzen duzunean **Kopiatu Astea** denbora sartzeko kontrolean.</span><span class="sxs-lookup"><span data-stu-id="1edef-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="1edef-118">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="1edef-118">**Resource Management**</span></span>

<span data-ttu-id="1edef-119">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="1edef-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="1edef-120">Erreserba luzatzen duzunean, erreserba gogorrari esleitutako erreserba egoera ez da zuzena.</span><span class="sxs-lookup"><span data-stu-id="1edef-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="1edef-121">Erreserba luzatzeak errespetatutako egoera errespetatzen du **Konprometituta** erreserba konfiguratzeko metadatuetan.</span><span class="sxs-lookup"><span data-stu-id="1edef-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="1edef-122">Baliozko erreserba-egoera zehazten ez denean, errore-mezua ez dago behar bezala lokalizatuta.</span><span class="sxs-lookup"><span data-stu-id="1edef-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="1edef-123">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="1edef-123">**Project Management**</span></span>

<span data-ttu-id="1edef-124">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="1edef-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="1edef-125">Proiektuak ezin dira moneta batean sortu eta erlazionatutako lanak beste moneta batean sartzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="1edef-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="1edef-126">**Salmentak**</span><span class="sxs-lookup"><span data-stu-id="1edef-126">**Sales**</span></span>

<span data-ttu-id="1edef-127">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="1edef-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="1edef-128">Prezio zerrenda kopiatzen denean, prezioak ez dira eguneratzen.</span><span class="sxs-lookup"><span data-stu-id="1edef-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="1edef-129">Aurrekontua irabazi gisa ixteak huts egiten du kostuaren xehetasunak jatorrizko balioa duenean.</span><span class="sxs-lookup"><span data-stu-id="1edef-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="1edef-130">**Proiektuaren zeregina** entitatean, **Aurreikusitako kostua** izena aldatu zaio **Aurreikusitako kostua (oinarria)**.</span><span class="sxs-lookup"><span data-stu-id="1edef-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="1edef-131">Fakturak sortu edo ezabatzen direnean erreferentziazko salbuespen nulua sortzen da.</span><span class="sxs-lookup"><span data-stu-id="1edef-131">A null reference exception is generated when invoices are created or deleted.</span></span>
