---
title: Zergatik da prezio lehenetsia zero uneko kostuen benetako gastuen kostua?
description: Uneko gastuen kostuan prezio lehenetsia 0 izatea arazoa konpontzeko.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.prod: Project Service
ms.technology: ''
ms.assetid: bc1ebc58-c733-4310-8435-572ed9a9fef9
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3fb678822877a61d141de75aea29b7d5cdf292c4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748857"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="a8561-103">Zergatik da prezio lehenetsia zero uneko kostuen benetako gastuen kostua?</span><span class="sxs-lookup"><span data-stu-id="a8561-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a8561-104">Hau ri buruzko FAQ aplikatzen expense emaitzetan non transakzio heredatzen da Expense eta transakzio mota ez dago Kostua.</span><span class="sxs-lookup"><span data-stu-id="a8561-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="a8561-105">Arazo-konpontzeari buruzko kostua tasak expense benetako kostua:</span><span class="sxs-lookup"><span data-stu-id="a8561-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="a8561-106">Erlazionatutako expense sarrera joan eta dela bat expense sarrera eremu ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="a8561-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="a8561-107">Jatorrizko expense sarrera zenbatekoa eremua bete behar ez, ondoren, duzu izan isolated arazoa.</span><span class="sxs-lookup"><span data-stu-id="a8561-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="a8561-108">Arazo hau merkatura, sortu berriro zenbatekoa baliogabea duen expense sarrera eta onartu da.</span><span class="sxs-lookup"><span data-stu-id="a8561-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
