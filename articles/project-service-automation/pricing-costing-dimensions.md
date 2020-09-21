---
title: Prezioak eta kostuen neurriak hasierako orria
description: Gai honek prezioen dimentsioen ikuspegi orokorra eskaintzen du.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 425d7bb8-9015-4f67-b9c9-cf3602e9afe8
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 2379d0d2e038f28a1a8df87a851e9bf7db7fe33f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748846"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="aa76e-103">Prezioak eta kostuen neurriak hasierako orria</span><span class="sxs-lookup"><span data-stu-id="aa76e-103">Pricing and costing dimensions home page</span></span>

<span data-ttu-id="aa76e-104">Prezioak eta kostuak ezartzeko giza baliabideetan erabiltzen diren dimentsioak bi kategoriatan sartzen dira:</span><span class="sxs-lookup"><span data-stu-id="aa76e-104">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="aa76e-105">Jendea</span><span class="sxs-lookup"><span data-stu-id="aa76e-105">People</span></span>
- <span data-ttu-id="aa76e-106">Planifikatutako lana</span><span class="sxs-lookup"><span data-stu-id="aa76e-106">Planned work</span></span>

<span data-ttu-id="aa76e-107">Hori dela eta, prezioen dimentsioko bi balore daude eskuragarri Project Service Automation-en (PSA):</span><span class="sxs-lookup"><span data-stu-id="aa76e-107">Because of this, there are two types of pricing dimension values available in Project Service Automation (PSA):</span></span> 

- <span data-ttu-id="aa76e-108">**Aukera multzoak**: balio multzo baterako enumerazio finkoak diren neurriak.</span><span class="sxs-lookup"><span data-stu-id="aa76e-108">**Option sets** - Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="aa76e-109">**Entitatean oinarritutako balioak**: balio multzo askotarikoak izan daitezkeen neurriak.</span><span class="sxs-lookup"><span data-stu-id="aa76e-109">**Entity-based values** - Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="aa76e-110">Prezio-dimentsioak</span><span class="sxs-lookup"><span data-stu-id="aa76e-110">Pricing dimensions</span></span>

