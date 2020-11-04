---
title: Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak
description: Gai honek produktuen katalogoan dauden elementuen kostua eta salmenta tasak konfiguratzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5178a9143536bf4b2573403125325017861cdd5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071103"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products"></a><span data-ttu-id="85364-103">Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak</span><span class="sxs-lookup"><span data-stu-id="85364-103">Set up cost and sales rates for catalog products</span></span>

<span data-ttu-id="85364-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="85364-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="85364-105">Produktuen katalogoko elementuen prezioak konfiguratzea Dynamics 365 Project Operations-en Dynamics 365 Sales-en bezalakoa da.</span><span class="sxs-lookup"><span data-stu-id="85364-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="85364-106">Produktuak Project Operations-en proiektuetan ezin direnez kalkulatu edo erabili, ez da beharrezkoa produktuen katalogoaren prezioak finkatzea proiektuen prezioen zerrendetan aurrekontu eta kontratuetarako.</span><span class="sxs-lookup"><span data-stu-id="85364-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="85364-107">Produktuen katalogoaren prezioak atalean ezarri behar dira **Produktuaren prezioa** aurrekontu, kontratu edo kontu baten eremua.</span><span class="sxs-lookup"><span data-stu-id="85364-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="85364-108">Ez ezarri produktu horien katalogoaren prezioak proiektu horietako entitateen prezioen zerrendetan.</span><span class="sxs-lookup"><span data-stu-id="85364-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="85364-109">Project Operations-en zerrendak proiektuaren eragiketetarako soilik dira.</span><span class="sxs-lookup"><span data-stu-id="85364-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="85364-110">Aplikazio espezifikoen negozio logika dago, prezioen zerrendak aurrekontu batetik kontratu batera kopiatzen dituena.</span><span class="sxs-lookup"><span data-stu-id="85364-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="85364-111">Emaitza kontratuaren araberako proiektuaren prezio-zerrenda da.</span><span class="sxs-lookup"><span data-stu-id="85364-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="85364-112">Kopiatze eragiketak aurrekontua irabazteko prozesua atzeratu dezake aurrekontuaren proiektuaren prezio zerrenda handiegia bada.</span><span class="sxs-lookup"><span data-stu-id="85364-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="85364-113">Produktuen prezioen zerrendak ez dira kopiatzen kontratuetako prezioen zerrenda pertsonalizatuak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="85364-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="85364-114">Horrek esan nahi du produktuen prezioen zerrendek ez dutela aurrekontua irabazteko prozesuaren errendimenduan eraginik.</span><span class="sxs-lookup"><span data-stu-id="85364-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
