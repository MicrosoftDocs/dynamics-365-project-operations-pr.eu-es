---
title: Proiektu-kontratuak
description: Gai honek proiektu mota eta finantzaketa iturri desberdinetarako sor ditzakezun proiektuen kontratuen adibideak eta kontratuak eta fakturak bezeroen fakturak nola kudeatu ditzakezu.
author: Yowelle
manager: AnnBe
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: b7d15523f1b22bb8813a47f9f822f12bc4162104
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071167"
---
# <a name="project-contracts"></a><span data-ttu-id="a9056-103">Proiektu-kontratuak</span><span class="sxs-lookup"><span data-stu-id="a9056-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="a9056-104">Artikulu honek proiektu mota eta finantzaketa iturri desberdinetarako sor ditzakezun proiektuen kontratuen adibideak eta kontratuak eta fakturak bezeroen fakturak nola kudeatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="a9056-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="a9056-105">Proiektu kontratu baterako sortzen duzun proiektu motak proiektuaren bezeroei fakturatzeko erabiltzen den metodoa zehazten du.</span><span class="sxs-lookup"><span data-stu-id="a9056-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="a9056-106">Proiektuaren kontratua eta lotutako proiektua alda ditzakezu, baina ezin duzu proiektu mota aldatu.</span><span class="sxs-lookup"><span data-stu-id="a9056-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="a9056-107">Proiektuaren kontratua erabiliz, proiektu bat edo gehiago faktura ditzakezu aldi berean.</span><span class="sxs-lookup"><span data-stu-id="a9056-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="a9056-108">Proiektuaren kontratuak proiektuaren egiturako azpiproiektu bakoitzeko fakturazio prozedura koherentea bermatzen ere laguntzen du.</span><span class="sxs-lookup"><span data-stu-id="a9056-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="a9056-109">Fakturatuko den proiektu guztiak proiektuaren kontratu batekin lotu behar du.</span><span class="sxs-lookup"><span data-stu-id="a9056-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="a9056-110">Proiektu kontratu baten ezarpenak proiektu kontratu horri lotutako proiektu eta azpiproiektu guztiei aplikatzen zaizkie.</span><span class="sxs-lookup"><span data-stu-id="a9056-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="a9056-111">Proiektuaren kontratu batek finantzazio iturri bat edo gehiago zehaztu ditzake.</span><span class="sxs-lookup"><span data-stu-id="a9056-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="a9056-112">Hori dela eta, fakturazioa hainbat finantzatzaileren artean bana dezakezu, finantziazio mugak ezarri finantziazio iturriek zehaztutako zenbatekoa baino gehiago faktura ez dezaten eta gastuak kobratzeko finantzaketa arauak konfiguratu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="a9056-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="a9056-113">Proiektuen kontratuetarako finantzaketa</span><span class="sxs-lookup"><span data-stu-id="a9056-113">Funding for project contracts</span></span>
<span data-ttu-id="a9056-114">Proiektuen kontratu batzuek zehazten dute hainbat alderdik partekatzen dutela proiektuaren kostuak finantzatzeko ardura.</span><span class="sxs-lookup"><span data-stu-id="a9056-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="a9056-115">Hona hemen zenbait adibideak:</span><span class="sxs-lookup"><span data-stu-id="a9056-115">Here are some examples:</span></span>

