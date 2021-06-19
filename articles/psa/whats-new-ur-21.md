---
title: Project Service Automation eguneratzearen 21, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 21. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: dd894f27baac70238d0bd9e9b1a21a9a499e1ea7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002312"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="ff2cd-103">Project Service Automation 21, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="ff2cd-103">Project Service Automation Update Release 21, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="ff2cd-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="ff2cd-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="ff2cd-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="ff2cd-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="ff2cd-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="ff2cd-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="ff2cd-109">Gai honek Project Service Automation V3, 21. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="ff2cd-110">Bertsio honen konpilazio-zenbakia V 3.10.32.50 da eta, oro har, 2020ko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="ff2cd-111">21. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="ff2cd-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="ff2cd-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="ff2cd-112">Bug fixes</span></span>

<span data-ttu-id="ff2cd-113">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="ff2cd-113">**Time and Expense**</span></span>

<span data-ttu-id="ff2cd-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="ff2cd-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="ff2cd-115">Biltegiratzean **Ordua sartzeko saretaren kontrola** Arbeletan, sareak ez du arbelaren sarearen edukiontziaren zabalera osoa.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="ff2cd-116">Ordu-zona zehatzetarako, **Ordua Sarrera** sareta kontrolak ez ditu erregistroak bistaratzen.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="ff2cd-117">Gaueko 21:00ak baino lehenagoko ordu sarrerak gaizki agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="ff2cd-118">Erabiltzaileak ezin dira gastuak bidali gastu kategoria bada, **Gastuen ordainagiria beharrezkoa da** ez du baliorik.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="ff2cd-119">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="ff2cd-119">**Resource Management**</span></span>

<span data-ttu-id="ff2cd-120">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="ff2cd-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="ff2cd-121">Erreserbak aktibo daude **Adiskidetzea** ikusteko.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="ff2cd-122">Baliabideen betetze generikoa falta zen balioztapena erreserbatzeko egoera baliozkoa dela ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="ff2cd-123">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="ff2cd-123">**Project Management**</span></span>

<span data-ttu-id="ff2cd-124">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="ff2cd-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="ff2cd-125">**Proiektua** eratutako sareta (**Baliabideen esleipena**, **Zeregin**, **Adiskidetzea** ikuspegia, **Gastuen kalkuluak**) jarraitu editagarriak, proiektu bat aktibo ez dagoenean ere.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-125">The **Project** form grids (**Resource Assignment**, **Task**, **Reconciliation** view, **Expense Estimates**) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="ff2cd-126">Bezero bikoiztuak ezin dira berretsi proiektuaren kontratuei lotuta dauden bezeroekin.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="ff2cd-127">Baliozko egutegirik ez duen baliabidea gehitzen denean, sistemak ez du erabiltzaileen errore-mezurik itzultzen.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="ff2cd-128">**Gehitu Ataza** Zereginen saretako botoian gaituta dago proiektua lotuta dagoenean **Microsoft Project gehigarria**.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="ff2cd-129">Ahalegina kontrolik gabe hazten da kategoria bateko zereginak kostu prezioa definituta daukan zereginarekin.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="ff2cd-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="ff2cd-130">**Sales**</span></span>

<span data-ttu-id="ff2cd-131">Hobekuntza hauek egin dira:</span><span class="sxs-lookup"><span data-stu-id="ff2cd-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="ff2cd-132">**Fakturen maiztasuna** eta **Fakturazio hasiera** aldatu dira **Fakturen egutegia** fitxa.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="ff2cd-133">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="ff2cd-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="ff2cd-134">**Salmenta prezioa, guztira** zero da (0) **Kategoria** nahiz eta **Funtzioa** zero ez den salmenta prezioa du.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="ff2cd-135">Bezeroek ezin dute aldatu balioa **Fakturaren egoera** eremua **Fakturatzeko prest** Neurrira egindako beste prozesu bat eremu gehigarri bat eguneratzen denean.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="ff2cd-136">**Eguneratu faktura-ildoak** botoiak bikoiztu lerro bat baino gehiago sor ditzake behin eta berriz hautatzen bada.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="ff2cd-137">**Eguneratu Prezioak** botoiak ez du funtzionatzen **Funtzioaren prezioak** azpisarea **Ikuspegi azkarra** forma.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-137">The **Update Prices** button doesn't work on the **Role Prices** subgrid in the **Quick View** form.</span></span>
- <span data-ttu-id="ff2cd-138">**Salmenta prezioen zerrenda ebaztea** logikak gaizki kudeatzen ditu ordu-zonak, prezioen zerrenden aukeraketa okerra sortuz.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="ff2cd-139">Proiektu batena **Benetako kostu totala** Zatiki kopuru bat desgaitu daiteke, sarrera bakar bat onartu ondoren.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="ff2cd-140">**Prezioen Ebazpena** logikak ez du erabilgarritasun errorerik ematen **Berreskuratutako RolePrice** ez du balorean **"Lehen Unitatea"** eta **"Prezioa Lehen Unitatean"** eremuak.</span><span class="sxs-lookup"><span data-stu-id="ff2cd-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]