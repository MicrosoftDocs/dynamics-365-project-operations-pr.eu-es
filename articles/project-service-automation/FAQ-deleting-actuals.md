---
title: Zergatik ezin ditut ezabatu erregistroak uneko datuak entitatetik?
description: Gai honek uneko entitateko erregistroak zergatik ezin dituzu ezabatu azaltzen du.
author: JPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.prod: Project Service
ms.technology: Applies to all versions of Project Service
ms.assetid: ff504c34-7337-474f-89e8-d8afdd1e0a98
ms.author: Jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5817940933c161dccac0fe549fabacbe57e7077a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748818"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="3af83-103">Zergatik ezin ditut ezabatu erregistroak uneko datuak entitatetik?</span><span class="sxs-lookup"><span data-stu-id="3af83-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3af83-104">Project Service Automation-ek (PSA) ez dizu egiteak ezabatzen uzten, beherantzko sistemetan finantza eraginak dituzten transakzioetarako egiaren iturri direlako.</span><span class="sxs-lookup"><span data-stu-id="3af83-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="3af83-105">Unekoak ezabatu balira, finantza-jakinarazpenen transakzioen osotasuna zalantzan jarri liteke.</span><span class="sxs-lookup"><span data-stu-id="3af83-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="3af83-106">Ikuskaritza-ibilbidea ezartzeko, bezeroek kutxako liburuak erabili beharko dituzte konpentsazio-transakzioak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="3af83-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

