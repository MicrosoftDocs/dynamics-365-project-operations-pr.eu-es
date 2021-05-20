---
title: Project Service Automation eguneratzearen 26, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 26. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: 669b3ca4601bdac483db4e1d7f55a8bf5b3d9661
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948809"
---
# <a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="8052d-103">Project Service Automation 26, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="8052d-103">Project Service Automation Update Release 26, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="8052d-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="8052d-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="8052d-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="8052d-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="8052d-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="8052d-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="8052d-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="8052d-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="8052d-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="8052d-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="8052d-109">Gai honek Project Service Automation 26, V3 eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="8052d-109">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="8052d-110">Bertsio honek V3.10.44.59 zenbakia du eta orokorrean eskuragarri dago 2020ko abenduan auto-eguneratze baten bidez.</span><span class="sxs-lookup"><span data-stu-id="8052d-110">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

## <a name="update-release-26"></a><span data-ttu-id="8052d-111">26. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="8052d-111">Update Release 26</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="8052d-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="8052d-112">Bug fixes</span></span>

<span data-ttu-id="8052d-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="8052d-113">**Time and Expense**</span></span>

<span data-ttu-id="8052d-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="8052d-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="8052d-115">Erabiltzaileek zeregina aldatu edo bidali duten denbora-sarrera batean alda dezakete.</span><span class="sxs-lookup"><span data-stu-id="8052d-115">Users are able to change the task on a time entry that has been approved/submitted.</span></span>
- <span data-ttu-id="8052d-116">"Objektuaren erreferentzia ez da ezarri" errorea denbora sarrera gordetzean.</span><span class="sxs-lookup"><span data-stu-id="8052d-116">"Object Reference Not Set" error when saving time entry.</span></span>
- <span data-ttu-id="8052d-117">Baliabideen esleipenetatik ordu sarrera inportatzeak denbora sarrera sortzen du okerreko Data eta Balioekin.</span><span class="sxs-lookup"><span data-stu-id="8052d-117">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>
- <span data-ttu-id="8052d-118">Project Service Automation eta Field Service aplikazioa instalatuta daudenean, **Berria** botoia birritan bistaratzen ari da komando-barran Field Service aplikazioan denbora sartzeko.</span><span class="sxs-lookup"><span data-stu-id="8052d-118">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>
- <span data-ttu-id="8052d-119">**Baimendu Unitatea** eta **Unitatea taldea** gelaxken eguneratzeak **Gastuen kalkuluak** saretan.</span><span class="sxs-lookup"><span data-stu-id="8052d-119">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>
- <span data-ttu-id="8052d-120">**Eguneratu denbora sarrera editatu** inprimakia barne **Denbora-lerroa**.</span><span class="sxs-lookup"><span data-stu-id="8052d-120">**Update Time Entry Edit** form includes **Timeline**.</span></span>
- <span data-ttu-id="8052d-121">Proiektuak ez diren denbora-sarreretarako denbora onartzeak sistema blokeatzen du proiektuak onartzeko eginkizuna bilatzean.</span><span class="sxs-lookup"><span data-stu-id="8052d-121">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="8052d-122">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="8052d-122">**Resource Management**</span></span>

<span data-ttu-id="8052d-123">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="8052d-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="8052d-124">Fitxategian baliozkotzea gehitu da **PostProjectCreate** plugina, lehen sortu behar den baldintza bat egiaztatzeko.</span><span class="sxs-lookup"><span data-stu-id="8052d-124">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>
- <span data-ttu-id="8052d-125">**Proiektu Taldeko kidea** azkar sortzeko inprimakiak erreferentzia nuluko salbuespena sortzen du eremuak inprimakitik kentzen badira.</span><span class="sxs-lookup"><span data-stu-id="8052d-125">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>
- <span data-ttu-id="8052d-126">Sortu urtebetean 12 orduz eskakizunak huts egingo du.</span><span class="sxs-lookup"><span data-stu-id="8052d-126">Generate requirements for 12 hours over 1 year will fail.</span></span>
- <span data-ttu-id="8052d-127">Errore-mezuaren erreferentzia nuluko salbuespena hobetu da baliabide-eskakizunak sortzean.</span><span class="sxs-lookup"><span data-stu-id="8052d-127">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="8052d-128">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="8052d-128">**Project Management**</span></span>

<span data-ttu-id="8052d-129">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="8052d-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="8052d-130">Fitxategian sortutako erreferentzia nuluen salbuespenari aurre egiteko baliozkotzea hobetu da **Aurreproiektuaren eguneratzea** plugina.</span><span class="sxs-lookup"><span data-stu-id="8052d-130">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>
- <span data-ttu-id="8052d-131">Microsoft Project mahaigaineko gehigarriak argitaratutako proiektuek esleitu gabeko lanak ezabatzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="8052d-131">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>
- <span data-ttu-id="8052d-132">Hemen gehitu da baliozkotze berria zeregin baten proiektuaren erreferentzia baliogabea denean erreferentzia nuluko salbuespenagatik **PreValidateProjectTaskUpdate** plugina.</span><span class="sxs-lookup"><span data-stu-id="8052d-132">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>
- <span data-ttu-id="8052d-133">Taldekideen saretak ez ditu zeregin desberdinak erakusten taldekideen erregistroan.</span><span class="sxs-lookup"><span data-stu-id="8052d-133">Team Member grid does not show distinct assignments on the team member record.</span></span>
- <span data-ttu-id="8052d-134">Hemen gehitu dira baliozkotze eta errore mezu berriak erreferentzia nuluko salbuespenagatik **PreProjectTaskDelete** plugina.</span><span class="sxs-lookup"><span data-stu-id="8052d-134">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="8052d-135">**Sales**</span><span class="sxs-lookup"><span data-stu-id="8052d-135">**Sales**</span></span>

<span data-ttu-id="8052d-136">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="8052d-136">The following issues have been fixed:</span></span>

- <span data-ttu-id="8052d-137">Aurrekontuan edo kontratuan proiektuan oinarritutako lerro bat hautatzerakoan **Iradokizuna** botoiak lehendik dagoen produktu batekin lotutako produktuan oinarritutako linea hautatzerakoan soilik egon behar du ikusgai.</span><span class="sxs-lookup"><span data-stu-id="8052d-137">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>
- <span data-ttu-id="8052d-138">Zatitu **Sortu_Product** pribilegioa **Create_ProjectContract** pribilegiotik.</span><span class="sxs-lookup"><span data-stu-id="8052d-138">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>
- <span data-ttu-id="8052d-139">Faktura lerro bat ezabatzeak erreferentzia huts hutsa eragiten du **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="8052d-139">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]