---
title: Produktuetan oinarritutako abagunearen lerroak - arina
description: Gai honek proiektuan oinarritutako abagunearen lerro-elementuei buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b826bf3a1320eee2758af7a094e9f1c2eac6a119
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764939"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="5db88-103">Produktuetan oinarritutako abagunearen lerroak - arina</span><span class="sxs-lookup"><span data-stu-id="5db88-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="5db88-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="5db88-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5db88-105">Produktuan oinarritutako abagunearen lerroak Abaguneko lerro-elementuak dira.</span><span class="sxs-lookup"><span data-stu-id="5db88-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="5db88-106">Lerro-elementu bereiziak bezeroari ematen zaion fakturan daude.</span><span class="sxs-lookup"><span data-stu-id="5db88-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="5db88-107">Fakturan ez dago beste zerbitzu osagarririk.</span><span class="sxs-lookup"><span data-stu-id="5db88-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="5db88-108">Lotutako gastua eta kontsumoa ez dira erlazionatutako proiektuetako zereginetan jarraitzen.</span><span class="sxs-lookup"><span data-stu-id="5db88-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="5db88-109">Produktuetan oinarritutako lerroak katalogoko elementuak edo idazteko produktuak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="5db88-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="5db88-110">Aukera baten produktuan oinarritutako lerroetako funtzionalitate gehienek Dynamics 365 Sales aplikazioak emandako funtzionalitatea jarraitzen dute.</span><span class="sxs-lookup"><span data-stu-id="5db88-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="5db88-111">Produktuan oinarritutako abagune-lerroei buruzko informazio gehiago lortzeko, ikusi [Gehitu produktuak abagune batean](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="5db88-111">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="5db88-112">**Bezeroaren aurrekontua** proiektuetan oinarritutako aukera-lerroetarako espezifikoa den kontzeptua da.</span><span class="sxs-lookup"><span data-stu-id="5db88-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="5db88-113">**Bezeroaren aurrekontua** eremuak bezeroak elementua ordaintzeko prest duen zenbatekoa jarraitzen du.</span><span class="sxs-lookup"><span data-stu-id="5db88-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="5db88-114">Aukera laburpenaren diru-sarreren metodoa denean **Kalkulatutako sistema**, aukera-lerroetako bezeroen aurrekontuaren balioak laburbiltzen dira kalkulatutako diru-sarrerak kalkulatzeko.</span><span class="sxs-lookup"><span data-stu-id="5db88-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 

