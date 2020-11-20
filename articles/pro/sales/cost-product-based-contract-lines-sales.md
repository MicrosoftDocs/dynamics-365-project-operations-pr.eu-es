---
title: Kudeatu produktuetan oinarritutako kontratuaren lerroen kostuak - arina
description: Gai honek sortzeari buruzko informazioa ematen du
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0e961bcf32a5dd662b7cd27a23eb5f664c45c292
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177226"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="5f1c9-103">Kudeatu produktuetan oinarritutako kontratuaren lerroen kostuak - arina</span><span class="sxs-lookup"><span data-stu-id="5f1c9-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="5f1c9-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="5f1c9-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="5f1c9-105">Dynamics 365 Project Operations-eko produktuetan oinarritutako kontratu lerroen artean daude **Kostuaren prezioa** eremua, produktuaren kostu prezioa gordetzen duena beheranzko errentagarritasunaren kalkuluetarako.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="5f1c9-106">Katalogoko produktu baterako produktuan oinarritutako kontratuaren lerroa sortzen denean, produktuan oinarritutako kontratuaren lerroaren kostua lehenetsita dago **Kostu estandarra** produktuaren katalogoaren eremua.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="5f1c9-107">Produktuen katalogoan **kostu estandarra** eremua Erakundearen oinarrizko monetan konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="5f1c9-108">Kontratuaren lineako kostu unitarioa lehenetsitakoan, kontratuko salmenten moneta bihurtuko da.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="5f1c9-109">Produktuetan oinarritutako kontratuaren lerroko unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="5f1c9-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="5f1c9-110">Produktuan oinarritutako kontratuaren lerro batean kostu unitarioa edukitzearen helburua salmenta bakoitzeko produktu baten kostu desberdinak ahalbidetzea da.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="5f1c9-111">Beharrezkoak ez diren arren, hornitzaileek produktuaren kostua beheratu dezakete bezeroaren kasuan.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="5f1c9-112">Hartu kontuan egoera hau:</span><span class="sxs-lookup"><span data-stu-id="5f1c9-112">Consider the following scenario:</span></span>

<span data-ttu-id="5f1c9-113">Fabrikam Robotics Adatum Corporation-en muntaia lerroetan beso robotikoak instalatzen ari da.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="5f1c9-114">Fabrikam-ek instalazio zerbitzuak eskaintzen ditu, baina beso robotikoak Trey Research-ek eskuratzen dira.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="5f1c9-115">Adatum Corporation-en beso robotikoak instalatzeak Trey Research-en industria bertikal berria irekitzen badu, Trey-k deskontu berezia eman diezaioke Fabrikam-i akordio horretarako.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="5f1c9-116">Kasu honetan, Fabrikam-ek produktuetan oinarritutako kontratu lerro bat sortzen du Arma Robotikoetarako eta kontratu honetarako kostu unitario bat sartzen du Trey Research-eko arma robotikoen kostu estandarretik ezberdina.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
