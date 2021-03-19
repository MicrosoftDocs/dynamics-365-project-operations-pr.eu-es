---
title: Baliabideen aurreikuspenak
description: Gai honek baliabideen aurreikuspenak kalkulatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 98a61746f172b50bf6fa29cb0d21462cd616f417
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286503"
---
# <a name="resource-estimates"></a><span data-ttu-id="9d994-103">Baliabideen aurreikuspenak</span><span class="sxs-lookup"><span data-stu-id="9d994-103">Resource estimates</span></span>

<span data-ttu-id="9d994-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="9d994-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9d994-105">Baliabideen kalkuluak lanaren banakako egituran definitutako denborazko ahaleginetik datoz, aplikagarriak diren prezioen dimentsioekin batera.</span><span class="sxs-lookup"><span data-stu-id="9d994-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="9d994-106">Normalean, kalkulua da **tasa/ordu rol bakoitzeko x ordu.**</span><span class="sxs-lookup"><span data-stu-id="9d994-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="9d994-107">Baliabide bakoitzaren denbora-faseko ahalegina baliabideak esleitzeko erregistroan gordetzen da.</span><span class="sxs-lookup"><span data-stu-id="9d994-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="9d994-108">Prezioak aurrez definitutako prezioen zerrendan gordetzen dira.</span><span class="sxs-lookup"><span data-stu-id="9d994-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="9d994-109">Unitate bihurketa dagokion prezioen zerrendan oinarrituta aplikatzen da.</span><span class="sxs-lookup"><span data-stu-id="9d994-109">Unit conversion is applied based on the applicable price list.</span></span>

![Baliabideen aurreikuspenak](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="9d994-111">Kostuaren prezioei eta kostuaren moneta lehenetsia</span><span class="sxs-lookup"><span data-stu-id="9d994-111">Default cost price and cost currency</span></span>

<span data-ttu-id="9d994-112">Kostuen prezioak Antolaketa Unitatetik lehenetsita daude.</span><span class="sxs-lookup"><span data-stu-id="9d994-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="9d994-113">Fakturazio-tasa eta salmenten moneta lehenetsia</span><span class="sxs-lookup"><span data-stu-id="9d994-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="9d994-114">Salmenta prezioak behin aplikatzen dira akordio bakoitzeko.</span><span class="sxs-lookup"><span data-stu-id="9d994-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="9d994-115">Salmenta prezioen zerrenda lehenetsitako hierarkia honako hau da:</span><span class="sxs-lookup"><span data-stu-id="9d994-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="9d994-116">Erakundea</span><span class="sxs-lookup"><span data-stu-id="9d994-116">Organization</span></span>
2. <span data-ttu-id="9d994-117">Bezeroa</span><span class="sxs-lookup"><span data-stu-id="9d994-117">Customer</span></span>
3. <span data-ttu-id="9d994-118">Eskaintza/Kontratua</span><span class="sxs-lookup"><span data-stu-id="9d994-118">Quote/contract</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]