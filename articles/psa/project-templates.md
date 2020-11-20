---
title: Proiektuen txantiloiak
description: Gai honek proiektuaren txantiloiak proiektuaren konfigurazio bizkorra egiteko erabiltzeko moduari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: 4fd618e15524c5cef5b6da9b282f449e3dfb7973
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122987"
---
# <a name="project-templates"></a><span data-ttu-id="9442b-103">Proiektuen txantiloiak</span><span class="sxs-lookup"><span data-stu-id="9442b-103">Project templates</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="9442b-104">Proiektuen txantiloia aurrez zehaztutako markoa da, proiektu bat azkar eta erraz hasten laguntzeko.</span><span class="sxs-lookup"><span data-stu-id="9442b-104">A project template is a predefined framework that helps you quickly and easily start a project.</span></span> <span data-ttu-id="9442b-105">Klik bakar batekin beste proiektu bat sortzeko aurrez definitutako txantiloia erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="9442b-105">You can use a predefined template to create a new project with a single click.</span></span> <span data-ttu-id="9442b-106">Proiektuei dagokienez, proiektuaren txantiloietarako baldintzak zehaztu beharko dituzu.</span><span class="sxs-lookup"><span data-stu-id="9442b-106">As for projects, you must define the prerequisites for project templates.</span></span> <span data-ttu-id="9442b-107">Proiektuaren egutegia zehaztu behar duzu proiektuaren txantiloi bakoitzerako, eta funtzioak eta prezio-zerrendak lehenetsi behar dira antolakuntzan, txantiloiaren osagaiek datu baliagarriak izan ditzaten.</span><span class="sxs-lookup"><span data-stu-id="9442b-107">You must define a project calendar for each project template, and roles and price lists must be predefined in the organization, so that the components of the template have useful data.</span></span>

<span data-ttu-id="9442b-108">Proiektuaren txantiloia hiru osagaik osatzen dute: antolaketak, proiektuaren kalkuluek eta proiektuaren taldekideek.</span><span class="sxs-lookup"><span data-stu-id="9442b-108">A project template consists of three components: a schedule, project estimates, and project team members.</span></span>

## <a name="schedule"></a><span data-ttu-id="9442b-109">Antolaketa</span><span class="sxs-lookup"><span data-stu-id="9442b-109">Schedule</span></span>

<span data-ttu-id="9442b-110">Proiektu baten txantiloiaren antolaketak proiektuko antolaketako elementu multzo bera du.</span><span class="sxs-lookup"><span data-stu-id="9442b-110">A schedule in a project template has the same set of elements as a schedule in a project.</span></span> <span data-ttu-id="9442b-111">Zereginen hierarkia bat sor dezakezu, funtzioak zereginekin esleitu ditzakezu, antolaketa atributuak zehaztu ditzakezu eta mendekotasunak ezarri ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="9442b-111">You can create a task hierarchy, associate roles with tasks, define schedule attributes, and set dependencies.</span></span> <span data-ttu-id="9442b-112">Proiektuaren txantiloiaren antolaketak zeregin bakoitzerako zeregin moduak ere onartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="9442b-112">A schedule in a project template also supports task modes for each task.</span></span> <span data-ttu-id="9442b-113">Beraz, programazio motorra onartzen du.</span><span class="sxs-lookup"><span data-stu-id="9442b-113">Therefore, it supports the scheduling engine.</span></span> <span data-ttu-id="9442b-114">Proiektuaren egutegia proiektuarekin lotu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="9442b-114">You must associate a project calendar with the project.</span></span> <span data-ttu-id="9442b-115">Lan-antolaketa sortzen duzunean, ez dago alderik proiektua txantiloi baten eta proiektua baten artean.</span><span class="sxs-lookup"><span data-stu-id="9442b-115">When you create a work schedule, there is no difference between a project template and a project.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="9442b-116">Proiektuaren aurreikuspenak</span><span class="sxs-lookup"><span data-stu-id="9442b-116">Project estimates</span></span>

<span data-ttu-id="9442b-117">Proiektuaren txantiloieko aurreikuspenek proiektuko aurreikuspenek bezala funtzionatzen dute.</span><span class="sxs-lookup"><span data-stu-id="9442b-117">Project estimates in a project template work the same way as project estimates in a project.</span></span> <span data-ttu-id="9442b-118">Hala ere, kostu- eta salmenta-prezioak parametroetan zehazten diren kostu lehenetsien eta salmenta prezioen zerrendetatik ateratzen dira.</span><span class="sxs-lookup"><span data-stu-id="9442b-118">However, the cost and sales prices are pulled from the default cost and sales price lists that are defined in the parameters.</span></span>

## <a name="creating-a-project-from-a-template"></a><span data-ttu-id="9442b-119">Sortu proiektua txantiloitik</span><span class="sxs-lookup"><span data-stu-id="9442b-119">Creating a project from a template</span></span>
 
<span data-ttu-id="9442b-120">Proiektuen txantiloi batetik proiektu bat sortzeko hainbat modu daude:</span><span class="sxs-lookup"><span data-stu-id="9442b-120">There are several ways to create a project from a project template:</span></span>

- <span data-ttu-id="9442b-121">Eskaintza batetik proiektua bat sortzen duzunean, proiektu-txantiloi bat aukera dezakezu **Sorrera bizkorra: proiektua** elkarrizketa-koadroan.</span><span class="sxs-lookup"><span data-stu-id="9442b-121">When you create a project from a quote, you can select a project template in the **Quick Create: Project** dialog box.</span></span>

