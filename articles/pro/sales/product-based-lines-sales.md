---
title: Produktuetan oinarritutako abagunearen lerroak
description: Gai honek proiektuan oinarritutako abagunearen lerro-elementuei buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070962"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="1a4c8-103">Produktuetan oinarritutako abagunearen lerroak</span><span class="sxs-lookup"><span data-stu-id="1a4c8-103">Product-based opportunity lines</span></span>

<span data-ttu-id="1a4c8-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="1a4c8-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1a4c8-105">Produktuan oinarritutako abagunearen lerroak Abaguneko lerro-elementuak dira.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="1a4c8-106">Lerro hauek bezeroari entregatzen zaizkio fakturako lineako elementu desberdin gisa, balio erantsiko beste zerbitzurik gabe.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="1a4c8-107">Lotutako gastua eta kontsumoa ez dira erlazionatutako proiektuetako zereginetan jarraitzen.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="1a4c8-108">Produktuetan oinarritutako lerroak katalogoko elementuak edo idazteko produktuak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="1a4c8-109">Aukera baten produktuan oinarritutako lerroetako funtzionalitate gehienek Dynamics 365 Sales aplikazioak emandako funtzionalitatea jarraitzen dute.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="1a4c8-110">Produktuan oinarritutako abagune-lerroei buruzko informazio gehiago lortzeko, ikusi [Gehitu produktuak abagune batean](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="1a4c8-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="1a4c8-111">Proiektuetan oinarritutako aukeretarako espezifikoa den produktuan oinarritutako aukera lerroen inguruko kontzeptu bat da **Bezeroen aurrekontua**.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="1a4c8-112">Erabili eremu hau bezeroak lineako elementuagatik ordaintzeko prest dagoen zenbatekoaren jarraipena egiteko.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="1a4c8-113">Aukera laburpenaren diru-sarreren metodoa ezarrita badago **Kalkulatutako sistema** , bezeroen aurrekontuaren produktuak eta proiektuetan oinarritutako lerroen arteko balioak laburbiltzen dira kalkulatutako diru-sarrerak kalkulatzeko.</span><span class="sxs-lookup"><span data-stu-id="1a4c8-113">If the revenue method of the Opportunity summary is set to **System Calculated** , the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
