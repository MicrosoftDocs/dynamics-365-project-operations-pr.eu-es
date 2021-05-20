---
title: Zehaztu proiektuen egutegiak
description: Gai honek egutegiaren txantiloia proiektu bati proiektuaren egutegia jarraitzeko nola aplikatu jakiteko informazioa eskaintzen du.
author: ruhercul
manager: AnnBe
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1d5642d7a2246dc878b2bc4f504f138b71d29a69
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981285"
---
# <a name="define-project-calendars"></a><span data-ttu-id="ee728-103">Zehaztu proiektuen egutegiak</span><span class="sxs-lookup"><span data-stu-id="ee728-103">Define project calendars</span></span>

<span data-ttu-id="ee728-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="ee728-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ee728-105">Proiektu bat sortzeko eta kudeatzeko, egutegiaren txantiloia aplikatu behar diozu proiektuari.</span><span class="sxs-lookup"><span data-stu-id="ee728-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="ee728-106">Egutegiaren txantiloiak proiektuaren atributu hauek definitzen ditu:</span><span class="sxs-lookup"><span data-stu-id="ee728-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="ee728-107">Lan orduak, hasiera eta amaiera orduak barne</span><span class="sxs-lookup"><span data-stu-id="ee728-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="ee728-108">Lanegunak</span><span class="sxs-lookup"><span data-stu-id="ee728-108">Working days</span></span>
- <span data-ttu-id="ee728-109">Egutegiko salbuespenak, esate baterako, lanik gabeko egunak</span><span class="sxs-lookup"><span data-stu-id="ee728-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="ee728-110">Proiektu bati aplikatu zaion egutegi txantiloia zure erakundearen ezarpenetan definitutako egutegi txantiloiaren kopia da.</span><span class="sxs-lookup"><span data-stu-id="ee728-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="ee728-111">Egutegiaren txantiloia aldatzen baduzu, aldaketa horiek ez dira proiektuaren lan orduetara hedatuko.</span><span class="sxs-lookup"><span data-stu-id="ee728-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="ee728-112">Proiektuaren lan orduak aldatzeko, txantiloi berria aplikatu behar da.</span><span class="sxs-lookup"><span data-stu-id="ee728-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="ee728-113">Zure erakundearentzako egutegi txantiloia sortzeko, bi baldintza nagusi daude:</span><span class="sxs-lookup"><span data-stu-id="ee728-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="ee728-114">Zehaztu txantiloiaren nahi duzun lan ordua erreserbatzeko baliabide berri bat edo dagoeneko erabiliz.</span><span class="sxs-lookup"><span data-stu-id="ee728-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="ee728-115">Sortu egutegiaren txantiloi berria eta lotu txantiloia erreserbatzeko baliabidearekin.</span><span class="sxs-lookup"><span data-stu-id="ee728-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="ee728-116">**Definitu txantiloiko lanorduak**</span><span class="sxs-lookup"><span data-stu-id="ee728-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="ee728-117">Joan **Baliabideak** \> **Baliabideak** atalera.</span><span class="sxs-lookup"><span data-stu-id="ee728-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="ee728-118">Sortu baliabide berri bat egutegiaren txantiloian erreferentzia egiteko edo hautatu lehendik dagoen baliabide bat.</span><span class="sxs-lookup"><span data-stu-id="ee728-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="ee728-119">Aukeratu **Lanorduak** baliabidearen fitxa eta bete argibideak [Ezarri baliabide baten lan orduak](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) egutegiko arauak konfiguratzeko.</span><span class="sxs-lookup"><span data-stu-id="ee728-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="ee728-120">**Sortu egutegiaren txantiloi berri bat**</span><span class="sxs-lookup"><span data-stu-id="ee728-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="ee728-121">Joan **Ezarpenak** \> **Egutegiko txantiloia**.</span><span class="sxs-lookup"><span data-stu-id="ee728-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="ee728-122">Aukeratu **Berria**, eta idatzi izena, deskribapena eta txantiloiaren baliabidea.</span><span class="sxs-lookup"><span data-stu-id="ee728-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="ee728-123">Baliabide bat egutegiaren txantiloian aipatzen denean, baliabidearen egutegiaren kopia egutegiaren txantiloiarekin lotzen da.</span><span class="sxs-lookup"><span data-stu-id="ee728-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="ee728-124">Kopiatutako txantiloiaren lanorduak aldatzen badituzu, aldaketa horiek ez dira egutegiko txantiloian automatikoki beteko.</span><span class="sxs-lookup"><span data-stu-id="ee728-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="ee728-125">Orain lan-txantiloia proiektuaren egutegi txantiloiarekin lotu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="ee728-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

