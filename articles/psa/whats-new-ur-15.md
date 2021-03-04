---
title: Project Service Automation eguneratzearen 15, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation eguneratzea 15, V3 bertsioko berritasunei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/27/2020
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
ms.openlocfilehash: 0ec6746c0d3a1a03ee56440c73d044df844046f8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143948"
---
# <a name="project-service-automation-update-release-15-v3"></a><span data-ttu-id="ef742-103">Project Service Automation 15, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="ef742-103">Project Service Automation Update Release 15, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="ef742-104">Atsegin handiz adierazten dugu Dynamics 365 Project Service Automation (PSA) aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="ef742-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="ef742-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="ef742-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="ef742-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="ef742-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="ef742-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroa eta joan soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="ef742-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="ef742-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="ef742-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="ef742-109">Gai honek PSA V3, 15. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="ef742-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 15.</span></span> <span data-ttu-id="ef742-110">Bertsio honek V3.10.5.28 konpilazio-zenbakia du eta, oro har, 2020ko urtarrilean jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="ef742-110">This version has a build number of V3.10.5.28 and is generally available through a self-update in January 2020.</span></span>

## <a name="update-release-15"></a><span data-ttu-id="ef742-111">15. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="ef742-111">Update Release 15</span></span> 

### <a name="enhancements"></a><span data-ttu-id="ef742-112">Hobekuntzak</span><span class="sxs-lookup"><span data-stu-id="ef742-112">Enhancements</span></span>

- <span data-ttu-id="ef742-113">Proiektuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="ef742-113">Project Management</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="ef742-114">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="ef742-114">Bug fixes</span></span>

- <span data-ttu-id="ef742-115">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="ef742-115">Time and Expense</span></span>

  - <span data-ttu-id="ef742-116">Konponduta: karga-erroreen kudeaketa gehitu da bateratze-ikuspegian.</span><span class="sxs-lookup"><span data-stu-id="ef742-116">Fixed: Add on-load error handling in the reconciliation view.</span></span>
  - <span data-ttu-id="ef742-117">Konponduta: Proiektuaren baliabide-gunea: **Zenbatekoa** berrizendatu da anbiguotasuna gutxitzeko.</span><span class="sxs-lookup"><span data-stu-id="ef742-117">Fixed: Project Resource Hub: Rename **Amount** to reduce ambiguity.</span></span>
  - <span data-ttu-id="ef742-118">Konponduta: **Kopiatu ordu-sarreren zutabeak** ikuspegia doitu da, mota barneratzeko.</span><span class="sxs-lookup"><span data-stu-id="ef742-118">Fixed: Adjust the view **Copy Time Entry Columns** to include the type.</span></span>
  - <span data-ttu-id="ef742-119">Konponduta: sareta-ikuspegian denbora-sarreraren iraupena zenbaki hamartarren emaitzekin editatzean, errore ezezaguna sortzea zenbait zenbakirekin.</span><span class="sxs-lookup"><span data-stu-id="ef742-119">Fixed: Editing time entry duration in the grid view using decimal numbers results in unknown error for some numbers.</span></span>

- <span data-ttu-id="ef742-120">Proiektuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="ef742-120">Project Management</span></span>

  - <span data-ttu-id="ef742-121">Konponduta: **Erabili Jarraipen-ikuspegian** goitibeherako menua aukeren zabaleran oinarrituta hedatzen da orain.</span><span class="sxs-lookup"><span data-stu-id="ef742-121">Fixed: The drop-down menu for **Use in Tracking View** now expands based on the width of the options.</span></span>
  - <span data-ttu-id="ef742-122">Konponduta: +13 ordu-eremutako baino gehiagotako proiektuak kudeatzean, zereginen kalkuluek emaitza okerrak bistara ditzakete.</span><span class="sxs-lookup"><span data-stu-id="ef742-122">Fixed: When managing projects in the +13 time zone, tasks calculations can display inaccurate results.</span></span>
  - <span data-ttu-id="ef742-123">Konponduta: **Taldekideen amaiera-ordua** zuzendu da 24 orduko egutegia erabiltzean.</span><span class="sxs-lookup"><span data-stu-id="ef742-123">Fixed: **Team Member End Time** has been corrected when using a 24-hour calendar.</span></span>
  - <span data-ttu-id="ef742-124">Konponduta: Berriro aktibatu da **BPF** **msdyn_project** inprimaki nagusian.</span><span class="sxs-lookup"><span data-stu-id="ef742-124">Fixed: Re-activated the **BPF** in **msdyn_project** main form.</span></span>
  - <span data-ttu-id="ef742-125">Konponduta: Esleipenen kalkuluak ez du egun bat baztertzen.</span><span class="sxs-lookup"><span data-stu-id="ef742-125">Fixed: Assignments calculation no longer ignores one day.</span></span>
  - <span data-ttu-id="ef742-126">Konponduta: jakinarazpen iragankor berri bat gehitu da proiektuaren inprimakian, erabiltzailearen eta proiektuaren ordu-eremuak desberdinak direnean.</span><span class="sxs-lookup"><span data-stu-id="ef742-126">Fixed: A new notification banner has been added to the project form when the time zone differs between user and project.</span></span>

- <span data-ttu-id="ef742-127">Sales</span><span class="sxs-lookup"><span data-stu-id="ef742-127">Sales</span></span>

  - <span data-ttu-id="ef742-128">Konponduta: Gutxi gorabeherako gastuen kategorien bilaketa erabil daiteke bikoiztuak iragazteko.</span><span class="sxs-lookup"><span data-stu-id="ef742-128">Fixed: Expense estimate category lookup can be used to filter duplicates.</span></span>
  - <span data-ttu-id="ef742-129">Konponduta: **PluginDomain.ExecuteInTryCatchBlock(..)** eremuko kodeak ez du ezkutatzen jada salbuespenaren jatorria.</span><span class="sxs-lookup"><span data-stu-id="ef742-129">Fixed: Code in **PluginDomain.ExecuteInTryCatchBlock(..)** no longer hides the origin of the exception.</span></span>
  - <span data-ttu-id="ef742-130">Konponduta: Ez duzu errore-mezurik jasoko **Proiektuaren bilaketa** eremuan **Eskaintzaren lerroa** inprimakian, 1000 proiektu baino gehiago daudenean.</span><span class="sxs-lookup"><span data-stu-id="ef742-130">Fixed: No longer get an error message in **Project lookup** in the **Quote Line** form when there are more than 1000 projects.</span></span>
  - <span data-ttu-id="ef742-131">Konponduta: gutxi gorabeherako lanen eta gutxi gorabeherako gastuen **Gutxi gorabeherakoak** saretak moneta-ikur zuzena bistaratzen du.</span><span class="sxs-lookup"><span data-stu-id="ef742-131">Fixed: **Estimates** grid for labor estimates and expense estimates now displays the correct currency symbol.</span></span>
  - <span data-ttu-id="ef742-132">Konponduta: Erakunde batek PSA 14. eguneratze-bertsiotik 15. eguneratze-bertsiora eguneratu ondoren, **Antolaketa** fitxa ez da agertuko hutsik **Proiektua** inprimakian.</span><span class="sxs-lookup"><span data-stu-id="ef742-132">Fixed: After an organization updates PSA from Update Release 14 to Update Release 15, the **Schedule** tab no longer appears as blank on the **Project** form.</span></span>
