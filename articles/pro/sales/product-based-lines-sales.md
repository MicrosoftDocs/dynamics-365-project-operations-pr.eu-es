---
title: Produktuetan oinarritutako abagunearen lerroak - arina
description: Gai honek proiektuan oinarritutako abagunearen lerro-elementuei buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7865da682ae607f017bf59ce1ae1addc9fefa60b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994481"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="0d3a2-103">Produktuetan oinarritutako abagunearen lerroak - arina</span><span class="sxs-lookup"><span data-stu-id="0d3a2-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="0d3a2-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="0d3a2-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0d3a2-105">Produktuan oinarritutako abagunearen lerroak Abaguneko lerro-elementuak dira.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="0d3a2-106">Lerro-elementu bereiziak bezeroari ematen zaion fakturan daude.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="0d3a2-107">Fakturan ez dago beste zerbitzu osagarririk.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="0d3a2-108">Lotutako gastua eta kontsumoa ez dira erlazionatutako proiektuetako zereginetan jarraitzen.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="0d3a2-109">Produktuetan oinarritutako lerroak katalogoko elementuak edo idazteko produktuak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="0d3a2-110">Aukera baten produktuan oinarritutako lerroetako funtzionalitate gehienek Dynamics 365 Sales aplikazioak emandako funtzionalitatea jarraitzen dute.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="0d3a2-111">Produktuan oinarritutako abagune-lerroei buruzko informazio gehiago lortzeko, ikusi [Gehitu produktuak abagune batean](/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="0d3a2-111">For more information about product-based opportunity lines, see [Add products to an opportunity](/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="0d3a2-112">**Bezeroaren aurrekontua** proiektuetan oinarritutako aukera-lerroetarako espezifikoa den kontzeptua da.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="0d3a2-113">**Bezeroaren aurrekontua** eremuak bezeroak elementua ordaintzeko prest duen zenbatekoa jarraitzen du.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="0d3a2-114">Aukera laburpenaren diru-sarreren metodoa denean **Kalkulatutako sistema**, aukera-lerroetako bezeroen aurrekontuaren balioak laburbiltzen dira kalkulatutako diru-sarrerak kalkulatzeko.</span><span class="sxs-lookup"><span data-stu-id="0d3a2-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 



[!INCLUDE[footer-include](../../includes/footer-banner.md)]