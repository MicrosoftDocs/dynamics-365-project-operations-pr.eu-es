---
title: Project Service Automation eguneratzearen 25, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 25. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 92dd74378457cf877e8ec26eb85a7883dda97d51
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000196"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a><span data-ttu-id="4acbb-103">Project Service Automation eguneratzearen 25, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="4acbb-103">What's new or changed in Project Service Automation Update Release 25, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="4acbb-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="4acbb-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="4acbb-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="4acbb-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="4acbb-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="4acbb-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="4acbb-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="4acbb-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="4acbb-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="4acbb-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="4acbb-109">Gai honek Project Service Automation V3 bertsio berrirako edo aldatutako ezaugarriak eta konponketak zerrendatzen ditu 25 bertsioa eguneratzea. Bertsio honek V 3.10.43.76 eraikuntza kopurua du eta, oro har, 2020ko urrian eguneratze automatikoaren bidez eskuragarri dago.</span><span class="sxs-lookup"><span data-stu-id="4acbb-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 25 This version has a build number of V 3.10.43.76 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-25"></a><span data-ttu-id="4acbb-110">25. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="4acbb-110">Update Release 25</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="4acbb-111">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="4acbb-111">Bug fixes</span></span>

<span data-ttu-id="4acbb-112">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="4acbb-112">**Time and Expense**</span></span>

<span data-ttu-id="4acbb-113">Arazo hau konpondu da:</span><span class="sxs-lookup"><span data-stu-id="4acbb-113">The following issue has been fixed:</span></span>

- <span data-ttu-id="4acbb-114">Lortutako tarte handiegia oinarritzat hartuta datu osagarriak erakusten dituen denbora sartzeko taula.</span><span class="sxs-lookup"><span data-stu-id="4acbb-114">Time entry chart showing additional data based on too large of an interval being retrieved.</span></span>

<span data-ttu-id="4acbb-115">**Baliabideen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="4acbb-115">**Resource Management**</span></span>

<span data-ttu-id="4acbb-116">Arazo hau konpondu da:</span><span class="sxs-lookup"><span data-stu-id="4acbb-116">The following issue has been fixed:</span></span>

- <span data-ttu-id="4acbb-117">Package Deployer-en kodea gehitu da Universal Resource Scheduling adabakien inportazioa bertsio altuagoa badago dagoeneko.</span><span class="sxs-lookup"><span data-stu-id="4acbb-117">Added package deployer code to skip the Universal Resource Scheduling patch import if a higher version patch already exists.</span></span>

<span data-ttu-id="4acbb-118">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="4acbb-118">**Project Management**</span></span>

<span data-ttu-id="4acbb-119">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="4acbb-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="4acbb-120">Biribiltze eta truke-tasaren desadostasunak zuzendu dira, proiektuaren jarraipen-sarean planifikatutako kostu okerrak sortuz.</span><span class="sxs-lookup"><span data-stu-id="4acbb-120">Corrected rounding and exchange rate discrepancies resulting in incorrect planned cost in the project tracking grid.</span></span>
- <span data-ttu-id="4acbb-121">Onartu bi erreakzio - sare edo gehiago bistaratzeko gaitasuna **Proiektua** forma.</span><span class="sxs-lookup"><span data-stu-id="4acbb-121">Support the ability to display two or more react grids on the **Project** form.</span></span>
- <span data-ttu-id="4acbb-122">Egutegiaren amaiera-datatik ataza bat esleitzeko gaitasuna zuzentzeko balioztapena eman da, eta horrek huts egin du baliabideen esleipenean.</span><span class="sxs-lookup"><span data-stu-id="4acbb-122">Provided validation to address the ability to assign a task past the calendar end date, which results in a failed resource assignment.</span></span>
- <span data-ttu-id="4acbb-123">Erroreen kudeaketa hobetu da honetatik sortutako Null Erreferentzia Salbuespenari aurre egiteko:</span><span class="sxs-lookup"><span data-stu-id="4acbb-123">Improved error handling to address Null Reference Exception generated from the following:</span></span>

    - <span data-ttu-id="4acbb-124">**PreValidateProjectTeamMemberCreate** plugina</span><span class="sxs-lookup"><span data-stu-id="4acbb-124">**PreValidateProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="4acbb-125">**PreValidateProjectTaskCreate** proiektuaren zeregina lotutako proiekturik gabe sortzen denean</span><span class="sxs-lookup"><span data-stu-id="4acbb-125">**PreValidateProjectTaskCreate** when a project task is created without an associated project</span></span>
    - <span data-ttu-id="4acbb-126">**PreProjectTeamMemberCreate** plugina</span><span class="sxs-lookup"><span data-stu-id="4acbb-126">**PreProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="4acbb-127">**PostProjectTeamMemberDelete** plugina</span><span class="sxs-lookup"><span data-stu-id="4acbb-127">**PostProjectTeamMemberDelete** plug-in</span></span>
    - <span data-ttu-id="4acbb-128">**PreValidateProjectTaskDelete** plugina</span><span class="sxs-lookup"><span data-stu-id="4acbb-128">**PreValidateProjectTaskDelete** plug-in</span></span>

<span data-ttu-id="4acbb-129">**Sales**</span><span class="sxs-lookup"><span data-stu-id="4acbb-129">**Sales**</span></span>

<span data-ttu-id="4acbb-130">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="4acbb-130">The following issues have been fixed:</span></span>

- <span data-ttu-id="4acbb-131">Erroreen tratamendua hobetu da Sortutako erreferentzia nuluen salbuespenak zuzentzeko **Kopiatu proiektua: Aurrekontuen HelperResource Management**.</span><span class="sxs-lookup"><span data-stu-id="4acbb-131">Improved error handling to address Null Reference Exceptions generated from **Copy Project: Estimates HelperResource Management**.</span></span>
- <span data-ttu-id="4acbb-132">**Ez dago fakturatzeko prest** batean **Denboraren eta materialaren fakturazio-zorroa** ez du fakturazio egoera garbitzen.</span><span class="sxs-lookup"><span data-stu-id="4acbb-132">**Not ready to Invoice** on a **Time and Material Billing Backlog** doesn't clear the billing status.</span></span>
- <span data-ttu-id="4acbb-133">Zuzendu da gaizki etiketatuta **Prezioak** botoiak botoian **Rolaren prezioa** eta **Katalogoko elementuak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="4acbb-133">Corrected mislabeled **Prices** buttons on the **Role Price** and **Catalog Items** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]