-   <span data-ttu-id="a9056-116">Zatiketa ugari dituen bezero handi batek proiektu baten finantzaketa zatiketa banatzea eskatzen du.</span><span class="sxs-lookup"><span data-stu-id="a9056-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="a9056-117">Zure enpresak proiektu handi baten kostuak kanpoko erakunde batekin partekatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="a9056-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="a9056-118">Errepide proiektu bat bi udalek batera finantzatzen dute.</span><span class="sxs-lookup"><span data-stu-id="a9056-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="a9056-119">Zubi proiektu bat gobernuaren beka batek eta korporazio pribatu batek finantzatzen dute.</span><span class="sxs-lookup"><span data-stu-id="a9056-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="a9056-120">Dynamics 365 Finance, transakzio bakar baten edo proiektu oso baten fakturazioa bezero, diru-laguntza edo erakunde anitzen artean bana dezakezu.</span><span class="sxs-lookup"><span data-stu-id="a9056-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="a9056-121">Hainbat finantzatzaile dituzten proiektuetan, finantzaketa-proiektu aurreratu baten finantzaketan laguntzen duten alderdi guztiei finantzazio-iturri deitzen zaie.</span><span class="sxs-lookup"><span data-stu-id="a9056-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="a9056-122">Bezeroa, erakundea edo beka finantzaketa iturri gisa definitu ondoren, finantzaketa arau bat edo gehiago esleitu daitezke.</span><span class="sxs-lookup"><span data-stu-id="a9056-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="a9056-123">Finantzazio arauek proiektuak finantzatzeko iturri desberdinetara nola esleitzen diren zehazten duten irizpideak jasotzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="a9056-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="a9056-124">Hornitutako artikuluak, hala nola, erosketa-eskaeretan eta erosketa-eskaeretan agertzen direnak ezin direnez banatu, kostuaren zenbatekoa ezin da banaketa-unean finantzaketa-iturri anitzen artean banatu.</span><span class="sxs-lookup"><span data-stu-id="a9056-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="a9056-125">Hori dela eta, finantzazio iturriaren balioa 0 (zero) izaten jarraitzen du inbentarioaren arazoa argitaratu arte.</span><span class="sxs-lookup"><span data-stu-id="a9056-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="a9056-126">Inbentarioaren arazoa argitaratzen denean, kostuaren zenbatekoa proiektuaren kontuak banatzeko arauen arabera banatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="a9056-127">Hona hemen fakturazioa finantzaketa iturri anitzen artean banatzeko errazago egin ditzakezun urrats batzuk:</span><span class="sxs-lookup"><span data-stu-id="a9056-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="a9056-128">Zehaztu proiektu baterako sartu diren transakzio guztiek proiektuaren kontratuaren salmenta moneta bera erabiltzen dutela.</span><span class="sxs-lookup"><span data-stu-id="a9056-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="a9056-129">Ezarri finantzazio mugak, finantzaketa iturri batek proiektu bati zehaztutako zenbatekoa baino gehiago fakturatzen ez dion moduan.</span><span class="sxs-lookup"><span data-stu-id="a9056-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="a9056-130">Konfiguratu langile, elementu, kategoria, kategoria talde eta transakzio mota bakoitzerako (edo transakzio mota guztietarako) finantzaketa arauak eta finantzaketa mugak.</span><span class="sxs-lookup"><span data-stu-id="a9056-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="a9056-131">Aukeratu aukerako hasiera eta amaiera datak finantzaketa arau bakoitza baliozkoa den aldia zehazteko.</span><span class="sxs-lookup"><span data-stu-id="a9056-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="a9056-132">Zehaztu finantzaketa iturri bakoitzak duen portzentajea.</span><span class="sxs-lookup"><span data-stu-id="a9056-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="a9056-133">Zehaztu zein den iturri finantzarioaren zuzkidura kalkuluak eragindako desberdintasunak biribiltzeko ardura.</span><span class="sxs-lookup"><span data-stu-id="a9056-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="a9056-134">Konfiguratu arauak, proiektuaren kostuak kanpoko bezeroei fakturatzeko eta barne erakundeei nola kobratuko zaizkien zehazteko.</span><span class="sxs-lookup"><span data-stu-id="a9056-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="a9056-135">Erregistratu transakzioak atxikitako finantzazio kontu batean, finantzaketa osagarria lortu arte edo kostuak barnean hartzea erabaki arte.</span><span class="sxs-lookup"><span data-stu-id="a9056-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="a9056-136">Transakzioarekin zer zerga talde lotu zehazteko, proiektuan zerga talde esleipena bilatu da.</span><span class="sxs-lookup"><span data-stu-id="a9056-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="a9056-137">Zerga taldeen esleipenik egin ez bada proiektu mailan, proiektuaren kontratua bilatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="a9056-138">Adibidez: finantzaketa iturri anitz (sinplea)</span><span class="sxs-lookup"><span data-stu-id="a9056-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="a9056-139">Ondorengo taulan finantzaketa-iturri anitzen artean finantzaketa esleipena kudeatzeko agertokiak eskaintzen dira.</span><span class="sxs-lookup"><span data-stu-id="a9056-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="a9056-140">Eszenatoki hauek hipotesi hauetan oinarritzen dira:</span><span class="sxs-lookup"><span data-stu-id="a9056-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="a9056-141">Lehentasun ezarpenak funtsak esleitzeko kontuan hartzen dira, beste finantzaketa arau irizpideak aplikatu aurretik.</span><span class="sxs-lookup"><span data-stu-id="a9056-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="a9056-142">Ez da zehaztu finantziazio araua baliozkoa denean d epea zehazteko.</span><span class="sxs-lookup"><span data-stu-id="a9056-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="a9056-143"><strong>Egoera</strong></span><span class="sxs-lookup"><span data-stu-id="a9056-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="a9056-144"><strong>Finantzaketa iturria</strong></span><span class="sxs-lookup"><span data-stu-id="a9056-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="a9056-145"><strong>Esleipenaren ehunekoa</strong></span><span class="sxs-lookup"><span data-stu-id="a9056-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="a9056-146"><strong>Esleipenaren lehentasuna</strong></span><span class="sxs-lookup"><span data-stu-id="a9056-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a9056-147">Kostuak finantzaketa-iturri batera bideratu nahi dituzu funtsak agortu arte, kostuak bigarren finantzaketa-iturri batera esleitu bere fondoak agortu arte eta, azkenik, gainerako kostuak hirugarren finantzaketa-iturri batera esleitu.</span><span class="sxs-lookup"><span data-stu-id="a9056-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="a9056-148">Finantzaketa　iturria　1</span><span class="sxs-lookup"><span data-stu-id="a9056-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="a9056-149">Finantzaketa　iturria　2</span><span class="sxs-lookup"><span data-stu-id="a9056-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="a9056-150">Finantzaketa　iturria　3</span><span class="sxs-lookup"><span data-stu-id="a9056-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-151">% 100</span><span class="sxs-lookup"><span data-stu-id="a9056-151">100%</span></span></li>
<li><span data-ttu-id="a9056-152">% 100</span><span class="sxs-lookup"><span data-stu-id="a9056-152">100%</span></span></li>
<li><span data-ttu-id="a9056-153">% 100</span><span class="sxs-lookup"><span data-stu-id="a9056-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-154">1</span><span class="sxs-lookup"><span data-stu-id="a9056-154">1</span></span></li>
<li><span data-ttu-id="a9056-155">2</span><span class="sxs-lookup"><span data-stu-id="a9056-155">2</span></span></li>
<li><span data-ttu-id="a9056-156">3</span><span class="sxs-lookup"><span data-stu-id="a9056-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a9056-157">Kostuen ehuneko 75 finantzaketa iturri batera eta ehuneko 25 bigarren finantzaketa iturri batera bideratu nahi duzu.</span><span class="sxs-lookup"><span data-stu-id="a9056-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="a9056-158">Finantzaketa iturri horietako bat agortzen denean, gainerako kostuak hirugarren finantzaketa iturri batetik ordaindu nahi dituzu.</span><span class="sxs-lookup"><span data-stu-id="a9056-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="a9056-159">Finantzaketa　iturria　1</span><span class="sxs-lookup"><span data-stu-id="a9056-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="a9056-160">Finantzaketa　iturria　2</span><span class="sxs-lookup"><span data-stu-id="a9056-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="a9056-161">Finantzaketa　iturria　3</span><span class="sxs-lookup"><span data-stu-id="a9056-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-162">% 75</span><span class="sxs-lookup"><span data-stu-id="a9056-162">75%</span></span></li>
<li><span data-ttu-id="a9056-163">% 25</span><span class="sxs-lookup"><span data-stu-id="a9056-163">25%</span></span></li>
<li><span data-ttu-id="a9056-164">% 100</span><span class="sxs-lookup"><span data-stu-id="a9056-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-165">1</span><span class="sxs-lookup"><span data-stu-id="a9056-165">1</span></span></li>
<li><span data-ttu-id="a9056-166">1</span><span class="sxs-lookup"><span data-stu-id="a9056-166">1</span></span></li>
<li><span data-ttu-id="a9056-167">2</span><span class="sxs-lookup"><span data-stu-id="a9056-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a9056-168">Kostuen ehuneko 75 finantzaketa iturri batera eta ehuneko 25 bigarren finantzaketa iturri batera bideratu nahi duzu.</span><span class="sxs-lookup"><span data-stu-id="a9056-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="a9056-169">Finantzaketa iturri horietako bat agortzen denean, zatitu egin nahi dituzu gainerako kostuak hirugarren finantzaketa-iturri baten eta laugarren finantzaketa-iturri baten artean.</span><span class="sxs-lookup"><span data-stu-id="a9056-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="a9056-170">Finantzaketa　iturria　1</span><span class="sxs-lookup"><span data-stu-id="a9056-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="a9056-171">Finantzaketa　iturria　2</span><span class="sxs-lookup"><span data-stu-id="a9056-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="a9056-172">Finantzaketa　iturria　3</span><span class="sxs-lookup"><span data-stu-id="a9056-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="a9056-173">Finantzaketa　iturria　4</span><span class="sxs-lookup"><span data-stu-id="a9056-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-174">% 75</span><span class="sxs-lookup"><span data-stu-id="a9056-174">75%</span></span></li>
<li><span data-ttu-id="a9056-175">% 25</span><span class="sxs-lookup"><span data-stu-id="a9056-175">25%</span></span></li>
<li><span data-ttu-id="a9056-176">% 50</span><span class="sxs-lookup"><span data-stu-id="a9056-176">50%</span></span></li>
<li><span data-ttu-id="a9056-177">% 50</span><span class="sxs-lookup"><span data-stu-id="a9056-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-178">1</span><span class="sxs-lookup"><span data-stu-id="a9056-178">1</span></span></li>
<li><span data-ttu-id="a9056-179">1</span><span class="sxs-lookup"><span data-stu-id="a9056-179">1</span></span></li>
<li><span data-ttu-id="a9056-180">2</span><span class="sxs-lookup"><span data-stu-id="a9056-180">2</span></span></li>
<li><span data-ttu-id="a9056-181">2</span><span class="sxs-lookup"><span data-stu-id="a9056-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a9056-182">Kostuen ehuneko lehenengo 25 finantzaketa iturri batera eta ehuneko gainerako bigarren finantzaketa iturri batera bideratu nahi duzu.</span><span class="sxs-lookup"><span data-stu-id="a9056-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="a9056-183">Finantzaketa　iturria　1</span><span class="sxs-lookup"><span data-stu-id="a9056-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="a9056-184">Finantzaketa　iturria　2</span><span class="sxs-lookup"><span data-stu-id="a9056-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-185">% 25</span><span class="sxs-lookup"><span data-stu-id="a9056-185">25%</span></span></li>
<li><span data-ttu-id="a9056-186">% 100</span><span class="sxs-lookup"><span data-stu-id="a9056-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="a9056-187">1</span><span class="sxs-lookup"><span data-stu-id="a9056-187">1</span></span></li>
<li><span data-ttu-id="a9056-188">2</span><span class="sxs-lookup"><span data-stu-id="a9056-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="a9056-189">Adibidez: finantzaketa iturri anitz (konplexua)</span><span class="sxs-lookup"><span data-stu-id="a9056-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="a9056-190">Hiru finantzaketa iturri dituzu, hurrenkera honetan erabili nahi dituzunak:</span><span class="sxs-lookup"><span data-stu-id="a9056-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="a9056-191">Erabili berdin 2 finantzaketa iturria eta 3 finantzaketa iturria 2. finantzaketa iturria agortu arte.</span><span class="sxs-lookup"><span data-stu-id="a9056-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="a9056-192">Jarraitu 3. finantziazio iturria erabiltzen, agortu arte.</span><span class="sxs-lookup"><span data-stu-id="a9056-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="a9056-193">Erabili 1. finantzaketa iturria 3. finantzaketa iturria agortu ondoren.</span><span class="sxs-lookup"><span data-stu-id="a9056-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="a9056-194">Helburua lortzeko, honako hau egin beharko duzu lehenbizi:</span><span class="sxs-lookup"><span data-stu-id="a9056-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="a9056-195">Ezarri 2. iturriaren eta 3. iturriaren finantzazio mugak, dagozkien zenbatekoetarako.</span><span class="sxs-lookup"><span data-stu-id="a9056-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="a9056-196">Sortu hurrengo finantzaketa-arauak:</span><span class="sxs-lookup"><span data-stu-id="a9056-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="a9056-197">1. araua (1. lehentasuna): transakzioen ehuneko 50 2. iturrira bideratu eta ehuneko 50 3. iturrira.</span><span class="sxs-lookup"><span data-stu-id="a9056-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="a9056-198">2. araua (2. lehentasuna): transakzioen ehunekoa 100 finantzaketa 3. iturrira bideratu.</span><span class="sxs-lookup"><span data-stu-id="a9056-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="a9056-199">3. araua (3. lehentasuna): transakzioen ehunekoa 100 finantzaketa 1. iturrira bideratu.</span><span class="sxs-lookup"><span data-stu-id="a9056-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="a9056-200">Konfigurazio honek funtzionatzen du, transakzioak arauen eta mugen arabera egiaztatzen direlako, horietako bat transakzioan aplikatzen den ala ez jakiteko.</span><span class="sxs-lookup"><span data-stu-id="a9056-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="a9056-201">Transakzioari arau edo muga zehatzik aplikatzen ez bazaio, Transakzio guztiak araua aplikatuko da.</span><span class="sxs-lookup"><span data-stu-id="a9056-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="a9056-202">Transakzio guztiak araua transakzio guztiekin bat dator.</span><span class="sxs-lookup"><span data-stu-id="a9056-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="a9056-203">Transakzio batekin bat datorren arau bat aurkitzen bada, arau horretan esleitutako portzentajea aplikatuko da lehenik, baina partidak ezarri diren mugen aurka egiaztatu ondoren.</span><span class="sxs-lookup"><span data-stu-id="a9056-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="a9056-204">Muga bat betetzen bada eta finantzaketa iturri baten funtsak agortzen badira, ez da kontuan hartzen finantzaketa mugarekin lotutako finantzaketa araua, eta programak aplikatzen duen hurrengo araua egiaztatzen du.</span><span class="sxs-lookup"><span data-stu-id="a9056-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="a9056-205">Zenbait kasutan, transakzio baten zati bat soilik esleitu daiteke arau baten arabera.</span><span class="sxs-lookup"><span data-stu-id="a9056-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="a9056-206">Hori gerta liteke transakzioa esleitzen denean mugara iristen delako.</span><span class="sxs-lookup"><span data-stu-id="a9056-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="a9056-207">Kasu horretan, kopuru horren araberako kopuru jakin bat bakarrik esleitzen da, hala nola ehuneko 50 finantzaketa iturri bakoitzari.</span><span class="sxs-lookup"><span data-stu-id="a9056-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="a9056-208">Atal honetan lehen deskribatzen den 1. arauko kasua da.</span><span class="sxs-lookup"><span data-stu-id="a9056-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="a9056-209">Gainerakoa sekuentziaren hurrengo arauaren arabera esleitzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="a9056-210">Hurrengo taulan eszenatoki hau zehatzago aztertzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="a9056-211"><strong>Fokua</strong></span><span class="sxs-lookup"><span data-stu-id="a9056-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="a9056-212"><strong>Xehetasunak</strong></span><span class="sxs-lookup"><span data-stu-id="a9056-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a9056-213">Finantzaketa arauak</span><span class="sxs-lookup"><span data-stu-id="a9056-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="a9056-214">1. araua (1. lehentasuna): transakzio guztiak.</span><span class="sxs-lookup"><span data-stu-id="a9056-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="a9056-215">2. diru iturria % 50-ean esleitu eta 3 % 50-ean.</span><span class="sxs-lookup"><span data-stu-id="a9056-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="a9056-216">2. araua (2. lehentasuna): transakzio guztiak.</span><span class="sxs-lookup"><span data-stu-id="a9056-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="a9056-217">3. finantziazio iturria % 100ean esleitu.</span><span class="sxs-lookup"><span data-stu-id="a9056-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="a9056-218">3. araua (2. lehentasuna): transakzio guztiak.</span><span class="sxs-lookup"><span data-stu-id="a9056-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="a9056-219">1. finantziazio iturria % 100ean esleitu.</span><span class="sxs-lookup"><span data-stu-id="a9056-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a9056-220">Finantzaketa mugak</span><span class="sxs-lookup"><span data-stu-id="a9056-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="a9056-221">Finantzaketa iturri 1 muga = 10,000.00</span><span class="sxs-lookup"><span data-stu-id="a9056-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="a9056-222">Finantzaketa iturri 2 muga = 500.00</span><span class="sxs-lookup"><span data-stu-id="a9056-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="a9056-223">Finantzaketa iturri 3 muga = 750.00</span><span class="sxs-lookup"><span data-stu-id="a9056-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a9056-224">1. transakzioa</span><span class="sxs-lookup"><span data-stu-id="a9056-224">Transaction 1</span></span></td>
<td><span data-ttu-id="a9056-225"><strong>Transakzioaren zenbatekoa:</strong> 100,00<strong>Finantzaketa:</strong> Transakzioa 1. arauaren arabera soilik ordaintzen da, transakzioa 1. araua aplikatu ondoren guztiz ordaindu delako.</span><span class="sxs-lookup"><span data-stu-id="a9056-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="a9056-226">Transakzioa berdin finantzatzen da 2. finantzaketa iturriaren eta 3. iturriaren artean.</span><span class="sxs-lookup"><span data-stu-id="a9056-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="a9056-227">Finantzaketa iturria 2: 50.00</span><span class="sxs-lookup"><span data-stu-id="a9056-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="a9056-228">Finantzaketa iturria 3: 50.00</span><span class="sxs-lookup"><span data-stu-id="a9056-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a9056-229">2. transakzioa</span><span class="sxs-lookup"><span data-stu-id="a9056-229">Transaction 2</span></span></td>
<td><span data-ttu-id="a9056-230"><strong>Transakzioaren zenbatekoa:</strong> 5.000,00<strong>Finantzaketa:</strong> Transakzioa hiru arauen arabera ordaintzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="a9056-231"><strong>1. araua</strong>
</span><span class="sxs-lookup"><span data-stu-id="a9056-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="a9056-232">Finantzaketa iturria 2: 450.00</span><span class="sxs-lookup"><span data-stu-id="a9056-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="a9056-233">Finantzaketa iturria 3: 450.00</span><span class="sxs-lookup"><span data-stu-id="a9056-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="a9056-234">
<strong>2. araua</strong>
</span><span class="sxs-lookup"><span data-stu-id="a9056-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="a9056-235">Finantzaketa iturria 3: 250.00 (= 750.00 – 50.00 – 450.00)</span><span class="sxs-lookup"><span data-stu-id="a9056-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="a9056-236">
<strong>3. araua</strong>
</span><span class="sxs-lookup"><span data-stu-id="a9056-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="a9056-237">Finantzaketa iturria 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span><span class="sxs-lookup"><span data-stu-id="a9056-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a9056-238">Finantzaketa iturri bakoitzerako banatzen diren funtsak guztira</span><span class="sxs-lookup"><span data-stu-id="a9056-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="a9056-239">Finantzaketa iturria 1: 3,850.00</span><span class="sxs-lookup"><span data-stu-id="a9056-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="a9056-240">Finantzaketa iturria 2: 500.00</span><span class="sxs-lookup"><span data-stu-id="a9056-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="a9056-241">Finantzaketa iturria 3: 750.00</span><span class="sxs-lookup"><span data-stu-id="a9056-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="a9056-242">Fakturazio arauak</span><span class="sxs-lookup"><span data-stu-id="a9056-242">Billing rules</span></span>
<span data-ttu-id="a9056-243">Bezero batekin proiektuaren kontratua negoziatzen duzunean, bezeroari proiektu bateko lana nola eta noiz fakturatu ahal diozun zehazten duzu.</span><span class="sxs-lookup"><span data-stu-id="a9056-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="a9056-244">Proiektuaren kontratua eta proiektua konfiguratu ondoren, proiektuaren fakturazio arauak ezar ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="a9056-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="a9056-245">Fakturazio arauak proiektuaren kontratuan zehaztutako proiektuaren baldintzetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="a9056-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="a9056-246">Sortu ditzakezun fakturazio arauak fakturazio arauarekin lotzen dituzun proiektuaren kontratuaren eta proiektu motaren araberakoak dira, esate baterako, Denbora eta materiala edo Prezio finkoa.</span><span class="sxs-lookup"><span data-stu-id="a9056-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="a9056-247">Fakturazio arau bat baino gehiago sor ditzakezu proiektuaren kontratu baterako.</span><span class="sxs-lookup"><span data-stu-id="a9056-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="a9056-248">Fakturazio arau bat ere esleitu diezaiekezu proiektu kontratu berarekin lotura duten eta fakturazio baldintza antzekoak dituzten hainbat proiekturi.</span><span class="sxs-lookup"><span data-stu-id="a9056-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="a9056-249">Fakturazio arau mota hauek ezar ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="a9056-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="a9056-250">**Entrega unitatea** - Bidali faktura bezero bati bidalketa unitate bat osatzean.</span><span class="sxs-lookup"><span data-stu-id="a9056-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="a9056-251">Bidalketa unitateak zehazten dituzu kontratuan.</span><span class="sxs-lookup"><span data-stu-id="a9056-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="a9056-252">**Aurrerapena** - Fakturatu bezero bati proiektuaren ehuneko jakin bat osatzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="a9056-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="a9056-253">Fakturazio-arau bat konfigura dezakezu egindako lanaren ehunekoa automatikoki kalkulatzeko, edo eskuz kalkula dezakezu egindako lanaren ehunekoa eta bezeroari fakturatzeko zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="a9056-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="a9056-254">**Mugarria** - Fakturatu bezero bati proiektuaren mugarriaren zenbateko osoa, mugarria lortzen denean.</span><span class="sxs-lookup"><span data-stu-id="a9056-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="a9056-255">**Kuota** - Fakturatu bezero bati zure zerbitzuengatik gehi kudeaketa-kuota bat, hau da, normalean zerbitzuen kostuaren ehuneko bat.</span><span class="sxs-lookup"><span data-stu-id="a9056-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="a9056-256">**Denbora eta materiala** - Proiektu batean erabiltzen diren denboraren eta materialen balioa fakturatzea bezeroari.</span><span class="sxs-lookup"><span data-stu-id="a9056-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="a9056-257">Fakturazio arau mota guztietarako, bezeroen fakturetatik proiektu bat adostutako fasera iritsi arte atxikitako ehuneko bat zehaztu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="a9056-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="a9056-258">Ordainketa atxikitzeko ehunekoa proiektuaren kontratuan zehazten da.</span><span class="sxs-lookup"><span data-stu-id="a9056-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="a9056-259">Zenbatekoa bezeroaren fakturan agertzen diren lerroen guztizko balioaren arabera kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="a9056-260">Hurrengorako **Denbora eta materiala** eta **Aurrerapena** fakturazio arauak, kargatzeko kategoriak esleitu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="a9056-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="a9056-261">Kobratu beharreko kategoriek bezeroen fakturetan sartu beharko liratekeen eragiketak adierazten dituzte.</span><span class="sxs-lookup"><span data-stu-id="a9056-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="a9056-262">Bezeroari fakturatzeko prest zaudenean, proiektuaren fakturazio zenbatekoa fakturazio arauen arabera kalkulatzen da eta proiektuaren faktura proposamena sortzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="a9056-263">Ondorengo ataletan proiektu baten fakturazio arauak nola konfiguratu eta kudeatu erakusten duten adibideak ematen dira.</span><span class="sxs-lookup"><span data-stu-id="a9056-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="a9056-264">Adibidez: Sortu fakturazio araua entregatutako unitate kopuruaren arabera</span><span class="sxs-lookup"><span data-stu-id="a9056-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="a9056-265">Zure erakundeak akordioa sinatzen du bezeroen langileei bost trebakuntza-saio emateko guztira 10.000 kostu dituela prestakuntza-saio bakoitzeko.</span><span class="sxs-lookup"><span data-stu-id="a9056-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="a9056-266">Prestakuntza saio bakoitzaren ondoren bezeroari fakturatzen diozu.</span><span class="sxs-lookup"><span data-stu-id="a9056-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="a9056-267">Kontratuaren fakturazio arauak konfiguratzen dituzunean, balio hauek erabiltzen dituzu:</span><span class="sxs-lookup"><span data-stu-id="a9056-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="a9056-268">Emateko unitatea entrenamendu saio bakarra da.</span><span class="sxs-lookup"><span data-stu-id="a9056-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="a9056-269">Unitatearen prezioa 10.000 da entrenamendu saio bakoitzeko.</span><span class="sxs-lookup"><span data-stu-id="a9056-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="a9056-270">Unitate kopurua bost entrenamendu saio da.</span><span class="sxs-lookup"><span data-stu-id="a9056-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="a9056-271">Prestakuntza saio bat amaitutakoan, 10.000 euroko faktura sor dezakezu, entregatu den lehenengo unitateari eta faktura bezeroari bidali.</span><span class="sxs-lookup"><span data-stu-id="a9056-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="a9056-272">Adibidez: Sortu fakturazio araua proiektuaren amaierako ehuneko jakin batean oinarrituta (eskuzko kalkulua)</span><span class="sxs-lookup"><span data-stu-id="a9056-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="a9056-273">Zure erakundeak, software aholkularitza enpresak, bezeroarekin akordioa egiten du bezeroak garatzen ari den produktu baten zati bat garatzeko.</span><span class="sxs-lookup"><span data-stu-id="a9056-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="a9056-274">Zure erakundeak onartzen du software kodea sei hilabetetan entregatzea.</span><span class="sxs-lookup"><span data-stu-id="a9056-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="a9056-275">Bezeroak onartzen du zure erakundeari 100.000 guztira ordaintzea lanagatik.</span><span class="sxs-lookup"><span data-stu-id="a9056-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="a9056-276">Fakturazio arau bat sortzen duzu bezeroari fakturatzeko proiektuan amaitutako lan portzentajearen arabera, kontratuan zehazten den moduan.</span><span class="sxs-lookup"><span data-stu-id="a9056-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="a9056-277">Lehenengo hilabetearen amaieran, bezeroarekin elkartuko zara egindako lanen ehunekoa zehazteko.</span><span class="sxs-lookup"><span data-stu-id="a9056-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="a9056-278">Zuk eta bezeroak proiektua aztertu ondoren, erabakitzen duzu proiektua ehuneko 15 amaituta dagoela.</span><span class="sxs-lookup"><span data-stu-id="a9056-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="a9056-279">Faktura bat sortu 15,000 (100,000 ehuneko 15) eta bidali bezeroari.</span><span class="sxs-lookup"><span data-stu-id="a9056-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="a9056-280">Adibidez: Sortu fakturazio araua proiektuaren amaierako ehuneko jakin batean oinarrituta (automatikoa kalkulua)</span><span class="sxs-lookup"><span data-stu-id="a9056-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="a9056-281">Zure erakundeak, software garapenerako enpresak, ados dago 30.000 euroko nomina kontabilitate pakete bat garatzea bezeroarentzat.</span><span class="sxs-lookup"><span data-stu-id="a9056-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="a9056-282">Bezeroak onartzen du onartzea zure erakundea oinarriztu osatutako lanaren ehunekoan.</span><span class="sxs-lookup"><span data-stu-id="a9056-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="a9056-283">Proiektuaren kostuak 20.000 direla kalkulatzen duzu.</span><span class="sxs-lookup"><span data-stu-id="a9056-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="a9056-284">Proiektuaren kontratuan fakturazio prozesuan erabiltzen dituzun lan kategoriak zehazten dira.</span><span class="sxs-lookup"><span data-stu-id="a9056-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="a9056-285">Fakturazio-arauak konfiguratzen dituzu kategoria bakoitzerako egindako lan portzentajearen fakturen zenbatekoak automatikoki kalkulatzen dituztenak.</span><span class="sxs-lookup"><span data-stu-id="a9056-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="a9056-286">Kategoria bakoitzerako aurrekontua konfiguratzen duzu:</span><span class="sxs-lookup"><span data-stu-id="a9056-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="a9056-287">**Garapena** - 15.000 kostua eta 20.000 sarrerak</span><span class="sxs-lookup"><span data-stu-id="a9056-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="a9056-288">**Instalazioa** - 5.000 kostua eta 10.000 sarrerak</span><span class="sxs-lookup"><span data-stu-id="a9056-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="a9056-289">Bezeroaren faktura lehenengo aldiz sortzen duzunean, fakturaren zenbatekoa automatikoki kalkulatzen da informazio hau oinarritzat hartuta:</span><span class="sxs-lookup"><span data-stu-id="a9056-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="a9056-290">Hilabete igarota, proiektuko langileak proiektuaren fitxa aurkezten du.</span><span class="sxs-lookup"><span data-stu-id="a9056-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="a9056-291">Langilearen orduen kostua 5.000 da garapenerako eta 1.000 instalazioetarako.</span><span class="sxs-lookup"><span data-stu-id="a9056-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="a9056-292">Garapen lana ehuneko 33 amaituta dago (5.000 benetako kostua / 15.000 aurrekontu kostua), eta instalazio lanak ehuneko 20 amaitu dira (1.000 benetako kostua / 5.000 aurrekontu kostua).</span><span class="sxs-lookup"><span data-stu-id="a9056-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="a9056-293">Fakturaren zenbatekoa 8.667 automatikoki kalkulatzen da (20.000 ehuneko 33 + 10.000 ehuneko 20).</span><span class="sxs-lookup"><span data-stu-id="a9056-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="a9056-294">8,667 faktura sortu eta bezeroari bidaliko diozu.</span><span class="sxs-lookup"><span data-stu-id="a9056-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="a9056-295">Adibidez: sortu fakturazio arau bat adostutako mugarrietan oinarrituta</span><span class="sxs-lookup"><span data-stu-id="a9056-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="a9056-296">Zure erakundeak, kudeaketa aholkularitza enpresak, ados dago bezeroak saltzeko asmoa duen kontsumo produktu baten merkatu ikerketak egitea.</span><span class="sxs-lookup"><span data-stu-id="a9056-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="a9056-297">Bezeroak onartzen du zure zerbitzuak hiru hilabetez erabiltzea, martxoan hasita, eta zure erakundeari 50.000 ordaintzea onartzen du.</span><span class="sxs-lookup"><span data-stu-id="a9056-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="a9056-298">Proiektuak hiru mugarri ditu:</span><span class="sxs-lookup"><span data-stu-id="a9056-298">The project has three milestones:</span></span>

