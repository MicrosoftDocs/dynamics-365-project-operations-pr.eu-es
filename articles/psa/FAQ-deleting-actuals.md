---
title: Zergatik ezin ditut ezabatu erregistroak uneko datuak entitatetik?
description: Gai honek uneko entitateko erregistroak zergatik ezin dituzu ezabatu azaltzen du.
author: JPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: f47e7ccd46642dc6129fbb3beac3c9490160d046
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071162"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="8aa2b-103">Zergatik ezin ditut ezabatu erregistroak uneko datuak entitatetik?</span><span class="sxs-lookup"><span data-stu-id="8aa2b-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8aa2b-104">Project Service Automation-ek (PSA) ez dizu egiteak ezabatzen uzten, beherantzko sistemetan finantza eraginak dituzten transakzioetarako egiaren iturri direlako.</span><span class="sxs-lookup"><span data-stu-id="8aa2b-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="8aa2b-105">Unekoak ezabatu balira, finantza-jakinarazpenen transakzioen osotasuna zalantzan jarri liteke.</span><span class="sxs-lookup"><span data-stu-id="8aa2b-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="8aa2b-106">Ikuskaritza-ibilbidea ezartzeko, bezeroek kutxako liburuak erabili beharko dituzte konpentsazio-transakzioak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="8aa2b-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