<span data-ttu-id="aa76e-111">PSA prezioen dimentsio multzo lehenetsia da.</span><span class="sxs-lookup"><span data-stu-id="aa76e-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="aa76e-112">Hauek ikus ditzakezu **Project Service** > **Parametroak** atalean.</span><span class="sxs-lookup"><span data-stu-id="aa76e-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="aa76e-113">Parametroen erregistroan, **Zenbatekoan oinarritutako prezioen dimentsioak** fitxan, egiaztatu **msdyn_resourcecategory** funtzioak eta **msdyn_organizationalunit** baliabideak antolatzeko unitateak **Salmentetan aplikagarria** eta **Kostuetan aplikagarria** eremuetan **Bai** aukera ezarrita dutela.</span><span class="sxs-lookup"><span data-stu-id="aa76e-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="aa76e-114">Horri esker, eginkizun eta antolaketa unitateen konbinazio bakoitzeko prezioa eta kostua konfiguratu ahal izango dituzu.</span><span class="sxs-lookup"><span data-stu-id="aa76e-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![Project Service-en parametroen pantaila-argazkia, "Salmentetan aplikagarria" eremua nabarmenduta dutela](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="aa76e-116">PSAren 3. bertsioaren berezko funtzio eta antolaketa unitateak prezioen dimentsio gisa erabiltzen aritu bazara, ez da aldaketarik egongo.</span><span class="sxs-lookup"><span data-stu-id="aa76e-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="aa76e-117">Project Service erabiltzen jarraitu dezakezu ohi bezala.</span><span class="sxs-lookup"><span data-stu-id="aa76e-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="aa76e-118">Baliabideen prezioa edo kostua behar baduzu atributu osagarriak erabiliz, eremu, entitate eta dimentsio pertsonalizatuak sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="aa76e-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="aa76e-119">Informazio gehiago lortzeko, ikusi honako gai hauek; hala ere, kontuan izan prozedurak bete behar dituzula beheko zerrendako ordenean:</span><span class="sxs-lookup"><span data-stu-id="aa76e-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="aa76e-120">Sortu eremu eta entitate pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="aa76e-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="aa76e-121">Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan</span><span class="sxs-lookup"><span data-stu-id="aa76e-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="aa76e-122">Ezarri eremu pertsonalizatuak prezio-dimentsio gisa</span><span class="sxs-lookup"><span data-stu-id="aa76e-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="aa76e-123">Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko</span><span class="sxs-lookup"><span data-stu-id="aa76e-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="aa76e-124">Giza baliabideen denborari prezio jartzea</span><span class="sxs-lookup"><span data-stu-id="aa76e-124">Pricing human resource time</span></span>
<span data-ttu-id="aa76e-125">Erakunde batek giza baliabideen denborari prezioa nola jartzen dion kontuan izan ohi da, erakundearen errentagarritasunean zuzenean eragiten duelako.</span><span class="sxs-lookup"><span data-stu-id="aa76e-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="aa76e-126">Lan egin finantza taldeekin eta praktikatu arduradunekin zure erakundea giza baliabideen denboraren faktura eta kostu tasak nola ezarri nahi dituen identifikatzeko prest dagoenean.</span><span class="sxs-lookup"><span data-stu-id="aa76e-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="aa76e-127">Prezioei buruzko beste gogoeta batzuk dira gaur egun prezioen dimentsioak ez dituzten eremuak edo entitateak berriro erabiltzea, baina zure erakundeak prezio dimentsio gisa aplikatzea.</span><span class="sxs-lookup"><span data-stu-id="aa76e-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="aa76e-128">**Transakzioen kategoria** (**msdyn_transactioncategory**) eta **Baliabide erreserbagarria** (**bookableresource**) motako eremuak hautagaien dimentsioen adibideak dira.</span><span class="sxs-lookup"><span data-stu-id="aa76e-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="aa76e-129">Zure prezioen dimentsioa taula bat edo aukera multzo izan behar den ere kontuan hartu beharko zenuke.</span><span class="sxs-lookup"><span data-stu-id="aa76e-129">You should also consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="aa76e-130">10 edo 12 gaindituko duten dimentsioen balioen aldaketak aurreikusten badituzu eta balio horietarako atributu gehigarriak behar badituzu, entitatea sortuko zenuke aukera multzo bat baino.</span><span class="sxs-lookup"><span data-stu-id="aa76e-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="aa76e-131">Aukera multzoa mantentzeak, hala nola balioak gehitzea edo kentzea, administratzailea edo garatzailea eskatzen du, mahai batean errenkada berriak gehitzea erabiltzaile gehienek egin dezakete.</span><span class="sxs-lookup"><span data-stu-id="aa76e-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="aa76e-132">Hurrengo adibidean, baliabideari dagokion funtzioaren eta hornikuntza-unitatearen arabera konfiguratutako fakturen tasak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="aa76e-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="aa76e-133">Kostu tasak, normalean, langilearen soldata-banda eta kide diren entitate unitatearen araberakoak dira.</span><span class="sxs-lookup"><span data-stu-id="aa76e-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="aa76e-134">Adibide honetan, faktura-tasa eta kostu-tasen taulak ondorengoak izango dira.</span><span class="sxs-lookup"><span data-stu-id="aa76e-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="aa76e-135">**Faktura-tasaren adibidea**</span><span class="sxs-lookup"><span data-stu-id="aa76e-135">**Sample bill rates**</span></span>

| <span data-ttu-id="aa76e-136">Funtzioa</span><span class="sxs-lookup"><span data-stu-id="aa76e-136">Role</span></span>        | <span data-ttu-id="aa76e-137">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="aa76e-137">Org Unit</span></span>    |<span data-ttu-id="aa76e-138">Unitatea</span><span class="sxs-lookup"><span data-stu-id="aa76e-138">Unit</span></span>      |<span data-ttu-id="aa76e-139">Prezioa</span><span class="sxs-lookup"><span data-stu-id="aa76e-139">Price</span></span>      |<span data-ttu-id="aa76e-140">Moneta</span><span class="sxs-lookup"><span data-stu-id="aa76e-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="aa76e-141">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="aa76e-141">Developer</span></span>   | <span data-ttu-id="aa76e-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="aa76e-142">Contoso US</span></span>  |<span data-ttu-id="aa76e-143">Hour</span><span class="sxs-lookup"><span data-stu-id="aa76e-143">Hour</span></span> | <span data-ttu-id="aa76e-144">200</span><span class="sxs-lookup"><span data-stu-id="aa76e-144">200</span></span>|<span data-ttu-id="aa76e-145">USD</span><span class="sxs-lookup"><span data-stu-id="aa76e-145">USD</span></span>     |
| <span data-ttu-id="aa76e-146">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="aa76e-146">Developer</span></span>   | <span data-ttu-id="aa76e-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="aa76e-147">Contoso India</span></span> |<span data-ttu-id="aa76e-148">Hour</span><span class="sxs-lookup"><span data-stu-id="aa76e-148">Hour</span></span>|   <span data-ttu-id="aa76e-149">112</span><span class="sxs-lookup"><span data-stu-id="aa76e-149">112</span></span>|<span data-ttu-id="aa76e-150">USD</span><span class="sxs-lookup"><span data-stu-id="aa76e-150">USD</span></span>     |


<span data-ttu-id="aa76e-151">**Kostu-tasen adibidea**</span><span class="sxs-lookup"><span data-stu-id="aa76e-151">**Sample cost rates**</span></span>

| <span data-ttu-id="aa76e-152">Soldata Banda</span><span class="sxs-lookup"><span data-stu-id="aa76e-152">Salary Band</span></span>     | <span data-ttu-id="aa76e-153">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="aa76e-153">Org Unit</span></span>    |<span data-ttu-id="aa76e-154">Unitatea</span><span class="sxs-lookup"><span data-stu-id="aa76e-154">Unit</span></span>      |<span data-ttu-id="aa76e-155">Prezioa</span><span class="sxs-lookup"><span data-stu-id="aa76e-155">Price</span></span>      |<span data-ttu-id="aa76e-156">Moneta</span><span class="sxs-lookup"><span data-stu-id="aa76e-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="aa76e-157">Nire company_Band1</span><span class="sxs-lookup"><span data-stu-id="aa76e-157">My company_Band1</span></span> | <span data-ttu-id="aa76e-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="aa76e-158">Contoso US</span></span>  |<span data-ttu-id="aa76e-159">Hour</span><span class="sxs-lookup"><span data-stu-id="aa76e-159">Hour</span></span> | <span data-ttu-id="aa76e-160">145</span><span class="sxs-lookup"><span data-stu-id="aa76e-160">145</span></span>|<span data-ttu-id="aa76e-161">USD</span><span class="sxs-lookup"><span data-stu-id="aa76e-161">USD</span></span>     |
| <span data-ttu-id="aa76e-162">Nire company_Band2</span><span class="sxs-lookup"><span data-stu-id="aa76e-162">My company_Band2</span></span> | <span data-ttu-id="aa76e-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="aa76e-163">Contoso India</span></span> |<span data-ttu-id="aa76e-164">Hour</span><span class="sxs-lookup"><span data-stu-id="aa76e-164">Hour</span></span>|   <span data-ttu-id="aa76e-165">67</span><span class="sxs-lookup"><span data-stu-id="aa76e-165">67</span></span>|<span data-ttu-id="aa76e-166">USD</span><span class="sxs-lookup"><span data-stu-id="aa76e-166">USD</span></span>     |
