---
title: Project Service Automation eguneratzearen 22, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 22. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
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
ms.openlocfilehash: 456ed68bc1d74c2c8e5d2420a3f5d1fb8e0465d6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126603"
---
# <a name="project-service-automation-update-release-22-v3"></a><span data-ttu-id="afd1f-103">Project Service Automation 22, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="afd1f-103">Project Service Automation Update Release 22, V3</span></span>

<span data-ttu-id="afd1f-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="afd1f-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="afd1f-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="afd1f-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="afd1f-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="afd1f-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="afd1f-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="afd1f-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="afd1f-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="afd1f-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="afd1f-109">Gai honek Project Service Automation V3, 22. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="afd1f-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 22.</span></span> <span data-ttu-id="afd1f-110">Bertsio honen konpilazio-zenbakia V 3.10.33.48 da eta, oro har, 2020ko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="afd1f-110">This version has a build number of V 3.10.33.48 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-22"></a><span data-ttu-id="afd1f-111">22. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="afd1f-111">Update Release 22</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="afd1f-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="afd1f-112">Bug fixes</span></span>



<span data-ttu-id="afd1f-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="afd1f-113">**Time and Expense**</span></span>

<span data-ttu-id="afd1f-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="afd1f-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="afd1f-115">**Denboraren sarrerak** ez dira automatikoki inportatu ondoren Ordua sarreren egutegian gehitzen.</span><span class="sxs-lookup"><span data-stu-id="afd1f-115">**Time entries** are not automatically added in the Time entries schedule after import.</span></span>
- <span data-ttu-id="afd1f-116">**Ordua Sarrera** sareko data hautatzaileak ez ditu erabiltzailearen eskualdeko ezarpenak ezagutzen.</span><span class="sxs-lookup"><span data-stu-id="afd1f-116">The **Time Entry** grid date picker does not recognize a user's regional settings.</span></span>

<span data-ttu-id="afd1f-117">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="afd1f-117">**Resource Management**</span></span>

<span data-ttu-id="afd1f-118">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="afd1f-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="afd1f-119">Eskuzko moduan, aldaketetara **Baliabideen esleipena** sarrerak ez dira ezagutzen sortzen **Baliabide Eskakizunak**.</span><span class="sxs-lookup"><span data-stu-id="afd1f-119">In manual mode, changes to **Resource Assignment** contours are not recognized when generating **Resource Requirements**.</span></span>
- <span data-ttu-id="afd1f-120">**Baliabide eskaerak** ez onartzen eskaera-egoera pertsonalizatuak.</span><span class="sxs-lookup"><span data-stu-id="afd1f-120">**Resource Requests** do not support custom request statuses.</span></span>

<span data-ttu-id="afd1f-121">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="afd1f-121">**Project Management**</span></span>

<span data-ttu-id="afd1f-122">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="afd1f-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="afd1f-123">EstimateGridControl gainean klik bikoitza erabiliz ez duzu holandeseko formatuko zenbakiak behar bezala analizatuko.</span><span class="sxs-lookup"><span data-stu-id="afd1f-123">Using double-click on EstimateGridControl will not correctly parse Dutch format numbers.</span></span>
- <span data-ttu-id="afd1f-124">Esleitutako orduak ez dira behar bezala eguneratzen zereginak Microsoft Project mahaigaineko bezero gehigarria erabiliz aldatzen direnean.</span><span class="sxs-lookup"><span data-stu-id="afd1f-124">Assigned hours do not update correctly when assignments are changed using the Microsoft Project desktop client add-in.</span></span>
- <span data-ttu-id="afd1f-125">Proiektuaren jarraipena eta zenbatespenen sareek salmenta okerraren moneta kodea erakusten dute kontratuaren moneta bezeroaren moneta baino ez denean eta erakundea moneta-kodeak ordez moneta ikurrak bistaratzeko konfiguratuta dago.</span><span class="sxs-lookup"><span data-stu-id="afd1f-125">Project Tracking and Estimates grids display incorrect sales currency code when contract currency is different than customer currency and organization is configured to display currency codes instead of currency symbols.</span></span>
- <span data-ttu-id="afd1f-126">Taldekide batek bukatutako datak egun bat gehituko du laneko ordutegia eguneko 24 ordukoa bada.</span><span class="sxs-lookup"><span data-stu-id="afd1f-126">A Team member's finish date will add one day if the work hour schedule is 24-hours per day.</span></span>
- <span data-ttu-id="afd1f-127">Proiektuen egutegian, zeregin bati Transakzio kategoria gehitzeak ez du auto-aurrezpena aktibatzen.</span><span class="sxs-lookup"><span data-stu-id="afd1f-127">On the Project Schedule, adding a Transaction Category to a task does not trigger auto save.</span></span>
- <span data-ttu-id="afd1f-128">Ondorengo errorea taldekide bat proiektuko txantiloiak gehitzerakoan agertzen da: "Baliabide eskakizunak ezin dira proiektuaren txantiloiekin lotu".</span><span class="sxs-lookup"><span data-stu-id="afd1f-128">The following error is displayed when adding a team member to the Project Template: "Resource requirements cannot be associated with project templates".</span></span> 
- <span data-ttu-id="afd1f-129">Zintaren arau script-ak "msdyn.Approval.CanApproveOrReject" denboraren akatsa bistaratzen du.</span><span class="sxs-lookup"><span data-stu-id="afd1f-129">Ribbon rule script "msdyn.Approval.CanApproveOrReject" displays a timeout error.</span></span>

<span data-ttu-id="afd1f-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="afd1f-130">**Sales**</span></span>

<span data-ttu-id="afd1f-131">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="afd1f-131">The following issues have been fixed:</span></span>

- <span data-ttu-id="afd1f-132">Balidazio-errore mezua ez da agertzen Kostuen Prezio Zerrenda hautatutakoan Prezio Zerrendako bilaketa-proiektuan "Aurrekontu Berrien Proiektuen Prezioen Zerrenda" inprimakian/erakundean.</span><span class="sxs-lookup"><span data-stu-id="afd1f-132">Validation error message not displayed when a Cost Price List is selected in Price List lookup on 'New Quote Project Price List' form/entity.</span></span>
- <span data-ttu-id="afd1f-133">Irabazitako aurrekontua ixteak ez du sortutako kontratura nabigatuko aurrekontuari atxikitako BPF bat azken fasean badago.</span><span class="sxs-lookup"><span data-stu-id="afd1f-133">Closing the quote as won does not navigate to the created contract if a BPF attached to the quote is in the final stage.</span></span>
- <span data-ttu-id="afd1f-134">**Saldu gabeko salmentak** kentzea Denborako sarrera gogorarazten denean kostu originalarekin lotzen da.</span><span class="sxs-lookup"><span data-stu-id="afd1f-134">Reversing **Unbilled Sales** is linked to original cost when a time entry is recalled.</span></span>
- <span data-ttu-id="afd1f-135">Hautatu ondoren **Baieztatu** botoian, fakturaren egoera ez da aldatuko **baieztatu** faktura freskatu ezean.</span><span class="sxs-lookup"><span data-stu-id="afd1f-135">After selecting the **Confirm** button, the invoice status doesn't change to **Confirmed** unless the invoice is refreshed.</span></span>
