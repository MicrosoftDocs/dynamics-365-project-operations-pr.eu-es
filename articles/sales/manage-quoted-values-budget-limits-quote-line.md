---
title: Proiektuetan oinarritutako eskaintzaren lerroak
description: Gai honek proiektu-lanaren produktuetan oinarritutako eskaintza-lerroak erabiltzeari buruzko lerroei buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 06a47c45dc3b3b174658e2fba14d3d2050aabf85
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070903"
---
# <a name="project-based-quote-lines"></a><span data-ttu-id="e9be9-103">Proiektuetan oinarritutako eskaintzaren lerroak</span><span class="sxs-lookup"><span data-stu-id="e9be9-103">Project-based quote lines</span></span>

<span data-ttu-id="e9be9-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="e9be9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e9be9-105">Proiektuetan oinarritutako aurrekontu lerroak proiektu baten konpromisoa kalkulatzen laguntzeko diseinatuta daude.</span><span class="sxs-lookup"><span data-stu-id="e9be9-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="e9be9-106">Proiektuan oinarritutako aurrekontu lerroaren egitura proiektuaren kalkuluen arabera hedatzen da, honako kontzeptu hauekin:</span><span class="sxs-lookup"><span data-stu-id="e9be9-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="e9be9-107">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="e9be9-107">Billing Method</span></span>
- <span data-ttu-id="e9be9-108">Proiektuaren esleipena</span><span class="sxs-lookup"><span data-stu-id="e9be9-108">Project Mapping</span></span>
- <span data-ttu-id="e9be9-109">Transakzio klaseak barne</span><span class="sxs-lookup"><span data-stu-id="e9be9-109">Included Transaction classes</span></span>
- <span data-ttu-id="e9be9-110">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="e9be9-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="e9be9-111">Aplikagarritasun konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="e9be9-111">Chargeability setup</span></span>
- <span data-ttu-id="e9be9-112">Aurrekontua Lerroaren xehetasunak erabiliz</span><span class="sxs-lookup"><span data-stu-id="e9be9-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="e9be9-113">Eskaintzaren lerroaren bezeroak</span><span class="sxs-lookup"><span data-stu-id="e9be9-113">Quote line Customers</span></span>

