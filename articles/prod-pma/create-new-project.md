---
title: Sortu proiektua
description: Gai honek proiektu berri bat sortzeari buruzko informazioa ematen du.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9b29340dc88aea888ea2f5ea975eaea59d014279
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270708"
---
# <a name="create-a-new-project"></a><span data-ttu-id="c5fdb-103">Sortu proiektua</span><span class="sxs-lookup"><span data-stu-id="c5fdb-103">Create a new project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="c5fdb-104">Osatu urrats hauek proiektu berria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-104">Complete the following steps to create a new project.</span></span>

1. <span data-ttu-id="c5fdb-105">**Proiektuaren kudeaketa** orria, hautatu **Proiektu berria**, eta idatzi hurrengo balioak:</span><span class="sxs-lookup"><span data-stu-id="c5fdb-105">On the **Project management** page, select **New project**, and enter the following values:</span></span>

    - <span data-ttu-id="c5fdb-106">**Proiektu mota:** Denbora eta materiala</span><span class="sxs-lookup"><span data-stu-id="c5fdb-106">**Project type:** Time and material</span></span>
    - <span data-ttu-id="c5fdb-107">**Proiektuaren izena:** XYZ berritzea 2. fasea</span><span class="sxs-lookup"><span data-stu-id="c5fdb-107">**Project name:** XYZ Upgrade Phase 2</span></span>
    - <span data-ttu-id="c5fdb-108">**Proiektu taldea:** TM\_WIP</span><span class="sxs-lookup"><span data-stu-id="c5fdb-108">**Project group:** TM\_WIP</span></span>
    - <span data-ttu-id="c5fdb-109">**Proiektuaren kontratua ID:** 00000002</span><span class="sxs-lookup"><span data-stu-id="c5fdb-109">**Project contract ID:** 00000002</span></span>

2. <span data-ttu-id="c5fdb-110">Hautatu **Sortu proiektua**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-110">Select **Create project**.</span></span>

## <a name="assign-a-resource-to-a-project"></a><span data-ttu-id="c5fdb-111">Esleitu baliabide bat proiektu bati</span><span class="sxs-lookup"><span data-stu-id="c5fdb-111">Assign a resource to a project</span></span>

1. <span data-ttu-id="c5fdb-112">Gainean **Langileak** orrialdean, **Langileak** zerrenda, hautatu erregistroa langilearentzat aurretik konfiguratu gaitasunak horretarako, eta ireki langilearen erregistroa.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-112">On the **Workers** page, in the **Workers** list, select the record for the worker that you previously set up competencies for, and open the worker record.</span></span>
2. <span data-ttu-id="c5fdb-113">Ekintza panelean, **Proiektua** fitxan, **Konfigurazioa** taldea, hautatu **Esleitu proiektuak**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-113">On the Action Pane, on the **Project** tab, in the **Setup** group, select **Assign projects**.</span></span>
3. <span data-ttu-id="c5fdb-114">Gainean **Baliabideak balioztatzeko proiektuaren esleipenak** orrialdean, **Proiektuak** fitxan, **Gehitu proiektua hautatutako proiektuei** eremua, iragazkia **XYZ berritzea 2. fasea** proiektua.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-114">On the **Resource validation project assignments** page, on the **Projects** tab, in the **Add the project to selected projects** field, filter on the **XYZ Upgrade Phase 2** project.</span></span>
4. <span data-ttu-id="c5fdb-115">**Gainerako proiektuak** panelean, hautatu proiektu bat eta, ondoren, hautatu gezi botoia gehitzeko **Aukeratutako proiektuak** panela.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-115">In the **Remaining projects** pane, select a project, and then select the arrow button to add it to the **Selected projects** pane.</span></span>

<span data-ttu-id="c5fdb-116">Baliabide batentzako kategoriak ere eska ditzakezu nahi duzun moduan.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-116">You can also assign categories for a resource as you require.</span></span> <span data-ttu-id="c5fdb-117">Kategoria mota bai da **Kostua** edo **Diru-sarrerak**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-117">The category type is either **Cost** or **Revenue**.</span></span> <span data-ttu-id="c5fdb-118">Kategoria mota zure erakundeak zehazten du.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-118">The category type is determined by your organization.</span></span> <span data-ttu-id="c5fdb-119">Baliabide batentzako kategoriarik esleitzen ez bada, Finantzak kostuen eta diru-sarreren orduen prezioen kategoria lehenetsia bilatzen du.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-119">If no categories are assigned for a resource, Finance looks up the default category on hour prices for cost and revenue.</span></span>

