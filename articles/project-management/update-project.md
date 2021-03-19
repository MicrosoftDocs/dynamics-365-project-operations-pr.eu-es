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
ms.openlocfilehash: 27444b072bdf7de55d6b38c30c1ea5fe66ed46ac
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286368"
---
# <a name="update-a-project"></a><span data-ttu-id="7752b-103">Eguneratu proiektu bat</span><span class="sxs-lookup"><span data-stu-id="7752b-103">Update a project</span></span>

<span data-ttu-id="7752b-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="7752b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7752b-105">Jarraian, proiektu bat sortu ondoren egunera daitezkeen eremuen laburpena eta eguneratzeak izan ditzakeen inplikazioen laburpena dago.</span><span class="sxs-lookup"><span data-stu-id="7752b-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="7752b-106">Proiektuaren xehetasun eremuak</span><span class="sxs-lookup"><span data-stu-id="7752b-106">Project detail fields</span></span>

- <span data-ttu-id="7752b-107">**Izena**: proiektuaren izenburua.</span><span class="sxs-lookup"><span data-stu-id="7752b-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="7752b-108">**Azalpena**: proiektuaren ikuspegi orokorra.</span><span class="sxs-lookup"><span data-stu-id="7752b-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="7752b-109">**Bezeroa**: Proiektua entregatuko duen enpresa.</span><span class="sxs-lookup"><span data-stu-id="7752b-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="7752b-110">**Egutegiaren txantiloia**: Proiektuaren lan orduak.</span><span class="sxs-lookup"><span data-stu-id="7752b-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="7752b-111">Eremua aldatzen denean, ordutegi osoa berriro kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="7752b-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="7752b-112">**Moneta**: proiektuaren moneta.</span><span class="sxs-lookup"><span data-stu-id="7752b-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="7752b-113">Eremu hau lehenetsitakoa da kontratazio unitatean definitutako monetan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="7752b-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="7752b-114">Kontratazio unitatea eguneratzen denean, eremua ere eguneratzen da.</span><span class="sxs-lookup"><span data-stu-id="7752b-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="7752b-115">**Kontratazio-unitatea**: salmenta irabaztea eta bezeroari lana eta zerbitzuak entregatzea kudeatzeaz arduratzen den enpresa-taldea edo zatiketa ordezkatzen duen antolakuntza-unitatea.</span><span class="sxs-lookup"><span data-stu-id="7752b-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="7752b-116">**Proiektu-kudeatzailea**: Denbora-sarrerak eta gastuak berrikusteko eta onartzeko eskumena duen proiektuko taldekidea.</span><span class="sxs-lookup"><span data-stu-id="7752b-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="7752b-117">Aurreikusi eremuak</span><span class="sxs-lookup"><span data-stu-id="7752b-117">Estimate fields</span></span>

- <span data-ttu-id="7752b-118">**Aurreikusitako hasiera-data**: Proiektua hasiko den eguna.</span><span class="sxs-lookup"><span data-stu-id="7752b-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="7752b-119">Eremu hau eguneratzen denean, proiektuko zereginak proportzionalki mugituko dira hasierako data berriarekin.</span><span class="sxs-lookup"><span data-stu-id="7752b-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="7752b-120">**Amaiera-data**: Proiektua amaitzeko data.</span><span class="sxs-lookup"><span data-stu-id="7752b-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="7752b-121">**Esfortzua**: Proiektuaren kalkulatutako ahalegina.</span><span class="sxs-lookup"><span data-stu-id="7752b-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="7752b-122">Zereginak proiektuari gehitzen zaizkionean, eremu hau jada ez da editagarria.</span><span class="sxs-lookup"><span data-stu-id="7752b-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="7752b-123">**Lan-kostuaren kalkulua**: Proiektuaren eskulanaren kostua.</span><span class="sxs-lookup"><span data-stu-id="7752b-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="7752b-124">Lan-kostuak proiektuari gehitzen zaizkionean, eremu hau jada ez da editagarria.</span><span class="sxs-lookup"><span data-stu-id="7752b-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="7752b-125">**Aurreikusitako gastuak**: Proiektuaren aurreikusitako gastuak.</span><span class="sxs-lookup"><span data-stu-id="7752b-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="7752b-126">Gastuak proiektuari gehitzen zaizkionean, eremu hau jada ez da editagarria.</span><span class="sxs-lookup"><span data-stu-id="7752b-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="7752b-127">Proiektuaren benetako datuen eremuak</span><span class="sxs-lookup"><span data-stu-id="7752b-127">Project actual fields</span></span>
- <span data-ttu-id="7752b-128">**Benetako hasiera**: Proiektua hasi zeneko data.</span><span class="sxs-lookup"><span data-stu-id="7752b-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="7752b-129">**Benetako amaiera**: Proiektu bat amaitutakoan eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="7752b-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="7752b-130">Proiektuaren egoera eremuak</span><span class="sxs-lookup"><span data-stu-id="7752b-130">Project status fields</span></span>

- <span data-ttu-id="7752b-131">**Proiektuaren egoera orokorra**: Proiektuaren zuzendariak emandako proiektuaren osasun orokorra.</span><span class="sxs-lookup"><span data-stu-id="7752b-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="7752b-132">**Iruzkinak**: Proiektuaren zuzendariak emandako proiektuaren egungo osasunari buruzko kontakizuna.</span><span class="sxs-lookup"><span data-stu-id="7752b-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]