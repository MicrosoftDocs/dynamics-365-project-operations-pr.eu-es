---
title: Proiektuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra
description: Gai honek proiektu-lanaren produktuetan oinarritutako eskaintza-lerroak erabiltzeari buruzko lerroei buruzko informazioa ematen du.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: b7076a4b9280472f8c30d0b58c3aa9b9bc86d651
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369856"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="0c634-103">Proiektuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="0c634-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="0c634-104">_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_</span><span class="sxs-lookup"><span data-stu-id="0c634-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="0c634-105">Proiektuetan oinarritutako aurrekontu lerroak proiektu baten konpromisoa kalkulatzen laguntzeko diseinatuta daude.</span><span class="sxs-lookup"><span data-stu-id="0c634-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="0c634-106">Proiektuan oinarritutako aurrekontu lerroaren egitura proiektuaren kalkuluen arabera hedatzen da, honako kontzeptu hauekin:</span><span class="sxs-lookup"><span data-stu-id="0c634-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="0c634-107">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="0c634-107">Billing Method</span></span>
- <span data-ttu-id="0c634-108">Proiektuen eta zereginen esleipena</span><span class="sxs-lookup"><span data-stu-id="0c634-108">Project and Task Mapping</span></span>
- <span data-ttu-id="0c634-109">Transakzio klaseak barne</span><span class="sxs-lookup"><span data-stu-id="0c634-109">Included Transaction classes</span></span>
- <span data-ttu-id="0c634-110">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="0c634-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="0c634-111">Aplikagarritasun konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="0c634-111">Chargeability setup</span></span>
- <span data-ttu-id="0c634-112">Aurrekontua Lerroaren xehetasunak erabiliz</span><span class="sxs-lookup"><span data-stu-id="0c634-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="0c634-113">Eskaintzaren lerroaren bezeroak</span><span class="sxs-lookup"><span data-stu-id="0c634-113">Quote line Customers</span></span>

