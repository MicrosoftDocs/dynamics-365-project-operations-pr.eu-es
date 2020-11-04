---
title: Baliabideen aurreikuspenak
description: Gai honek baliabideen aurreikuspenak kalkulatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070956"
---
# <a name="resource-estimates"></a><span data-ttu-id="a8d30-103">Baliabideen aurreikuspenak</span><span class="sxs-lookup"><span data-stu-id="a8d30-103">Resource estimates</span></span>

<span data-ttu-id="a8d30-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="a8d30-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a8d30-105">Baliabideen kalkuluak lanaren banakako egituran definitutako denborazko ahaleginetik datoz, aplikagarriak diren prezioen dimentsioekin batera.</span><span class="sxs-lookup"><span data-stu-id="a8d30-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="a8d30-106">Normalean, kalkulua da **tasa/ordu rol bakoitzeko x ordu.**</span><span class="sxs-lookup"><span data-stu-id="a8d30-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="a8d30-107">Baliabide bakoitzaren denbora-faseko ahalegina baliabideak esleitzeko erregistroan gordetzen da.</span><span class="sxs-lookup"><span data-stu-id="a8d30-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="a8d30-108">Prezioak aurrez definitutako prezioen zerrendan gordetzen dira.</span><span class="sxs-lookup"><span data-stu-id="a8d30-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="a8d30-109">Unitate bihurketa dagokion prezioen zerrendan oinarrituta aplikatzen da.</span><span class="sxs-lookup"><span data-stu-id="a8d30-109">Unit conversion is applied based on the applicable price list.</span></span>

![Baliabideen aurreikuspenak](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="a8d30-111">Kostuaren prezioei eta kostuaren moneta lehenetsia</span><span class="sxs-lookup"><span data-stu-id="a8d30-111">Default cost price and cost currency</span></span>

<span data-ttu-id="a8d30-112">Kostuen prezioak Antolaketa Unitatetik lehenetsita daude.</span><span class="sxs-lookup"><span data-stu-id="a8d30-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="a8d30-113">Fakturazio-tasa eta salmenten moneta lehenetsia</span><span class="sxs-lookup"><span data-stu-id="a8d30-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="a8d30-114">Salmenta prezioak behin aplikatzen dira akordio bakoitzeko.</span><span class="sxs-lookup"><span data-stu-id="a8d30-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="a8d30-115">Salmenta prezioen zerrenda lehenetsitako hierarkia honako hau da:</span><span class="sxs-lookup"><span data-stu-id="a8d30-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="a8d30-116">Erakundea</span><span class="sxs-lookup"><span data-stu-id="a8d30-116">Organization</span></span>
2. <span data-ttu-id="a8d30-117">Bezeroa</span><span class="sxs-lookup"><span data-stu-id="a8d30-117">Customer</span></span>
3. <span data-ttu-id="a8d30-118">Eskaintza/Kontratua</span><span class="sxs-lookup"><span data-stu-id="a8d30-118">Quote/contract</span></span>
