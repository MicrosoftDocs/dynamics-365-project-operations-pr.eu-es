---
title: Proiektuetan oinarritutako eskaintzaren lerroak (Pro)
description: Gai honek proiektu-lanaren produktuetan oinarritutako eskaintza-lerroak erabiltzeari buruzko lerroei buruzko informazioa ematen du. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907837"
---
# <a name="project-based-quote-lines-pro"></a><span data-ttu-id="b61da-104">Proiektuetan oinarritutako eskaintzaren lerroak (Pro)</span><span class="sxs-lookup"><span data-stu-id="b61da-104">Project-based quote lines (Pro)</span></span>

<span data-ttu-id="b61da-105">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="b61da-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b61da-106">Proiektuetan oinarritutako aurrekontu lerroak proiektu baten konpromisoa kalkulatzen laguntzeko diseinatuta daude.</span><span class="sxs-lookup"><span data-stu-id="b61da-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="b61da-107">Proiektuan oinarritutako aurrekontu lerroaren egitura proiektuaren kalkuluen arabera hedatzen da, honako kontzeptu hauekin:</span><span class="sxs-lookup"><span data-stu-id="b61da-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="b61da-108">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="b61da-108">Billing Method</span></span>
- <span data-ttu-id="b61da-109">Proiektuen eta zereginen esleipena</span><span class="sxs-lookup"><span data-stu-id="b61da-109">Project and Task Mapping</span></span>
- <span data-ttu-id="b61da-110">Transakzio klaseak barne</span><span class="sxs-lookup"><span data-stu-id="b61da-110">Included Transaction classes</span></span>
- <span data-ttu-id="b61da-111">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="b61da-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="b61da-112">Aplikagarritasun konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="b61da-112">Chargeability setup</span></span>
- <span data-ttu-id="b61da-113">Aurrekontua Lerroaren xehetasunak erabiliz</span><span class="sxs-lookup"><span data-stu-id="b61da-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="b61da-114">Eskaintzaren lerroaren bezeroak</span><span class="sxs-lookup"><span data-stu-id="b61da-114">Quote line Customers</span></span>

