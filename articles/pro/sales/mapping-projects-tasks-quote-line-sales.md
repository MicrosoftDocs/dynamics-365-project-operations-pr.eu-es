---
title: Esleitu proiektuak eta zereginak proiektuetan oinarritutako eskaintzaren lerro batean
description: Gai honek proiektuak eta zereginak proiektuetan oinarritutako ataza lerro batera mapatzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 871d323136cd982bd48ed9aa2b9c34017951d2d8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130698"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="49d44-103">Esleitu proiektuak eta zereginak proiektuetan oinarritutako eskaintzaren lerro batean</span><span class="sxs-lookup"><span data-stu-id="49d44-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="49d44-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="49d44-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="49d44-105">Proiektuetan oinarritutako aurrekontu lerroetan, dagoeneko aurrekontu lerro batekin lotuta dagoen proiektu baten zeregin zehatzak mapatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="49d44-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="49d44-106">Zereginak aurrekontu lerro batera mapatzen dituzunean, aurrekontu lerroan zehaztu dituzun elementu hauek zeregin horiei soilik aplikatuko zaizkie:</span><span class="sxs-lookup"><span data-stu-id="49d44-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="49d44-107">Fakturazio-metodoa</span><span class="sxs-lookup"><span data-stu-id="49d44-107">Billing method</span></span>
- <span data-ttu-id="49d44-108">Kobragarritasun-aukerak</span><span class="sxs-lookup"><span data-stu-id="49d44-108">Chargeability options</span></span>
- <span data-ttu-id="49d44-109">Ez gainditzeko mugak</span><span class="sxs-lookup"><span data-stu-id="49d44-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="49d44-110">Bezeroak</span><span class="sxs-lookup"><span data-stu-id="49d44-110">Customers</span></span>

<span data-ttu-id="49d44-111">Adibidez, fase bat prezio finkoa duen eta beste fase guztiak denbora eta materialak diren proiektu bat izan dezakezu.</span><span class="sxs-lookup"><span data-stu-id="49d44-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="49d44-112">Kasu honetan, lehen fasea eta haren seme-alaba guztiak, fase horretako aurrekontu lerroarekin lotu ditzakezu prezio finkoaren fakturazio metodoarekin.</span><span class="sxs-lookup"><span data-stu-id="49d44-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="49d44-113">Ondoren, beste fase guztiak denboran eta materialetan oinarritutako aurrekontu lerroarekin lotu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="49d44-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="49d44-114">Lotu zereginak proiektuan oinarritutako eskaintzaren lerroak</span><span class="sxs-lookup"><span data-stu-id="49d44-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="49d44-115">Atazak kokapen hauetako aurrekontu lerroekin lotu ditzakezu:</span><span class="sxs-lookup"><span data-stu-id="49d44-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="49d44-116">**Proiektua** orrialdea > **Zereginen fakturazioa** fitxa (optimoa)</span><span class="sxs-lookup"><span data-stu-id="49d44-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="49d44-117">**Aipatu lerroa** orrialdea > **Kobratzeko zereginak** fitxa</span><span class="sxs-lookup"><span data-stu-id="49d44-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="49d44-118">Proiektua orritik</span><span class="sxs-lookup"><span data-stu-id="49d44-118">From the Project page</span></span>

