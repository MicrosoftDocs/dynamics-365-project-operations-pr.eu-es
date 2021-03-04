---
title: Konfiguratu gastuen kudeaketa
description: Artikulu honek Gastuen kudeaketa konfiguratu aurretik plangintza prozesuan zehar hartu behar dituzun gogoetak eta erabakiak deskribatzen ditu Microsoft Dynamics 365 Finance-n.
author: KimANelson
manager: AnnBe
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: db3529597c662a326730cf6a0b855ae865f0dce5
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960322"
---
# <a name="configure-expense-management"></a><span data-ttu-id="71258-103">Konfiguratu gastuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="71258-103">Configure expense management</span></span>

<span data-ttu-id="71258-104">Gai honek Gastuen kudeaketa konfiguratu aurretik plangintza prozesuan zehar hartu behar dituzun gogoetak eta erabakiak deskribatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="71258-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="71258-105">Gastuen kudeaketan, ordainketa metodoei, bidaia eskaerei, gastuen txostenei, gidalerroei eta abarri buruzko informazioa gorde dezakezu.</span><span class="sxs-lookup"><span data-stu-id="71258-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="71258-106">Gastuak kudeatzeko konfigurazioa planifikatzerakoan hartzen dituzun erabaki asko zure erakundearen hierarkian eta finantza egituran oinarritzen direnez, arlo horietako plangintza dokumentuak kontsultatu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="71258-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="71258-107">Enpresen arteko gastuak</span><span class="sxs-lookup"><span data-stu-id="71258-107">Intercompany expenses</span></span>

<span data-ttu-id="71258-108">Enpresen arteko gastuak gaitzen dituzunean, pertsona juridikoei eta langileei beste pertsona juridiko baten izenean gastuak egitea baimentzen diezu eta ordainketa zure erakundeko enpleguko pertsona juridikoari kobratzen diozu.</span><span class="sxs-lookup"><span data-stu-id="71258-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="71258-109">Adibidez, A entitate juridikoko langile batek B entitate juridikorako proiektu bat burutzen du eta proiektuak bidaiari lotutako gastuak ditu.</span><span class="sxs-lookup"><span data-stu-id="71258-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="71258-110">Enpresen arteko gastuak gaituta badaude, langileak gastu txostena aurkeztu ahal izango du, gastua B entitate juridikoari bidaliko diona, eta gastua A. entitate juridikoak ordaindu beharko du. Zure erakundeak pertsona juridiko anitz ez baditu, ez duzu Enpresen arteko gastuak gaitu behar dituzte.</span><span class="sxs-lookup"><span data-stu-id="71258-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="71258-111">**Erabakia:** Enpresen arteko gastuak gaitu nahi dituzu?</span><span class="sxs-lookup"><span data-stu-id="71258-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="71258-112">Finantza-kudeaketa</span><span class="sxs-lookup"><span data-stu-id="71258-112">Financial management</span></span>

<span data-ttu-id="71258-113">Gastuen kudeaketa oso integratuta dago zure erakundearen finantza kudeaketarekin.</span><span class="sxs-lookup"><span data-stu-id="71258-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="71258-114">Gastuak kudeatzeko konfigurazio asko zure erakundearen ekonomiari buruz hartu dituzun erabakietan oinarrituko dira.</span><span class="sxs-lookup"><span data-stu-id="71258-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="71258-115">Ondorengo ataletan plangintza eta erabakiak behar dituzten hainbat arlo deskribatzen dira, zure erakundearen finantza erabakietan eta zure zuzendaritza taldearen orientazioetan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="71258-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="71258-116">Eguneko dietak</span><span class="sxs-lookup"><span data-stu-id="71258-116">Per diems</span></span>

<span data-ttu-id="71258-117">Zure erakundeak eskaintzen dituen dietak langileak zehaztu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="71258-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="71258-118">Dietak normalean otorduak, ostatua eta bestelako gastuak bezalako gastuak estaltzeko erabiltzen direnez, zure erakundeak eskaintzen dituen dieten hobarien arauak sor ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="71258-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="71258-119">eguneko tasak urteko garaian, bidaiaren kokapenean edo bietan oinarrituta egon daitezke.</span><span class="sxs-lookup"><span data-stu-id="71258-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="71258-120">Eguneko araua definitzen duzunean, eguneko tasaren ehuneko bat gordeko dela zehaztu dezakezu langileak osagarriak diren otorduak edo zerbitzuak jasotzen baditu.</span><span class="sxs-lookup"><span data-stu-id="71258-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="71258-121">Halaber, eguneko tasen mailak ere defini ditzakezu langilearen bidaiari aplikatu ahal izateko gutxieneko eta gehieneko ordu kopurua ere ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="71258-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="71258-122">**Erabakiak:**</span><span class="sxs-lookup"><span data-stu-id="71258-122">**Decisions:**</span></span>

