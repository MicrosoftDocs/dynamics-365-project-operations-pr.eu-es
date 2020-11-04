---
title: Prezioak eta kostuen neurriak hasierako orria
description: Gai honek prezioen dimentsioen ikuspegi orokorra eskaintzen du.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 515a2e2e518614884b414ca43702e8bfea2c6919
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071077"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="855c4-103">Prezioak eta kostuen neurriak hasierako orria</span><span class="sxs-lookup"><span data-stu-id="855c4-103">Pricing and costing dimensions home page</span></span>

<span data-ttu-id="855c4-104">Proiektuetan oinarritutako erakundeetan eskulanaren prezioak eta kostuak ezartzeko erabilitako dimentsioek atributu hauek eragiten dituzte:</span><span class="sxs-lookup"><span data-stu-id="855c4-104">The dimensions used to set labor pricing and costing in project-based organizations are influenced by the following attributes:</span></span>

- <span data-ttu-id="855c4-105">Esperientzia, funtzio edo geografiaren antzeko lanak egiten dituzten pertsonak</span><span class="sxs-lookup"><span data-stu-id="855c4-105">People doing work similar to their experience, role, or geography</span></span>
- <span data-ttu-id="855c4-106">Bere konplexutasunaren edo eguneko orduaren antzera egin beharreko lana</span><span class="sxs-lookup"><span data-stu-id="855c4-106">Work to be performed similar to its complexity or time of day</span></span>

<span data-ttu-id="855c4-107">Lanaren joera hauen izaera tipikoa eta lana burutzeko behar diren pertsonak kontuan hartuta, bi zerbitzu mota daude eskuragarri Project Service Automation-en:</span><span class="sxs-lookup"><span data-stu-id="855c4-107">Given the typical nature of these attrubutes of the work and the people required to perform the work, there are two types of pricing dimension values available in Project Service Automation:</span></span> 

- <span data-ttu-id="855c4-108">**Aukera multzoak** : balio multzo baterako enumerazio finkoak diren atributuak.</span><span class="sxs-lookup"><span data-stu-id="855c4-108">**Option sets** - Attributes that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="855c4-109">**Entitateetan oinarritutako balioak** - Mugatuak diren baina denbora zehar alda daitezkeen balio multzo anitza izan dezaketen atributuak.</span><span class="sxs-lookup"><span data-stu-id="855c4-109">**Entity-based values** - Attributes that can have a varied set of values that are finite but can change over time.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="855c4-110">Prezioen dimentsioak</span><span class="sxs-lookup"><span data-stu-id="855c4-110">Pricing dimensions</span></span>

