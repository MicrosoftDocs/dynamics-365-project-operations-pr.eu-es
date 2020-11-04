---
title: Proiektuaren eskaintak aztertzea
description: Gai honek proiektuaren eskaintzak aztertzeari buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0d9cefafcce33297146cae81d9ba7e68ab79aeb6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071152"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="7443a-103">Proiektuaren eskaintak aztertzea</span><span class="sxs-lookup"><span data-stu-id="7443a-103">Analysis of project quotes</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="7443a-104">Dynamics 365 Project Service Automation-ek errentagarritasuna balioesteko proiektuaren eskaintzak aztertzen ditu.</span><span class="sxs-lookup"><span data-stu-id="7443a-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="7443a-105">Eskaintza bezeroaren itxaropenekin nola lotzen den aztertzen da, entrega-data edo bukaera-data eta aurrekontuei buruzkoak.</span><span class="sxs-lookup"><span data-stu-id="7443a-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="7443a-106">Errentagarritasun-analisia</span><span class="sxs-lookup"><span data-stu-id="7443a-106">Profitability analysis</span></span>

<span data-ttu-id="7443a-107">Project Service Automation-ek errentagarritasuna aztertzen du marjina gordina eta doitutako marjina gordina erabiliz.</span><span class="sxs-lookup"><span data-stu-id="7443a-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="7443a-108">Marjina gordina formula hau erabiliz kalkulatzen da:</span><span class="sxs-lookup"><span data-stu-id="7443a-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="7443a-109">Doitutako marjina gordina formula hau erabiliz kalkulatzen da:</span><span class="sxs-lookup"><span data-stu-id="7443a-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="7443a-110">Marjina gordinaren eta doitutako marjina gordinaren balioak marjina zabalan desberdinak badira, eskaintzako lanaren zatirik handiena kargagabea delako.</span><span class="sxs-lookup"><span data-stu-id="7443a-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="7443a-111">Bezeroak espero duenaren analisia</span><span class="sxs-lookup"><span data-stu-id="7443a-111">Analysis of customer expectations</span></span>

<span data-ttu-id="7443a-112">Eskaintzak aztertu eta diagramak sor ditzakezu bezeroen itxaropenen arabera, antolaketari eta aurrekontuei dagokienez, eremu hauek lortzeko balioak sartzen badituzu:</span><span class="sxs-lookup"><span data-stu-id="7443a-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="7443a-113">**Eskatutako entrega-data** eremua eskaintzaren goiburuan.</span><span class="sxs-lookup"><span data-stu-id="7443a-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="7443a-114">**Bezeroaren aurrekontua** eremua eskaintzaren lerro bakoitzeko (proiektuan oinarritutako lerroetarako eta produktuetan oinarritutako lerroetarako).</span><span class="sxs-lookup"><span data-stu-id="7443a-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="7443a-115">Antolaketaren inguruko bezeroen itxaropenen analisia eskaintzaren lerroaren azken dataren eskaintza aldez aurretik eskatutako entrega-datarekin alderatuz egiten da eskaintzaren lerro guztietan.</span><span class="sxs-lookup"><span data-stu-id="7443a-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="7443a-116">Bezeroaren aurrekontuen itxaropenaren analisia bezeroaren aurrekontuaren guztizko zenbatekoa eskaintzaren lerroarekin konparatuz egiten da.</span><span class="sxs-lookup"><span data-stu-id="7443a-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>