- <span data-ttu-id="71258-123">Per diem arau lehenetsiak lehen eta azken egunetarako:</span><span class="sxs-lookup"><span data-stu-id="71258-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="71258-124">Zein da langile batek egun baterako eska dezakeen eta eguneko dietak jaso ditzakeen gutxieneko ordu kopurua?</span><span class="sxs-lookup"><span data-stu-id="71258-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="71258-125">Lehen eguneko eta azken eguneko otorduetarako eskaintzen den kopurua murriztu al da?</span><span class="sxs-lookup"><span data-stu-id="71258-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="71258-126">Murrizketarik badago, zein da murrizketaren ehunekoa?</span><span class="sxs-lookup"><span data-stu-id="71258-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="71258-127">Lehen eguneko eta azken eguneko hoteletarako eskaintzen den kopurua murriztu al da?</span><span class="sxs-lookup"><span data-stu-id="71258-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="71258-128">Murrizketarik badago, zein da murrizketaren ehunekoa?</span><span class="sxs-lookup"><span data-stu-id="71258-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="71258-129">Lehen eguneko eta azken bestelako gastuetarako eskaintzen den kopurua murriztu al da?</span><span class="sxs-lookup"><span data-stu-id="71258-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="71258-130">Murrizketarik badago, zein da murrizketaren ehunekoa?</span><span class="sxs-lookup"><span data-stu-id="71258-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="71258-131">Eguneko dietaren arau lehenetsiak:</span><span class="sxs-lookup"><span data-stu-id="71258-131">Default per diem rules:</span></span>

    - <span data-ttu-id="71258-132">Ba al dago ehuneko dietako hobaria otordu bakoitzeko, adibidez, otordua osagarria bada?</span><span class="sxs-lookup"><span data-stu-id="71258-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="71258-133">Murrizketarik badago, zein da otordu bakoitzaren murrizketaren ehunekoa?</span><span class="sxs-lookup"><span data-stu-id="71258-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="71258-134">Otorduen murrizketa eguneko, bidaia bakoitzeko edo eguneko otordu kopuruaren arabera kalkulatzen da?</span><span class="sxs-lookup"><span data-stu-id="71258-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="71258-135">Eguneko zenbatekoak modu arruntean biribildu edo biribildu behar al dira?</span><span class="sxs-lookup"><span data-stu-id="71258-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="71258-136">Dietak 24 orduko epean edo egun natural batean kalkulatzen dira?</span><span class="sxs-lookup"><span data-stu-id="71258-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="71258-137">Kokapenean oinarritutako eguneko arauak:</span><span class="sxs-lookup"><span data-stu-id="71258-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="71258-138">Eguneko tasak aldatu egiten dira kokapenaren arabera?</span><span class="sxs-lookup"><span data-stu-id="71258-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="71258-139">Zer kokapen sartzen dira?</span><span class="sxs-lookup"><span data-stu-id="71258-139">What locations are included?</span></span>
    - <span data-ttu-id="71258-140">Eguneko tasak kokapenaren arabera aldatzen badira, kokapen bakoitzerako, zein ehuneko kopuru ematen da honako gastu mota hauetarako:</span><span class="sxs-lookup"><span data-stu-id="71258-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="71258-141">Otorduak</span><span class="sxs-lookup"><span data-stu-id="71258-141">Meals</span></span>
        - <span data-ttu-id="71258-142">Hotela</span><span class="sxs-lookup"><span data-stu-id="71258-142">Hotel</span></span>
        - <span data-ttu-id="71258-143">Bestelako gastuak</span><span class="sxs-lookup"><span data-stu-id="71258-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="71258-144">Gastuak kudeatzeko aldizkariak eta kontuak</span><span class="sxs-lookup"><span data-stu-id="71258-144">Expense management journals and accounts</span></span>

<span data-ttu-id="71258-145">Gastuen kudeaketak aldizkari eta kontu bat baino gehiago erabiltzea eskatzen du.</span><span class="sxs-lookup"><span data-stu-id="71258-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="71258-146">Adibidez, erabaki behar duzu ea kontu bera erabiltzen den kutxako aurrerakinetan eta kreditu txartelen auzietan.</span><span class="sxs-lookup"><span data-stu-id="71258-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="71258-147">**Erabakiak:**</span><span class="sxs-lookup"><span data-stu-id="71258-147">**Decisions:**</span></span>

