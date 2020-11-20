---
title: Proiektuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra - arina
description: Gai honek proiektu-lanaren produktuetan oinarritutako eskaintza-lerroak erabiltzeari buruzko lerroei buruzko informazioa ematen du. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: be1663c0d226fa19fe4b9df566e16d215f1fc08e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181077"
---
# <a name="project-based-quote-lines-overview---lite"></a><span data-ttu-id="3ac28-104">Proiektuetan oinarritutako eskaintzaren lerroen ikuspegi orokorra - arina</span><span class="sxs-lookup"><span data-stu-id="3ac28-104">Project-based quote lines overview - lite</span></span>

<span data-ttu-id="3ac28-105">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="3ac28-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3ac28-106">Proiektuetan oinarritutako aurrekontu lerroak proiektu baten konpromisoa kalkulatzen laguntzeko diseinatuta daude.</span><span class="sxs-lookup"><span data-stu-id="3ac28-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="3ac28-107">Proiektuan oinarritutako aurrekontu lerroaren egitura proiektuaren kalkuluen arabera hedatzen da, honako kontzeptu hauekin:</span><span class="sxs-lookup"><span data-stu-id="3ac28-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="3ac28-108">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-108">Billing Method</span></span>
- <span data-ttu-id="3ac28-109">Proiektuen eta zereginen esleipena</span><span class="sxs-lookup"><span data-stu-id="3ac28-109">Project and Task Mapping</span></span>
- <span data-ttu-id="3ac28-110">Transakzio klaseak barne</span><span class="sxs-lookup"><span data-stu-id="3ac28-110">Included Transaction classes</span></span>
- <span data-ttu-id="3ac28-111">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="3ac28-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="3ac28-112">Aplikagarritasun konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="3ac28-112">Chargeability setup</span></span>
- <span data-ttu-id="3ac28-113">Aurrekontua Lerroaren xehetasunak erabiliz</span><span class="sxs-lookup"><span data-stu-id="3ac28-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="3ac28-114">Eskaintzaren lerroaren bezeroak</span><span class="sxs-lookup"><span data-stu-id="3ac28-114">Quote line Customers</span></span>