<span data-ttu-id="49d44-119">**Proiektua** orrialdeak zereginak lerroen artean lotzeko esperientzia ezin hobea eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="49d44-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="49d44-120">Orrialde hau erabil dezakezu zeregin anitz hautatzeko eta haiek guztiak, haurren zereginak gehituta hautatutako aurrekontu lerroarekin lotzeko.</span><span class="sxs-lookup"><span data-stu-id="49d44-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="49d44-121">**Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxan, egiaztatu **Proiektua** eremua bete da.</span><span class="sxs-lookup"><span data-stu-id="49d44-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="49d44-122">**Zereginak barne** eremuan, hautatu **Aukeratutako zereginak soilik**.</span><span class="sxs-lookup"><span data-stu-id="49d44-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="49d44-123">Gorde proiektuetan oinarritutako eskaintzaren lerroa.</span><span class="sxs-lookup"><span data-stu-id="49d44-123">Save the project-based quote line.</span></span> <span data-ttu-id="49d44-124">Inprimakia freskatzean, **Kobratzeko zereginak** fitxa pantailetan.</span><span class="sxs-lookup"><span data-stu-id="49d44-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="49d44-125">**Orokorra** fitxan, hautatu proiektuaren esteka **Proiektua** eremutik.</span><span class="sxs-lookup"><span data-stu-id="49d44-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="49d44-126">**Proiektua** orrialdean, hautatu **Zereginaren fakturazioa** fitxan.</span><span class="sxs-lookup"><span data-stu-id="49d44-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="49d44-127">Bigarren saretan, zeregin zehatzen fakturazio konfigurazioari aplikatzen zaiona, hautatu zeregin bat edo gehiago eta, ondoren, hautatu **Elkartu aurrekontu lerroak**.</span><span class="sxs-lookup"><span data-stu-id="49d44-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="49d44-128">Agertzen den elkarrizketa-orrian, hautatu aurrekontuan proiektuan oinarritutako aurrekontu lerroak bistaratuko dituen aurrekontu lerroa.</span><span class="sxs-lookup"><span data-stu-id="49d44-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="49d44-129">**Fakturazio mota** eremuan, adierazi zeregin horiek kargagarriak edo kargagarriak ez diren.</span><span class="sxs-lookup"><span data-stu-id="49d44-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="49d44-130">Hautatu kontrol laukia elkarteak hautatutako zereginen seme-alaben zereginak sartu behar dituen ala ez adierazteko.</span><span class="sxs-lookup"><span data-stu-id="49d44-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="49d44-131">Laukia markatuta hautatutako atazetako haurren zereginak aurrekontu lerroarekin lotuko dira.</span><span class="sxs-lookup"><span data-stu-id="49d44-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="49d44-132">Hautatu **Ados** elkarrizketa ixteko.</span><span class="sxs-lookup"><span data-stu-id="49d44-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="49d44-133">Aipatu lerroaren orrian</span><span class="sxs-lookup"><span data-stu-id="49d44-133">From the Quote line page</span></span>

<span data-ttu-id="49d44-134">Proiektuaren zereginak lotu ditzakezu **Kobratzeko zereginak** fitxa **Aipatu lerroa** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="49d44-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="49d44-135">Proiektuaren zereginak lerroak aipatzeko lotzeko lekurik onena da **Zereginen fakturazioa** fitxan **Proiektua** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="49d44-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="49d44-136">Zereginak lotzen badituzu **Kobratzeko zereginak** fitxatik **Aipatu lerroa** orrialdean, proiektu bakoitza eskuz lotu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="49d44-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="49d44-137">**Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxan, egiaztatu proiektu bat hautatuta dagoela **Proiektua** eremuan.</span><span class="sxs-lookup"><span data-stu-id="49d44-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="49d44-138">**Zereginak barne** eremuan, hautatu **Aukeratutako zereginak soilik**.</span><span class="sxs-lookup"><span data-stu-id="49d44-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="49d44-139">Gorde proiektuetan oinarritutako eskaintzaren lerroa.</span><span class="sxs-lookup"><span data-stu-id="49d44-139">Save the project-based quote line.</span></span> <span data-ttu-id="49d44-140">Inprimakia freskatzean, **Kobratzeko zereginak** fitxa pantailetan.</span><span class="sxs-lookup"><span data-stu-id="49d44-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="49d44-141">**Kobratzeko zereginak** fitxan, hautatu **Gehitu aurrekontu lerroaren zeregina**.</span><span class="sxs-lookup"><span data-stu-id="49d44-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="49d44-142">**Aipatu lerro zeregina** orrialdean, **Zereginak** eremuan, hautatu zeregina eta **Fakturazio mota** eremua, hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="49d44-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="49d44-143">Itxi orria.</span><span class="sxs-lookup"><span data-stu-id="49d44-143">Close the page.</span></span> <span data-ttu-id="49d44-144">Aukeratutako zeregina aurrekontu lerroarekin lotuta dago orain.</span><span class="sxs-lookup"><span data-stu-id="49d44-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="49d44-145">Askatu zereginak proiektuan oinarritutako eskaintzaren lerroetatik</span><span class="sxs-lookup"><span data-stu-id="49d44-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="49d44-146">Proiektua orritik</span><span class="sxs-lookup"><span data-stu-id="49d44-146">From the Project page</span></span>

