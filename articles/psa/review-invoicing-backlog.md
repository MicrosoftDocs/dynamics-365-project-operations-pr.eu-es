---
title: Berrikusi proiektuen eta proiektuen kontratuen fakturazioaren lana
description: Gai honek denbora, gastua eta produktuen atzerapenak nola berrikusi eta fakturaziorako prest daudela markatzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: ''
ms.author: rumant
ms.date: 03/11/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: eb6d942d61bf8b5d20afb75c88716132a596bcbd
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071245"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="81384-103">Berrikusi proiektuen eta proiektuen kontratuen fakturazioaren lana</span><span class="sxs-lookup"><span data-stu-id="81384-103">Review the invoicing backlog on projects and project contracts</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="81384-104">Transakzioa faktura sortzeko eta prozesatzeko prest dagoenean, transakzioa **Fakturatzeko prest** gisa markatu beharko litzateke.</span><span class="sxs-lookup"><span data-stu-id="81384-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="81384-105">Gai honetan sortu daitezkeen transakzio motak deskribatzen dira.</span><span class="sxs-lookup"><span data-stu-id="81384-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="81384-106">Berrikusi denbora eta materialen fakturazioaren lana</span><span class="sxs-lookup"><span data-stu-id="81384-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="81384-107">Proiektu baterako denbora edo gastu sarrera bat bidaltzen eta onartzen denean, PSA-k proiektu bat sortzen du.</span><span class="sxs-lookup"><span data-stu-id="81384-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="81384-108">Proiektuaren eta transakzioen klasearen konbinazioa denbora eta materialen proiektu baterako kontratuaren lerro bati esleitzen bazaio, sarrera onartzean benetako bi datu sortzen dira:</span><span class="sxs-lookup"><span data-stu-id="81384-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="81384-109">Benetako kostua</span><span class="sxs-lookup"><span data-stu-id="81384-109">Cost actual</span></span> 
- <span data-ttu-id="81384-110">Fakturatu gabeko benetako salmentak</span><span class="sxs-lookup"><span data-stu-id="81384-110">Unbilled sales actual</span></span>

<span data-ttu-id="81384-111">Fakturatu gabeko benetako salmentek fakturazioaren lana adierazten du eta fakturazio-egoera **Fakturatzeko prest** egon behar da.</span><span class="sxs-lookup"><span data-stu-id="81384-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="81384-112">Proiektuaren faktura sortzen denean, **Fakturatzeko prest** gisa markatuta dauden fakturatu gabeko benetako salmentak fakturen lerroko xehetasun gisa kopiatzen dira.</span><span class="sxs-lookup"><span data-stu-id="81384-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="81384-113">Denbora eta materialei dagokien fakturazioaren lana ikusteko, joan **Salmentak** \> **Fakturazioa** \> **Denboraren eta materialaren fakturazioaren atala**.</span><span class="sxs-lookup"><span data-stu-id="81384-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="81384-114">Hautatu fakturatzeko prest dauden fakturatu gabeko benetako salmenta guztiak eta, ondoren, hautatu **Fakturatzeko prest**.</span><span class="sxs-lookup"><span data-stu-id="81384-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="81384-115">Datu erreal horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.</span><span class="sxs-lookup"><span data-stu-id="81384-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![Denbora eta materialen fakturazioaren lana](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="81384-117">Berrikusi produktuaren fakturazioaren lana</span><span class="sxs-lookup"><span data-stu-id="81384-117">Review the product billing backlog</span></span>

<span data-ttu-id="81384-118">PSA-n, proiektuko kontratuak produktuetan oinarritutako kontratuaren lerroak dituenean, lerro horiek fakturaziorako kontsideratzen dira proiektuaren kontratuaren faktura sortzen den bakoitzean.</span><span class="sxs-lookup"><span data-stu-id="81384-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="81384-119">**Fakturatzeko prest** gisa markatuta dauden kontratuaren lerroak dituen edozein produktu proiektuaren fakturan kopiatzen da proiektuaren faktura-lerro gisa.</span><span class="sxs-lookup"><span data-stu-id="81384-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="81384-120">Produktuen fakturazio lana berrikusteko, joan **Salmentak** \> **Fakturazioa** \> **Produktuen fakturazioaren lana** aukerara.</span><span class="sxs-lookup"><span data-stu-id="81384-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="81384-121">Hautatu fakturatzeko prest dauden produktuan oinarritutako kontratuaren lerro guztiak eta, ondoren, hautatu **Fakturatzeko prest**.</span><span class="sxs-lookup"><span data-stu-id="81384-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="81384-122">Lerro horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.</span><span class="sxs-lookup"><span data-stu-id="81384-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![Produktuaren fakturazioaren lana](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="81384-124">Berrikusi prezio finkoko kontratuen mugarriak</span><span class="sxs-lookup"><span data-stu-id="81384-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="81384-125">Prezio finkoko fakturazio-metodoa duen proiektuaren kontratuaren lerro bakoitzak zehaztu beharko ditu kontratuaren mugarriak.</span><span class="sxs-lookup"><span data-stu-id="81384-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="81384-126">Kontratuaren mugarriak horiek **Fakturatzeko prest** gisa markatuta daudenean soilik fakturatu daitezke.</span><span class="sxs-lookup"><span data-stu-id="81384-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="81384-127">Fakturazio-mugarriak berrikusteko, joan **Salmentak** \> **Fakturazioa** \> **Prezio finkoen mugarriak** atalera.</span><span class="sxs-lookup"><span data-stu-id="81384-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="81384-128">Hautatu fakturatzeko prest dauden mugarriak eta, ondoren, hautatu **Fakturatzeko prest**.</span><span class="sxs-lookup"><span data-stu-id="81384-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="81384-129">Mugarri horien fakturazio-egoera aldatu egingo da **Fakturatzeko prest** egoerara.</span><span class="sxs-lookup"><span data-stu-id="81384-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![Prezio finkoaren mugarriak](media/FPBacklog.png)
