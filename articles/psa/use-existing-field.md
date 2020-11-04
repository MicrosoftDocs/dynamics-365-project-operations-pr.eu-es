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
ms.openlocfilehash: 415e346f88e60cb064f3327bfb35e21bd1c89014
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071114"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="15a9e-103">Erabili Project Service-en lehendik dagoen eremua prezio-dimentsio gisa</span><span class="sxs-lookup"><span data-stu-id="15a9e-103">Use an existing field in Project Service as a pricing dimension</span></span>

<span data-ttu-id="15a9e-104">Project Service Automation-ek (PSA) arlo asko ditu proiektuaren erakundeetan baliabideetan oinarritutako prezioen prezio-dimentsio gisa erabil daitekeen **Benetakoak** entitatean.</span><span class="sxs-lookup"><span data-stu-id="15a9e-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="15a9e-105">Adibidez, eremu arrunt bat **Baliabide erreserbagarria** da.</span><span class="sxs-lookup"><span data-stu-id="15a9e-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="15a9e-106">Baliteke 20-30 baliabide fakturagarri baino gutxiago dituzten enpresa txikien iritziz, baliabide bakoitzerako faktura eta kostu tasak edukitzea ikuspegi sinpleagoa izatea.</span><span class="sxs-lookup"><span data-stu-id="15a9e-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="15a9e-107">Hala ere, langileen fakturazioa hazten den neurrian, hori mantentzea ezinezkoa izan liteke baliabideen kostua eta fakturen tasak aldatzen hasten direnean baliabideak sustatzen diren, esperientzia gehiago eskuratzen duten edo gaitasun multzo desberdinak eskuratzen dituzten bitartean.</span><span class="sxs-lookup"><span data-stu-id="15a9e-107">However, as the billable workforce grows, this could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill sets.</span></span> <span data-ttu-id="15a9e-108">Ikuspegi honek oraindik tamaina jakin bateko enpresetarako funtzionatzen duenez, ikusi [Erabili baliabide erreserbagarri bat prezio-dimentsio gisa](bookable-resource-pricing-dimension.md) gaia, lehendik dagoen Project Service-ren eremu bat prezio-dimentsio gisa nola erabil daitekeen ulertzeko.</span><span class="sxs-lookup"><span data-stu-id="15a9e-108">Because this approach still works for companies of a certain size, see the topic, [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="15a9e-109">Beste adibide bat transakzioaen kategoria da.</span><span class="sxs-lookup"><span data-stu-id="15a9e-109">Another example is that of transaction category.</span></span> <span data-ttu-id="15a9e-110">Bezeroek eta inplementatzaileek PSA-ko transakzioen kategoria erabili dute lana sailkatzeko eta eremua erabili dute prezioa eta kostua lanaren kategorian oinarrituta ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="15a9e-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="15a9e-111">Informazio gehiago lortzeko, ikusi [Erabili transakzioen kategoria prezio-dimentsio gisa](transaction-category-pricing-dimension.md).</span><span class="sxs-lookup"><span data-stu-id="15a9e-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>