- <span data-ttu-id="71258-148">Zein liburu aldizkarietara bidaltzen dira onartutako gastuen txostenak?</span><span class="sxs-lookup"><span data-stu-id="71258-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="71258-149">Zein kontu erabiltzen da dirua aurreratzeko?</span><span class="sxs-lookup"><span data-stu-id="71258-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="71258-150">Diru aurrerakinak berehala bidali behar al dira?</span><span class="sxs-lookup"><span data-stu-id="71258-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="71258-151">Ordainketa-metodoak</span><span class="sxs-lookup"><span data-stu-id="71258-151">Payment methods</span></span>

<span data-ttu-id="71258-152">Langileei zure negozioaren izenean gastuak egitea baimentzen diezunean, langileek erabil ditzaketen ordainketa moduak definitu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="71258-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="71258-153">Adibidez, langileei dirua edo korporazioko kreditu txartela erabiltzeko baimena eman diezaiekezu.</span><span class="sxs-lookup"><span data-stu-id="71258-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="71258-154">Baliteke langileei kreditu txartel pertsonalak erabiltzea baimentzea eta, ondoren, langileak itzultzea.</span><span class="sxs-lookup"><span data-stu-id="71258-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="71258-155">Onartzen dituzun ordainketa modu bakoitzerako erabaki hauek hartu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="71258-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="71258-156">**Erabakiak:**</span><span class="sxs-lookup"><span data-stu-id="71258-156">**Decisions:**</span></span>

- <span data-ttu-id="71258-157">Zein ordainketa modu onartzen dira?</span><span class="sxs-lookup"><span data-stu-id="71258-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="71258-158">Noren jabe da ordainketa metodoaren gastuak?</span><span class="sxs-lookup"><span data-stu-id="71258-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="71258-159">Ba al dago offset kontu mota bat?</span><span class="sxs-lookup"><span data-stu-id="71258-159">Is there an offset account type?</span></span> <span data-ttu-id="71258-160">Offset kontu mota badago, zer da?</span><span class="sxs-lookup"><span data-stu-id="71258-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="71258-161">Desplazamendu-kontu bat badago, zein da kontua?</span><span class="sxs-lookup"><span data-stu-id="71258-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="71258-162">Ordainketa metodoa kreditu txartela bada, ordainketa metodoa inportatutako transakzioekin bakarrik erabili behar al da?</span><span class="sxs-lookup"><span data-stu-id="71258-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="71258-163">Gastu kategoriak eta kategoria partekatuak</span><span class="sxs-lookup"><span data-stu-id="71258-163">Expense categories and shared categories</span></span>

<span data-ttu-id="71258-164">Langileek gastuen txosten bat sortzen dutenean, erregistratzen duten gastu bakoitza gastu-kategoria batekin lotu behar da.</span><span class="sxs-lookup"><span data-stu-id="71258-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="71258-165">Gastuen kategoriak zure erakundeko pertsona juridikoetan parteka daitezkeen kategoria partekatuetatik eratortzen dira.</span><span class="sxs-lookup"><span data-stu-id="71258-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="71258-166">Kategoria hauek Proiektuen kudeaketan eta kontabilitatean ere parteka daitezke, zure erakundea definitzeko moduaren arabera.</span><span class="sxs-lookup"><span data-stu-id="71258-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="71258-167">Zure erakundearen definizioan eta ezarpen taldearen gidalerroetan oinarrituta, Gastuen kudeaketan erabiltzen diren kategoriak Gastuen kudeaketan soilik erabiliko diren edo beste arlo batzuetan partekatu behar diren zehaztu behar duzu Proiektu-kudeaketaren eta kontabilitatearen eta Gastuen kudeaketaren artean.</span><span class="sxs-lookup"><span data-stu-id="71258-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="71258-168">Kontuan izan kategoria horiek Proiektuen edo gastuen eta ekoizpenaren artean parteka daitezkeela, baina ez gastuen eta ekoizpenaren artean.</span><span class="sxs-lookup"><span data-stu-id="71258-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="71258-169">Gastu kategoria bakoitzerako erabaki hauek hartu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="71258-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="71258-170">**Erabakiak:**</span><span class="sxs-lookup"><span data-stu-id="71258-170">**Decisions:**</span></span>

