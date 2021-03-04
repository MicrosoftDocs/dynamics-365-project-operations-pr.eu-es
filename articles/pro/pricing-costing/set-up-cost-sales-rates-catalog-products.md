---
title: Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak - arina
description: Gai honek produktuen katalogoan dauden elementuen kostua eta salmenta tasak konfiguratzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5e851193df8151821e112e01a9f33df5afee7df7
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764534"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="9fc2f-103">Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak - arina</span><span class="sxs-lookup"><span data-stu-id="9fc2f-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="9fc2f-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="9fc2f-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="9fc2f-105">Produktuen katalogoko elementuen prezioak ezartzea Dynamics 365 Project Operations Dynamics 365 Sales-en bezalakoa da.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="9fc2f-106">Project Operations-en, produktuak ezin dira kalkulatu edo proiektuetan erabili, beraz, produktuen katalogoaren prezioak ez dira zehaztu behar proiektuen prezioen zerrendetan aurrekontuetan eta kontratuetan.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="9fc2f-107">Erabili **Produktuaren prezioa** aurrekontu, kontratu edo kontu baten eremua produktuen katalogoaren prezioak ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="9fc2f-108">Ez ezarri produktuen katalogoaren prezioak proiektuaren prezioen zerrendetan.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="9fc2f-109">Project Operations-en zerrendak proiektuaren eragiketetarako soilik dira.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="9fc2f-110">Aplikazio espezifikoen negozio logikak prezio zerrendak aurrekontu batetik kontratu batera kopiatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="9fc2f-111">Emaitza kontratuaren araberako proiektuaren prezio-zerrenda da.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="9fc2f-112">Kopiatze eragiketak aurrekontua irabazteko prozesua atzeratu dezake aurrekontuaren proiektuaren prezio zerrenda handiegia bada.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="9fc2f-113">Produktuen prezioen zerrendak ez dira kopiatzen kontratuetako prezioen zerrenda pertsonalizatuak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="9fc2f-114">Kopiatzerik ez dagoenez, aurrekontuaren prozesuaren errendimenduak ez du eraginik.</span><span class="sxs-lookup"><span data-stu-id="9fc2f-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>