> ![Sorrera bizkorra: proiektuaren elkarrizketa-koadroa](media/project-11.png)

- <span data-ttu-id="9442b-123">Proiektua sortzen duzunean **Proiektu berria** hautatuta, **Proiektua** orria agertzen da erregistroa gorde aurretik.</span><span class="sxs-lookup"><span data-stu-id="9442b-123">When you create a project by selecting **New Project**, the **Project** page appears before the record is saved.</span></span> <span data-ttu-id="9442b-124">**Aukeratu txantiloia** eremuan, hautatu aurrez definitutako proiektuen txantiloiak antolakuntzan.</span><span class="sxs-lookup"><span data-stu-id="9442b-124">In the **Pick a Template** field, select one of the predefined project templates in the organization.</span></span>
- <span data-ttu-id="9442b-125">Erabili **Sortu Proiektua txantiloi batetik** aukera **Txantiloiaren entitatea** orrian.</span><span class="sxs-lookup"><span data-stu-id="9442b-125">Use **Create Project from a Template** on the **Template Entity** page.</span></span>

## <a name="copying-components-of-template-to-project"></a><span data-ttu-id="9442b-126">Txantiloiko osagaiak proiektuan kopiatzea</span><span class="sxs-lookup"><span data-stu-id="9442b-126">Copying components of template to project</span></span>

<span data-ttu-id="9442b-127">Proiektuaren txantiloiaren osagaiak proiektu batean kopiatzean, zenbait birbidalketa gerta daitezke, proiektuaren ezarpenen arabera.</span><span class="sxs-lookup"><span data-stu-id="9442b-127">When you copy the components of a project template to a project, a few overrides can occur, depending on the settings in the project.</span></span>

### <a name="copying-the-schedule"></a><span data-ttu-id="9442b-128">Kopiatu antolaketa</span><span class="sxs-lookup"><span data-stu-id="9442b-128">Copying the schedule</span></span>

<span data-ttu-id="9442b-129">Proiektuen txantiloi batetik antolaketa koipiatzen duzunean, proiektuaren egutegia txantilokoaren desberdina bada, proiektuko eguteko lanorduak aplikatzen dira zereginaren antolaketan.</span><span class="sxs-lookup"><span data-stu-id="9442b-129">When you copy the schedule from a project template, if the project has a different project calendar than the template, work hours from the project's calendar are applied to the task schedule.</span></span> <span data-ttu-id="9442b-130">Horrela, antolaketa doitzen da backing proiektua egutegiarekin bat etortzeko.</span><span class="sxs-lookup"><span data-stu-id="9442b-130">In this way, the schedule is adjusted to match the backing project calendar.</span></span> <span data-ttu-id="9442b-131">Era berean, antolaketako lehenengo zereginak proiektuaren hasiera-data hartzen du, eta gainerako hierarkiaren antolaketa eguneratu egiten da txantiloian zehaztutako iraupenean eta mendekotasunean oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="9442b-131">Similarly, the first task on the schedule takes the project's start date, and the schedule of the rest of the hierarchy is updated based on the duration and dependencies that are specified in the template.</span></span> 

### <a name="copying-project-estimates"></a><span data-ttu-id="9442b-132">Kopiatu proiektuaren aurreikuspenak</span><span class="sxs-lookup"><span data-stu-id="9442b-132">Copying project estimates</span></span> 

<span data-ttu-id="9442b-133">Proiektuen aurreikuspenaren lerroetan kopiatzean, prezio-zerrendak eguneratzen dira.</span><span class="sxs-lookup"><span data-stu-id="9442b-133">When you copy across project estimate lines, the price lists are updated.</span></span> <span data-ttu-id="9442b-134">Kostuen prezio-zerrendarako, eguneratze horiek proiektuaren unitate jabetzan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="9442b-134">For the cost price list, these updates are based on the owning unit of the project.</span></span> <span data-ttu-id="9442b-135">Salmenten prezio-zerrendarako, bezeroan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="9442b-135">For the sales price list, they are based on the customer.</span></span> <span data-ttu-id="9442b-136">Salmenta entitate bati esleitutako proiektuetarako, unitate-kostua eta salmenta-prezioak prezio-zerrenden arabera zehazten dira.</span><span class="sxs-lookup"><span data-stu-id="9442b-136">For projects that are associated with a sales entity, the unit cost and sales prices are determined based on these price lists.</span></span>

### <a name="copying-a-project-team"></a><span data-ttu-id="9442b-137">Kopiatu proiektuaren taldea</span><span class="sxs-lookup"><span data-stu-id="9442b-137">Copying a project team</span></span>

<span data-ttu-id="9442b-138">Proiektu-talde bat proiektuaren txantiloitik proiektura kopiatzen denean, baliabideak orokorrak kopiatzen dira txantiloian zehaztutako gaitasun eta trebetasunekin batera.</span><span class="sxs-lookup"><span data-stu-id="9442b-138">When a project team is copied from a project template to a project, the generic resources are copied, together with the skills and proficiencies that are defined in the template.</span></span> <span data-ttu-id="9442b-139">Baliabide orokorren esleipenak ere mantendu egiten dira proiektuaren txantiloian zeudelako.</span><span class="sxs-lookup"><span data-stu-id="9442b-139">Generic resource assignments are also maintained as they were in the project template.</span></span> <span data-ttu-id="9442b-140">Baliabide izendatuak ez dira onartzen proiektuaren txantiloietan.</span><span class="sxs-lookup"><span data-stu-id="9442b-140">Named resources aren't supported in project templates.</span></span>