- <span data-ttu-id="71258-171">Zer da gastu-kategoria?</span><span class="sxs-lookup"><span data-stu-id="71258-171">What is the expense category?</span></span> <span data-ttu-id="71258-172">Adibide gisa, hegaldien, hotelaren edo kilometrajearen kategoriak daude.</span><span class="sxs-lookup"><span data-stu-id="71258-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="71258-173">Gastuen kategoria Proiektuen kudeaketan eta kontabilitatean ere erabil al daiteke?</span><span class="sxs-lookup"><span data-stu-id="71258-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="71258-174">Zer da gastu mota?</span><span class="sxs-lookup"><span data-stu-id="71258-174">What is the expense type?</span></span>
- <span data-ttu-id="71258-175">Zein da gastu kategoriako ordainketa modu lehenetsia?</span><span class="sxs-lookup"><span data-stu-id="71258-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="71258-176">Gastu kategoriako gastuak banatu behar al dira?</span><span class="sxs-lookup"><span data-stu-id="71258-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="71258-177">Zein da gastu-kategoriako kontu lehenetsi nagusia?</span><span class="sxs-lookup"><span data-stu-id="71258-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="71258-178">Zein da gastuen kategorian lehenetsitako salmenten gaineko zerga taldea?</span><span class="sxs-lookup"><span data-stu-id="71258-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="71258-179">Ordainketa modu osagarriak onartzen al dira gastuen kategorian?</span><span class="sxs-lookup"><span data-stu-id="71258-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="71258-180">Ordainketa modu osagarriak onartzen badira, zer dira?</span><span class="sxs-lookup"><span data-stu-id="71258-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="71258-181">Ba al dago azpikategoririk gastu kategoria honetan?</span><span class="sxs-lookup"><span data-stu-id="71258-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="71258-182">Azpikategoriak badaude, erabaki hauek ere hartu beharko dituzu:</span><span class="sxs-lookup"><span data-stu-id="71258-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="71258-183">Zerga berreskuratzetik kanpo dago azpikategorietako bat?</span><span class="sxs-lookup"><span data-stu-id="71258-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="71258-184">Zein da azpikategorien salmenten gaineko zergaren taldea?</span><span class="sxs-lookup"><span data-stu-id="71258-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="71258-185">Gastuen kategoria Proiektuen kudeaketan eta kontabilitatean ere erabiltzen bada, erantzun gainerako galderei.</span><span class="sxs-lookup"><span data-stu-id="71258-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="71258-186">Bestela, joan hurrengo atalera.</span><span class="sxs-lookup"><span data-stu-id="71258-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="71258-187">Zein kostu kontu erabiliko dira ondorengo gastuetarako?</span><span class="sxs-lookup"><span data-stu-id="71258-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="71258-188">Kostua</span><span class="sxs-lookup"><span data-stu-id="71258-188">Cost</span></span>
    - <span data-ttu-id="71258-189">Nominen esleipena</span><span class="sxs-lookup"><span data-stu-id="71258-189">Payroll allocation</span></span>
    - <span data-ttu-id="71258-190">WIP - kostuaren balioa</span><span class="sxs-lookup"><span data-stu-id="71258-190">WIP-cost value</span></span>
    - <span data-ttu-id="71258-191">Kostua-elementua</span><span class="sxs-lookup"><span data-stu-id="71258-191">Cost-item</span></span>
    - <span data-ttu-id="71258-192">WIP-kostuaren balioa-elementua</span><span class="sxs-lookup"><span data-stu-id="71258-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="71258-193">Metatutako galera</span><span class="sxs-lookup"><span data-stu-id="71258-193">Accrued loss</span></span>
    - <span data-ttu-id="71258-194">WIP-metatutako galera</span><span class="sxs-lookup"><span data-stu-id="71258-194">WIP-accrued loss</span></span>

