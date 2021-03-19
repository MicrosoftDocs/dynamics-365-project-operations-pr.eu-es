---
title: Project Operations eremuak prezio-dimentsio gisa
description: Gai honek Dynamics 365 Project Operations-en eremuak prezio-dimentsio gisa erabiltzeari buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 04b823e8237590a294ed0706e64d0ecb9d2cf56f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274623"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="44a1f-103">Project Operations eremuak prezio-dimentsio gisa</span><span class="sxs-lookup"><span data-stu-id="44a1f-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="44a1f-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="44a1f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="44a1f-105">**Benetako datuak** entitateak baliabideetan oinarritutako prezioen prezio-dimentsio gisa erabil daitezkeen eremu asko ditu.</span><span class="sxs-lookup"><span data-stu-id="44a1f-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="44a1f-106">Adibidez, eremu arrunt bat **Baliabide erreserbagarria** da.</span><span class="sxs-lookup"><span data-stu-id="44a1f-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="44a1f-107">Baliteke 20-30 baliabide fakturagarri baino gutxiago dituzten enpresa txikien iritziz, baliabide bakoitzerako faktura eta kostu tasak edukitzea ikuspegi sinpleagoa izatea.</span><span class="sxs-lookup"><span data-stu-id="44a1f-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="44a1f-108">Hala ere, fakturatzeko plantilla hazten den neurrian, baliabideen araberako tasak mantentzea ez da errealista bihur daiteke.</span><span class="sxs-lookup"><span data-stu-id="44a1f-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="44a1f-109">Baliabideen kostua eta fakturazio tasak aldatzen hasten dira baliabideak sustatu, esperientzia gehiago lortzen edo beste gaitasun multzo bat eskuratzen duten heinean.</span><span class="sxs-lookup"><span data-stu-id="44a1f-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="44a1f-110">Beste adibide bat transakzioaen kategoria da.</span><span class="sxs-lookup"><span data-stu-id="44a1f-110">Another example is that of transaction category.</span></span> <span data-ttu-id="44a1f-111">Bezeroek eta inplementatzaileek transakzioen kategoria erabili dute lana sailkatzeko eta eremua erabili dute prezioa eta kostua lanaren kategorian oinarrituta ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="44a1f-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]