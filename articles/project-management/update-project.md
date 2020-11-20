---
title: Eguneratu proiektu bat
description: Gai honek proiektuak eguneratzeari buruzko informazioa eskaintzen du Project Operations-en.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8bcbc6c5a62d252398d541649647fbad49006a0c
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131418"
---
# <a name="update-a-project"></a><span data-ttu-id="7270e-103">Eguneratu proiektu bat</span><span class="sxs-lookup"><span data-stu-id="7270e-103">Update a project</span></span>

<span data-ttu-id="7270e-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="7270e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7270e-105">Jarraian, proiektu bat sortu ondoren egunera daitezkeen eremuen laburpena eta eguneratzeak izan ditzakeen inplikazioen laburpena dago.</span><span class="sxs-lookup"><span data-stu-id="7270e-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="7270e-106">Proiektuaren xehetasun eremuak</span><span class="sxs-lookup"><span data-stu-id="7270e-106">Project detail fields</span></span>

- <span data-ttu-id="7270e-107">**Izena**: proiektuaren izenburua.</span><span class="sxs-lookup"><span data-stu-id="7270e-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="7270e-108">**Azalpena**: proiektuaren ikuspegi orokorra.</span><span class="sxs-lookup"><span data-stu-id="7270e-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="7270e-109">**Bezeroa**: Proiektua entregatuko duen enpresa.</span><span class="sxs-lookup"><span data-stu-id="7270e-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="7270e-110">**Egutegiaren txantiloia**: Proiektuaren lan orduak.</span><span class="sxs-lookup"><span data-stu-id="7270e-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="7270e-111">Eremua aldatzen denean, ordutegi osoa berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="7270e-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="7270e-112">**Moneta**: proiektuaren moneta.</span><span class="sxs-lookup"><span data-stu-id="7270e-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="7270e-113">Eremu hau lehenetsitakoa da kontratazio unitatean definitutako monetan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="7270e-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="7270e-114">Kontratazio unitatea eguneratzen denean, eremua ere eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="7270e-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="7270e-115">**Kontratazio-unitatea**: salmenta irabaztea eta bezeroari lana eta zerbitzuak entregatzea kudeatzeaz arduratzen den enpresa-taldea edo zatiketa ordezkatzen duen antolakuntza-unitatea.</span><span class="sxs-lookup"><span data-stu-id="7270e-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="7270e-116">**Proiektu-kudeatzailea**: Denbora-sarrerak eta gastuak berrikusteko eta onartzeko eskumena duen proiektuko taldekidea.</span><span class="sxs-lookup"><span data-stu-id="7270e-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="7270e-117">Aurreikusi eremuak</span><span class="sxs-lookup"><span data-stu-id="7270e-117">Estimate fields</span></span>

- <span data-ttu-id="7270e-118">**Aurreikusitako hasiera-data**: Proiektua hasiko den eguna.</span><span class="sxs-lookup"><span data-stu-id="7270e-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="7270e-119">Eremu hau eguneratzen denean, proiektuko zereginak proportzionalki mugituko dira hasierako data berriarekin.</span><span class="sxs-lookup"><span data-stu-id="7270e-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="7270e-120">**Amaiera-data**: Proiektua amaitzeko data.</span><span class="sxs-lookup"><span data-stu-id="7270e-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="7270e-121">**Esfortzua**: Proiektuaren kalkulatutako ahalegina.</span><span class="sxs-lookup"><span data-stu-id="7270e-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="7270e-122">Zereginak proiektuari gehitzen zaizkionean, eremu hau jada ez da editagarria.</span><span class="sxs-lookup"><span data-stu-id="7270e-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="7270e-123">**Lan-kostuaren kalkulua**: Proiektuaren eskulanaren kostua.</span><span class="sxs-lookup"><span data-stu-id="7270e-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="7270e-124">Lan-kostuak proiektuari gehitzen zaizkionean, eremu hau jada ez da editagarria.</span><span class="sxs-lookup"><span data-stu-id="7270e-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="7270e-125">**Aurreikusitako gastuak**: Proiektuaren aurreikusitako gastuak.</span><span class="sxs-lookup"><span data-stu-id="7270e-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="7270e-126">Gastuak proiektuari gehitzen zaizkionean, eremu hau jada ez da editagarria.</span><span class="sxs-lookup"><span data-stu-id="7270e-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="7270e-127">Proiektuaren benetako datuen eremuak</span><span class="sxs-lookup"><span data-stu-id="7270e-127">Project actual fields</span></span>
- <span data-ttu-id="7270e-128">**Benetako hasiera**: Proiektua hasi zeneko data.</span><span class="sxs-lookup"><span data-stu-id="7270e-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="7270e-129">**Benetako amaiera**: Proiektu bat amaitutakoan eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="7270e-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="7270e-130">Proiektuaren egoera eremuak</span><span class="sxs-lookup"><span data-stu-id="7270e-130">Project status fields</span></span>

- <span data-ttu-id="7270e-131">**Proiektuaren egoera orokorra**: Proiektuaren zuzendariak emandako proiektuaren osasun orokorra.</span><span class="sxs-lookup"><span data-stu-id="7270e-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="7270e-132">**Iruzkinak**: Proiektuaren zuzendariak emandako proiektuaren egungo osasunari buruzko kontakizuna.</span><span class="sxs-lookup"><span data-stu-id="7270e-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>