<span data-ttu-id="855c4-111">PSA prezioen dimentsio multzo lehenetsia da.</span><span class="sxs-lookup"><span data-stu-id="855c4-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="855c4-112">Hauek ikus ditzakezu **Project Service** > **Parametroak** atalean.</span><span class="sxs-lookup"><span data-stu-id="855c4-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="855c4-113">Parametroen erregistroan, **Zenbatekoan oinarritutako prezioen dimentsioak** fitxan, egiaztatu **msdyn_resourcecategory** funtzioak eta **msdyn_organizationalunit** baliabideak antolatzeko unitateak **Salmentetan aplikagarria** eta **Kostuetan aplikagarria** eremuetan **Bai** aukera ezarrita dutela.</span><span class="sxs-lookup"><span data-stu-id="855c4-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="855c4-114">Horri esker, eginkizun eta antolaketa unitateen konbinazio bakoitzeko prezioa eta kostua konfiguratu ahal izango dituzu.</span><span class="sxs-lookup"><span data-stu-id="855c4-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![Project Service-en parametroen pantaila-argazkia, "Salmentetan aplikagarria" eremua nabarmenduta dutela](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="855c4-116">PSAren 3. bertsioaren berezko funtzio eta antolaketa unitateak prezioen dimentsio gisa erabiltzen aritu bazara, ez da aldaketarik egongo.</span><span class="sxs-lookup"><span data-stu-id="855c4-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="855c4-117">Project Service erabiltzen jarraitu dezakezu ohi bezala.</span><span class="sxs-lookup"><span data-stu-id="855c4-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="855c4-118">Baliabideen prezioa edo kostua behar baduzu atributu osagarriak erabiliz, eremu, entitate eta dimentsio pertsonalizatuak sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="855c4-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="855c4-119">Informazio gehiago lortzeko, ikusi honako gai hauek; hala ere, kontuan izan prozedurak bete behar dituzula beheko zerrendako ordenean:</span><span class="sxs-lookup"><span data-stu-id="855c4-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="855c4-120">Sortu eremu eta entitate pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="855c4-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="855c4-121">Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan</span><span class="sxs-lookup"><span data-stu-id="855c4-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="855c4-122">Konfiguratu eremu pertsonalizatuak prezio-dimentsio gisa </span><span class="sxs-lookup"><span data-stu-id="855c4-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="855c4-123">Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko</span><span class="sxs-lookup"><span data-stu-id="855c4-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="855c4-124">Giza baliabideen denborari prezio jartzea</span><span class="sxs-lookup"><span data-stu-id="855c4-124">Pricing human resource time</span></span>
<span data-ttu-id="855c4-125">Erakunde batek giza baliabideen denborari prezioa nola jartzen dion kontuan izan ohi da, erakundearen errentagarritasunean zuzenean eragiten duelako.</span><span class="sxs-lookup"><span data-stu-id="855c4-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="855c4-126">Lan egin finantza taldeekin eta praktikatu arduradunekin zure erakundea giza baliabideen denboraren faktura eta kostu tasak nola ezarri nahi dituen identifikatzeko prest dagoenean.</span><span class="sxs-lookup"><span data-stu-id="855c4-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="855c4-127">Prezioei buruzko beste gogoeta batzuk dira gaur egun prezioen dimentsioak ez dituzten eremuak edo entitateak berriro erabiltzea, baina zure erakundeak prezio dimentsio gisa aplikatzea.</span><span class="sxs-lookup"><span data-stu-id="855c4-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="855c4-128">**Transakzioen kategoria** ( **msdyn_transactioncategory** ) eta **Baliabide erreserbagarria** ( **bookableresource** ) motako eremuak hautagaien dimentsioen adibideak dira.</span><span class="sxs-lookup"><span data-stu-id="855c4-128">Fields like **Transaction Category** ( **msdyn_transactioncategory** ) and **Bookable Resource** ( **bookableresource** ) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="855c4-129">Zure prezioen dimentsioa taula bat edo aukera multzo izan behar den ere hausnartu beharko zenuke.</span><span class="sxs-lookup"><span data-stu-id="855c4-129">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="855c4-130">10 edo 12 gaindituko duten dimentsioen balioen aldaketak aurreikusten badituzu eta balio horietarako atributu gehigarriak behar badituzu, sortu entitate bat aukera multzo bat sortu beharrean.</span><span class="sxs-lookup"><span data-stu-id="855c4-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, create an entity rather than an option set.</span></span> <span data-ttu-id="855c4-131">Aukera multzoa mantentzeak, hala nola balioak gehitzea edo kentzea, administratzailea edo garatzailea eskatzen du, mahai batean errenkada berriak gehitzea negozio-erabiltzaile gehienek egin dezakete.</span><span class="sxs-lookup"><span data-stu-id="855c4-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most business users.</span></span>

<span data-ttu-id="855c4-132">Hurrengo adibidean, baliabideari dagokion funtzioaren eta hornikuntza-unitatearen arabera konfiguratutako fakturen tasak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="855c4-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="855c4-133">Kostu tasak, normalean, langilearen soldata-banda eta kide diren entitate unitatearen araberakoak dira.</span><span class="sxs-lookup"><span data-stu-id="855c4-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="855c4-134">Adibide honetan, faktura-tasa eta kostu-tasen taulak ondorengoak izango dira.</span><span class="sxs-lookup"><span data-stu-id="855c4-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="855c4-135">**Faktura-tasaren adibidea**</span><span class="sxs-lookup"><span data-stu-id="855c4-135">**Sample bill rates**</span></span>

| <span data-ttu-id="855c4-136">Funtzioa</span><span class="sxs-lookup"><span data-stu-id="855c4-136">Role</span></span>        | <span data-ttu-id="855c4-137">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="855c4-137">Org Unit</span></span>    |<span data-ttu-id="855c4-138">Unitatea</span><span class="sxs-lookup"><span data-stu-id="855c4-138">Unit</span></span>      |<span data-ttu-id="855c4-139">Prezioa</span><span class="sxs-lookup"><span data-stu-id="855c4-139">Price</span></span>      |<span data-ttu-id="855c4-140">Moneta</span><span class="sxs-lookup"><span data-stu-id="855c4-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="855c4-141">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="855c4-141">Developer</span></span>   | <span data-ttu-id="855c4-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="855c4-142">Contoso US</span></span>  |<span data-ttu-id="855c4-143">Hour</span><span class="sxs-lookup"><span data-stu-id="855c4-143">Hour</span></span> | <span data-ttu-id="855c4-144">200</span><span class="sxs-lookup"><span data-stu-id="855c4-144">200</span></span>|<span data-ttu-id="855c4-145">USD</span><span class="sxs-lookup"><span data-stu-id="855c4-145">USD</span></span>     |
| <span data-ttu-id="855c4-146">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="855c4-146">Developer</span></span>   | <span data-ttu-id="855c4-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="855c4-147">Contoso India</span></span> |<span data-ttu-id="855c4-148">Hour</span><span class="sxs-lookup"><span data-stu-id="855c4-148">Hour</span></span>|   <span data-ttu-id="855c4-149">112</span><span class="sxs-lookup"><span data-stu-id="855c4-149">112</span></span>|<span data-ttu-id="855c4-150">USD</span><span class="sxs-lookup"><span data-stu-id="855c4-150">USD</span></span>     |


<span data-ttu-id="855c4-151">**Kostu-tasen adibidea**</span><span class="sxs-lookup"><span data-stu-id="855c4-151">**Sample cost rates**</span></span>

| <span data-ttu-id="855c4-152">Soldata Banda</span><span class="sxs-lookup"><span data-stu-id="855c4-152">Salary Band</span></span>     | <span data-ttu-id="855c4-153">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="855c4-153">Org Unit</span></span>    |<span data-ttu-id="855c4-154">Unitatea</span><span class="sxs-lookup"><span data-stu-id="855c4-154">Unit</span></span>      |<span data-ttu-id="855c4-155">Prezioa</span><span class="sxs-lookup"><span data-stu-id="855c4-155">Price</span></span>      |<span data-ttu-id="855c4-156">Moneta</span><span class="sxs-lookup"><span data-stu-id="855c4-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="855c4-157">Nire company_Band1</span><span class="sxs-lookup"><span data-stu-id="855c4-157">My company_Band1</span></span> | <span data-ttu-id="855c4-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="855c4-158">Contoso US</span></span>  |<span data-ttu-id="855c4-159">Hour</span><span class="sxs-lookup"><span data-stu-id="855c4-159">Hour</span></span> | <span data-ttu-id="855c4-160">145</span><span class="sxs-lookup"><span data-stu-id="855c4-160">145</span></span>|<span data-ttu-id="855c4-161">USD</span><span class="sxs-lookup"><span data-stu-id="855c4-161">USD</span></span>     |
| <span data-ttu-id="855c4-162">Nire company_Band2</span><span class="sxs-lookup"><span data-stu-id="855c4-162">My company_Band2</span></span> | <span data-ttu-id="855c4-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="855c4-163">Contoso India</span></span> |<span data-ttu-id="855c4-164">Hour</span><span class="sxs-lookup"><span data-stu-id="855c4-164">Hour</span></span>|   <span data-ttu-id="855c4-165">67</span><span class="sxs-lookup"><span data-stu-id="855c4-165">67</span></span>|<span data-ttu-id="855c4-166">USD</span><span class="sxs-lookup"><span data-stu-id="855c4-166">USD</span></span>     |
