---
title: Sortu proiektu-txantiloiak
description: Nola sortu proiektu-txantiloia Project Service-n
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: efc404131208e1c971cb091cf174c1f4707552f0
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149348"
---
# <a name="create-a-project-template-project-service"></a><span data-ttu-id="ae584-103">Nola sortu proiektu-txantiloia (Project Service)</span><span class="sxs-lookup"><span data-stu-id="ae584-103">Create a project template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="ae584-104">Proiektua duzu ordu gorde txantiloiak enpresaren erregularki bids projects moten antzeko baduzu.</span><span class="sxs-lookup"><span data-stu-id="ae584-104">Project templates save you time if your company regularly bids on similar types of projects.</span></span> <span data-ttu-id="ae584-105">Funtzio multzo eta estimatua proiektua mota ordu estandarra eskaintzen dute.</span><span class="sxs-lookup"><span data-stu-id="ae584-105">They provide a standard set of roles and estimated hours for a type of project.</span></span> <span data-ttu-id="ae584-106">Kontu buruentzako eta proiektua kudeatzaileak sor dezakezu projects oinarrituta proiektua txantiloi bat, edo txantiloia kopiatu eta hauetako euren egin dute.</span><span class="sxs-lookup"><span data-stu-id="ae584-106">Account managers and project managers can create projects based on a project template, or they can copy the template and make one of their own.</span></span>  
  
## <a name="components-of-project-template"></a><span data-ttu-id="ae584-107">Proiektua txantiloiaren osagaiak</span><span class="sxs-lookup"><span data-stu-id="ae584-107">Components of project template</span></span>
 <span data-ttu-id="ae584-108">Txantiloi proiektua hiru osagai zikloek dituzte:</span><span class="sxs-lookup"><span data-stu-id="ae584-108">A project template consists of three components:</span></span>  
  
- <span data-ttu-id="ae584-109">**Lan egin diren kanpaina-xehatzea egitura**: lana diren kanpaina-xehatzea egitura proiektua txantiloian proiektuan bai elementuak multzo da.</span><span class="sxs-lookup"><span data-stu-id="ae584-109">**Work breakdown structure**: A work breakdown structure in a project template has the same set of elements as in the project.</span></span> <span data-ttu-id="ae584-110">Sortu zeregin bat hierarkia, zeregin, zehaztu antolaketa atributu, ez diren menpekotasunak ezarri eta Gantt, datu guztiak ikusiko funtzioak erlazionatu.</span><span class="sxs-lookup"><span data-stu-id="ae584-110">You can create a task hierarchy, associate roles to task, define schedule attributes, set dependencies and view all the data in the Gantt.</span></span> <span data-ttu-id="ae584-111">Aplikazioko txantiloiak proiektua egitura diren kanpaina-xehatzea lan ere laguntza zeregin moduak bakoitza.</span><span class="sxs-lookup"><span data-stu-id="ae584-111">The work breakdown structure in project templates also support task modes for each task.</span></span> <span data-ttu-id="ae584-112">Ez dago proiektua txantiloi bat eta proiektua bat arteko aldea ez lan-antolaketa sortzen dituzunean.</span><span class="sxs-lookup"><span data-stu-id="ae584-112">There is no difference between a project template and a project when creating work schedule.</span></span>  
  
