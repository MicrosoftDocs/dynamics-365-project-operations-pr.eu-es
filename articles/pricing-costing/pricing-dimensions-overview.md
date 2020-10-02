---
title: Prezioen dimentsioen informazio orokorra
description: Gai honek prezio-dimentsioei buruzko informazioa eskaintzen du Dynamics 365 Project Operations-en.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fe2ab3a1b12c00e346e27709d66b5a0cb81a3b56
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898201"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="f00ed-103">Prezioen dimentsioen informazio orokorra</span><span class="sxs-lookup"><span data-stu-id="f00ed-103">Pricing dimensions overview</span></span>

<span data-ttu-id="f00ed-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="f00ed-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f00ed-105">Prezioak eta kostuak ezartzeko giza baliabideetan erabiltzen diren dimentsioak bi kategoriatan sartzen dira:</span><span class="sxs-lookup"><span data-stu-id="f00ed-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="f00ed-106">Jendea</span><span class="sxs-lookup"><span data-stu-id="f00ed-106">People</span></span>
- <span data-ttu-id="f00ed-107">Planifikatutako lana</span><span class="sxs-lookup"><span data-stu-id="f00ed-107">Planned work</span></span>

<span data-ttu-id="f00ed-108">Hori dela eta, prezioen dimentsioko bi balore daude eskuragarri:</span><span class="sxs-lookup"><span data-stu-id="f00ed-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="f00ed-109">**Aukera multzoak**: balio multzo baterako enumerazio finkoak diren neurriak.</span><span class="sxs-lookup"><span data-stu-id="f00ed-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="f00ed-110">**Entitatean oinarritutako balioak**: balio multzo askotarikoak izan daitezkeen neurriak.</span><span class="sxs-lookup"><span data-stu-id="f00ed-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="f00ed-111">Prezioen dimentsioak</span><span class="sxs-lookup"><span data-stu-id="f00ed-111">Pricing dimensions</span></span>

<span data-ttu-id="f00ed-112">Dynamics 365 Project Operations prezioen dimentsio multzo lehenetsiekin hornitzen da.</span><span class="sxs-lookup"><span data-stu-id="f00ed-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="f00ed-113">Prezio-dimentsio horiek ikus ditzakezu **Project Operations** > **Parametroak** atalean.</span><span class="sxs-lookup"><span data-stu-id="f00ed-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="f00ed-114">Parametroen erregistroan, **Zenbatekoan oinarritutako prezioen dimentsioak** fitxan, egiaztatu **msdyn_resourcecategory** funtzioak eta **msdyn_organizationalunit** baliabideak antolatzeko unitateak **Salmentetan aplikagarria** eta **Kostuetan aplikagarria** eremuetan **Bai** aukera ezarrita dutela.</span><span class="sxs-lookup"><span data-stu-id="f00ed-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="f00ed-115">Eremu horiek gaituta dituzula, eginkizun eta antolaketa unitateen konbinazio bakoitzeko prezioa eta kostua konfiguratu ahal izango dituzu.</span><span class="sxs-lookup"><span data-stu-id="f00ed-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="f00ed-116">Baliabideen prezioa edo kostua behar baduzu atributu osagarriak erabiliz, eremu, entitate eta dimentsio pertsonalizatuak sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="f00ed-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="f00ed-117">Giza baliabideen denborari prezio jartzea</span><span class="sxs-lookup"><span data-stu-id="f00ed-117">Pricing human resource time</span></span>
<span data-ttu-id="f00ed-118">Erakunde batek giza baliabideen denborari prezioa nola jartzen dion kontuan izan ohi da, erakundearen errentagarritasunean zuzenean eragiten duelako.</span><span class="sxs-lookup"><span data-stu-id="f00ed-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="f00ed-119">Lan egin finantza taldeekin eta praktikatu arduradunekin zure erakundea giza baliabideen denboraren faktura eta kostu tasak nola ezarri nahi dituen identifikatzeko prest dagoenean.</span><span class="sxs-lookup"><span data-stu-id="f00ed-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="f00ed-120">Prezioei buruzko beste gogoeta batzuk dira gaur egun prezioen dimentsioak ez dituzten eremuak edo entitateak berriro erabiltzea, baina zure erakundeak prezio dimentsio gisa aplikatzea.</span><span class="sxs-lookup"><span data-stu-id="f00ed-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="f00ed-121">**Transakzioen kategoria** (**msdyn_transactioncategory**) eta **Baliabide erreserbagarria** (**bookableresource**) motako eremuak hautagaien dimentsioen adibideak dira.</span><span class="sxs-lookup"><span data-stu-id="f00ed-121">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="f00ed-122">Zure prezioen dimentsioa taula bat edo aukera multzo izan behar den ere hausnartu beharko zenuke.</span><span class="sxs-lookup"><span data-stu-id="f00ed-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="f00ed-123">10 edo 12 gaindituko duten dimentsioen balioen aldaketak aurreikusten badituzu eta balio horietarako atributu gehigarriak behar badituzu, entitatea sortuko zenuke aukera multzo bat baino.</span><span class="sxs-lookup"><span data-stu-id="f00ed-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="f00ed-124">Aukera multzoa mantentzeak, hala nola balioak gehitzea edo kentzea, administratzailea edo garatzailea eskatzen du, mahai batean errenkada berriak gehitzea erabiltzaile gehienek egin dezakete.</span><span class="sxs-lookup"><span data-stu-id="f00ed-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="f00ed-125">Hurrengo adibidean, baliabideari dagokion funtzioaren eta hornikuntza-unitatearen arabera konfiguratutako fakturen tasak erakusten dira.</span><span class="sxs-lookup"><span data-stu-id="f00ed-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="f00ed-126">Kostu tasak, normalean, langilearen soldata-banda eta kide diren entitate unitatearen araberakoak dira.</span><span class="sxs-lookup"><span data-stu-id="f00ed-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="f00ed-127">Adibide honetan, faktura-tasa eta kostu-tasen taulak ondorengoak izango dira.</span><span class="sxs-lookup"><span data-stu-id="f00ed-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="f00ed-128">**Faktura-tasaren adibidea**</span><span class="sxs-lookup"><span data-stu-id="f00ed-128">**Sample bill rates**</span></span>

