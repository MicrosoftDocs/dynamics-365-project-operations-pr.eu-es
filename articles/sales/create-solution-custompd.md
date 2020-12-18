---
title: Sortu prezio-dimentsio pertsonalizatuetarako soluzioa
description: Gai honek prezio-dimentsio pertsonalizatuetarako soluzioak sortzeko informazioa eskaintzen du.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 441501dff23d16960381b3f9fb4b2cceba2b3ba5
ms.sourcegitcommit: 869bde007805ef255f61b03937e4a44aeef61df9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/12/2020
ms.locfileid: "4513955"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="85edd-103">Sortu prezio-dimentsio pertsonalizatuetarako soluzioa</span><span class="sxs-lookup"><span data-stu-id="85edd-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="85edd-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="85edd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="85edd-105">Prezio pertsonalizatuen dimentsio aldaketa guztiek beste irtenbide batean egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="85edd-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="85edd-106">Praktika on garrantzitsu honek malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du.</span><span class="sxs-lookup"><span data-stu-id="85edd-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="85edd-107">Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **Kudeatuta** soluzio gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="85edd-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="85edd-108">Sortu prezio-dimentsio pertsonalizatuetarako soluzioa</span><span class="sxs-lookup"><span data-stu-id="85edd-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="85edd-109">Aukeratu **Ezarpenak** > **Soluzioak** eta, ondoren, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="85edd-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="85edd-110">Eman izena irtenbideari, *<your organization name> prezioen neurriak*.</span><span class="sxs-lookup"><span data-stu-id="85edd-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="85edd-111">Sartu geratzen den informazioa eta, ondoren, hautatu **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="85edd-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![Prezio-dimentsio pertsonalizatuen dimentsio-soluzioa sortzea](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="85edd-113">Gehitu beharrezko entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="85edd-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="85edd-114">Gehitu Project Service entitate hauek zure prezioen soluziora prezioen soluzioan eskema aldaketa garrantzitsuak egiteko.</span><span class="sxs-lookup"><span data-stu-id="85edd-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="85edd-115">Prozedura hau amaitu ondoren, entitateek prezioen dimentsio berriak ezagutuko dituzte.</span><span class="sxs-lookup"><span data-stu-id="85edd-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="85edd-116">Hautatu **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **<*zure erakundearen izena*> prezioen dimentsioak** atalean.</span><span class="sxs-lookup"><span data-stu-id="85edd-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="85edd-117">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Gehitu badaudenak** > **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="85edd-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="85edd-118">**Soluzio-osagaiak** elkarrizketa-koadroan, hautatu aukera hauetariko bat:</span><span class="sxs-lookup"><span data-stu-id="85edd-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="85edd-119">**Unekoa"**</span><span class="sxs-lookup"><span data-stu-id="85edd-119">**Actual**</span></span>
   - <span data-ttu-id="85edd-120">**Baliabide erreserbagarria**</span><span class="sxs-lookup"><span data-stu-id="85edd-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="85edd-121">**Aurreikuspenaren lerroa**</span><span class="sxs-lookup"><span data-stu-id="85edd-121">**Estimate Line**</span></span>
   - <span data-ttu-id="85edd-122">**Proiektuaren zeregina**</span><span class="sxs-lookup"><span data-stu-id="85edd-122">**Project Task**</span></span>
   - <span data-ttu-id="85edd-123">**Fakturaren lerroaren xehetasunak**</span><span class="sxs-lookup"><span data-stu-id="85edd-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="85edd-124">**Kutxako liburuaren lerroa**</span><span class="sxs-lookup"><span data-stu-id="85edd-124">**Journal Line**</span></span>
   - <span data-ttu-id="85edd-125">**Proiektu-kontratuaren lerroko xehetasunak**</span><span class="sxs-lookup"><span data-stu-id="85edd-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="85edd-126">**Proiektu-taldeko kidea**</span><span class="sxs-lookup"><span data-stu-id="85edd-126">**Project Team Member**</span></span>
   - <span data-ttu-id="85edd-127">**Eskaintzaren lerroaren xehetasunak**</span><span class="sxs-lookup"><span data-stu-id="85edd-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="85edd-128">**Funtzio-prezioaren gainprezioa**</span><span class="sxs-lookup"><span data-stu-id="85edd-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="85edd-129">**Funtzioaren prezioa**</span><span class="sxs-lookup"><span data-stu-id="85edd-129">**Role Price**</span></span>
   - <span data-ttu-id="85edd-130">**Denbora-sarrera**</span><span class="sxs-lookup"><span data-stu-id="85edd-130">**Time Entry**</span></span>
 
   ![Gehitu lehendik dauden entitateak prezio-dimentsioaren soluzioari](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="85edd-132">Entitate bakoitzerako, berrikusi gehitzen diren osagaiak eta entitate bakoitzaren entitateen aktiboen behin betiko zerrenda.</span><span class="sxs-lookup"><span data-stu-id="85edd-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="85edd-133">Sartu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak.</span><span class="sxs-lookup"><span data-stu-id="85edd-133">Include all forms and views for each of the selected entities.</span></span>

  ![Gehitutako entitateak](./media/solution-component-selection.png)


5.  <span data-ttu-id="85edd-135">Hautatutako entitateen menpeko entitateak sartzeko eskatzen zaizunean, hautatu **Ez, ez sartu beharrezko osagaiak**.</span><span class="sxs-lookup"><span data-stu-id="85edd-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![Menpeko erakundeak barne](./media/Do-not-include-required.png)
