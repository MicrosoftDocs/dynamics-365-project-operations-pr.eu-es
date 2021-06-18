---
title: Project Service Automation eguneratzearen 24, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 24. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c95a9dcada4fbf6c462df29d450aaafab4e73aa5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000241"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="32705-103">Project Service Automation 24, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="32705-103">Project Service Automation Update Release 24, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="32705-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="32705-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="32705-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="32705-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="32705-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="32705-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="32705-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="32705-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="32705-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="32705-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="32705-109">Gai honek Project Service Automation V3, 24. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="32705-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="32705-110">Bertsio honek V3.10.42.43 konpilazio-zenbakia du eta, oro har, 2020ko urrian jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="32705-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="32705-111">24. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="32705-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="32705-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="32705-112">Bug fixes</span></span>

<span data-ttu-id="32705-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="32705-113">**Sales**</span></span>

<span data-ttu-id="32705-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="32705-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="32705-115">Arazoa produktuen prezio-zerrenda lehenetsia ezartzean.</span><span class="sxs-lookup"><span data-stu-id="32705-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="32705-116">Eskaintza irabaztearen errendimendua motela da txertatutako prezioen zerrenda eta funtzio-prezioen erregistroen kopia dela-eta.</span><span class="sxs-lookup"><span data-stu-id="32705-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="32705-117">**Proiektuaren kontratua/Salmenten atala** > **Produktu-lerroaren elementua / Eskaera-lerroaren kantitatea** automatikoki biribiltzen da hurbilen dagoen zenbaki osora.</span><span class="sxs-lookup"><span data-stu-id="32705-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="32705-118">Igo sistemaren pribilegioak prezio-zerrendak irakurtzean.</span><span class="sxs-lookup"><span data-stu-id="32705-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="32705-119">Kopiatu bezeroaren **address1_freighttermscode** eta **address1_shippingmethodcode** helbide-eremuak Eskaintza/Eskaera eremuetan.</span><span class="sxs-lookup"><span data-stu-id="32705-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="32705-120">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="32705-120">**Time and Expense**</span></span>

<span data-ttu-id="32705-121">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="32705-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="32705-122">**Denbora sartzeko sareta** eremuak ez du onartzen **Data soilik** denboraren portaera.</span><span class="sxs-lookup"><span data-stu-id="32705-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="32705-123">**Denboraren sarrera** ez da automatikoki freskatzen.</span><span class="sxs-lookup"><span data-stu-id="32705-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="32705-124">Eskuz freskatu behar da.</span><span class="sxs-lookup"><span data-stu-id="32705-124">A manual refresh is required.</span></span>
- <span data-ttu-id="32705-125">Ezin dira inportatu esleipen bateko denbora-sarrerak baliabidearen esleipenetako etenaldi bat (0 ordu) dagoenean.</span><span class="sxs-lookup"><span data-stu-id="32705-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="32705-126">Denbora-sarrera bat sortzerakoan, ezarri hasiera **msdyn_date** gisa.</span><span class="sxs-lookup"><span data-stu-id="32705-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="32705-127">Gaitu berriro denbora-sarreraren edizio masiboa.</span><span class="sxs-lookup"><span data-stu-id="32705-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="32705-128">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="32705-128">**Resource Management**</span></span>

<span data-ttu-id="32705-129">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="32705-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="32705-130">Eskakizunik ez duen egun barneko erreserba baten egoera eguneratzen saiatzean null-ref salbuespena agertuko da.</span><span class="sxs-lookup"><span data-stu-id="32705-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="32705-131">Errorea **Adiskidetzearen ikuspegia** kargatzean.</span><span class="sxs-lookup"><span data-stu-id="32705-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="32705-132">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="32705-132">**Project Management**</span></span>

<span data-ttu-id="32705-133">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="32705-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="32705-134">**Proiektuaren antolaketa** eremuan, **Eskuzkoa** aukera **Automatikoa** aldatzean, automatikoki gordetzea ez da osatzen.</span><span class="sxs-lookup"><span data-stu-id="32705-134">In the **Project Schedule**, when changing from **Manual** to **Auto**, auto save is not completing.</span></span>
- <span data-ttu-id="32705-135">Gastuen kostuak ez dira kalkulatu behar **Proiektuaren jarraipen-sareta** eremuaren bariantzan.</span><span class="sxs-lookup"><span data-stu-id="32705-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="32705-136">**Aurreikuspenen etiketa** zutabeen portaera ez da koherentea kargatzean, **Denbora-fasea** mota aldatzean.</span><span class="sxs-lookup"><span data-stu-id="32705-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="32705-137">Baliteke proiektuaren benetako kostuak ez islatzea **Benetako datuak** aukeraren guztizkoak.</span><span class="sxs-lookup"><span data-stu-id="32705-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="32705-138">**Aurreikuspeneko amaiera-data** aukera, **Laburpena** fitxakoa, ez dator bat **WBS antolaketa** aukerakoarekin.</span><span class="sxs-lookup"><span data-stu-id="32705-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="32705-139">Koska kentzeko **Eguneratu benetako orduak** eremuak ez du ongi funtzionatzen.</span><span class="sxs-lookup"><span data-stu-id="32705-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="32705-140">**BU** erroak ez du sortu proiektu baten kanpoko Proiektu-kudeatzailea.</span><span class="sxs-lookup"><span data-stu-id="32705-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="32705-141">**Gastuen aurreikuspenak** eremuko zereginean edo kategorian egindako aldaketak ez dira iraun.</span><span class="sxs-lookup"><span data-stu-id="32705-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="32705-142">**Kontratuaren kopia** eremuak fakturen antolaketak kopiatzen ditu eta egoera exekutatzen du.</span><span class="sxs-lookup"><span data-stu-id="32705-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="32705-143">**Freskatu benetako datuak** botoiak gaizki kalkulatzen ditu laburpen-zereginak.</span><span class="sxs-lookup"><span data-stu-id="32705-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="32705-144">Microsoft Project Add-in: konpondu erreferentzia-errore hutsa talde-kideren batek baliabide-unitate huts bat baldin badu.</span><span class="sxs-lookup"><span data-stu-id="32705-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]