## <a name="set-up-project-resource-and-role-characteristics"></a><span data-ttu-id="c5fdb-120">Ezarri proiektuaren baliabideen eta rolen ezaugarriak</span><span class="sxs-lookup"><span data-stu-id="c5fdb-120">Set up project resource and role characteristics</span></span>

<span data-ttu-id="c5fdb-121">Proiektu kudeatzaile batek proiektuaren baliabideen funtzionalitatea erabil dezake proiektuan beharrezkoak diren rolak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-121">A project manager can use the project resourcing functionality to create the roles that are required for the project.</span></span> <span data-ttu-id="c5fdb-122">Rolak erabil daitezke baliabideak erreserbatzen direnean berretsitako baliabideak oraindik ezezagunak badira.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-122">Roles can be used if confirmed resources are still unknown when resources are being reserved.</span></span> <span data-ttu-id="c5fdb-123">Eginkizunak aldi baterako gorde daitezke aurreikusitako baliabide gisa, proiektuaren plangintza faseak jarraitu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-123">Roles can be temporarily reserved as planned resources, so that you can continue the project planning stages.</span></span>

<span data-ttu-id="c5fdb-124">[![Rol baten adibidea](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span><span class="sxs-lookup"><span data-stu-id="c5fdb-124">[![Example of a role](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span></span> 

<span data-ttu-id="c5fdb-125">**Eszenatokia:** Contoso kontratatu zen onartutako proiektuen karta duen Denbora eta material proiektu bat osatzeko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-125">**Scenario:** Contoso was hired to complete a Time and material project that has an approved project charter.</span></span> <span data-ttu-id="c5fdb-126">Proiektu zuzendari gaztea proiektuaren esparrua osatzen ari da oraindik.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-126">The junior project manager is still completing the scope of the project.</span></span> <span data-ttu-id="c5fdb-127">Baliabideen kudeatzailea proiektu berrian lan egiteko gordetako baliabide zehatzak identifikatzen ari da.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-127">The resource manager is currently identifying specific resources that will be reserved to work on the new project.</span></span> <span data-ttu-id="c5fdb-128">Proiektuaren izaera kritikoa dela eta, proiektuaren babesleak proiektu nagusiko zuzendaria eskatu zuen eginkizunetako bat izateko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-128">Because of the critical nature of the project, the project sponsor requested Senior project manager as one of the roles.</span></span> <span data-ttu-id="c5fdb-129">Baliabideen kudeatzaileak baliabide berria eskuratu behar du eta sistemako rola definitu behar du, proiektuaren kudeatzaile juniorrak proiektuaren plangintza egitean baliabideen informazioa behar badu.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-129">The resource manager must acquire the new resource and define the role in the system in case the junior project manager requires the resource information during project planning.</span></span>

<span data-ttu-id="c5fdb-130">Ondorengo pausoek erakusten dute baliabideen kudeatzaileak proiektuaren arduradun nagusiaren eginkizuna nola konfigura dezakeen eta baliabideen ezaugarriak harekin lotzen dituen.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-130">The following steps show how the resource manager can set up the Senior project manager role and associate resource characteristics with it.</span></span> <span data-ttu-id="c5fdb-131">Geroago, eginkizuna eskatutako baliabideen eskumenekin bat datozen baliabide erabilgarriak bilatzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-131">Later, the role can be used to search for available resources that match the required resource competencies.</span></span>

1. <span data-ttu-id="c5fdb-132">**Konfigurazio-funtzioak** orria, hautatu **Berria**, eta idatzi hurrengo balioak:</span><span class="sxs-lookup"><span data-stu-id="c5fdb-132">On the **Setup roles** page, select **New**, and enter the following values:</span></span>

    - <span data-ttu-id="c5fdb-133">**Rolaren IDa:** Proiektu zuzendari nagusia</span><span class="sxs-lookup"><span data-stu-id="c5fdb-133">**Role ID:** Senior Project Manager</span></span>
    - <span data-ttu-id="c5fdb-134">**Deskribapena:** Proiektu zuzendari nagusia</span><span class="sxs-lookup"><span data-stu-id="c5fdb-134">**Description:** Senior Project Manager</span></span>

2. <span data-ttu-id="c5fdb-135">Hautatu **Sortu**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-135">Select **Create**.</span></span>
3. <span data-ttu-id="c5fdb-136">Aukeratu **Proiektu zuzendari nagusia** rola, eta hautatu **Ezaugarriak konfiguratu**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-136">Select the **Senior Project Manager** role, and then select **Configure characteristics**.</span></span>
4. <span data-ttu-id="c5fdb-137">**Ezaugarri mota** eremua, hautatu **Gaitasuna**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-137">In the **Characteristics type** field, select **Skill**.</span></span>
5. <span data-ttu-id="c5fdb-138">**Erabilgarri dauden ezaugarriak** eremuan, sartu bilatu beharreko trebetasuna.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-138">In the **Available characteristics** field, enter the skill to search for.</span></span>
6. <span data-ttu-id="c5fdb-139">**Ezaugarrien mota** eremua, hautatu **Ziurtagiria**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-139">In the **Characteristic type** field, select **Certificate**.</span></span>
7. <span data-ttu-id="c5fdb-140">**Erabilgarri dauden ezaugarriak** eremuan, sartu bilatu beharreko ziurtagiri mota.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-140">In the **Available characteristics** field, enter the certificate type to search for.</span></span>

## <a name="assign-a-project-resource-to-a-project"></a><span data-ttu-id="c5fdb-141">Esleitu proiektuaren baliabide bat proiektu bati</span><span class="sxs-lookup"><span data-stu-id="c5fdb-141">Assign a project resource to a project</span></span>

1. <span data-ttu-id="c5fdb-142">Gainean **Proiektu guztiak** orria, hautatu **XYZ berritzea 2. fasea** proiektua.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-142">On the **All projects** page, select the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="c5fdb-143">Gainean **Proiektu taldea eta programazioa** fitxa, hautatu **Gehitu**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-143">On the **Project team and scheduling** tab, select **Add**.</span></span>
3. <span data-ttu-id="c5fdb-144">**Rola** eremua, hautatu **Taldekidea**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-144">In the **Role** field, select **Team member**.</span></span>
4. <span data-ttu-id="c5fdb-145">Hautatu **Erreserbatu egutegia**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-145">Select **Book from calendar**.</span></span>
5. <span data-ttu-id="c5fdb-146">Gainean **Baliabideen erabilgarritasuna** orrialdea, hautatu **Ikusi ezarpenak**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-146">On the **Resource availability** page, select **View settings**.</span></span>
6. <span data-ttu-id="c5fdb-147">Gainean **Doitu ikuspegiaren ezarpenak** orrian, sartu balio hauek:</span><span class="sxs-lookup"><span data-stu-id="c5fdb-147">On the **Adjust view settings** page, enter the following values:</span></span>

    - <span data-ttu-id="c5fdb-148">**Data tartea ikusteko formatua:** Eguna</span><span class="sxs-lookup"><span data-stu-id="c5fdb-148">**Format for date range view:** Day</span></span>
    - <span data-ttu-id="c5fdb-149">**Bistaratu erabilgarritasunaren deskribapenak:** Bai</span><span class="sxs-lookup"><span data-stu-id="c5fdb-149">**Display availability descriptions:** Yes</span></span>
    - <span data-ttu-id="c5fdb-150">**Gainerako edukiera bistaratu:** Bai</span><span class="sxs-lookup"><span data-stu-id="c5fdb-150">**Display remaining capacity:** Yes</span></span>

7. <span data-ttu-id="c5fdb-151">Baliabide-zerrendan, hautatu baliabidea.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-151">In the list of resources, select a resource.</span></span>
8. <span data-ttu-id="c5fdb-152">Aukeratu **Liburu gogorra** eta **Edukiera osoa**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-152">Select **Hard book** and **Full capacity**.</span></span>

## <a name="assign-a-resource-to-a-default-role"></a><span data-ttu-id="c5fdb-153">Esleitu baliabidea lehenetsitako funtzioa</span><span class="sxs-lookup"><span data-stu-id="c5fdb-153">Assign a resource to a default role</span></span>

<span data-ttu-id="c5fdb-154">Proiektu edo baliabideen kudeatzaileek proiektu baterako gorde daitezkeen baliabideak sakondu ditzakete.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-154">To help project or resource managers can drill down further on the resources that can be reserved for a project.</span></span> <span data-ttu-id="c5fdb-155">Rol lehenetsia lehendik dagoen baliabide batekin edo eskuratu berri den baliabide batekin lotu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-155">You can associate a default role with an existing resource or a newly acquired resource.</span></span> <span data-ttu-id="c5fdb-156">Adibidez, Daniel kontratatu zutenean, esperientzia eta trebetasunak zituen Enpresa analista papera betetzeko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-156">For example, when Daniel was hired, he had the experience and skills to fill the Business analyst role.</span></span> <span data-ttu-id="c5fdb-157">Baliabideen kudeatzaileak rol hau Danielen lehenetsitako rol gisa izendatu du.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-157">The resource manager assigned this role as Daniel's default role.</span></span> <span data-ttu-id="c5fdb-158">Hori dela eta, baliabideen zuzendariak Daniel gehitu zuen proiektuetan lan egiteko erabilgarri dauden negozio analista multzo batean.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-158">Therefore, the resource manager added Daniel to a pool of business analysts who are available to work on projects.</span></span>

<span data-ttu-id="c5fdb-159">Baliabideak erreserbatu bitartean, proiektuen arduradunek proiektuetan lan egiteko erabilgarri dauden rol baliabideak iragazi ditzakete.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-159">During resource reservation, project managers can filter the role resources that are available to work on projects.</span></span> <span data-ttu-id="c5fdb-160">Informazio hori irizpide gisa erabil dezakete, baliabideen betetzean irizpide anitzeko erabakien analisia egiten dutenean.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-160">They can use this information as one criterion when they perform multi-criteria decision analysis during resource fulfillment.</span></span> <span data-ttu-id="c5fdb-161">Iragazkiari beste baliabide batzuen ezaugarriak ere gehi ditzakete proiektu jakin baterako trebetasunak, hezkuntza eta esperientzia zehatzak dituzten baliabideak bilatzeko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-161">They can also add other resource characteristics to the filter to search for resources that have specific skills, education, and experience for a given project.</span></span>

<span data-ttu-id="c5fdb-162">**Eszenatokia:** Onartutako proiektua hasi da, eta proiektuaren zuzendari nagusiaren eginkizuna planifikatutako baliabide gisa gorde da proiektuaren plangintza fasean.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-162">**Scenario:** An approved project has started, and the Senior project manager role was reserved as a planned resource during the project planning stage.</span></span> <span data-ttu-id="c5fdb-163">Baliabideen kudeatzaileak baliabide bat eskuratu du orain Senior proiektuaren kudeatzaile rola betetzeko.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-163">The resource manager has now acquired a resource to fulfill the Senior project manager role.</span></span>

1. <span data-ttu-id="c5fdb-164">Gainean **Baliabideen zerrenda** orrialdea, hautatu **Daniel Goldschmidt**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-164">On the **Resources list** page, select **Daniel Goldschmidt**.</span></span>
2. <span data-ttu-id="c5fdb-165">**Baliabide-funtzioa** orria, hautatu **Berria**, eta idatzi hurrengo balioak:</span><span class="sxs-lookup"><span data-stu-id="c5fdb-165">On the **Resource role** page, select **New**, and enter the following values:</span></span>

    - <span data-ttu-id="c5fdb-166">**Eraginkorra:** Sartu uneko data.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-166">**Effective:** Enter the current date.</span></span>
    - <span data-ttu-id="c5fdb-167">**Iraungipena:** Sartu **Inoiz ez**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-167">**Expiration:** Enter **Never**.</span></span>
    - <span data-ttu-id="c5fdb-168">**Funtzioa:** Idatzi **Proiektu zuzendari nagusia**.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-168">**Role:** Enter **Senior Project Manager**.</span></span>

3. <span data-ttu-id="c5fdb-169">Aukeratu **Gorde**, eta gero itxi orria.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-169">Select **Save**, and then close the page.</span></span>
4. <span data-ttu-id="c5fdb-170">Gainean **Konpetentziak** fitxa, gehitu **ProjectMgmt** trebetasuna eta **PMP** ziurtagiria.</span><span class="sxs-lookup"><span data-stu-id="c5fdb-170">On the **Competencies** tab, add the **ProjectMgmt** skill and the **PMP** certificate.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]