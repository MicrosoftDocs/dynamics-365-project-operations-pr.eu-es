---
title: Prezioen dimentsioen informazio orokorra
description: Gai honek Dynamics 365 Project Operations-eko prezio-dimentsioei buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 11/30/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ff675823d84c6e2b83be1e313f881bd672e53981
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275388"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="5e709-103">Prezioen dimentsioen informazio orokorra</span><span class="sxs-lookup"><span data-stu-id="5e709-103">Pricing dimensions overview</span></span>

<span data-ttu-id="5e709-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="5e709-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5e709-105">Prezioak eta kostuak ezartzeko giza baliabideetan erabiltzen diren dimentsioak bi kategoriatan sartzen dira:</span><span class="sxs-lookup"><span data-stu-id="5e709-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="5e709-106">Jendea</span><span class="sxs-lookup"><span data-stu-id="5e709-106">People</span></span>
- <span data-ttu-id="5e709-107">Planifikatutako lana</span><span class="sxs-lookup"><span data-stu-id="5e709-107">Planned work</span></span>

<span data-ttu-id="5e709-108">Hori dela eta, prezioen dimentsioko bi balore daude eskuragarri:</span><span class="sxs-lookup"><span data-stu-id="5e709-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="5e709-109">**Aukera multzoak**: balio multzo baterako enumerazio finkoak diren neurriak.</span><span class="sxs-lookup"><span data-stu-id="5e709-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="5e709-110">**Entitatean oinarritutako balioak**: balio multzo askotarikoak izan daitezkeen neurriak.</span><span class="sxs-lookup"><span data-stu-id="5e709-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="5e709-111">Prezioen dimentsioak</span><span class="sxs-lookup"><span data-stu-id="5e709-111">Pricing dimensions</span></span>

<span data-ttu-id="5e709-112">Dynamics 365 Project Operations prezioen dimentsio multzo lehenetsia da.</span><span class="sxs-lookup"><span data-stu-id="5e709-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="5e709-113">Prezio-dimentsio horiek ikus ditzakezu **Project Operations** > **Parametroak** atalean.</span><span class="sxs-lookup"><span data-stu-id="5e709-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="5e709-114">Parametroen erregistroan, **Zenbatekoan oinarritutako prezioen dimentsioak** fitxan, egiaztatu **msdyn_resourcecategory** funtzioak eta **msdyn_organizationalunit** baliabideak antolatzeko unitateak **Salmentetan aplikagarria** eta **Kostuetan aplikagarria** eremuetan **Bai** aukera ezarrita dutela.</span><span class="sxs-lookup"><span data-stu-id="5e709-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="5e709-115">Eremu horiek gaituta dituzula, eginkizun eta antolaketa unitateen konbinazio bakoitzeko prezioa eta kostua konfiguratu ahal izango dituzu.</span><span class="sxs-lookup"><span data-stu-id="5e709-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

![Project Service-en parametroen pantaila-argazkia, "Salmentetan aplikagarria" eremua nabarmenduta dutela](media/PS-OOB-parameters.png)

<span data-ttu-id="5e709-117">Baliabideen prezioa edo kostua behar baduzu atributu osagarriak erabiliz, eremu, entitate eta dimentsio pertsonalizatuak sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="5e709-117">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="5e709-118">Informazio gehiagorako, ikus gai hauek.</span><span class="sxs-lookup"><span data-stu-id="5e709-118">For more information, see the following topics.</span></span> 
  
  > [!NOTE]
  > <span data-ttu-id="5e709-119">Izapideak zerrendatutako ordenan bete behar dira.</span><span class="sxs-lookup"><span data-stu-id="5e709-119">The procedures must be completed in the order they are listed.</span></span>