<span data-ttu-id="b61da-115">Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa.</span><span class="sxs-lookup"><span data-stu-id="b61da-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="b61da-116">Eremu horiei esker, proiektuaren inguruko lanen estimazio zehatza eta zehatza egiteko oinarriak ezartzen dira.</span><span class="sxs-lookup"><span data-stu-id="b61da-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="b61da-117">**Eremua**</span><span class="sxs-lookup"><span data-stu-id="b61da-117">**Field**</span></span> | <span data-ttu-id="b61da-118">**Garrantzia, xedea eta orientazioa**</span><span class="sxs-lookup"><span data-stu-id="b61da-118">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="b61da-119">**Downstream eragina**</span><span class="sxs-lookup"><span data-stu-id="b61da-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="b61da-120">Izena</span><span class="sxs-lookup"><span data-stu-id="b61da-120">Name</span></span> | <span data-ttu-id="b61da-121">Estimatzen ari den aurrekontuaren osagai diskretua identifikatzen lagunduko dizun aurrekontuaren lerroaren izena.</span><span class="sxs-lookup"><span data-stu-id="b61da-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="b61da-122">Aurrekontua lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-123">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="b61da-123">Billing Method</span></span> | <span data-ttu-id="b61da-124">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroan dagokion eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="b61da-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="b61da-125">Eremu honek Dynamics 365 Project Operations-ek onartzen dituen kontratazio eredu nagusiak biltzen ditu:</span><span class="sxs-lookup"><span data-stu-id="b61da-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="b61da-126">- Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="b61da-126">- Fixed price</span></span></br><span data-ttu-id="b61da-127">- Denbora eta materiala.</span><span class="sxs-lookup"><span data-stu-id="b61da-127">- Time and material.</span></span>| <span data-ttu-id="b61da-128">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-129">Project</span><span class="sxs-lookup"><span data-stu-id="b61da-129">Project</span></span> | <span data-ttu-id="b61da-130">Erabili aukerako eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="b61da-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="b61da-131">Proiektu bat aurrekontu lerro batera mapeatzen denean, kargagarriak diren atazak ezartzen laguntzen du eta proiektuan oinarritutako aurrekontua aurrekontuaren lerroan aurrekontuaren lerroaren xehetasun gisa ekartzen laguntzen du.</span><span class="sxs-lookup"><span data-stu-id="b61da-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="b61da-132">Proiektu bat proiektuan oinarritutako aurrekontu lerro batera mapatuta ez dagoenean, aurrekontua eskuz sortu beharko litzateke aurrekontu lerroaren xehetasun bakoitza sortuz.</span><span class="sxs-lookup"><span data-stu-id="b61da-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="b61da-133">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="b61da-134">Gehitutako zereginak</span><span class="sxs-lookup"><span data-stu-id="b61da-134">Included Tasks</span></span> | <span data-ttu-id="b61da-135">Aipu lerro hau hautatutako proiektuaren proiektuko zeregin guztietarako edo batzuetarako erabiltzen den adierazten du.</span><span class="sxs-lookup"><span data-stu-id="b61da-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="b61da-136">Eremuak balio hauek izan ditzake:</span><span class="sxs-lookup"><span data-stu-id="b61da-136">This field has the following possible values:</span></span></br><span data-ttu-id="b61da-137">- Proiektuaren zeregin guztiak</span><span class="sxs-lookup"><span data-stu-id="b61da-137">- All project tasks</span></span></br><span data-ttu-id="b61da-138">- Hautatutako proiektu-zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="b61da-138">- Selected project tasks only</span></span></br><span data-ttu-id="b61da-139">Eremu honetako balio hutsa balioaren baliokidea da **Proiektuaren zeregin guztiak** aukera.</span><span class="sxs-lookup"><span data-stu-id="b61da-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="b61da-140">**Aukeratutako proiektuaren zereginak soilik** hautatzen denean proiektuaren orrian, **Zereginen fakturazio konfigurazioa** fitxak zeregin zehatzak hautatzeko aukera ematen du aurrekontu lerro honekin lotzeko.</span><span class="sxs-lookup"><span data-stu-id="b61da-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="b61da-141">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-142">Idatzi denbora</span><span class="sxs-lookup"><span data-stu-id="b61da-142">Include Time</span></span> | <span data-ttu-id="b61da-143">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="b61da-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="b61da-144">**Ez** balioak adierazten du denbora-transakzioak edo lan-kostuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="b61da-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="b61da-145">**Bai** balioak adierazten du denbora-transakzioak edo lan-kostuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="b61da-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="b61da-146">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-147">Idatzi gastua</span><span class="sxs-lookup"><span data-stu-id="b61da-147">Include Expense</span></span> | <span data-ttu-id="b61da-148">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako gastuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="b61da-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="b61da-149">**Ez** balioak adierazten du gastuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="b61da-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="b61da-150">**Bai** balioak adierazten du gastuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="b61da-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="b61da-151">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerro baten gainean kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-152">Idatzi prezioa</span><span class="sxs-lookup"><span data-stu-id="b61da-152">Include Fee</span></span> | <span data-ttu-id="b61da-153">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako komisioak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="b61da-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="b61da-154">**Ez** balioak adierazten du komisioak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="b61da-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="b61da-155">**Bai** balioak adierazten du komisioak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="b61da-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="b61da-156">Eremuaren balioa eskaintzaren lerro honetatik sortzen den Proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-157">Eskainitako zenbatekoa</span><span class="sxs-lookup"><span data-stu-id="b61da-157">Quoted Amount</span></span> | <span data-ttu-id="b61da-158">Proiektuan oinarritutako aurrekontu lerro honetan aurreikusitako lan guztiari bezeroari aipatuko zaion zenbatekoa da.</span><span class="sxs-lookup"><span data-stu-id="b61da-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="b61da-159">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroaren **Bezeroaren aurrekontua** eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="b61da-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="b61da-160">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="b61da-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="b61da-161">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-162">Aurreikusitako zerga</span><span class="sxs-lookup"><span data-stu-id="b61da-162">Estimated Tax</span></span> | <span data-ttu-id="b61da-163">Eremu editagarria da erabiltzaileak aurrekontu lerroan zenbatetsitako zerga kopurua gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="b61da-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="b61da-164">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zerga-zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="b61da-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="b61da-165">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-166">Eskainitako zenbatekoa, zergaren ondoren</span><span class="sxs-lookup"><span data-stu-id="b61da-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="b61da-167">Eremu hau zerga ondorengo aurrekontuaren zenbatekoa da eta irakurtzeko soilik da.</span><span class="sxs-lookup"><span data-stu-id="b61da-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="b61da-168">Eremu honetako zenbatekoa honela kalkulatzen da *Aipatutako zenbatekoa + Zerga*.</span><span class="sxs-lookup"><span data-stu-id="b61da-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="b61da-169">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-170">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="b61da-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="b61da-171">Eremu hau editagarria da eta proiektu bat duten aurrekontu lerroetan soilik dago erabilgarri **Denbora eta materiala** fakturazio metodoa.</span><span class="sxs-lookup"><span data-stu-id="b61da-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="b61da-172">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="b61da-173">Bezeroaren aurrekontua</span><span class="sxs-lookup"><span data-stu-id="b61da-173">Customer Budget</span></span> | <span data-ttu-id="b61da-174">Eremu hau editagarria da eta balio hori aukera-lerroan dagokion eremutik kopiatzen da, abagunea eskaintza batetik sorten bada.</span><span class="sxs-lookup"><span data-stu-id="b61da-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="b61da-175">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="b61da-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="b61da-176">Proiektuetan oinarritutako aurrekontu lerroen Orokorra fitxako eremuen baliozkotze arauak</span><span class="sxs-lookup"><span data-stu-id="b61da-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="b61da-177">**1. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat aurrekontuaren lerroan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="b61da-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="b61da-178">**2. araua**: **Zereginak barne** eremua hutsik badago, edo ezarrita badago **Proiektuaren zeregin guztiak**, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontu lerro batean bakarrik sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="b61da-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="b61da-179">**3. araua**: **Zereginak barne** eremua **Hautatutako proiektuaren zereginak soilik** gisa ezarrita badago, proiektu bat eta transakzio klase jakin bat aurrekontuaren proiektuan oinarritutako aurrekontuan sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="b61da-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="b61da-180">**4. araua**: Aukera batek aurrekontu ugari baditu, aurrekontu desberdinetako aurrekontu lerroak egon daitezke, proiektu bera aipatzen dutenak eta transakzio klase bera barne hartzen dutenak.</span><span class="sxs-lookup"><span data-stu-id="b61da-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="b61da-181">**5. araua**: Aurrekontuak aukera berekoak ez badira, ezin dute proiektu eta transakzio klase bera sartu.</span><span class="sxs-lookup"><span data-stu-id="b61da-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="b61da-182">
                    <strong>Abagunea</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="b61da-183">
                    <strong>Eskaintza</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="b61da-184">
                    <strong>Eskaintzaren lerroa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="b61da-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="b61da-186">
                    <strong>Gehitutako zereginak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="b61da-187">
                    <strong>Idatzi denbora</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="b61da-188">
                    <strong>Idatzi gastua</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="b61da-189">
                    <strong>Sartu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="b61da-190">
                    <strong>Prezioa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="b61da-191">
                    <strong>Baliozkoa/Baliogabea da</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="b61da-192">
                    <strong>Arrazoia</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b61da-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-193">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-194">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-195">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-196">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-197">Hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-198">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-199">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-200">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-201">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="b61da-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-202">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="b61da-202">Violation of Rule #2.</span></span> <span data-ttu-id="b61da-203">P1 proiektuaren denbora, gastuak eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="b61da-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-204">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-205">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-206">QL2</span><span class="sxs-lookup"><span data-stu-id="b61da-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-207">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-208">Hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-209">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-210">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-211">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-211">Yes</span></span> </p>
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
<span data-ttu-id="b61da-212">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-213">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-214">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-215">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-216">Hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-217">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-218">+Ez</span><span class="sxs-lookup"><span data-stu-id="b61da-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-219">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-220">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="b61da-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-221">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="b61da-221">Violation of Rule #2.</span></span> <span data-ttu-id="b61da-222">P1 proiektuaren denbora eta tasak aurrekontu lerroetan, QL1 eta QL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="b61da-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-223">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-224">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-225">QL2</span><span class="sxs-lookup"><span data-stu-id="b61da-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-226">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-227">Hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-228">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-229">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-230">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-230">Yes</span></span> </p>
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
<span data-ttu-id="b61da-231">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-232">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-233">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-234">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-235">Hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-236">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-237">+Ez</span><span class="sxs-lookup"><span data-stu-id="b61da-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-238">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-239">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="b61da-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="b61da-240">P1 proiektuaren denbora eta tasak QL1-en sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="b61da-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="b61da-241">P1 proiektuaren gastuak QL2n sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="b61da-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="b61da-242">Aurrekontu lerro bakoitzean sartzen den horretan ez dago gainjartzerik, eta balio du.</span><span class="sxs-lookup"><span data-stu-id="b61da-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-243">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-244">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-245">QL2</span><span class="sxs-lookup"><span data-stu-id="b61da-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-246">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-247">Hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-248">+Ez</span><span class="sxs-lookup"><span data-stu-id="b61da-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-249">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-250">+Ez</span><span class="sxs-lookup"><span data-stu-id="b61da-250">No</span></span> </p>
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
<span data-ttu-id="b61da-251">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-252">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-253">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-254">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-255">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="b61da-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-256">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-257">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-258">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-259">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="b61da-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-260">2. araua haustea eta gehiago</span><span class="sxs-lookup"><span data-stu-id="b61da-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="b61da-261">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="b61da-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="b61da-262">QL2-k P1 proiektu osorako Denbora, Gastuak eta Tasak barne hartzen ditu eta Q1-n sartutakoarekin gainjartzen da.</span><span class="sxs-lookup"><span data-stu-id="b61da-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-263">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-264">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-265">QL2</span><span class="sxs-lookup"><span data-stu-id="b61da-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-266">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-267">Hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-268">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-269">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-270">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-270">Yes</span></span> </p>
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
<span data-ttu-id="b61da-271">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-272">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-273">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-274">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-275">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="b61da-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-276">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-277">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-278">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-279">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="b61da-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-280">3. arauaren eta abarren arabera,</span><span class="sxs-lookup"><span data-stu-id="b61da-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="b61da-281">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="b61da-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="b61da-282">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="b61da-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="b61da-283">Balidazio osagarri bakarra QL1-eko zereginen azpimultzoaren inguruan kokatzen da, QL2-ren zereginen azpimultzoarekin alderatuta.</span><span class="sxs-lookup"><span data-stu-id="b61da-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="b61da-284">Honek gainjartzerik ez dagoela ziurtatzen du.</span><span class="sxs-lookup"><span data-stu-id="b61da-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="b61da-285">Sistemak zereginak lotzen dituenean egiten du.</span><span class="sxs-lookup"><span data-stu-id="b61da-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-286">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-287">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-288">QL2</span><span class="sxs-lookup"><span data-stu-id="b61da-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-289">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-290">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="b61da-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-291">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-292">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-293">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-293">Yes</span></span> </p>
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
<span data-ttu-id="b61da-294">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-295">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-296">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-297">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-298">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-299">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-300">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-301">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="b61da-302">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="b61da-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-303">5. arauan oinarrituta, Q1 eta Q2 aukera berdineko bi komatxo dira, beraz, biek proiektu baten osagai berberak kalkula ditzakete.</span><span class="sxs-lookup"><span data-stu-id="b61da-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-304">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-305">2H</span><span class="sxs-lookup"><span data-stu-id="b61da-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-306">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-307">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-308">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-309">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-310">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-311">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-311">Yes</span></span> </p>
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
<span data-ttu-id="b61da-312">O1</span><span class="sxs-lookup"><span data-stu-id="b61da-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-313">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-314">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-315">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-316">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-317">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-318">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-319">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="b61da-320">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="b61da-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="b61da-321">4. arauan oinarrituta, Q1 eta Q2 aukera desberdineko bi komatxo dira, beraz, proiektu berean ezin dira osagai berberak kalkulatu.</span><span class="sxs-lookup"><span data-stu-id="b61da-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="b61da-322">O2</span><span class="sxs-lookup"><span data-stu-id="b61da-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="b61da-323">1H</span><span class="sxs-lookup"><span data-stu-id="b61da-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-324">QL1</span><span class="sxs-lookup"><span data-stu-id="b61da-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-325">A1</span><span class="sxs-lookup"><span data-stu-id="b61da-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="b61da-326">Proiektuaren zeregin guztiak edo hutsik</span><span class="sxs-lookup"><span data-stu-id="b61da-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-327">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="b61da-328">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="b61da-329">Yes</span><span class="sxs-lookup"><span data-stu-id="b61da-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="b61da-330">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="b61da-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