-   <span data-ttu-id="a9056-299">1. mugarria: bildu kontsumitzaileen datuak - martxoaren 31</span><span class="sxs-lookup"><span data-stu-id="a9056-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="a9056-300">2. mugarria: kontsumitzaileen datuak aztertu - apirilaren 30a</span><span class="sxs-lookup"><span data-stu-id="a9056-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="a9056-301">3. mugarria: aurkeztu produktuaren bideragarritasun proposamena - Maiatzak 31</span><span class="sxs-lookup"><span data-stu-id="a9056-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="a9056-302">Bezeroa ados dago zure erakundeari 10.000 ordaintzea lehen mugarriagatik, 20.000 bigarren mugarriagatik eta 20.000 hirugarren mugarriagatik.</span><span class="sxs-lookup"><span data-stu-id="a9056-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="a9056-303">Proiektuaren kontratua konfiguratzen duzunean, bezeroari fakturatzea onartzen duzu amaitutako mugarrian oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="a9056-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="a9056-304">Fakturazio arauaren konfigurazioak urrats hauek ditu:</span><span class="sxs-lookup"><span data-stu-id="a9056-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="a9056-305">Definitu proiektuaren mugarriak.</span><span class="sxs-lookup"><span data-stu-id="a9056-305">Define the project milestones.</span></span>
-   <span data-ttu-id="a9056-306">Mugarri bakoitza amaitutakoan bezeroari fakturatzeko zenbatekoa definitu.</span><span class="sxs-lookup"><span data-stu-id="a9056-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="a9056-307">Martxoaren 31n lehenengo mugarria amaitzen denean, mugarria amaituta dagoela markatuko duzu eta, ondoren, 10.000 euroko faktura sortu eta bezeroari bidaliko diozu.</span><span class="sxs-lookup"><span data-stu-id="a9056-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="a9056-308">Ezin duzu mugarri baten faktura sortu mugarria osatuta dagoela markatu arte.</span><span class="sxs-lookup"><span data-stu-id="a9056-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="a9056-309">Adibidez: sortu fakturazio arau bat zerbitzuetan eta kudeaketa kuotan oinarrituta dagoena</span><span class="sxs-lookup"><span data-stu-id="a9056-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="a9056-310">Zure erakundeak, kudeaketa aholkularitza enpresak, ados dago merkatua ikertzea, bezeroak, txikizkako enpresa batek garatzen duen produktu baten bideragarritasuna ebaluatzeko.</span><span class="sxs-lookup"><span data-stu-id="a9056-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="a9056-311">Hitzarmenaren baldintzetan zehazten da zure kudeaketa aholkulari nagusien zerbitzuak emango dituzula, hauek ikerketa denbora eta materialen arabera egingo baitute.</span><span class="sxs-lookup"><span data-stu-id="a9056-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="a9056-312">Bezeroak 100 orduko ordaintzea onartzen du, gehi ehuneko 10eko kudeaketa kuota bat proiektuari kobratzen zaizkion aholkularitza orduengatik.</span><span class="sxs-lookup"><span data-stu-id="a9056-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="a9056-313">Proiektuaren kontratua konfiguratzen duzunean, sortu fakturazio araua, ehuneko 10eko kudeaketa kuota gehitzeko proiektuari kobratzen zaizkion aholkularitza orduetan.</span><span class="sxs-lookup"><span data-stu-id="a9056-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="a9056-314">Bezeroarentzako faktura sortzen duzunean, bezeroari ehuneko 10eko kudeaketa kuota gehitzen zaio kontsultarako orduen kostua.</span><span class="sxs-lookup"><span data-stu-id="a9056-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="a9056-315">Adibidez, hiru aholkulariek proiektuan guztira 200 ordu landu badituzte, 22.000 euroko faktura sortzen da kalkulu hau oinarritzat hartuta:</span><span class="sxs-lookup"><span data-stu-id="a9056-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="a9056-316">200 ordu 100 orduko = 20.000</span><span class="sxs-lookup"><span data-stu-id="a9056-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="a9056-317">Kudeaketa ehuneko 10 = 2.000</span><span class="sxs-lookup"><span data-stu-id="a9056-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="a9056-318">Guztira faktura kopurua = 22,000</span><span class="sxs-lookup"><span data-stu-id="a9056-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="a9056-319">Tasak bezero bati zergapetzen badizkio eta proiektuaren kontratuan salmenten gaineko zerga talde bat hautatzen baduzu, salmenten gaineko zerga taldea automatikoki sartuko da tasen fakturazio arauan.</span><span class="sxs-lookup"><span data-stu-id="a9056-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="a9056-320">Adibidez: Sortu fakturazio araua denboraren eta materialen balioarekin</span><span class="sxs-lookup"><span data-stu-id="a9056-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="a9056-321">Zure erakundeak, software aholkularitza enpresak, bost aholkulari tekniko eskaintzea onartzen du datozen sei hilabeteetan bezeroarentzako softwarearen garapen proiektuan lan egiteko.</span><span class="sxs-lookup"><span data-stu-id="a9056-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="a9056-322">Bezeroak 150 aholku ematen ditu kontsulta ordu bakoitzeko, bulegoko materialaren kostua gehituta.</span><span class="sxs-lookup"><span data-stu-id="a9056-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="a9056-323">Zure erakundeak faktura bat bidaltzen dio bezeroari hil bakoitzaren amaieran.</span><span class="sxs-lookup"><span data-stu-id="a9056-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="a9056-324">Proiektuaren kontratua konfiguratzen duzunean, bezeroari hilero fakturatzea onartzen duzu proiektuan denbora eta materiala lortzeko.</span><span class="sxs-lookup"><span data-stu-id="a9056-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="a9056-325">Informazio hau biltzen duen fakturazio araua sortzen duzu:</span><span class="sxs-lookup"><span data-stu-id="a9056-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="a9056-326">Kontratuaren epea sei hilabetekoa da.</span><span class="sxs-lookup"><span data-stu-id="a9056-326">The contract period is six months.</span></span>
-   <span data-ttu-id="a9056-327">Aholkularitza denbora 150 orduko kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="a9056-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="a9056-328">Bulegoko materiala kostuaren arabera fakturatzen da, eta proiektuaren kostu osoa ez da 10.000 baino handiagoa izan behar.</span><span class="sxs-lookup"><span data-stu-id="a9056-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="a9056-329">Bezeroaren faktura sortzen duzu proiektuan zehar hilabete natural bakoitzaren amaieran.</span><span class="sxs-lookup"><span data-stu-id="a9056-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="a9056-330">Lehenengo hilabetean, guztira 800 ordu grabatzen dituzte aholkulariek proiektuan.</span><span class="sxs-lookup"><span data-stu-id="a9056-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="a9056-331">Proiektuari kargatzen zaizkion bulegoko materialen kostua 2.000 da.</span><span class="sxs-lookup"><span data-stu-id="a9056-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="a9056-332">Hori dela eta, hilaren amaieran 122.000 faktura sortzen dituzu, hau da, 800 orduko 150 orduko kalkulua, gehi 2.000 bulegoko materialetarako.</span><span class="sxs-lookup"><span data-stu-id="a9056-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>



