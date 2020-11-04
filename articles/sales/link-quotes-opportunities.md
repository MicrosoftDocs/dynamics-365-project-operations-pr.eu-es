---
title: Sortu proiektuen eskaintzak abaguneetan
description: Gai honek abagune batetik proiektuaren eskaintzak sortzeari buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 606098473db479d0015e3a7a3c01a3d3b6de9db1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070948"
---
# <a name="create-project-quotes-from-opportunities"></a><span data-ttu-id="7738d-103">Sortu proiektuen eskaintzak abaguneetan</span><span class="sxs-lookup"><span data-stu-id="7738d-103">Create project quotes from opportunities</span></span>

<span data-ttu-id="7738d-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="7738d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7738d-105">Aurrekontuak proiektuaren aukeren arabera sor daitezke modu hauetan:</span><span class="sxs-lookup"><span data-stu-id="7738d-105">Quotes can be created from project opportunities in the following ways:</span></span>

- <span data-ttu-id="7738d-106">**Eskaintzak** fitxatik **Proiektuaren abagunea** orrialdean</span><span class="sxs-lookup"><span data-stu-id="7738d-106">From the **Quotes** tab on the **Project Opportunity** page</span></span>
- <span data-ttu-id="7738d-107">Abagune-salmenten prozesu-fluxuetatik</span><span class="sxs-lookup"><span data-stu-id="7738d-107">From the Opportunity sales process flow</span></span>
- <span data-ttu-id="7738d-108">Lehendik dagoen aurrekontu batean aukeraren erreferentzia eguneratuta</span><span class="sxs-lookup"><span data-stu-id="7738d-108">By updating the opportunity reference on an existing quote</span></span>

## <a name="from-the-quotes-tab-of-the-project-opportunity-page"></a><span data-ttu-id="7738d-109">Proiektuaren abagunea orrialdearen Eskaintzak fitxatik</span><span class="sxs-lookup"><span data-stu-id="7738d-109">From the Quotes tab of the Project Opportunity page</span></span>

<span data-ttu-id="7738d-110">Abagune batetik proiektuaren eskaintza sortzeko, egin urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="7738d-110">To create a project quote from an opportunity, complete the following steps.</span></span>

1. <span data-ttu-id="7738d-111">Ireki **Proiektuaren abagunea** orria eta hautatu **Eskaintzak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="7738d-111">Open the **Project Opportunity** page and select the **Quotes** tab.</span></span> 
2. <span data-ttu-id="7738d-112">**Eskaintzak** azpisaretan, hautatu **+** proiektuaren eskaintza berri bat sortzeko aukeran abagunean.</span><span class="sxs-lookup"><span data-stu-id="7738d-112">On the **Quotes** sub-grid, select the **+** to create a new project quote based on the opportunity.</span></span> <span data-ttu-id="7738d-113">Aukera lerro guztiak eta horrekin lotutako Proiektuen prezio zerrenda guztiak aukeraren aurrekontu berrian kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="7738d-113">All of the opportunity lines and related Project price lists are copied to the new quote from the opportunity.</span></span>

## <a name="from-the-opportunity-sales-process-flow"></a><span data-ttu-id="7738d-114">Abagune-salmenten prozesu-fluxuetatik</span><span class="sxs-lookup"><span data-stu-id="7738d-114">From the Opportunity sales process flow</span></span>

<span data-ttu-id="7738d-115">Abaguneko salmenten prozesuaren fluxutik eskaintza bat sortzeko, egin urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="7738d-115">To create a quote from the Opportunity sales process flow, complete the following steps.</span></span>

