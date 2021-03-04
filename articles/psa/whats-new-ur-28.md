---
title: Project Service Automation eguneratzearen 28, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 28. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 2c50d6bdc033836e1259a2fd12b78015280d8093
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150608"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a><span data-ttu-id="22af0-103">Project Service Automation eguneratzearen 28, V3 bertsioko berrikuntzak edo aldaketak</span><span class="sxs-lookup"><span data-stu-id="22af0-103">What's new or changed in Project Service Automation Update Release 28, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="22af0-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="22af0-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="22af0-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="22af0-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="22af0-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="22af0-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="22af0-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="22af0-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="22af0-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="22af0-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="22af0-109">Gai honek Project Service Automation V3 bertsio berrirako edo aldatutako ezaugarriak eta konponketak zerrendatzen ditu 28 bertsioa eguneratzea. Bertsio honek V3.10.46.32 eraikuntza kopurua du eta, oro har, 2021eko urtarrilean eguneratze automatikoaren bidez eskuragarri dago.</span><span class="sxs-lookup"><span data-stu-id="22af0-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 28 This version has a build number of V3.10.46.32 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-28"></a><span data-ttu-id="22af0-110">28. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="22af0-110">Update Release 28</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="22af0-111">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="22af0-111">Bug fixes</span></span>

<span data-ttu-id="22af0-112">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="22af0-112">**Time and Expense**</span></span>

<span data-ttu-id="22af0-113">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="22af0-113">The following issues have been fixed:</span></span>

- <span data-ttu-id="22af0-114">Erabiltzaileek erabil dezakete **Edizio masiboa** onartu eta bidali diren denbora-sarrerak eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="22af0-114">Users can use **Bulk Edit** to update time entries that have been approved and submitted.</span></span>

<span data-ttu-id="22af0-115">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="22af0-115">**Project Management**</span></span>

<span data-ttu-id="22af0-116">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="22af0-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="22af0-117">Ataza GUID zenbaki gisa interpretatzen den kasuetan, ezin dira atazak editatu erabilita **Editatu zeregina** zintan **Lanen banaketaren egitura** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="22af0-117">In cases where the task GUID is interpreted as a number, tasks can't be opened for edit using **Edit Task** in the ribbon on the **Work Breakdown Structure** page.</span></span>

<span data-ttu-id="22af0-118">**Sales**</span><span class="sxs-lookup"><span data-stu-id="22af0-118">**Sales**</span></span>

<span data-ttu-id="22af0-119">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="22af0-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="22af0-120">Erreferentzia nuluko salbuespena sortzen da **GetEstimatesForProject** plugina deitzen da.</span><span class="sxs-lookup"><span data-stu-id="22af0-120">A null reference exception is generated when the **GetEstimatesForProject** plug-in is invoked.</span></span>
- <span data-ttu-id="22af0-121">**Markatu fakturatzeko prest** mugarriko saretan atributuak partzialki eguneratzen ditu soilik, **FakturaEgoera** atributua, eguneratu dena.</span><span class="sxs-lookup"><span data-stu-id="22af0-121">**Mark ready to invoice** on the milestone grid only partially updates attributes, except for the **InvoiceStatus** attribute, which is updated.</span></span>