<span data-ttu-id="3ac28-115">Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa.</span><span class="sxs-lookup"><span data-stu-id="3ac28-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="3ac28-116">Eremu horiei esker, proiektuaren inguruko lanen estimazio zehatza eta zehatza egiteko oinarriak ezartzen dira.</span><span class="sxs-lookup"><span data-stu-id="3ac28-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="3ac28-117">**Eremua**</span><span class="sxs-lookup"><span data-stu-id="3ac28-117">**Field**</span></span> | <span data-ttu-id="3ac28-118">**Azalpena**</span><span class="sxs-lookup"><span data-stu-id="3ac28-118">**Description**</span></span> | <span data-ttu-id="3ac28-119">**Downstream eragina**</span><span class="sxs-lookup"><span data-stu-id="3ac28-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="3ac28-120">Eman izena</span><span class="sxs-lookup"><span data-stu-id="3ac28-120">Name</span></span> | <span data-ttu-id="3ac28-121">Estimatzen ari den aurrekontuaren osagai diskretua identifikatzen lagunduko dizun aurrekontuaren lerroaren izena.</span><span class="sxs-lookup"><span data-stu-id="3ac28-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="3ac28-122">Aurrekontua lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-123">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-123">Billing Method</span></span> | <span data-ttu-id="3ac28-124">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroan dagokion eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="3ac28-125">Eremu honek Dynamics 365 Project Operations-ek onartzen dituen kontratazio eredu nagusiak biltzen ditu:</span><span class="sxs-lookup"><span data-stu-id="3ac28-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="3ac28-126">- Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-126">- Fixed price</span></span></br><span data-ttu-id="3ac28-127">- Denbora eta materiala.</span><span class="sxs-lookup"><span data-stu-id="3ac28-127">- Time and material.</span></span>| <span data-ttu-id="3ac28-128">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-129">Project</span><span class="sxs-lookup"><span data-stu-id="3ac28-129">Project</span></span> | <span data-ttu-id="3ac28-130">Erabili aukerako eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="3ac28-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="3ac28-131">Proiektu bat aurrekontu lerro batera mapeatzen denean, kargagarriak diren atazak ezartzen laguntzen du eta proiektuan oinarritutako aurrekontua aurrekontuaren lerroan aurrekontuaren lerroaren xehetasun gisa ekartzen laguntzen du.</span><span class="sxs-lookup"><span data-stu-id="3ac28-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="3ac28-132">Proiektu bat proiektuan oinarritutako aurrekontu lerro batera mapatuta ez dagoenean, aurrekontua eskuz sortu beharko litzateke aurrekontu lerroaren xehetasun bakoitza sortuz.</span><span class="sxs-lookup"><span data-stu-id="3ac28-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="3ac28-133">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="3ac28-134">Gehitutako zereginak</span><span class="sxs-lookup"><span data-stu-id="3ac28-134">Included Tasks</span></span> | <span data-ttu-id="3ac28-135">Aipu lerro hau hautatutako proiektuaren proiektuko zeregin guztietarako edo batzuetarako erabiltzen den adierazten du.</span><span class="sxs-lookup"><span data-stu-id="3ac28-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="3ac28-136">Eremuak balio hauek izan ditzake:</span><span class="sxs-lookup"><span data-stu-id="3ac28-136">This field has the following possible values:</span></span></br><span data-ttu-id="3ac28-137">- Proiektuaren zeregin guztiak</span><span class="sxs-lookup"><span data-stu-id="3ac28-137">- All project tasks</span></span></br><span data-ttu-id="3ac28-138">- Hautatutako proiektu-zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="3ac28-138">- Selected project tasks only</span></span></br><span data-ttu-id="3ac28-139">Eremu honetako balio hutsa balioaren baliokidea da **Proiektuaren zeregin guztiak** aukera.</span><span class="sxs-lookup"><span data-stu-id="3ac28-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="3ac28-140">**Aukeratutako proiektuaren zereginak soilik** hautatzen denean proiektuaren orrian, **Zereginen fakturazio konfigurazioa** fitxak zeregin zehatzak hautatzeko aukera ematen du aurrekontu lerro honekin lotzeko.</span><span class="sxs-lookup"><span data-stu-id="3ac28-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="3ac28-141">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-142">Idatzi denbora</span><span class="sxs-lookup"><span data-stu-id="3ac28-142">Include Time</span></span> | <span data-ttu-id="3ac28-143">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="3ac28-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="3ac28-144">**Ez** balioak adierazten du denbora-transakzioak edo lan-kostuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="3ac28-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="3ac28-145">**Bai** balioak adierazten du denbora-transakzioak edo lan-kostuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="3ac28-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="3ac28-146">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-147">Idatzi gastua</span><span class="sxs-lookup"><span data-stu-id="3ac28-147">Include Expense</span></span> | <span data-ttu-id="3ac28-148">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako gastuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="3ac28-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="3ac28-149">**Ez** balioak adierazten du gastuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="3ac28-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="3ac28-150">**Bai** balioak adierazten du gastuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="3ac28-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="3ac28-151">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerro baten gainean kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-152">Idatzi prezioa</span><span class="sxs-lookup"><span data-stu-id="3ac28-152">Include Fee</span></span> | <span data-ttu-id="3ac28-153">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako komisioak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="3ac28-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="3ac28-154">**Ez** balioak adierazten du komisioak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="3ac28-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="3ac28-155">**Bai** balioak adierazten du komisioak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="3ac28-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="3ac28-156">Eremuaren balioa eskaintzaren lerro honetatik sortzen den Proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-157">Eskainitako zenbatekoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-157">Quoted Amount</span></span> | <span data-ttu-id="3ac28-158">Proiektuan oinarritutako aurrekontu lerro honetan aurreikusitako lan guztiari bezeroari aipatuko zaion zenbatekoa da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="3ac28-159">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroaren **Bezeroaren aurrekontua** eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="3ac28-160">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="3ac28-161">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-162">Aurreikusitako zerga</span><span class="sxs-lookup"><span data-stu-id="3ac28-162">Estimated Tax</span></span> | <span data-ttu-id="3ac28-163">Eremu editagarria da erabiltzaileak aurrekontu lerroan zenbatetsitako zerga kopurua gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="3ac28-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="3ac28-164">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zerga-zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="3ac28-165">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-166">Eskainitako zenbatekoa, zergaren ondoren</span><span class="sxs-lookup"><span data-stu-id="3ac28-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="3ac28-167">Eremu hau zerga ondorengo aurrekontuaren zenbatekoa da eta irakurtzeko soilik da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="3ac28-168">Eremu honetako zenbatekoa honela kalkulatzen da *Aipatutako zenbatekoa + Zerga*.</span><span class="sxs-lookup"><span data-stu-id="3ac28-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="3ac28-169">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-170">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="3ac28-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="3ac28-171">Eremu hau editagarria da eta proiektu bat duten aurrekontu lerroetan soilik dago erabilgarri **Denbora eta materiala** fakturazio metodoa.</span><span class="sxs-lookup"><span data-stu-id="3ac28-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="3ac28-172">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="3ac28-173">Bezeroaren aurrekontua</span><span class="sxs-lookup"><span data-stu-id="3ac28-173">Customer Budget</span></span> | <span data-ttu-id="3ac28-174">Eremu hau editagarria da eta balio hori aukera-lerroan dagokion eremutik kopiatzen da, abagunea eskaintza batetik sorten bada.</span><span class="sxs-lookup"><span data-stu-id="3ac28-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="3ac28-175">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="3ac28-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="3ac28-176">Proiektuetan oinarritutako aurrekontu lerroen Orokorra fitxako eremuen baliozkotze arauak</span><span class="sxs-lookup"><span data-stu-id="3ac28-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="3ac28-177">**1. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat aurrekontuaren lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="3ac28-178">**2. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontu lerro batean bakarrik sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="3ac28-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="3ac28-179">**3. araua**: **Zereginak barne** eremua **Hautatutako proiektuaren zereginak soilik** gisa ezarrita badago, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontuan sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="3ac28-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="3ac28-180">**4. araua**: Aukera batek aurrekontu ugari baditu, aurrekontu desberdinetako aurrekontu lerroak egon daitezke, proiektu bera aipatzen dutenak eta transakzio klase bera barne hartzen dutenak.</span><span class="sxs-lookup"><span data-stu-id="3ac28-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="3ac28-181">**5. araua**: Aurrekontuak aukera berekoak ez badira, ezin dute proiektu eta transakzio klase bera sartu.</span><span class="sxs-lookup"><span data-stu-id="3ac28-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="3ac28-182">
                    <strong>Abagunea</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="3ac28-183">
                    <strong>Eskaintza</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="3ac28-184">
                    <strong>Eskaintzaren lerroa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="3ac28-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="3ac28-186">
                    <strong>Gehitutako zereginak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="3ac28-187">
                    <strong>Idatzi denbora</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="3ac28-188">
                    <strong>Idatzi gastua</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="3ac28-189">
                    <strong>Sartu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="3ac28-190">
                    <strong>Prezioa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="3ac28-191">
                    <strong>Baliozkoa/Baliogabea da</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="3ac28-192">
                    <strong>Arrazoia</strong>
                </span><span class="sxs-lookup"><span data-stu-id="3ac28-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-193">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-194">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-195">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-196">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-197">Hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-198">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-199">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-200">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-201">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="3ac28-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-202">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="3ac28-202">Violation of Rule #2.</span></span> <span data-ttu-id="3ac28-203">P1 proiektuaren denbora, gastuak eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="3ac28-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-204">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-205">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-206">QL2</span><span class="sxs-lookup"><span data-stu-id="3ac28-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-207">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-208">Hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-209">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-210">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-211">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-211">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-212">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-213">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-214">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-215">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-216">Hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-217">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-218">+Ez</span><span class="sxs-lookup"><span data-stu-id="3ac28-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-219">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-220">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="3ac28-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-221">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="3ac28-221">Violation of Rule #2.</span></span> <span data-ttu-id="3ac28-222">P1 proiektuaren denbora eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="3ac28-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-223">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-224">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-225">QL2</span><span class="sxs-lookup"><span data-stu-id="3ac28-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-226">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-227">Hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-228">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-229">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-230">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-230">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-231">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-232">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-233">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-234">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-235">Hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-236">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-237">+Ez</span><span class="sxs-lookup"><span data-stu-id="3ac28-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-238">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-239">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="3ac28-240">P1 proiektuaren denbora eta tasak QL1-en sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="3ac28-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="3ac28-241">P1 proiektuaren gastuak QL2n sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="3ac28-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="3ac28-242">Aurrekontu lerro bakoitzean sartzen den horretan ez dago gainjartzerik, eta balio du.</span><span class="sxs-lookup"><span data-stu-id="3ac28-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-243">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-244">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-245">QL2</span><span class="sxs-lookup"><span data-stu-id="3ac28-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-246">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-247">Hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-248">+Ez</span><span class="sxs-lookup"><span data-stu-id="3ac28-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-249">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-250">+Ez</span><span class="sxs-lookup"><span data-stu-id="3ac28-250">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-251">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-252">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-253">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-254">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-255">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="3ac28-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-256">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-257">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-258">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-259">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="3ac28-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-260">2. araua haustea eta gehiago</span><span class="sxs-lookup"><span data-stu-id="3ac28-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="3ac28-261">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="3ac28-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="3ac28-262">QL2-k P1 proiektu osorako Denbora, Gastuak eta Tasak barne hartzen ditu eta Q1-n sartutakoarekin gainjartzen da.</span><span class="sxs-lookup"><span data-stu-id="3ac28-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-263">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-264">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-265">QL2</span><span class="sxs-lookup"><span data-stu-id="3ac28-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-266">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-267">Hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-268">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-269">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-270">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-270">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-271">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-272">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-273">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-274">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-275">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="3ac28-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-276">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-277">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-278">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-279">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-280">3. arauaren eta abarren arabera,</span><span class="sxs-lookup"><span data-stu-id="3ac28-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="3ac28-281">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="3ac28-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="3ac28-282">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="3ac28-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="3ac28-283">Balidazio osagarri bakarra QL1-eko zereginen azpimultzoaren inguruan kokatzen da, QL2-ren zereginen azpimultzoarekin alderatuta.</span><span class="sxs-lookup"><span data-stu-id="3ac28-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="3ac28-284">Honek gainjartzerik ez dagoela ziurtatzen du.</span><span class="sxs-lookup"><span data-stu-id="3ac28-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="3ac28-285">Sistemak zereginak lotzen dituenean egiten du.</span><span class="sxs-lookup"><span data-stu-id="3ac28-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-286">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-287">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-288">QL2</span><span class="sxs-lookup"><span data-stu-id="3ac28-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-289">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-290">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="3ac28-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-291">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-292">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-293">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-293">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-294">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-295">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-296">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-297">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-298">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-299">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-300">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-301">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="3ac28-302">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-303">5. arauan oinarrituta, Q1 eta Q2 aukera berdineko bi komatxo dira, beraz, biek proiektu baten osagai berberak kalkula ditzakete.</span><span class="sxs-lookup"><span data-stu-id="3ac28-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-304">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-305">2H</span><span class="sxs-lookup"><span data-stu-id="3ac28-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-306">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-307">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-308">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-309">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-310">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-311">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-311">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-312">O1</span><span class="sxs-lookup"><span data-stu-id="3ac28-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-313">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-314">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-315">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-316">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-317">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-318">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-319">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="3ac28-320">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="3ac28-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="3ac28-321">4. arauan oinarrituta, Q1 eta Q2 aukera desberdineko bi komatxo dira, beraz, proiektu berean ezin dira osagai berberak kalkulatu.</span><span class="sxs-lookup"><span data-stu-id="3ac28-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="3ac28-322">O2</span><span class="sxs-lookup"><span data-stu-id="3ac28-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="3ac28-323">1H</span><span class="sxs-lookup"><span data-stu-id="3ac28-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-324">QL1</span><span class="sxs-lookup"><span data-stu-id="3ac28-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-325">A1</span><span class="sxs-lookup"><span data-stu-id="3ac28-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="3ac28-326">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="3ac28-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-327">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="3ac28-328">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="3ac28-329">Yes</span><span class="sxs-lookup"><span data-stu-id="3ac28-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="3ac28-330">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="3ac28-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