1. <span data-ttu-id="7738d-116">Abaguneko salmenten prozesuaren fluxutik, ireki Abagunea.</span><span class="sxs-lookup"><span data-stu-id="7738d-116">From the Opportunity sales process flow, open the Opportunity.</span></span>
2. <span data-ttu-id="7738d-117">Hautatu **Gaitu** fasea.</span><span class="sxs-lookup"><span data-stu-id="7738d-117">Select the **Qualify** stage.</span></span> 
3. <span data-ttu-id="7738d-118">Aukeratu **Hurrengoa** eta, ondoren, hautatu **+ Sortu** aurrekontu berria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="7738d-118">Select **Next** and then select **+ Create** to create a new quote.</span></span> <span data-ttu-id="7738d-119">Eskaintza berri honetako **Laburpena** fitxako informazio gehiena abagunetik lehenetsiko da.</span><span class="sxs-lookup"><span data-stu-id="7738d-119">Most of the information on the **Summary** tab for this new quote will have defaulted from the opportunity.</span></span> 
4. <span data-ttu-id="7738d-120">Idatzi falta den edozein informazio edo eguneratu lehenetsitako balioak behar bezala **Laburpena** fitxa.</span><span class="sxs-lookup"><span data-stu-id="7738d-120">Enter in any required information that is missing, or update defaulted values as necessary on the **Summary** tab,</span></span>
5. <span data-ttu-id="7738d-121">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="7738d-121">Select **Save**.</span></span> <span data-ttu-id="7738d-122">Aurrekontu berria sortu eta aukerarekin lotzen da.</span><span class="sxs-lookup"><span data-stu-id="7738d-122">The new quote is created and associated to the opportunity.</span></span> <span data-ttu-id="7738d-123">Orain aurrekontuaren informazioa ikus dezakezu **Eskaintzak** fitxategiaren fitxa **Abagunea** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="7738d-123">You can now view the quote information on the **Quotes** tab of the **Opportunity** page.</span></span> 

   <span data-ttu-id="7738d-124">Abagunea salmenta prozesua hurrengo fasera pasatzen da, **Proposatu**.</span><span class="sxs-lookup"><span data-stu-id="7738d-124">The Opportunity sales process moves to the next stage, **Propose**.</span></span>


## <a name="by-updating-the-opportunity-reference-on-an-existing-quote"></a><span data-ttu-id="7738d-125">Lehendik dagoen aurrekontu batean aukeraren erreferentzia eguneratuta</span><span class="sxs-lookup"><span data-stu-id="7738d-125">By updating the opportunity reference on an existing quote</span></span>

<span data-ttu-id="7738d-126">Lehendik dagoen aurrekontua Aukera batekin lotu daiteke.</span><span class="sxs-lookup"><span data-stu-id="7738d-126">An existing quote can be linked to an Opportunity.</span></span> <span data-ttu-id="7738d-127">Bete urrats hauek lehendik dagoen aurrekontu baten Aukera informazioa eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="7738d-127">Complete the following steps to update the Opportunity information on an existing quote.</span></span>

1. <span data-ttu-id="7738d-128">Ireki **Eskaintza** orria eta hautatu **Laburpena** fitxa.</span><span class="sxs-lookup"><span data-stu-id="7738d-128">Open the **Quote** page and select the **Summary** tab.</span></span>
2. <span data-ttu-id="7738d-129">**Abagunea** eremuan, hautatu aurrekontuarekin estekatu nahi duzun aukera.</span><span class="sxs-lookup"><span data-stu-id="7738d-129">In the **Opportunity** field, select the opportunity that you want to link to the quote.</span></span> <span data-ttu-id="7738d-130">Aurrekontua ikusi ahal izango duzu **Eskaintzak** Aukeraren sareta.</span><span class="sxs-lookup"><span data-stu-id="7738d-130">You can see the quote in the **Quotes** grid of the Opportunity.</span></span> 
3. <span data-ttu-id="7738d-131">Aukera salmenta prozesua erabiliz, aukera hurrengo fasera pasa daiteke, **Proposatu**.</span><span class="sxs-lookup"><span data-stu-id="7738d-131">Using the Opportunity sales process, the opportunity can be moved to the next stage, **Propose**.</span></span> 

   <span data-ttu-id="7738d-132">Aukera etapa honetara mugitzen duzunean, aurrekontu hau aukera honekin lotutako aurrekontuen zerrendatik hauta dezakezu.</span><span class="sxs-lookup"><span data-stu-id="7738d-132">When you move an opportunity to this stage, you can select this quote from a list of quotes associated with this opportunity.</span></span> <span data-ttu-id="7738d-133">Aurrekontu hau hautatzeak berarekin aurrera egiten duzula adierazten du.</span><span class="sxs-lookup"><span data-stu-id="7738d-133">Selecting this quote indicates that you're moving forward with it.</span></span>

   <span data-ttu-id="7738d-134">Aukerarekin lotutako gainerako aurrekontu guztiak erabilgarri eta aktibo egongo dira horietako bat irabazi arte.</span><span class="sxs-lookup"><span data-stu-id="7738d-134">All the other quotes associated with the Opportunity will still be available and active until one of them is won.</span></span> <span data-ttu-id="7738d-135">Salmenta prozesua aurreko fasera eraman dezakezu **Gaitu** , eta aukeratu beste aurrekontu batekin aurrera egiteko.</span><span class="sxs-lookup"><span data-stu-id="7738d-135">You can move the sales process back to the previous stage **Qualify** , and pick another quote to move forward with.</span></span>