1. [<span data-ttu-id="5e709-120">Sortu prezio-dimentsio pertsonalizatuetarako soluzioa</span><span class="sxs-lookup"><span data-stu-id="5e709-120">Create a solution for custom pricing dimensions</span></span>](../sales/create-solution-custompd.md)
2. [<span data-ttu-id="5e709-121">Sortu eremu eta entitate pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="5e709-121">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md)
3. [<span data-ttu-id="5e709-122">Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan </span><span class="sxs-lookup"><span data-stu-id="5e709-122">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
4. [<span data-ttu-id="5e709-123">Konfiguratu eremu pertsonalizatuak prezio-dimentsio gisa </span><span class="sxs-lookup"><span data-stu-id="5e709-123">Set up custom fields as pricing dimensions</span></span>](set-up-custom-fields-pricing-dimensions.md)
5. [<span data-ttu-id="5e709-124">Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko</span><span class="sxs-lookup"><span data-stu-id="5e709-124">Update plug-in attributes to include new pricing dimensions</span></span>](update-plugin-attributes-pd.md)


## <a name="pricing-human-resource-time"></a><span data-ttu-id="5e709-125">Giza baliabideen denborari prezio jartzea</span><span class="sxs-lookup"><span data-stu-id="5e709-125">Pricing human resource time</span></span>
<span data-ttu-id="5e709-126">Erakunde batek giza baliabideen denborari prezioa nola jartzen dion kontuan izan ohi da, erakundearen errentagarritasunean zuzenean eragiten duelako.</span><span class="sxs-lookup"><span data-stu-id="5e709-126">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="5e709-127">Lan egin finantza taldeekin eta praktikatu arduradunekin zure erakundea giza baliabideen denboraren faktura eta kostu tasak nola ezarri nahi dituen identifikatzeko prest dagoenean.</span><span class="sxs-lookup"><span data-stu-id="5e709-127">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="5e709-128">Prezioei buruzko beste gogoeta batzuk dira gaur egun prezioen dimentsioak ez dituzten eremuak edo entitateak berriro erabiltzea, baina zure erakundeak prezio dimentsio gisa aplikatzea.</span><span class="sxs-lookup"><span data-stu-id="5e709-128">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="5e709-129">**Transakzioen kategoria** (**msdyn_transactioncategory**) eta **Baliabide erreserbagarria** (**bookableresource**) motako eremuak hautagaien dimentsioen adibideak dira.</span><span class="sxs-lookup"><span data-stu-id="5e709-129">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="5e709-130">Zure prezioen dimentsioa taula bat edo aukera multzo izan behar den ere hausnartu beharko zenuke.</span><span class="sxs-lookup"><span data-stu-id="5e709-130">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="5e709-131">10 edo 12 gaindituko duten dimentsioen balioen aldaketak aurreikusten badituzu eta balio horietarako atributu gehigarriak behar badituzu, entitatea sortuko zenuke aukera multzo bat baino.</span><span class="sxs-lookup"><span data-stu-id="5e709-131">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="5e709-132">Aukera multzoa mantentzeak, hala nola balioak gehitzea edo kentzea, administratzailea edo garatzailea eskatzen du, mahai batean errenkada berriak gehitzea erabiltzaile gehienek egin dezakete.</span><span class="sxs-lookup"><span data-stu-id="5e709-132">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="5e709-133">Hurrengo adibidean, baliabideari dagokion funtzioaren eta hornikuntza-unitatearen arabera konfiguratutako fakturen tasak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="5e709-133">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="5e709-134">Kostu tasak, normalean, langilearen soldata-banda eta kide diren entitate unitatearen araberakoak dira.</span><span class="sxs-lookup"><span data-stu-id="5e709-134">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="5e709-135">Adibide honetan, faktura-tasa eta kostu-tasen taulak ondorengoak izango dira.</span><span class="sxs-lookup"><span data-stu-id="5e709-135">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="5e709-136">**Faktura-tasaren adibidea**</span><span class="sxs-lookup"><span data-stu-id="5e709-136">**Sample bill rates**</span></span>

| <span data-ttu-id="5e709-137">Funtzioa</span><span class="sxs-lookup"><span data-stu-id="5e709-137">Role</span></span>        | <span data-ttu-id="5e709-138">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="5e709-138">Org Unit</span></span>    |<span data-ttu-id="5e709-139">Unitatea</span><span class="sxs-lookup"><span data-stu-id="5e709-139">Unit</span></span>      |<span data-ttu-id="5e709-140">Prezioa</span><span class="sxs-lookup"><span data-stu-id="5e709-140">Price</span></span>      |<span data-ttu-id="5e709-141">Moneta</span><span class="sxs-lookup"><span data-stu-id="5e709-141">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="5e709-142">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="5e709-142">Developer</span></span>   | <span data-ttu-id="5e709-143">Contoso US</span><span class="sxs-lookup"><span data-stu-id="5e709-143">Contoso US</span></span>  |<span data-ttu-id="5e709-144">Hour</span><span class="sxs-lookup"><span data-stu-id="5e709-144">Hour</span></span> | <span data-ttu-id="5e709-145">200</span><span class="sxs-lookup"><span data-stu-id="5e709-145">200</span></span>|<span data-ttu-id="5e709-146">USD</span><span class="sxs-lookup"><span data-stu-id="5e709-146">USD</span></span>     |
| <span data-ttu-id="5e709-147">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="5e709-147">Developer</span></span>   | <span data-ttu-id="5e709-148">Contoso India</span><span class="sxs-lookup"><span data-stu-id="5e709-148">Contoso India</span></span> |<span data-ttu-id="5e709-149">Hour</span><span class="sxs-lookup"><span data-stu-id="5e709-149">Hour</span></span>|   <span data-ttu-id="5e709-150">112</span><span class="sxs-lookup"><span data-stu-id="5e709-150">112</span></span>|<span data-ttu-id="5e709-151">USD</span><span class="sxs-lookup"><span data-stu-id="5e709-151">USD</span></span>     |


<span data-ttu-id="5e709-152">**Kostu-tasen adibidea**</span><span class="sxs-lookup"><span data-stu-id="5e709-152">**Sample cost rates**</span></span>

| <span data-ttu-id="5e709-153">Soldata Banda</span><span class="sxs-lookup"><span data-stu-id="5e709-153">Salary Band</span></span>     | <span data-ttu-id="5e709-154">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="5e709-154">Org Unit</span></span>    |<span data-ttu-id="5e709-155">Unitatea</span><span class="sxs-lookup"><span data-stu-id="5e709-155">Unit</span></span>      |<span data-ttu-id="5e709-156">Prezioa</span><span class="sxs-lookup"><span data-stu-id="5e709-156">Price</span></span>      |<span data-ttu-id="5e709-157">Moneta</span><span class="sxs-lookup"><span data-stu-id="5e709-157">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="5e709-158">Nire company_Band1</span><span class="sxs-lookup"><span data-stu-id="5e709-158">My company_Band1</span></span> | <span data-ttu-id="5e709-159">Contoso US</span><span class="sxs-lookup"><span data-stu-id="5e709-159">Contoso US</span></span>  |<span data-ttu-id="5e709-160">Hour</span><span class="sxs-lookup"><span data-stu-id="5e709-160">Hour</span></span> | <span data-ttu-id="5e709-161">145</span><span class="sxs-lookup"><span data-stu-id="5e709-161">145</span></span>|<span data-ttu-id="5e709-162">USD</span><span class="sxs-lookup"><span data-stu-id="5e709-162">USD</span></span>     |
| <span data-ttu-id="5e709-163">Nire company_Band2</span><span class="sxs-lookup"><span data-stu-id="5e709-163">My company_Band2</span></span> | <span data-ttu-id="5e709-164">Contoso India</span><span class="sxs-lookup"><span data-stu-id="5e709-164">Contoso India</span></span> |<span data-ttu-id="5e709-165">Hour</span><span class="sxs-lookup"><span data-stu-id="5e709-165">Hour</span></span>|   <span data-ttu-id="5e709-166">67</span><span class="sxs-lookup"><span data-stu-id="5e709-166">67</span></span>|<span data-ttu-id="5e709-167">USD</span><span class="sxs-lookup"><span data-stu-id="5e709-167">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]