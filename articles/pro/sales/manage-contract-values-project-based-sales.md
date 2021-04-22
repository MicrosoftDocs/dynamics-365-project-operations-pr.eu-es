---
title: Proiektuetan oinarritutako kontratuaren lerroen ikuspegi orokorra
description: Gai honek proiektuan oinarritutako kontratu lerroekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 824fdd54d7b513b49afd1a6d76d3387df81418e2
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858143"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="38e50-103">Proiektuetan oinarritutako kontratuaren lerroen ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="38e50-103">Project-based contract lines overview</span></span>

<span data-ttu-id="38e50-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="38e50-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="38e50-105">Dynamics 365 Project Operations proiektuan oinarritutako kontratu lerroak proiektu batean egindako lanen osagai zehatzen aurrekontua eta fakturazio akordioak atxikitzeko diseinatuta daude.</span><span class="sxs-lookup"><span data-stu-id="38e50-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="38e50-106">Proiektuan oinarritutako kontratu lerroaren egitura proiektuaren kalkuluen eta fakturazio eszenatokietarako hedatzen da, honako kontzeptu hauekin:</span><span class="sxs-lookup"><span data-stu-id="38e50-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="38e50-107">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="38e50-107">Billing method</span></span>
- <span data-ttu-id="38e50-108">Proiektuen eta zereginen esleipena</span><span class="sxs-lookup"><span data-stu-id="38e50-108">Project and task mapping</span></span>
- <span data-ttu-id="38e50-109">Transakzio klaseak barne</span><span class="sxs-lookup"><span data-stu-id="38e50-109">Included transaction classes</span></span>
- <span data-ttu-id="38e50-110">Ez gainditzeko muga</span><span class="sxs-lookup"><span data-stu-id="38e50-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="38e50-111">Aplikagarritasun konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="38e50-111">Chargeability setup</span></span>
- <span data-ttu-id="38e50-112">Aurrekontuak kontratuaren lineako xehetasunak erabiliz</span><span class="sxs-lookup"><span data-stu-id="38e50-112">Estimates using contract line details</span></span>
- <span data-ttu-id="38e50-113">Kontratuaren lerroaren bezeroa</span><span class="sxs-lookup"><span data-stu-id="38e50-113">Contract line customers</span></span>