<span data-ttu-id="49d44-147">Metodoak orrialdeak zereginak lerroen artetik askatzeko esperientzia ezin hobea eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="49d44-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="49d44-148">Zeregin anitz hautatzeko eta haiek guztiak, haurren zereginak gehituta hautatutako aurrekontu lerrotik askatzeko.</span><span class="sxs-lookup"><span data-stu-id="49d44-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="49d44-149">**Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxan,**Proiektua** eremuan, hautatu proiektuaren esteka.</span><span class="sxs-lookup"><span data-stu-id="49d44-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="49d44-150">**Proiektua** orrialdean, hautatu **Zereginaren fakturazioa** fitxan.</span><span class="sxs-lookup"><span data-stu-id="49d44-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="49d44-151">Bigarren saretan, zeregin zehatzen fakturazio konfigurazioari aplikatzen zaiona, hautatu zeregin bat edo gehiago eta, ondoren, hautatu **Askatu aurrekontu lerroak**.</span><span class="sxs-lookup"><span data-stu-id="49d44-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="49d44-152">Agertzen den elkarrizketa-orrian, hautatu aurrekontu lerroa.</span><span class="sxs-lookup"><span data-stu-id="49d44-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="49d44-153">Hautatu kontrol laukia elkarteak hautatutako zereginen seme-alaben zereginak ere kendu behar diren ala ez adierazteko.</span><span class="sxs-lookup"><span data-stu-id="49d44-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="49d44-154">Laukia markatuta hautatutako atazetako haurren zereginak aurrekontu lerrotik askatuko dira.</span><span class="sxs-lookup"><span data-stu-id="49d44-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="49d44-155">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="49d44-155">Select **OK**.</span></span> <span data-ttu-id="49d44-156">Abisu mezu batek jakinarazten dizu elkarte hau kentzen baduzu, zereginean aurretik grabatutako datuak alderantzika litezkeela.</span><span class="sxs-lookup"><span data-stu-id="49d44-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="49d44-157">Aukeratu **Ados** zereginaren eta proiektuan oinarritutako aurrekontu lerroaren arteko lotura jarraitzeko eta kentzeko.</span><span class="sxs-lookup"><span data-stu-id="49d44-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="49d44-158">Aipatu lerroaren orrian</span><span class="sxs-lookup"><span data-stu-id="49d44-158">From the Quote line page</span></span>

<span data-ttu-id="49d44-159">Proiektuaren zereginak ere aska ditzakezu **Kobratzeko zereginak** fitxa **Aipatu lerroa** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="49d44-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="49d44-160">**Kobratzeko zereginak** fitxan, hautatu **Ezabatu aurrekontu lerroaren zeregina**.</span><span class="sxs-lookup"><span data-stu-id="49d44-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="49d44-161">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="49d44-161">Select **OK**.</span></span> <span data-ttu-id="49d44-162">Abisu mezu batek jakinarazten dizu elkarte hau kentzen baduzu, zereginean aurretik grabatutako datuak alderantzika litezkeela.</span><span class="sxs-lookup"><span data-stu-id="49d44-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="49d44-163">Aukeratu **Ados** zereginaren eta proiektuan oinarritutako aurrekontu lerroaren arteko lotura jarraitzeko eta kentzeko.</span><span class="sxs-lookup"><span data-stu-id="49d44-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="49d44-164">Prozedura honek ez du zeregina proiektutik ezabatzen.</span><span class="sxs-lookup"><span data-stu-id="49d44-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="49d44-165">Zereginen elkartea proiektuan oinarritutako aurrekontu lerroatik bakarrik kentzen du.</span><span class="sxs-lookup"><span data-stu-id="49d44-165">It only removes the task association from the project-based quote line.</span></span>