<span data-ttu-id="e9be9-114">Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa.</span><span class="sxs-lookup"><span data-stu-id="e9be9-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="e9be9-115">Eremu horiei esker, proiektuaren inguruko lanen estimazio zehatza eta zehatza egiteko oinarriak ezartzen dira.</span><span class="sxs-lookup"><span data-stu-id="e9be9-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="e9be9-116">**Eremua**</span><span class="sxs-lookup"><span data-stu-id="e9be9-116">**Field**</span></span> | <span data-ttu-id="e9be9-117">**Garrantzia, xedea eta orientazioa**</span><span class="sxs-lookup"><span data-stu-id="e9be9-117">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="e9be9-118">**Downstream eragina**</span><span class="sxs-lookup"><span data-stu-id="e9be9-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e9be9-119">Izena</span><span class="sxs-lookup"><span data-stu-id="e9be9-119">Name</span></span> | <span data-ttu-id="e9be9-120">Estimatzen ari den aurrekontuaren osagai diskretua identifikatzen lagunduko dizun aurrekontuaren lerroaren izena.</span><span class="sxs-lookup"><span data-stu-id="e9be9-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="e9be9-121">Aurrekontua lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-122">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="e9be9-122">Billing Method</span></span> | <span data-ttu-id="e9be9-123">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroan dagokion eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="e9be9-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="e9be9-124">Eremu honek Dynamics 365 Project Operations-ek onartzen dituen kontratazio eredu nagusiak biltzen ditu:</span><span class="sxs-lookup"><span data-stu-id="e9be9-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="e9be9-125">- Prezio finkoa</span><span class="sxs-lookup"><span data-stu-id="e9be9-125">- Fixed price</span></span></br><span data-ttu-id="e9be9-126">- Denbora eta materiala.</span><span class="sxs-lookup"><span data-stu-id="e9be9-126">- Time and material.</span></span>| <span data-ttu-id="e9be9-127">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-128">Project</span><span class="sxs-lookup"><span data-stu-id="e9be9-128">Project</span></span> | <span data-ttu-id="e9be9-129">Erabili aukerako eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="e9be9-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="e9be9-130">Proiektu bat aurrekontu lerro batera mapeatzen denean, kargagarriak diren atazak ezartzen laguntzen du eta proiektuan oinarritutako aurrekontua aurrekontuaren lerroan aurrekontuaren lerroaren xehetasun gisa ekartzen laguntzen du.</span><span class="sxs-lookup"><span data-stu-id="e9be9-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="e9be9-131">Proiektu bat proiektuan oinarritutako aurrekontu lerro batera mapatuta ez dagoenean, aurrekontua eskuz sortu beharko litzateke aurrekontu lerroaren xehetasun bakoitza sortuz.</span><span class="sxs-lookup"><span data-stu-id="e9be9-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="e9be9-132">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-133">Idatzi denbora</span><span class="sxs-lookup"><span data-stu-id="e9be9-133">Include Time</span></span> | <span data-ttu-id="e9be9-134">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="e9be9-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="e9be9-135">**Ez** balioak adierazten du denbora-transakzioak edo lan-kostuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="e9be9-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="e9be9-136">**Bai** balioak adierazten du denbora-transakzioak edo lan-kostuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="e9be9-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="e9be9-137">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-138">Idatzi gastua</span><span class="sxs-lookup"><span data-stu-id="e9be9-138">Include Expense</span></span> | <span data-ttu-id="e9be9-139">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako gastuak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="e9be9-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="e9be9-140">**Ez** balioak adierazten du gastuak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="e9be9-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="e9be9-141">**Bai** balioak adierazten du gastuak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="e9be9-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="e9be9-142">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerro baten gainean kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-143">Idatzi prezioa</span><span class="sxs-lookup"><span data-stu-id="e9be9-143">Include Fee</span></span> | <span data-ttu-id="e9be9-144">**Bai**/**Ez** banderak adierazten du hautatutako proiektuaren denborako komisioak aurrekontu lerro honetako aurrekontuan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="e9be9-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="e9be9-145">**Ez** balioak adierazten du komisioak ez direla sartuko aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="e9be9-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="e9be9-146">**Bai** balioak adierazten du komisioak sartuko direla aurrekontu honen eskaintzaren lerroan.</span><span class="sxs-lookup"><span data-stu-id="e9be9-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="e9be9-147">Eremuaren balioa eskaintzaren lerro honetatik sortzen den Proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-148">Eskainitako zenbatekoa</span><span class="sxs-lookup"><span data-stu-id="e9be9-148">Quoted Amount</span></span> | <span data-ttu-id="e9be9-149">Proiektuan oinarritutako aurrekontu lerro honetan aurreikusitako lan guztiari bezeroari aipatuko zaion zenbatekoa da.</span><span class="sxs-lookup"><span data-stu-id="e9be9-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="e9be9-150">Aukera batetik sortutako aurrekontuan, balio hori aukera-lerroaren **Bezeroaren aurrekontua** eremutik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="e9be9-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="e9be9-151">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="e9be9-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="e9be9-152">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-153">Aurreikusitako zerga</span><span class="sxs-lookup"><span data-stu-id="e9be9-153">Estimated Tax</span></span> | <span data-ttu-id="e9be9-154">Eremu editagarria da erabiltzaileak aurrekontu lerroan zenbatetsitako zerga kopurua gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="e9be9-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="e9be9-155">Proiektuan oinarritutako aurrekontu lerroak lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta aurrekontuaren lerroaren xehetasunetan agertzen den zerga-zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="e9be9-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="e9be9-156">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-157">Eskainitako zenbatekoa, zergaren ondoren</span><span class="sxs-lookup"><span data-stu-id="e9be9-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="e9be9-158">Eremu hau zerga ondorengo aurrekontuaren zenbatekoa da eta irakurtzeko soilik da.</span><span class="sxs-lookup"><span data-stu-id="e9be9-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="e9be9-159">Eremu honetako zenbatekoa honela kalkulatzen da *Aipatutako zenbatekoa + Zerga*.</span><span class="sxs-lookup"><span data-stu-id="e9be9-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="e9be9-160">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-161">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="e9be9-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="e9be9-162">Eremu hau editagarria da eta proiektu bat duten aurrekontu lerroetan soilik dago erabilgarri **Denbora eta materiala** fakturazio metodoa.</span><span class="sxs-lookup"><span data-stu-id="e9be9-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="e9be9-163">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="e9be9-164">Bezeroaren aurrekontua</span><span class="sxs-lookup"><span data-stu-id="e9be9-164">Customer Budget</span></span> | <span data-ttu-id="e9be9-165">Eremu hau editagarria da eta balio hori aukera-lerroan dagokion eremutik kopiatzen da, abagunea eskaintza batetik sorten bada.</span><span class="sxs-lookup"><span data-stu-id="e9be9-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="e9be9-166">Eremuaren balioa eskaintzaren lerro honetatik sortzen den proiektuaren kontratu lerroan kopiatu da aurrekontua irabazten denean.</span><span class="sxs-lookup"><span data-stu-id="e9be9-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="e9be9-167">Proiektuetan oinarritutako aurrekontu lerroen Orokorra fitxako eremuen baliozkotze arauak</span><span class="sxs-lookup"><span data-stu-id="e9be9-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="e9be9-168">**1. araua** : Aukeratutako proiektuaren transakzio klase jakin bat proiektuaren araberako aurrekontuaren lerro bakarrean bakarrik sar daiteke.</span><span class="sxs-lookup"><span data-stu-id="e9be9-168">**Rule 1** : A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="e9be9-169">**2. araua** : Aukera batek aurrekontu ugari baditu, aurrekontu desberdinetako aurrekontu lerroak egon daitezke, proiektu bera aipatzen dutenak eta transakzio klase bera barne hartzen dutenak.</span><span class="sxs-lookup"><span data-stu-id="e9be9-169">**Rule 2** : If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="e9be9-170">**3. araua** : Aurrekontuak aukera berekoak ez badira, ezin dute proiektu eta transakzio klase bera sartu.</span><span class="sxs-lookup"><span data-stu-id="e9be9-170">**Rule 3** : If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="e9be9-171">
                    <strong>Abagunea</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="e9be9-172">
                    <strong>Eskaintza</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="e9be9-173">
                    <strong>Eskaintzaren lerroa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="e9be9-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="e9be9-175">
                    <strong>Idatzi denbora</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="e9be9-176">
                    <strong>Idatzi gastua</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="e9be9-177">
                    <strong>Sartu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="e9be9-178">
                    <strong>prezioa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="e9be9-179">
                    <strong>Baliozkoa/Baliogabea da</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="e9be9-180">
                    <strong>Arrazoia</strong>
                </span><span class="sxs-lookup"><span data-stu-id="e9be9-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e9be9-181">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-182">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-183">QL1</span><span class="sxs-lookup"><span data-stu-id="e9be9-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-184">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-185">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-186">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-187">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-188">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="e9be9-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-189">1. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="e9be9-189">Violation of Rule #1.</span></span> <span data-ttu-id="e9be9-190">P1 proiektuaren denbora, gastuak eta tasak bi aurrekontu lerroetan, QL1 eta QL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="e9be9-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e9be9-191">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-192">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-193">QL2</span><span class="sxs-lookup"><span data-stu-id="e9be9-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-194">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-195">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-196">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-197">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-197">Yes</span></span> </p>
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
<span data-ttu-id="e9be9-198">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-199">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-200">QL1</span><span class="sxs-lookup"><span data-stu-id="e9be9-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-201">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-202">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-203">+Ez</span><span class="sxs-lookup"><span data-stu-id="e9be9-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-204">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-205">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="e9be9-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-206">1. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="e9be9-206">Violation of Rule #1.</span></span> <span data-ttu-id="e9be9-207">P1 proiektuaren denbora eta tasak bi aurrekontu lerroetan, QL1 eta QL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="e9be9-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e9be9-208">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-209">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-210">QL2</span><span class="sxs-lookup"><span data-stu-id="e9be9-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-211">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-212">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-213">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-214">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-214">Yes</span></span> </p>
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
<span data-ttu-id="e9be9-215">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-216">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-217">QL1</span><span class="sxs-lookup"><span data-stu-id="e9be9-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-218">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-219">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-220">+Ez</span><span class="sxs-lookup"><span data-stu-id="e9be9-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-221">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-222">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="e9be9-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="e9be9-223">P1 proiektuaren denbora eta tasak QL1-en sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="e9be9-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="e9be9-224">P1 proiektuaren gastuak QL2n sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="e9be9-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="e9be9-225">Aurrekontu lerro bakoitzean sartzen den horretan ez dago gainjartzerik, beraz, balio du.</span><span class="sxs-lookup"><span data-stu-id="e9be9-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e9be9-226">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-227">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-228">QL2</span><span class="sxs-lookup"><span data-stu-id="e9be9-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-229">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-230">+Ez</span><span class="sxs-lookup"><span data-stu-id="e9be9-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-231">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-232">+Ez</span><span class="sxs-lookup"><span data-stu-id="e9be9-232">No</span></span> </p>
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
<span data-ttu-id="e9be9-233">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-234">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-235">QL1</span><span class="sxs-lookup"><span data-stu-id="e9be9-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-236">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-237">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-238">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-239">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-240">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="e9be9-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-241">1. araua haustea eta gehiago</span><span class="sxs-lookup"><span data-stu-id="e9be9-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="e9be9-242">Q1ean P1 proiektu osoko denbora, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="e9be9-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="e9be9-243">QL2-k P1 proiektu osorako Denbora, Gastuak eta Tasak barne hartzen ditu eta Q1-n sartutakoarekin gainjartzen da.</span><span class="sxs-lookup"><span data-stu-id="e9be9-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e9be9-244">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-245">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-246">QL2</span><span class="sxs-lookup"><span data-stu-id="e9be9-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-247">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-248">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-249">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-250">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-250">Yes</span></span> </p>
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
<span data-ttu-id="e9be9-251">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-252">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-253">QL1</span><span class="sxs-lookup"><span data-stu-id="e9be9-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-254">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-255">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-256">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-257">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="e9be9-258">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="e9be9-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-259">2. arauan oinarrituta, Q1 eta Q2 aukera berdineko bi komatxo dira, beraz, biek proiektu baten osagai berberak kalkula ditzakete.</span><span class="sxs-lookup"><span data-stu-id="e9be9-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e9be9-260">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-261">2H</span><span class="sxs-lookup"><span data-stu-id="e9be9-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-262">QL1 Q2n</span><span class="sxs-lookup"><span data-stu-id="e9be9-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-263">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-264">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-265">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-266">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-266">Yes</span></span> </p>
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
<span data-ttu-id="e9be9-267">O1</span><span class="sxs-lookup"><span data-stu-id="e9be9-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-268">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-269">QL1</span><span class="sxs-lookup"><span data-stu-id="e9be9-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-270">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-271">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-272">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-273">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="e9be9-274">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="e9be9-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="e9be9-275">3. arauan oinarrituta, Q1 eta Q2 aukera desberdineko bi komatxo dira, beraz, proiektu berean ezin dira osagai berberak kalkulatu.</span><span class="sxs-lookup"><span data-stu-id="e9be9-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="e9be9-276">O2</span><span class="sxs-lookup"><span data-stu-id="e9be9-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="e9be9-277">1H</span><span class="sxs-lookup"><span data-stu-id="e9be9-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-278">QL1</span><span class="sxs-lookup"><span data-stu-id="e9be9-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-279">A1</span><span class="sxs-lookup"><span data-stu-id="e9be9-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-280">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="e9be9-281">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="e9be9-282">Yes</span><span class="sxs-lookup"><span data-stu-id="e9be9-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="e9be9-283">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="e9be9-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

