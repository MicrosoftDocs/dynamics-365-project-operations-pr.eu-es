---
title: Sortu prezio-dimentsioen soluzio pertsonalizatuak
description: Gai honek prezio pertsonalizatuko neurriak sortzerakoan irtenbide pertsonalizatua nola sortu azaltzen du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d8117d6f6bcedc97264401fc941470f34efb1ae
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284973"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="9f4de-103">Sortu prezio-dimentsioen soluzio pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="9f4de-103">Create custom solutions for pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> <span data-ttu-id="9f4de-104">Prezio pertsonalizatuen dimentsio aldaketa guztiek beste irtenbide batean egon behar dute.</span><span class="sxs-lookup"><span data-stu-id="9f4de-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="9f4de-105">Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du.</span><span class="sxs-lookup"><span data-stu-id="9f4de-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="9f4de-106">Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **Kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="9f4de-106">After you make the required changes, export this solution as a **Managed solution**, and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="9f4de-107">Aukeratu **Ezarpenak** > **Soluzioak** eta, ondoren, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="9f4de-107">Select **Settings** > **Solutions**, and then select **New**.</span></span> 
2. <span data-ttu-id="9f4de-108">Soluzioari eman **\<your organization name> prezio-dimentsioak** izena, sartu gainerako beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.</span><span class="sxs-lookup"><span data-stu-id="9f4de-108">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>

> ![Sortu prezio-dimentsioetarako soluzio pertsonalizatua](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="9f4de-110">Gehitu beharrezko entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan</span><span class="sxs-lookup"><span data-stu-id="9f4de-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="9f4de-111">Project Service-eko entitate hauek gehitu beharko dituzu prezio-soluzioan.</span><span class="sxs-lookup"><span data-stu-id="9f4de-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="9f4de-112">Osatu prozedura honen urratsak prezio-soluzioaren eskema garrantzitsu batzuk egiteko, entitateak prezio-dimentsio berriez jabetzeko.</span><span class="sxs-lookup"><span data-stu-id="9f4de-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="9f4de-113">Hautatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name>prezio-dimentsioa**.</span><span class="sxs-lookup"><span data-stu-id="9f4de-113">Select **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="9f4de-114">Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Gehitu badaudenak** > **Entitateak**.</span><span class="sxs-lookup"><span data-stu-id="9f4de-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="9f4de-115">**Soluzio-osagaiak** elkarrizketa-koadroan, hautatu aukera hauetariko bat:</span><span class="sxs-lookup"><span data-stu-id="9f4de-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="9f4de-116">Unekoa"</span><span class="sxs-lookup"><span data-stu-id="9f4de-116">Actual</span></span>
- <span data-ttu-id="9f4de-117">Baliabide erreserbagarria</span><span class="sxs-lookup"><span data-stu-id="9f4de-117">Bookable Resource</span></span>
- <span data-ttu-id="9f4de-118">Aurreikuspenaren lerroa</span><span class="sxs-lookup"><span data-stu-id="9f4de-118">Estimate Line</span></span>
- <span data-ttu-id="9f4de-119">Proiektuaren zeregina</span><span class="sxs-lookup"><span data-stu-id="9f4de-119">Project Task</span></span>
- <span data-ttu-id="9f4de-120">Fakturaren lerroaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="9f4de-120">Invoice Line Detail</span></span>
- <span data-ttu-id="9f4de-121">Kutxako liburuaren lerroa</span><span class="sxs-lookup"><span data-stu-id="9f4de-121">Journal Line</span></span>
- <span data-ttu-id="9f4de-122">Proiektu-kontratuaren lerroko xehetasunak</span><span class="sxs-lookup"><span data-stu-id="9f4de-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="9f4de-123">Proiektu-taldeko kidea</span><span class="sxs-lookup"><span data-stu-id="9f4de-123">Project Team Member</span></span>
- <span data-ttu-id="9f4de-124">Eskaintzaren lerroaren xehetasunak</span><span class="sxs-lookup"><span data-stu-id="9f4de-124">Quote Line Detail</span></span>
- <span data-ttu-id="9f4de-125">Funtzio-prezioaren gainprezioa</span><span class="sxs-lookup"><span data-stu-id="9f4de-125">Role Price Markup</span></span>
- <span data-ttu-id="9f4de-126">Funtzioaren prezioa</span><span class="sxs-lookup"><span data-stu-id="9f4de-126">Role Price</span></span> 
- <span data-ttu-id="9f4de-127">Denbora-sarrera</span><span class="sxs-lookup"><span data-stu-id="9f4de-127">Time Entry</span></span> 

> ![Gehitu lehendik dauden entitateak prezio-dimentsioen soluzioari](media/Existing-entities-to-PD-solution.png)

> ![Hautatu soluzioaren osagaiak](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="9f4de-130">Ziurtatu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak sartzea.</span><span class="sxs-lookup"><span data-stu-id="9f4de-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="9f4de-131">Hautatutako entitateen menpeko erakunderen bat eskatuko zaizunean, hautatu **Ez** aukeran.</span><span class="sxs-lookup"><span data-stu-id="9f4de-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![Ez sartu erlazionatutako osagaiak](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]