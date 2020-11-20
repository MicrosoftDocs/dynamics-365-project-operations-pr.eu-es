---
title: Project Service Automation eguneratzearen 23, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 23. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: 07f1a274914d7e641ddf2fd42f377dce1da7f815
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131103"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="6ffc0-103">Project Service Automation 23, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="6ffc0-103">Project Service Automation Update Release 23, V3</span></span>

<span data-ttu-id="6ffc0-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="6ffc0-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="6ffc0-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="6ffc0-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="6ffc0-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="6ffc0-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="6ffc0-109">Gai honek Project Service Automation V3, 23. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="6ffc0-110">Bertsio honek V3.10.34.30 konpilazio-zenbakia du eta, oro har, 2020ko abuztuan jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="6ffc0-111">23. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="6ffc0-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="6ffc0-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="6ffc0-112">Bug fixes</span></span>

<span data-ttu-id="6ffc0-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="6ffc0-113">**Time and Expense**</span></span>

<span data-ttu-id="6ffc0-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="6ffc0-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="6ffc0-115">Kudeatu ertzeko kasua **Proiektuko talde-kidea ezabatzea** eremuan, salbuespen esanguratsua eskaintzeko.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="6ffc0-116">Esleipenak inportatzean kentzeko pantaila huts bat sortzen da.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="6ffc0-117">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="6ffc0-117">**Resource Management**</span></span>

<span data-ttu-id="6ffc0-118">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="6ffc0-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="6ffc0-119">**Baliabideen erabilera-saretaren baliabide-txartela** eremuak datu okerrak erakusten ditu denbora-eskala bost egunetik gorakoa denean.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="6ffc0-120">Bezeroek erreserbatzeko baliabide bat sortzen dutenean, pluginak tarteka huts egiten du baliabidea automatikoki Microsoft Office 365 talde batean gehitzerakoan.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="6ffc0-121">**Adiskidetzea** ikuspegiak eskuzko ingeradak gaizki erakusten ditu **Astea** edo **Hilabetea** ikuspegian.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="6ffc0-122">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="6ffc0-122">**Project Management**</span></span>

<span data-ttu-id="6ffc0-123">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="6ffc0-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="6ffc0-124">**RetrieveMultiple for usersettings** entitate kopuru gehiegizkoak errendimendu okerra eragiten ari dira proiektuen onarpenetarako eta bestelako eragiketetarako.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="6ffc0-125">**Zereginen plangintza** saretaren baliabideen bilaketa proiektu-taldeko bost talde-kideri erakustera mugatuta dago.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="6ffc0-126">**Zereginen plangintza** saretaren baliabideen bilaketak ez du iragazten baliabide inaktiborik.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="6ffc0-127">Eskuzko moduak ez du espero bezala funtzionatzen zereginen xehetasunen egituraren plangintzaren proiektuan.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="6ffc0-128">**Zereginen plangintza** saretak **Transakzio inaktiboen kategoriak** erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="6ffc0-129">**Baliabideen esleipena** saretak gaizki biribiltzen du zeregin batek hainbat zeregin dituenean.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="6ffc0-130">Biribiltzeko balioak planifikatutako kostuaren eta benetako kostuaren artean desberdinak dira zeregin bakar baterako.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="6ffc0-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="6ffc0-131">**Sales**</span></span>

<span data-ttu-id="6ffc0-132">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="6ffc0-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="6ffc0-133">**Eskuratu transakzio kategoria guztiak** bi aldiz sakatuta lerro anitz sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="6ffc0-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>
