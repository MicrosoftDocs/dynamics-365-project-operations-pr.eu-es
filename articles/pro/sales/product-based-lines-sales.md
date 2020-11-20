---
title: Produktuetan oinarritutako abagunearen lerroak - arina
description: Gai honek proiektuan oinarritutako abagunearen lerro-elementuei buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fd32bedb94cf36f706c112a845f342d9dde19805
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176299"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="a2b16-103">Produktuetan oinarritutako abagunearen lerroak - arina</span><span class="sxs-lookup"><span data-stu-id="a2b16-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="a2b16-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="a2b16-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a2b16-105">Produktuan oinarritutako abagunearen lerroak Abaguneko lerro-elementuak dira.</span><span class="sxs-lookup"><span data-stu-id="a2b16-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="a2b16-106">Lerro hauek bezeroari entregatzen zaizkio fakturako lineako elementu desberdin gisa, balio erantsiko beste zerbitzurik gabe.</span><span class="sxs-lookup"><span data-stu-id="a2b16-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="a2b16-107">Lotutako gastua eta kontsumoa ez dira erlazionatutako proiektuetako zereginetan jarraitzen.</span><span class="sxs-lookup"><span data-stu-id="a2b16-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="a2b16-108">Produktuetan oinarritutako lerroak katalogoko elementuak edo idazteko produktuak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="a2b16-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="a2b16-109">Aukera baten produktuan oinarritutako lerroetako funtzionalitate gehienek Dynamics 365 Sales aplikazioak emandako funtzionalitatea jarraitzen dute.</span><span class="sxs-lookup"><span data-stu-id="a2b16-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="a2b16-110">Produktuan oinarritutako abagune-lerroei buruzko informazio gehiago lortzeko, ikusi [Gehitu produktuak abagune batean](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="a2b16-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="a2b16-111">Proiektuetan oinarritutako aukeretarako espezifikoa den produktuan oinarritutako aukera lerroen inguruko kontzeptu bat da **Bezeroen aurrekontua**.</span><span class="sxs-lookup"><span data-stu-id="a2b16-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="a2b16-112">Erabili eremu hau bezeroak lineako elementuagatik ordaintzeko prest dagoen zenbatekoaren jarraipena egiteko.</span><span class="sxs-lookup"><span data-stu-id="a2b16-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="a2b16-113">Aukera laburpenaren diru-sarreren metodoa ezarrita badago **Kalkulatutako sistema**, bezeroen aurrekontuaren produktuak eta proiektuetan oinarritutako lerroen arteko balioak laburbiltzen dira kalkulatutako diru-sarrerak kalkulatzeko.</span><span class="sxs-lookup"><span data-stu-id="a2b16-113">If the revenue method of the Opportunity summary is set to **System Calculated**, the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