<span data-ttu-id="38e50-114">Ondorengo taulan eremuko eremuak biltzen dira **Orokorra** proiektuan oinarritutako kontratu-lerroen fitxa, proiektuan oinarritutako lan zehatza eta finkatua finkatzeko eta fakturazio moldaketak egiteko oinarriak finkatzen laguntzen dutenak.</span><span class="sxs-lookup"><span data-stu-id="38e50-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="38e50-115">Eremua</span><span class="sxs-lookup"><span data-stu-id="38e50-115">Field</span></span> | <span data-ttu-id="38e50-116">Deskribapena</span><span class="sxs-lookup"><span data-stu-id="38e50-116">Description</span></span> | <span data-ttu-id="38e50-117">Downstream eragina</span><span class="sxs-lookup"><span data-stu-id="38e50-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="38e50-118">**Izena**</span><span class="sxs-lookup"><span data-stu-id="38e50-118">**Name**</span></span> | <span data-ttu-id="38e50-119">Kontratuaren lerroaren izena.</span><span class="sxs-lookup"><span data-stu-id="38e50-119">Name of the contract line.</span></span> <span data-ttu-id="38e50-120">Honek kalkulatzen ari den kontratuaren osagai diskretua identifikatzen du.</span><span class="sxs-lookup"><span data-stu-id="38e50-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="38e50-121">Aurrekontu batetik sortutako proiektu kontratu baterako, balio hori proiektuan oinarritutako aurrekontu lerroaren dagokion balio batetik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="38e50-122">Faktura sortzen denean kontratu lerro honetatik sortzen den proiektuaren faktura lerroan kopiatutako izena.</span><span class="sxs-lookup"><span data-stu-id="38e50-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="38e50-123">**Fakturazio-metodoa**</span><span class="sxs-lookup"><span data-stu-id="38e50-123">**Billing Method**</span></span> | <span data-ttu-id="38e50-124">Aurrekontu batetik sortutako proiektu kontratu baterako, aurrekontuaren lerroaren dagokion balio batetik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="38e50-125">Hau da aukera multzo, Project Operations-ek onartzen dituzten bi kontratazio eredu nagusiak adierazten dituena:</span><span class="sxs-lookup"><span data-stu-id="38e50-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="38e50-126">- **Prezio finkoa**</span><span class="sxs-lookup"><span data-stu-id="38e50-126">- **Fixed Price**</span></span></br><span data-ttu-id="38e50-127">- **Denbora eta materiala**</span><span class="sxs-lookup"><span data-stu-id="38e50-127">- **Time and Material**</span></span> | <span data-ttu-id="38e50-128">Aipatutako kontratu lerroaren fakturazio metodoan oinarrituta, benetako transakzioa prozesatuko da.</span><span class="sxs-lookup"><span data-stu-id="38e50-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="38e50-129">Benetakoak aipatzen duen kontratu lerroak denbora eta materiala fakturatzeko metodoa badu, kostuen eta fakturatu gabeko salmenten benetako erregistroak sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="38e50-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="38e50-130">Benetakoak aipatzen duen kontratu-lerroak prezio finkoko fakturazio-metodoa badu, benetako kostua soilik sortzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="38e50-131">**Project**</span><span class="sxs-lookup"><span data-stu-id="38e50-131">**Project**</span></span> | <span data-ttu-id="38e50-132">Erabili eremu hau konpromiso horretan lana emateko erabiliko den proiektua identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="38e50-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="38e50-133">Balio hau honekin batera erabiliko da **Zereginak barne** eta **Barne transakzio klaseak** kontratu-lerroaren erreferentzia benetako edo kalkulatutako linea-erregistro batean ebazteko.</span><span class="sxs-lookup"><span data-stu-id="38e50-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="38e50-134">**Gehitutako zereginak**</span><span class="sxs-lookup"><span data-stu-id="38e50-134">**Included Tasks**</span></span> | <span data-ttu-id="38e50-135">Kontratu lerro honek hautatutako proiektuaren proiektuko zeregin guztiak edo zereginen azpimultzo bat bakarrik biltzen dituen adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="38e50-136">Aukera multzo bat da, balore hauek ditu:</span><span class="sxs-lookup"><span data-stu-id="38e50-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="38e50-137">- **Proiektuen zeregin guztiak**</span><span class="sxs-lookup"><span data-stu-id="38e50-137">- **All Project Tasks**</span></span></br><span data-ttu-id="38e50-138">- - **Hautatutako proiektu-zereginak soilik**.</span><span class="sxs-lookup"><span data-stu-id="38e50-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="38e50-139">Eremu honetako balio huts bat hautatzearen berdina da **Proiektuaren zeregin guztiak**.</span><span class="sxs-lookup"><span data-stu-id="38e50-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="38e50-140">**Aukeratutako zereginak soilik** hautatuta dago, zeregin zehatzak hautatu eta kontratu lerro honekin lotu ditzakezu **Zereginen fakturazio konfigurazioa** fitxan **Proiektua** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="38e50-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="38e50-141">Balio hau honekin batera erabiliko da **Proiektua** eta **Barne transakzio klaseak** kontratu-lerroaren erreferentzia benetako edo aurrekontuko lerro erregistro batean ebazteko.</span><span class="sxs-lookup"><span data-stu-id="38e50-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="38e50-142">**Idatzi denbora**</span><span class="sxs-lookup"><span data-stu-id="38e50-142">**Include Time**</span></span> | <span data-ttu-id="38e50-143">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren denborako transakzioak edo lan kostuak kontratuaren lerro honetan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="38e50-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="38e50-144">**Ez** balioak kontratuaren lerroan sartzen ez diren transakzioak edo denbora-transakzioak adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="38e50-145">**Bai** balioak egingo dutela adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="38e50-146">Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko.</span><span class="sxs-lookup"><span data-stu-id="38e50-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="38e50-147">**Idatzi gastua**</span><span class="sxs-lookup"><span data-stu-id="38e50-147">**Include Expense**</span></span> | <span data-ttu-id="38e50-148">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren gastuen kostuak kontratuaren lerro honetan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="38e50-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="38e50-149">**Ez** balioak kontratuaren lerroan sartzen ez diren gastuen kostuak adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="38e50-150">**Bai** balioak egingo dutela adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="38e50-151">Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko.</span><span class="sxs-lookup"><span data-stu-id="38e50-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="38e50-152">**Sartu materialak**</span><span class="sxs-lookup"><span data-stu-id="38e50-152">**Include Materials**</span></span> | <span data-ttu-id="38e50-153">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren materialaren kostuak kontratuaren lerro honetan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="38e50-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="38e50-154">**Ez** balioa adierazten du materialaren kostuak kontratuaren lerro honetan ez diren sartuko.</span><span class="sxs-lookup"><span data-stu-id="38e50-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="38e50-155">**Bai** balioak egingo dutela adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="38e50-156">Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko.</span><span class="sxs-lookup"><span data-stu-id="38e50-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="38e50-157">**Idatzi prezioa**</span><span class="sxs-lookup"><span data-stu-id="38e50-157">**Include Fee**</span></span> | <span data-ttu-id="38e50-158">**Bai**/**Ez** balioa adierazten du hautatutako proiektuaren komisioak kontratuaren lerro honetan sartuko diren.</span><span class="sxs-lookup"><span data-stu-id="38e50-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="38e50-159">**Ez** balioak kontratuaren lerroan sartzen ez diren zergak adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="38e50-160">**Bai** balioak egingo dutela adierazten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="38e50-161">Balio hori proiektuarekin batera erabiltzen da kontratu-lerroaren erreferentzia benetako edo kalkulu-lerro erregistro batean ebazteko.</span><span class="sxs-lookup"><span data-stu-id="38e50-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="38e50-162">**Kontratatutako zenbatekoa**</span><span class="sxs-lookup"><span data-stu-id="38e50-162">**Contracted Amount**</span></span> | <span data-ttu-id="38e50-163">Prezio finkoko kontratu lerroan, zenbateko hori bezeroari fakturatuko zaion hitzarmenaren balioa da, kontratu lerro honi lotutako lan osagai guztiengatik.</span><span class="sxs-lookup"><span data-stu-id="38e50-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="38e50-164">Denboraren eta materialaren kontratuaren lerroan, zenbateko hori bezeroari fakturatuko zaion aurreikusitako balioa da, kontratu lerro honi lotutako lan osagai guztiengatik.</span><span class="sxs-lookup"><span data-stu-id="38e50-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="38e50-165">Aurrekontu batetik sortutako proiektu kontratu baterako, aurrekontuaren lerroaren dagokion balio batetik kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="38e50-166">Proiektuan oinarritutako kontratu lerro batek lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta kontratuaren lerroaren xehetasunen zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="38e50-167">Kontratu-lerroak lerroaren xehetasunak dituenean, balio hori alda daiteke lerroaren xehetasunen zenbatekoak aldatuta.</span><span class="sxs-lookup"><span data-stu-id="38e50-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="38e50-168">Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarrien gaineko zerga aurretik zenbatekoa sortzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="38e50-169">**Aurreikusitako zerga**</span><span class="sxs-lookup"><span data-stu-id="38e50-169">**Estimated Tax**</span></span> | <span data-ttu-id="38e50-170">Erabiltzaileak eremu hau alda dezake, aurreikusitako zergaren zenbatekoa kontratu lerroan sartzeko.</span><span class="sxs-lookup"><span data-stu-id="38e50-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="38e50-171">Proiektuan oinarritutako kontratu lerro batek lerroaren xehetasunak dituenean, eremu hau blokeatuta dago editatzeko eta kontratuaren lerroaren xehetasunen zerga-zenbatekoaren arabera laburbiltzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="38e50-172">Kontratu-lerroak lerroaren xehetasunak dituenean, balio hori alda daiteke lerroaren xehetasunen zerga-zenbatekoak aldatuta.</span><span class="sxs-lookup"><span data-stu-id="38e50-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="38e50-173">Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarrien gaineko zerga sortzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="38e50-174">**Kontratatutako zenbatekoa, zergaren ondoren**</span><span class="sxs-lookup"><span data-stu-id="38e50-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="38e50-175">Kontratatuaren lerroaren zenbatekoa zergaren ondoren.</span><span class="sxs-lookup"><span data-stu-id="38e50-175">The contract line amount after tax.</span></span> <span data-ttu-id="38e50-176">Eremu hau irakurtzeko soilik da eta honela kalkulatzen da **Kontratatutako zenbatekoa + Zerga**.</span><span class="sxs-lookup"><span data-stu-id="38e50-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="38e50-177">Prezio finkoko kontratu lerroan, balio hori aldizkako fakturazio mugarriak sortzeko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="38e50-178">**Ez gainditzeko muga**</span><span class="sxs-lookup"><span data-stu-id="38e50-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="38e50-179">Erabiltzaileak eremu hau edita dezake eta fakturazio metodoa denbora eta material gisa ezarrita duten proiektuetan oinarritutako kontratu lerroetan bakarrik dago erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="38e50-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="38e50-180">Erabiltzaileak eremu hau edita dezake.</span><span class="sxs-lookup"><span data-stu-id="38e50-180">The user can edit this field.</span></span> <span data-ttu-id="38e50-181">Denboraz eta materialaz egindako benetako batek kontratu-lerro hau denboraz eta materialez aipatzen duenean, benetako zenbatekoa kontratu-lerroan gainditu ezin den mugaren arabera ebaluatzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="38e50-182">Ebaluazio hori dagoeneko gastatutako eta konprometitutako zenbatekoak kontabilizatu ondoren amaitzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="38e50-183">**Bezeroaren aurrekontua**</span><span class="sxs-lookup"><span data-stu-id="38e50-183">**Customer Budget**</span></span> | <span data-ttu-id="38e50-184">Eremu hau editagarria da eta aurrekontuaren lerroaren dagokion balio batetik kopiatzen da kontratua eskaintza batetik sortu bada.</span><span class="sxs-lookup"><span data-stu-id="38e50-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="38e50-185">Eremu hau informaziorako bakarrik erabiltzen da eta ez du beheranzko esangurarik.</span><span class="sxs-lookup"><span data-stu-id="38e50-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="38e50-186">Proiektuetan oinarritutako kontratu lerroen Orokorreko fitxako aukeren baliozkotze arauak</span><span class="sxs-lookup"><span data-stu-id="38e50-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="38e50-187">1. araua: **Zereginak barne** eremua hutsik dago edo ezarrita dago **Proiektuaren zeregin guztiak**, proiektuaren zeregin guztiak kontratu lerroan sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="38e50-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="38e50-188">2. araua: **Zereginak barne** eremua hutsik dago edo esplizituki ezarrita dago **Proiektuaren zeregin guztiak**, proiektu bat eta transakzio klase jakin bat proiektuan oinarritutako kontratu lerro batean bakarrik sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="38e50-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="38e50-189">3. araua: **Zereginak barne** eremua ezarrita dago **Hautatutako proiektuak soilik**, proiektu bat eta transakzio klase jakin bat kontratuaren proiektuan oinarritutako kontratuaren hainbat lerrotan sar daitezke.</span><span class="sxs-lookup"><span data-stu-id="38e50-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="38e50-190">
                    <strong>Kontratua</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="38e50-191">
                    <strong>Kontratuaren lerroa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="38e50-192">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="38e50-193">
                    <strong>Gehitutako zereginak</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="38e50-194">
                    <strong>Idatzi denbora</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="38e50-195">
                    <strong>Idatzi gastua</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="38e50-196">
                    <strong>Materialak barne</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="38e50-197">
                    <strong>Gehitu</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="38e50-198">
                    <strong>Tasa</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="38e50-199">
                    <strong>Baliozkoa/Baliogabea da</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="38e50-200">
                    <strong>Arrazoia</strong>
                </span><span class="sxs-lookup"><span data-stu-id="38e50-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-201">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-202">CL1</span><span class="sxs-lookup"><span data-stu-id="38e50-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-203">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-204">Hutsik</span><span class="sxs-lookup"><span data-stu-id="38e50-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-205">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-206">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-207">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-208">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-209">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="38e50-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-210">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="38e50-210">Violation of Rule #2.</span></span> <span data-ttu-id="38e50-211">P1 proiektuaren denbora, gastuak, materialak eta tasak Kontratuaren lerroetan, CL1 eta CL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="38e50-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-212">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-213">CL2</span><span class="sxs-lookup"><span data-stu-id="38e50-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-214">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-215">Hutsik</span><span class="sxs-lookup"><span data-stu-id="38e50-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-216">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-217">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-218">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-219">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-220">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-221">CL1</span><span class="sxs-lookup"><span data-stu-id="38e50-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-222">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-223">Hutsik</span><span class="sxs-lookup"><span data-stu-id="38e50-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-224">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-225">No</span><span class="sxs-lookup"><span data-stu-id="38e50-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-226">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-227">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-228">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="38e50-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-229">2. araua haustea.</span><span class="sxs-lookup"><span data-stu-id="38e50-229">Violation of Rule #2.</span></span> <span data-ttu-id="38e50-230">P1 proiektuaren denbora, materialak eta tasak Kontratuaren lerroetan, CL1 eta CL2 barne daude.</span><span class="sxs-lookup"><span data-stu-id="38e50-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-231">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-232">CL2</span><span class="sxs-lookup"><span data-stu-id="38e50-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-233">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-234">Hutsik</span><span class="sxs-lookup"><span data-stu-id="38e50-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-235">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-236">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-237">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-238">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-239">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-240">CL1</span><span class="sxs-lookup"><span data-stu-id="38e50-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-241">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-242">Hutsik</span><span class="sxs-lookup"><span data-stu-id="38e50-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-243">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-244">No</span><span class="sxs-lookup"><span data-stu-id="38e50-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-245">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-246">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-247">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="38e50-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-248">P1 proiektuaren denbora, materialak eta tasak CL1 barne daude.</span><span class="sxs-lookup"><span data-stu-id="38e50-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="38e50-249">P1 proiektuaren gastuak QL2n sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="38e50-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="38e50-250">Kontratuaren lerro bakoitzean sartzen denaren gainetik ez dago gainjartzerik eta, beraz, baliozkoa da.</span><span class="sxs-lookup"><span data-stu-id="38e50-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-251">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-252">CL2</span><span class="sxs-lookup"><span data-stu-id="38e50-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-253">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-254">Hutsik</span><span class="sxs-lookup"><span data-stu-id="38e50-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-255">No</span><span class="sxs-lookup"><span data-stu-id="38e50-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-256">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-257">No</span><span class="sxs-lookup"><span data-stu-id="38e50-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-258">No</span><span class="sxs-lookup"><span data-stu-id="38e50-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-259">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-260">CL1</span><span class="sxs-lookup"><span data-stu-id="38e50-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-261">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-262">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="38e50-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-263">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-264">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-265">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-266">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-267">Baliogabea da</span><span class="sxs-lookup"><span data-stu-id="38e50-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-268">2. araua haustea</span><span class="sxs-lookup"><span data-stu-id="38e50-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="38e50-269">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, materialak, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="38e50-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="38e50-270">CL2-k P1 proiektu osorako denbora, materialak, gastuak eta tasak biltzen ditu eta, beraz, C1-en sartutakoarekin gainjartzen da.</span><span class="sxs-lookup"><span data-stu-id="38e50-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-271">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-272">CL2</span><span class="sxs-lookup"><span data-stu-id="38e50-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-273">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-274">Hutsik</span><span class="sxs-lookup"><span data-stu-id="38e50-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-275">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-276">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-277">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-278">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-279">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-280">CL1</span><span class="sxs-lookup"><span data-stu-id="38e50-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-281">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-282">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="38e50-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-283">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-284">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-285">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-286">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-287">Baliozkoa</span><span class="sxs-lookup"><span data-stu-id="38e50-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="38e50-288">3. arauaren arabera</span><span class="sxs-lookup"><span data-stu-id="38e50-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="38e50-289">P1 proiektuan P1 proiektuaren zereginen azpimultzo baten denbora, gastuak, materialak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="38e50-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="38e50-290">CL2k barne ditu P1 proiektuaren zereginen azpimultzo baten denbora, materiala, gastuak eta tasak sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="38e50-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="38e50-291">Balidazio osagarri bakarra CL1-eko zereginen azpimultzoaren inguruan kokatzen da, CL2-ren zereginen azpimultzoaren desberdina dela gainjartzerik ez dagoela ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="38e50-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="38e50-292">Sistemak zereginak lotzen dituenean egiten du.</span><span class="sxs-lookup"><span data-stu-id="38e50-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="38e50-293">C1</span><span class="sxs-lookup"><span data-stu-id="38e50-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="38e50-294">CL2</span><span class="sxs-lookup"><span data-stu-id="38e50-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-295">A1</span><span class="sxs-lookup"><span data-stu-id="38e50-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="38e50-296">Hautatutako zereginak soilik</span><span class="sxs-lookup"><span data-stu-id="38e50-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-297">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="38e50-298">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-299">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="38e50-300">Yes</span><span class="sxs-lookup"><span data-stu-id="38e50-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
