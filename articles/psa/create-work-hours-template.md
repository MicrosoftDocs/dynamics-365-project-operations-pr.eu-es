---
title: Sortu lanorduen-txantiloia
description: Gai honek nola sortu lanorduen txantiloiak Project Service-n deskribatzen du.
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
ms.openlocfilehash: 525f601ad6fee902cb6d5c128b596cc2d33f30c4
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981240"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="80834-103">Sortu lanorduen txantiloiak (Project Service)</span><span class="sxs-lookup"><span data-stu-id="80834-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="80834-104">Proiektu bat sortzeko eta kudeatzeko, egutegiaren txantiloia aplikatu behar diozu proiektuari.</span><span class="sxs-lookup"><span data-stu-id="80834-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="80834-105">Egutegiaren txantiloiak proiektuaren atributu hauek definitzen ditu:</span><span class="sxs-lookup"><span data-stu-id="80834-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="80834-106">Lan orduak, hasiera eta amaiera orduak barne</span><span class="sxs-lookup"><span data-stu-id="80834-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="80834-107">Lanegunak</span><span class="sxs-lookup"><span data-stu-id="80834-107">Working days</span></span>
- <span data-ttu-id="80834-108">Egutegiko salbuespenak, esate baterako, lanik gabeko egunak</span><span class="sxs-lookup"><span data-stu-id="80834-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="80834-109">Proiektu bati aplikatu zaion egutegi txantiloia zure erakundearen ezarpenetan definitutako egutegi txantiloiaren kopia da.</span><span class="sxs-lookup"><span data-stu-id="80834-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="80834-110">Egutegiaren txantiloia aldatzen baduzu, aldaketa horiek ez dira proiektuaren lan orduetara hedatuko.</span><span class="sxs-lookup"><span data-stu-id="80834-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="80834-111">Proiektuaren lan orduak aldatzeko, txantiloi berria aplikatu behar da.</span><span class="sxs-lookup"><span data-stu-id="80834-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="80834-112">Zure erakundearentzako egutegi txantiloia sortzeko, bi baldintza nagusi daude:</span><span class="sxs-lookup"><span data-stu-id="80834-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="80834-113">Zehaztu txantiloiaren nahi duzun lan ordua erreserbatzeko baliabide berri bat edo dagoeneko erabiliz.</span><span class="sxs-lookup"><span data-stu-id="80834-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="80834-114">Sortu egutegiaren txantiloi berria eta lotu txantiloia erreserbatzeko baliabidearekin.</span><span class="sxs-lookup"><span data-stu-id="80834-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="80834-115">**Definitu txantiloiko lanorduak**</span><span class="sxs-lookup"><span data-stu-id="80834-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="80834-116">Joan **Baliabideak** \> **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="80834-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="80834-117">Sortu baliabide berri bat egutegiaren txantiloian erreferentzia egiteko edo hautatu lehendik dagoen baliabide bat.</span><span class="sxs-lookup"><span data-stu-id="80834-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="80834-118">Aukeratu **Lanorduak** baliabidearen fitxa eta bete argibideak [Ezarri baliabide baten lan orduak](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) egutegiko arauak konfiguratzeko.</span><span class="sxs-lookup"><span data-stu-id="80834-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="80834-119">**Sortu egutegiaren txantiloi berri bat**</span><span class="sxs-lookup"><span data-stu-id="80834-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="80834-120">Joan **Ezarpenak** \> **Egutegiko txantiloia**.</span><span class="sxs-lookup"><span data-stu-id="80834-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="80834-121">Aukeratu **Berria**, eta idatzi izena, deskribapena eta txantiloiaren baliabidea.</span><span class="sxs-lookup"><span data-stu-id="80834-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="80834-122">Baliabide bat egutegiaren txantiloian aipatzen denean, baliabidearen egutegiaren kopia egutegiaren txantiloiarekin lotzen da.</span><span class="sxs-lookup"><span data-stu-id="80834-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="80834-123">Kopiatutako txantiloiaren lanorduak aldatzen badituzu, aldaketa horiek ez dira egutegiko txantiloian automatikoki beteko.</span><span class="sxs-lookup"><span data-stu-id="80834-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="80834-124">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="80834-124">See Also</span></span>  
 [<span data-ttu-id="80834-125">Konfiguratu baliabideak</span><span class="sxs-lookup"><span data-stu-id="80834-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
