---
title: Erabili Project Service-en lehendik dagoen eremua prezio-dimentsio gisa
description: Gai honek lehendik dauden Project Service-ren eremuak prezio-dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
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
ms.openlocfilehash: 8bc3a1df7669dac43b45d781448ed5c795a65be4
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144129"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="99c01-103">Erabili Project Service-en lehendik dagoen eremua prezio-dimentsio gisa</span><span class="sxs-lookup"><span data-stu-id="99c01-103">Use an existing field in Project Service as a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="99c01-104">Project Service Automation-ek (PSA) arlo asko ditu proiektuaren erakundeetan baliabideetan oinarritutako prezioen prezio-dimentsio gisa erabil daitekeen **Benetakoak** entitatean.</span><span class="sxs-lookup"><span data-stu-id="99c01-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="99c01-105">Adibidez, eremu arrunt bat **Baliabide erreserbagarria** da.</span><span class="sxs-lookup"><span data-stu-id="99c01-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="99c01-106">Baliteke 20-30 baliabide fakturagarri baino gutxiago dituzten enpresa txikien iritziz, baliabide bakoitzerako faktura eta kostu tasak edukitzea ikuspegi sinpleagoa izatea.</span><span class="sxs-lookup"><span data-stu-id="99c01-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="99c01-107">Hala ere, langileen fakturazioa hazten den neurrian, tarifa zehatzak mantentzea ezinezkoa izan liteke baliabideen kostua eta fakturen tasak aldatzen hasten direnean baliabideak sustatzen diren, esperientzia gehiago eskuratzen duten edo gaitasun multzo desberdina eskuratzen duzun bitartean.</span><span class="sxs-lookup"><span data-stu-id="99c01-107">However, as the billable workforce grows, specific rates could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill set.</span></span> <span data-ttu-id="99c01-108">Ikuspegi honek oraindik tamaina jakin bateko enpresetarako funtzionatzen duenez, ikusi [Erabili baliabide erreserbagarri bat prezio-dimentsio gisa](bookable-resource-pricing-dimension.md), lehendik dagoen Project Service-ren eremu bat prezio-dimentsio gisa nola erabil daitekeen ulertzeko.</span><span class="sxs-lookup"><span data-stu-id="99c01-108">Because this approach still works for companies of a certain size, see [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="99c01-109">Beste adibide bat transakzioaen kategoria da.</span><span class="sxs-lookup"><span data-stu-id="99c01-109">Another example is that of transaction category.</span></span> <span data-ttu-id="99c01-110">Bezeroek eta inplementatzaileek PSA-ko transakzioen kategoria erabili dute lana sailkatzeko eta eremua erabili dute prezioa eta kostua lanaren kategorian oinarrituta ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="99c01-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="99c01-111">Informazio gehiago lortzeko, ikusi [Erabili transakzioen kategoria prezio-dimentsio gisa](transaction-category-pricing-dimension.md).</span><span class="sxs-lookup"><span data-stu-id="99c01-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>
