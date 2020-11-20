---
title: Zergatik da prezio lehenetsia zero uneko kostuen benetako gastuen kostua?
description: Uneko gastuen kostuan prezio lehenetsia 0 izatea arazoa konpontzeko.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
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
ms.openlocfilehash: 306f169ee25d42ac3c9e63fa70956b9c50315829
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122103"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="5b852-103">Zergatik da prezio lehenetsia zero uneko kostuen benetako gastuen kostua?</span><span class="sxs-lookup"><span data-stu-id="5b852-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="5b852-104">Hau ri buruzko FAQ aplikatzen expense emaitzetan non transakzio heredatzen da Expense eta transakzio mota ez dago Kostua.</span><span class="sxs-lookup"><span data-stu-id="5b852-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="5b852-105">Arazo-konpontzeari buruzko kostua tasak expense benetako kostua:</span><span class="sxs-lookup"><span data-stu-id="5b852-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="5b852-106">Erlazionatutako expense sarrera joan eta dela bat expense sarrera eremu ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="5b852-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="5b852-107">Jatorrizko expense sarrera zenbatekoa eremua bete behar ez, ondoren, duzu izan isolated arazoa.</span><span class="sxs-lookup"><span data-stu-id="5b852-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="5b852-108">Arazo hau merkatura, sortu berriro zenbatekoa baliogabea duen expense sarrera eta onartu da.</span><span class="sxs-lookup"><span data-stu-id="5b852-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