| <span data-ttu-id="f00ed-129">Funtzioa</span><span class="sxs-lookup"><span data-stu-id="f00ed-129">Role</span></span>        | <span data-ttu-id="f00ed-130">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="f00ed-130">Org Unit</span></span>    |<span data-ttu-id="f00ed-131">Unitatea</span><span class="sxs-lookup"><span data-stu-id="f00ed-131">Unit</span></span>      |<span data-ttu-id="f00ed-132">Prezioa</span><span class="sxs-lookup"><span data-stu-id="f00ed-132">Price</span></span>      |<span data-ttu-id="f00ed-133">Moneta</span><span class="sxs-lookup"><span data-stu-id="f00ed-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="f00ed-134">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="f00ed-134">Developer</span></span>   | <span data-ttu-id="f00ed-135">Contoso US</span><span class="sxs-lookup"><span data-stu-id="f00ed-135">Contoso US</span></span>  |<span data-ttu-id="f00ed-136">Hour</span><span class="sxs-lookup"><span data-stu-id="f00ed-136">Hour</span></span> | <span data-ttu-id="f00ed-137">200</span><span class="sxs-lookup"><span data-stu-id="f00ed-137">200</span></span>|<span data-ttu-id="f00ed-138">USD</span><span class="sxs-lookup"><span data-stu-id="f00ed-138">USD</span></span>     |
| <span data-ttu-id="f00ed-139">Garatzailea</span><span class="sxs-lookup"><span data-stu-id="f00ed-139">Developer</span></span>   | <span data-ttu-id="f00ed-140">Contoso India</span><span class="sxs-lookup"><span data-stu-id="f00ed-140">Contoso India</span></span> |<span data-ttu-id="f00ed-141">Hour</span><span class="sxs-lookup"><span data-stu-id="f00ed-141">Hour</span></span>|   <span data-ttu-id="f00ed-142">112</span><span class="sxs-lookup"><span data-stu-id="f00ed-142">112</span></span>|<span data-ttu-id="f00ed-143">USD</span><span class="sxs-lookup"><span data-stu-id="f00ed-143">USD</span></span>     |


<span data-ttu-id="f00ed-144">**Kostu-tasen adibidea**</span><span class="sxs-lookup"><span data-stu-id="f00ed-144">**Sample cost rates**</span></span>

| <span data-ttu-id="f00ed-145">Soldata Banda</span><span class="sxs-lookup"><span data-stu-id="f00ed-145">Salary Band</span></span>     | <span data-ttu-id="f00ed-146">Erakunde-unitatea</span><span class="sxs-lookup"><span data-stu-id="f00ed-146">Org Unit</span></span>    |<span data-ttu-id="f00ed-147">Unitatea</span><span class="sxs-lookup"><span data-stu-id="f00ed-147">Unit</span></span>      |<span data-ttu-id="f00ed-148">Prezioa</span><span class="sxs-lookup"><span data-stu-id="f00ed-148">Price</span></span>      |<span data-ttu-id="f00ed-149">Moneta</span><span class="sxs-lookup"><span data-stu-id="f00ed-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="f00ed-150">Nire company_Band1</span><span class="sxs-lookup"><span data-stu-id="f00ed-150">My company_Band1</span></span> | <span data-ttu-id="f00ed-151">Contoso US</span><span class="sxs-lookup"><span data-stu-id="f00ed-151">Contoso US</span></span>  |<span data-ttu-id="f00ed-152">Hour</span><span class="sxs-lookup"><span data-stu-id="f00ed-152">Hour</span></span> | <span data-ttu-id="f00ed-153">145</span><span class="sxs-lookup"><span data-stu-id="f00ed-153">145</span></span>|<span data-ttu-id="f00ed-154">USD</span><span class="sxs-lookup"><span data-stu-id="f00ed-154">USD</span></span>     |
| <span data-ttu-id="f00ed-155">Nire company_Band2</span><span class="sxs-lookup"><span data-stu-id="f00ed-155">My company_Band2</span></span> | <span data-ttu-id="f00ed-156">Contoso India</span><span class="sxs-lookup"><span data-stu-id="f00ed-156">Contoso India</span></span> |<span data-ttu-id="f00ed-157">Hour</span><span class="sxs-lookup"><span data-stu-id="f00ed-157">Hour</span></span>|   <span data-ttu-id="f00ed-158">67</span><span class="sxs-lookup"><span data-stu-id="f00ed-158">67</span></span>|<span data-ttu-id="f00ed-159">USD</span><span class="sxs-lookup"><span data-stu-id="f00ed-159">USD</span></span>     |