<span data-ttu-id="0c634-114">Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa.</span><span class="sxs-lookup"><span data-stu-id="0c634-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="0c634-115">Eremu horiei esker, proiektuaren inguruko lanen estimazio zehatza eta zehatza egiteko oinarriak ezartzen dira.</span><span class="sxs-lookup"><span data-stu-id="0c634-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="0c634-116">**Eremua**</span><span class="sxs-lookup"><span data-stu-id="0c634-116">**Field**</span></span> | <span data-ttu-id="0c634-117">**Azalpena**</span><span class="sxs-lookup"><span data-stu-id="0c634-117">**Description**</span></span> | <span data-ttu-id="0c634-118">**Downstream eragina**</span><span class="sxs-lookup"><span data-stu-id="0c634-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="0c634-119">Izena</span><span class="sxs-lookup"><span data-stu-id="0c634-119">Name</span></span> | <span data-ttu-id="0c634-120">Estimatzen ari den aurrekontuaren osagai diskretua identifikatzen laguntzen duen aurrekontuaren lerroaren izena.</span><span class="sxs-lookup"><span data-stu-id="0c634-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="0c634-121">Aurrekontua lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="0c634-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-122">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="0c634-122">Billing Method</span></span> | <span data-ttu-id="0c634-123">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroan dagokion eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="0c634-124">Eremu honek Dynamics 365 Project Operations-ek onartzen dituen bi kontratazio-eredu nagusiak biltzen ditu:</span><span class="sxs-lookup"><span data-stu-id="0c634-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="0c634-125">- Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="0c634-125">- Fixed price</span></span></br><span data-ttu-id="0c634-126">- Denbora eta materiala.</span><span class="sxs-lookup"><span data-stu-id="0c634-126">- Time and material.</span></span>| <span data-ttu-id="0c634-127">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-128">Project</span><span class="sxs-lookup"><span data-stu-id="0c634-128">Project</span></span> | <span data-ttu-id="0c634-129">Erabili aukerako eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="0c634-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="0c634-130">Proiektu bat aurrekontu lerro batera mapeatzen denean, kargagarriak diren atazak ezartzen laguntzen du eta proiektuan oinarritutako aurrekontua aurrekontuaren lerroan aurrekontuaren lerroaren xehetasun gisa ekartzen laguntzen du.</span><span class="sxs-lookup"><span data-stu-id="0c634-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="0c634-131">Proiektu bat proiektuan oinarritutako aurrekontu lerro batera mapatuta ez dagoenean, aurrekontua eskuz sortu beharko litzateke aurrekontu lerroaren xehetasun bakoitza sortuz.</span><span class="sxs-lookup"><span data-stu-id="0c634-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="0c634-132">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="0c634-133">Gehitutako zereginak</span><span class="sxs-lookup"><span data-stu-id="0c634-133">Included Tasks</span></span> | <span data-ttu-id="0c634-134">Aipu lerro hau hautatutako proiektuaren proiektuko zeregin guztietarako edo batzuetarako erabiltzen den adierazten du.</span><span class="sxs-lookup"><span data-stu-id="0c634-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="0c634-135">Eremuak balio hauek izan ditzake:</span><span class="sxs-lookup"><span data-stu-id="0c634-135">This field has the following possible values:</span></span></br><span data-ttu-id="0c634-136">- Proiektuaren zeregin guztiak</span><span class="sxs-lookup"><span data-stu-id="0c634-136">- All project tasks</span></span></br><span data-ttu-id="0c634-137">- Hautatutako proiektu-zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="0c634-137">- Selected project tasks only</span></span></br><span data-ttu-id="0c634-138">Eremu honetako balio hutsa balioaren baliokidea da **Proiektuaren zeregin guztiak** aukera.</span><span class="sxs-lookup"><span data-stu-id="0c634-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="0c634-139">**Aukeratutako proiektuaren zereginak soilik** proiektuaren orrian hautatzen da **Zereginen fakturazio konfigurazioa** fitxak zeregin zehatzak hautatzeko aukera ematen du aurrekontu lerro honekin lotzeko.</span><span class="sxs-lookup"><span data-stu-id="0c634-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="0c634-140">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-141">Idatzi denbora</span><span class="sxs-lookup"><span data-stu-id="0c634-141">Include Time</span></span> | <span data-ttu-id="0c634-142">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="0c634-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-143">**Ez** balioak adierazten du denbora-transakzioak edo lan-kostuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0c634-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-144">**Bai** balioak adierazten du denbora-transakzioak edo lan-kostuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0c634-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="0c634-145">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-146">Idatzi gastua</span><span class="sxs-lookup"><span data-stu-id="0c634-146">Include Expense</span></span> | <span data-ttu-id="0c634-147">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren gastuen kostuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="0c634-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-148">**Ez** balioak adierazten du gastuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0c634-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-149">**Bai** balioak adierazten du gastuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0c634-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="0c634-150">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-151">Sartu materiala</span><span class="sxs-lookup"><span data-stu-id="0c634-151">Include Material</span></span> | <span data-ttu-id="0c634-152">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren materialaren kostuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="0c634-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-153">**Ez** balioa adierazten du materialaren kostuak aurrekontu lerro honetako aurrekontuan ez diren sartuko.</span><span class="sxs-lookup"><span data-stu-id="0c634-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-154">**Bai** balioa adierazten du materialaren kostuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="0c634-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="0c634-155">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-156">Idatzi prezioa</span><span class="sxs-lookup"><span data-stu-id="0c634-156">Include Fee</span></span> | <span data-ttu-id="0c634-157">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren kostuen aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="0c634-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-158">**Ez** balioak adierazten du komisioak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0c634-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="0c634-159">**Bai** balioak adierazten du komisioak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="0c634-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="0c634-160">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-161">Eskainitako zenbatekoa</span><span class="sxs-lookup"><span data-stu-id="0c634-161">Quoted Amount</span></span> | <span data-ttu-id="0c634-162">Proiektuan oinarritutako aurrekontu lerro honetan aurreikusitako lan guztiari bezeroari aipatuko zaion zenbatekoa da.</span><span class="sxs-lookup"><span data-stu-id="0c634-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="0c634-163">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroaren **Bezeroaren aurrekontua** eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="0c634-164">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="0c634-165">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-166">Aurreikusitako zerga</span><span class="sxs-lookup"><span data-stu-id="0c634-166">Estimated Tax</span></span> | <span data-ttu-id="0c634-167">Eremu editagarria da erabiltzaileak aurrekontu lerroan zenbatetsitako zerga kopurua gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="0c634-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="0c634-168">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zerga-zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="0c634-169">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-170">Eskainitako zenbatekoa, zergaren ondoren</span><span class="sxs-lookup"><span data-stu-id="0c634-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="0c634-171">Eremu hau zerga ondorengo aurrekontuaren zenbatekoa da eta irakurtzeko soilik da.</span><span class="sxs-lookup"><span data-stu-id="0c634-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="0c634-172">Eremu honetako zenbatekoa honela kalkulatzen da *Aipatutako zenbatekoa + Zerga*.</span><span class="sxs-lookup"><span data-stu-id="0c634-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="0c634-173">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-174">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="0c634-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="0c634-175">Eremu hau editagarria da eta proiektu bat duten aurrekontu lerroetan soilik dago erabilgarri **Denbora eta materiala** fakturazio metodoa.</span><span class="sxs-lookup"><span data-stu-id="0c634-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="0c634-176">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="0c634-177">Bezeroaren aurrekontua</span><span class="sxs-lookup"><span data-stu-id="0c634-177">Customer Budget</span></span> | <span data-ttu-id="0c634-178">Eremu hau editagarria da eta balio hori aukera-lerroan dagokion eremutik kopiatzen da, abagunea eskaintza batetik sorten bada.</span><span class="sxs-lookup"><span data-stu-id="0c634-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="0c634-179">Balio hori aurrekontua irabazten denean aurrekontu lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="0c634-180">Proiektuetan oinarritutako aurrekontu lerroen Orokorra fitxako eremuen baliozkotze arauak</span><span class="sxs-lookup"><span data-stu-id="0c634-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="0c634-181">**1. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat aurrekontuaren lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="0c634-182">**2. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontu lerro batean bakarrik sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="0c634-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="0c634-183">**3. araua**: **Zereginak barne** eremua **Hautatutako proiektuaren zereginak soilik** gisa ezarrita badago, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontuan sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="0c634-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="0c634-184">**4. araua**: Aukera batek aurrekontu ugari baditu, aurrekontu desberdinetako aurrekontu lerroak egon daitezke, proiektu bera aipatzen dutenak eta transakzio klase bera barne hartzen dutenak.</span><span class="sxs-lookup"><span data-stu-id="0c634-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="0c634-185">**5. araua**: Aurrekontuak aukera berekoak ez badira, ezin dute proiektu eta transakzio klase bera sartu.</span><span class="sxs-lookup"><span data-stu-id="0c634-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="0c634-186">
                    <strong>Abagunea</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="0c634-187">
                    <strong>Eskaintza</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="0c634-188">
                    <strong>Eskaintzaren lerroa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="0c634-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="0c634-190">
                    <strong>Gehitutako zereginak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="0c634-191">
                    <strong>Idatzi denbora</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="0c634-192">
                    <strong>Idatzi gastua</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="0c634-193">
                    <strong>Sartu materiala</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="0c634-194">
                    <strong>Gehitu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="0c634-195">
                    <strong>Tasa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="0c634-196">
                    <strong>Baliozkoa/Baliogabea da</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="0c634-197">
                    <strong>Arrazoia</strong>
                </span><span class="sxs-lookup"><span data-stu-id="0c634-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-198">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-199">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-200">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-201">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-202">Hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-203">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-204">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-205">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-206">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-207">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="0c634-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-208">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="0c634-208">Violation of Rule #2.</span></span> <span data-ttu-id="0c634-209">P1 proiektuaren denbora, gastuak eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude</span><span class="sxs-lookup"><span data-stu-id="0c634-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-210">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-211">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-212">QL2</span><span class="sxs-lookup"><span data-stu-id="0c634-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-213">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-214">Hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-215">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-216">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-217">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-218">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-219">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-220">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-221">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-222">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-223">Hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-224">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-225">No</span><span class="sxs-lookup"><span data-stu-id="0c634-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-226">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-227">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-228">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="0c634-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-229">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="0c634-229">Violation of Rule #2.</span></span> <span data-ttu-id="0c634-230">P1 proiektuaren denbora, materialak eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude</span><span class="sxs-lookup"><span data-stu-id="0c634-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-231">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-232">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-233">QL2</span><span class="sxs-lookup"><span data-stu-id="0c634-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-234">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-235">Hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-236">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-237">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-238">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-239">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-240">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-241">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-242">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-243">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-244">Hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-245">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-246">No</span><span class="sxs-lookup"><span data-stu-id="0c634-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-247">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-248">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-249">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="0c634-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-250">P1 proiektuaren denbora, materialak eta tasak QL1 barne daude</span><span class="sxs-lookup"><span data-stu-id="0c634-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="0c634-251">P1 proiektuaren gastuak QL2n sartzen dira</span><span class="sxs-lookup"><span data-stu-id="0c634-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="0c634-252">Aurrekontu lerro bakoitzean sartzen denaren gainetik ez dago gainjartzerik eta, beraz, baliozkoa da.</span><span class="sxs-lookup"><span data-stu-id="0c634-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-253">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-254">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-255">QL2</span><span class="sxs-lookup"><span data-stu-id="0c634-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-256">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-257">Hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-258">No</span><span class="sxs-lookup"><span data-stu-id="0c634-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-259">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-260">No</span><span class="sxs-lookup"><span data-stu-id="0c634-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-261">No</span><span class="sxs-lookup"><span data-stu-id="0c634-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-262">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-263">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-264">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-265">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-266">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="0c634-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-267">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-268">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-269">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-270">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-271">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="0c634-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-272">2. araua haustea</span><span class="sxs-lookup"><span data-stu-id="0c634-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="0c634-273">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira</span><span class="sxs-lookup"><span data-stu-id="0c634-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="0c634-274">QL2-k P1 proiektu osorako denbora, gastuak eta tasak biltzen ditu eta, beraz, Q1-en sartutakoarekin gainjartzen da.</span><span class="sxs-lookup"><span data-stu-id="0c634-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-275">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-276">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-277">QL2</span><span class="sxs-lookup"><span data-stu-id="0c634-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-278">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-279">Hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-280">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-281">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-282">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-283">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-284">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-285">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-286">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-287">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-288">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="0c634-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-289">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-290">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-291">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-292">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-293">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="0c634-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-294">3. arauaren arabera,</span><span class="sxs-lookup"><span data-stu-id="0c634-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="0c634-295">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="0c634-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="0c634-296">QL2k proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="0c634-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="0c634-297">Balidazio osagarri bakarra QL1-eko zereginen azpimultzoaren inguruan kokatzen da, QL2-ren zereginen azpimultzoaren desberdina dela gainjartzerik ez dagoela ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="0c634-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="0c634-298">Sistemak zereginak lotzen dituenean egiten du.</span><span class="sxs-lookup"><span data-stu-id="0c634-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-299">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-300">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-301">QL2</span><span class="sxs-lookup"><span data-stu-id="0c634-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-302">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-303">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="0c634-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-304">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-305">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-306">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-307">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-308">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-309">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-310">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-311">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-312">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-313">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-314">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-315">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-316">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-317">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="0c634-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-318">5. arauaren arabera, Q1 eta Q2 aukera berdineko bi komatxo dira, beraz, biek proiektu baten osagai berberak kalkula ditzakete.</span><span class="sxs-lookup"><span data-stu-id="0c634-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-319">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-320">2H</span><span class="sxs-lookup"><span data-stu-id="0c634-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-321">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-322">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-323">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-324">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-325">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-326">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-327">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-328">O1</span><span class="sxs-lookup"><span data-stu-id="0c634-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-329">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-330">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-331">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-332">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-333">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-334">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-335">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-336">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-337">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="0c634-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="0c634-338">4. arauaren arabera, Q1 eta Q2 aukera desberrdineko bi komatxo dira, beraz, biek proiektu berean osagai berberak kalkula ditzakete.</span><span class="sxs-lookup"><span data-stu-id="0c634-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="0c634-339">O2</span><span class="sxs-lookup"><span data-stu-id="0c634-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="0c634-340">1H</span><span class="sxs-lookup"><span data-stu-id="0c634-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="0c634-341">QL1</span><span class="sxs-lookup"><span data-stu-id="0c634-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-342">A1</span><span class="sxs-lookup"><span data-stu-id="0c634-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="0c634-343">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="0c634-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="0c634-344">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="0c634-345">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="0c634-346">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="0c634-347">Yes</span><span class="sxs-lookup"><span data-stu-id="0c634-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
