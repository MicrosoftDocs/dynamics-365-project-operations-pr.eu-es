---
title: Project Operations eremuak prezio-dimentsio gisa
description: Gai honek eremuak prezio-dimentsioei gisa erabiltzeari buruzko informazioa eskaintzen du Dynamics 365 Project Operations-en.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 3ddf3098e45fdc9b99067b64df05e2adc0b6ad05
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896401"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="55bd3-103">Project Operations eremuak prezio-dimentsio gisa</span><span class="sxs-lookup"><span data-stu-id="55bd3-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="55bd3-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="55bd3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="55bd3-105">**Benetako datuak** entitateak baliabideetan oinarritutako prezioen prezio-dimentsio gisa erabil daitezkeen eremu asko ditu.</span><span class="sxs-lookup"><span data-stu-id="55bd3-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="55bd3-106">Adibidez, eremu arrunt bat **Baliabide erreserbagarria** da.</span><span class="sxs-lookup"><span data-stu-id="55bd3-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="55bd3-107">Baliteke 20-30 baliabide fakturagarri baino gutxiago dituzten enpresa txikien iritziz, baliabide bakoitzerako faktura eta kostu tasak edukitzea ikuspegi sinpleagoa izatea.</span><span class="sxs-lookup"><span data-stu-id="55bd3-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="55bd3-108">Hala ere, fakturatzeko plantilla hazten den neurrian, baliabideen araberako tasak mantentzea ez da errealista bihur daiteke.</span><span class="sxs-lookup"><span data-stu-id="55bd3-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="55bd3-109">Baliabideen kostua eta fakturazio tasak aldatzen hasten dira baliabideak sustatu, esperientzia gehiago lortzen edo beste gaitasun multzo bat eskuratzen duten heinean.</span><span class="sxs-lookup"><span data-stu-id="55bd3-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="55bd3-110">Beste adibide bat transakzioaen kategoria da.</span><span class="sxs-lookup"><span data-stu-id="55bd3-110">Another example is that of transaction category.</span></span> <span data-ttu-id="55bd3-111">Bezeroek eta inplementatzaileek transakzioen kategoria erabili dute lana sailkatzeko eta eremua erabili dute prezioa eta kostua lanaren kategorian oinarrituta ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="55bd3-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>