- <span data-ttu-id="ae584-113">**Proiektua estimates**: Proiektua estimates txantiloiak aplikazioan era berean lan duten projects ez bezala, kasuetan izan ezik, prezio-zerrenda lortzeko kostua defaulting eta prezioak salmenta beti dira lehenetsia kostua eta salmentak prezio-zerrendak zehaztutako [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parametroak.</span><span class="sxs-lookup"><span data-stu-id="ae584-113">**Project estimates**: Project estimates in templates work the same way as they do in projects, except the price lists for defaulting the cost and sales prices are always the default cost and sales price lists defined in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parameters.</span></span> <span data-ttu-id="ae584-114">Funtzionalitate gainerako proiektua bat bai berdina da.</span><span class="sxs-lookup"><span data-stu-id="ae584-114">The rest of the functionality is the same as in a project.</span></span>  
  
- <span data-ttu-id="ae584-115">**Proiektu-taldearen trebakuntza**: proiektu-txantiloirako proiektua taldeak sortzean, ezin duzu erreserbatu izendun baliabiderik txantiloian.</span><span class="sxs-lookup"><span data-stu-id="ae584-115">**Project team formation**: When forming a project team for a project template, you can’t book a named resource in a template.</span></span> <span data-ttu-id="ae584-116">Erabil dezakezu **Sortu Proiektua Taldearen** orokorra baliabide multzo bat sortu behar diren kanpaina-xehatzea egitura lan egin atalean.</span><span class="sxs-lookup"><span data-stu-id="ae584-116">You can use **Generate Project Team** in the work breakdown structure to generate a set of generic resources.</span></span> <span data-ttu-id="ae584-117">Ere zehaztu dezakezu beharrezko trebakuntza eta proficiencies baliabide orokorra.</span><span class="sxs-lookup"><span data-stu-id="ae584-117">You can also specify required skills and proficiencies for generic resources.</span></span> <span data-ttu-id="ae584-118">Ezin duzu ordezko bookable baliabide bat proiektua txantiloiak duen baliabide orokorra.</span><span class="sxs-lookup"><span data-stu-id="ae584-118">You can’t substitute a generic resource with a bookable resource in project templates.</span></span>  
  
## <a name="create-a-project-from-a-template"></a><span data-ttu-id="ae584-119">Sortu proiektua txantiloitik</span><span class="sxs-lookup"><span data-stu-id="ae584-119">Create a project from a template</span></span>  
 <span data-ttu-id="ae584-120">Sor ditzakezu proiektua bat txantiloietatik hurrengo modu hauek daude:</span><span class="sxs-lookup"><span data-stu-id="ae584-120">You can create a project from a template in these following ways:</span></span>  
  
-   <span data-ttu-id="ae584-121">Eskaintzatik proiektua bat sortzeko, proiektu-txantiloi bat aukera dezakezu proiektua bizkor sortzeko inprimakian.</span><span class="sxs-lookup"><span data-stu-id="ae584-121">When creating a project from the quote, you can choose a project template in the project quick create form.</span></span>  
  
-   <span data-ttu-id="ae584-122">Sakatuz proiektua bat sortzean **Berria Proiektua**, proiektua inprimakian bistaratzen erregistroa gorde aurretik.</span><span class="sxs-lookup"><span data-stu-id="ae584-122">When creating a project by clicking **New Project**, the project form displays before you save the record.</span></span> <span data-ttu-id="ae584-123">Bertatik, saka dezakezu **txantiloi bat Aukeratu** eremu aurretik zehaztutako proiektua txantiloiak erakundean zerrendatik hautatu.</span><span class="sxs-lookup"><span data-stu-id="ae584-123">From here, you can click **Pick a template** field to choose from the list of pre-defined project templates in your organization.</span></span>  
  
-   <span data-ttu-id="ae584-124">Sakatu **Sortu proiektua txantiloi batetik** **Proiektu-txantiloia** orrian, txantiloitik proiektu bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="ae584-124">Click **Create project from a template** on the **Project Template** page to create a project from the template.</span></span>  
  
## <a name="copying-components-of-a-template-to-a-project"></a><span data-ttu-id="ae584-125">Txantiloiko osagaiak proiektuan kopiatzea</span><span class="sxs-lookup"><span data-stu-id="ae584-125">Copying components of a template to a project</span></span>  
 <span data-ttu-id="ae584-126">Aplikaziora proiektua bat txantiloi bat osagaiak kopiatzen dituzunean daude gauza buruzko jakin behar duzu.</span><span class="sxs-lookup"><span data-stu-id="ae584-126">When you copy components of a template into a project, there are a few things you should know about.</span></span>  
  
 <span data-ttu-id="ae584-127">**Lan egin diren kanpaina-xehatzea egitura kopiatzen**: kopiatzen Duzunean lan diren kanpaina-xehatzea egitura proiektua txantiloi batetik proiektuan txantiloia baino proiektua beste egutegi bat badu, proiektua, egutegi batetik lanorduekin lan egin aplikatuko zereginak antolaketan.</span><span class="sxs-lookup"><span data-stu-id="ae584-127">**Copying a work breakdown structure**: When you copy the work breakdown structure from a project template, if the project has a different project calendar than the template, the work hours from the project’s calendar will be applied to the schedule of tasks.</span></span> <span data-ttu-id="ae584-128">Antolaketa backing proiektua egutegiarekin egokitzen.</span><span class="sxs-lookup"><span data-stu-id="ae584-128">This adjusts the schedule to the backing project calendar.</span></span> <span data-ttu-id="ae584-129">Similarly, lana diren kanpaina-xehatzea egitura, zeregina lehen ez ditu irauten proiektua, hasiera-data, beraz gainerako, zeregina hierarkia eta iraupena-txantiloia lan diren kanpaina-xehatzea egitura zehazten menpekotasunak oinarrituta eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="ae584-129">Similarly, the first task on the work breakdown structure takes the project’s start date, so the rest of the task hierarchy schedule is updated based on the duration and dependencies specified in the template’s work breakdown structure.</span></span>  
  
 <span data-ttu-id="ae584-130">**Proiektua estimates kopiatzen**: kopiatzen Dituzunean proiektua dagozkionak lineak zehar, prezio-zerrendak karpeetako zure proiektua kostua prezio-zerrenda eta salmenta-prezio-zerrendako bezero-unitatea oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="ae584-130">**Copying project estimates**: When you copy across project estimate lines, price lists are updated based on the owning unit of the project for the cost price list and customer for the sales price list.</span></span> <span data-ttu-id="ae584-131">Unitate-kostua eta prezioak salmenta batetik erlazionatutako entitate salmenta projects, prezio-zerrendak horiek zehazten dituzte.</span><span class="sxs-lookup"><span data-stu-id="ae584-131">The unit cost and sales prices are determined from these price lists on projects that are associated to a sales entity.</span></span>  
  
 <span data-ttu-id="ae584-132">**Taldeak proiektua kopiatzen**: Denean duzu kopiatu proiektua talde-txantiloiaren proiektua bat, baliabideak orokorra dira kopiatzen zehar, bai eta trebakuntza proficiencies txantiloian zehaztuta.</span><span class="sxs-lookup"><span data-stu-id="ae584-132">**Copying a project team**: When you copy the project team from the template to a project, the generic resources are copied across, along with the skills and proficiencies defined in the template.</span></span> <span data-ttu-id="ae584-133">Baliabide orokorra esleipenetan proiektua txantiloi bai ere mantenduko dira.</span><span class="sxs-lookup"><span data-stu-id="ae584-133">Generic resource assignments are also maintained as in the project template.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="ae584-134">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="ae584-134">See Also</span></span>  
 [<span data-ttu-id="ae584-135">Proiektu-kudeatzailearen gida</span><span class="sxs-lookup"><span data-stu-id="ae584-135">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