- <span data-ttu-id="71258-195">Zein gastu kontu erabiliko dira ondorengorako?</span><span class="sxs-lookup"><span data-stu-id="71258-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="71258-196">Fakturatutako diru-sarrerak</span><span class="sxs-lookup"><span data-stu-id="71258-196">Invoiced revenue</span></span>
    - <span data-ttu-id="71258-197">Metatutako diru-sarrerak-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="71258-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="71258-198">WIP-salmenten balioa</span><span class="sxs-lookup"><span data-stu-id="71258-198">WIP-sales value</span></span>
    - <span data-ttu-id="71258-199">Metatutako diru-sarrerak-produkzioa</span><span class="sxs-lookup"><span data-stu-id="71258-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="71258-200">WIP-ekoizpena</span><span class="sxs-lookup"><span data-stu-id="71258-200">WIP-production</span></span>
    - <span data-ttu-id="71258-201">Metatutako diru-sarrerak-errentagarritasuna</span><span class="sxs-lookup"><span data-stu-id="71258-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="71258-202">WIP-irabaziak</span><span class="sxs-lookup"><span data-stu-id="71258-202">WIP-profit</span></span>
    - <span data-ttu-id="71258-203">Metatutako diru-sarrera-harpidetza</span><span class="sxs-lookup"><span data-stu-id="71258-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="71258-204">WIP-harpidetza</span><span class="sxs-lookup"><span data-stu-id="71258-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="71258-205">Zergak</span><span class="sxs-lookup"><span data-stu-id="71258-205">Taxes</span></span>

<span data-ttu-id="71258-206">Gastuekin lotutako zergetarako, zehaztu behar duzu zer sartzen den edo gaituta dagoen gastuen txostenetan.</span><span class="sxs-lookup"><span data-stu-id="71258-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="71258-207">**Erabakiak:**</span><span class="sxs-lookup"><span data-stu-id="71258-207">**Decisions:**</span></span>

- <span data-ttu-id="71258-208">Salmenten gaineko zerga sartuta al dago gastuen zenbatekoetan?</span><span class="sxs-lookup"><span data-stu-id="71258-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="71258-209">Zerga berreskuratzea gaitu behar al da gastuetan?</span><span class="sxs-lookup"><span data-stu-id="71258-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="71258-210">Liburu nagusia kontutan hartuta, AEBetako salmenten gaineko zerga aplikatzea eta zerga arauak erabiltzea erabaki baduzu, ezin duzu gastuen gaineko zerga berreskuratzea gaitu.</span><span class="sxs-lookup"><span data-stu-id="71258-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="71258-211">(AEBetako salmenten gaineko zerga aplikatzeko eta zergen arauak erabiltzeko, ezarri **Salmenten gaineko zergen gaineko zergen arauak aplikatzea** aukera **Bai**.)</span><span class="sxs-lookup"><span data-stu-id="71258-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="71258-212">Gidalerroak</span><span class="sxs-lookup"><span data-stu-id="71258-212">Policies</span></span>

<span data-ttu-id="71258-213">Gastuen berri emateko gidalerroak sortuz, zure erakundeari denbora eta dirua aurrezten lagun diezaiokezu langileek bere izenean gastuak sortzen dituztenean.</span><span class="sxs-lookup"><span data-stu-id="71258-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="71258-214">Politikek langileek aurrekontuan jarraituko dutela bermatzen dute, beharrezko informazio guztia eskaintzen dute eta dirua eskatzen duten moduan soilik gastatzen dute.</span><span class="sxs-lookup"><span data-stu-id="71258-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="71258-215">Honako erabaki hauek hartu behar dituzu sortzen dituzun gastuen txosteneko politika bakoitzerako eta gastuen txostenak onartzeko gidalerro bakoitzerako.</span><span class="sxs-lookup"><span data-stu-id="71258-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="71258-216">**Erabakiak:**</span><span class="sxs-lookup"><span data-stu-id="71258-216">**Decisions:**</span></span>

- <span data-ttu-id="71258-217">Nola du izena politikak?</span><span class="sxs-lookup"><span data-stu-id="71258-217">What is the name of the policy?</span></span>
- <span data-ttu-id="71258-218">Zertarako gastu politika?</span><span class="sxs-lookup"><span data-stu-id="71258-218">What is the expense policy for?</span></span>
- <span data-ttu-id="71258-219">Aurretik enpresen arteko gastuak gaitzea erabaki baduzu, zure erakundeko zein enpresari aplikatuko zaie politika hau?</span><span class="sxs-lookup"><span data-stu-id="71258-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="71258-220">Noiz bihurtzen da politika eraginkorra?</span><span class="sxs-lookup"><span data-stu-id="71258-220">When does the policy become effective?</span></span>
- <span data-ttu-id="71258-221">Noiz iraungitzen da politika?</span><span class="sxs-lookup"><span data-stu-id="71258-221">When does the policy expire?</span></span>
- <span data-ttu-id="71258-222">Zein da politika araua?</span><span class="sxs-lookup"><span data-stu-id="71258-222">What is the policy rule?</span></span>
- <span data-ttu-id="71258-223">Zein da politikaren arauaren irteera?</span><span class="sxs-lookup"><span data-stu-id="71258-223">What is the outcome of the policy rule?</span></span>
