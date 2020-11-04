---
title: Produktuetan oinarritutako kontratuaren lerroen kostuak kudeatzea
description: Gai honek sortzeari buruzko informazioa ematen du
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7dfb9425174dddee52f9ee64f7a963e48a6bca70
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/20/2020
ms.locfileid: "4071267"
---
# <a name="costing-product-based-contract-lines"></a><span data-ttu-id="0ab13-103">Produktuetan oinarritutako kontratuaren lerroen kostuak kudeatzea</span><span class="sxs-lookup"><span data-stu-id="0ab13-103">Costing product-based contract lines</span></span>

<span data-ttu-id="0ab13-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="0ab13-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="0ab13-105">Dynamics 365 Project Operations-eko produktuetan oinarritutako kontratu lerroen artean daude **Kostuaren prezioa** eremua, produktuaren kostu prezioa gordetzen duena beheranzko errentagarritasunaren kalkuluetarako.</span><span class="sxs-lookup"><span data-stu-id="0ab13-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="0ab13-106">Katalogoko produktu baterako produktuan oinarritutako kontratuaren lerroa sortzen denean, produktuan oinarritutako kontratuaren lerroaren kostua lehenetsita dago **Kostu estandarra** produktuaren katalogoaren eremua.</span><span class="sxs-lookup"><span data-stu-id="0ab13-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="0ab13-107">Produktuen katalogoan **kostu estandarra** eremua Erakundearen oinarrizko monetan konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="0ab13-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="0ab13-108">Kontratuaren lineako kostu unitarioa lehenetsitakoan, kontratuko salmenten moneta bihurtuko da.</span><span class="sxs-lookup"><span data-stu-id="0ab13-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="0ab13-109">Produktuetan oinarritutako kontratuaren lerroko unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="0ab13-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="0ab13-110">Produktuan oinarritutako kontratuaren lerro batean kostu unitarioa edukitzearen helburua salmenta bakoitzeko produktu baten kostu desberdinak ahalbidetzea da.</span><span class="sxs-lookup"><span data-stu-id="0ab13-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="0ab13-111">Beharrezkoak ez diren arren, hornitzaileek produktuaren kostua beheratu dezakete bezeroaren kasuan.</span><span class="sxs-lookup"><span data-stu-id="0ab13-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="0ab13-112">Hartu kontuan egoera hau:</span><span class="sxs-lookup"><span data-stu-id="0ab13-112">Consider the following scenario:</span></span>

<span data-ttu-id="0ab13-113">Fabrikam Robotics Adatum Corporation-en muntaia lerroetan beso robotikoak instalatzen ari da.</span><span class="sxs-lookup"><span data-stu-id="0ab13-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="0ab13-114">Fabrikam-ek instalazio zerbitzuak eskaintzen ditu, baina beso robotikoak Trey Research-ek eskuratzen dira.</span><span class="sxs-lookup"><span data-stu-id="0ab13-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="0ab13-115">Adatum Corporation-en beso robotikoak instalatzeak Trey Research-en industria bertikal berria irekitzen badu, Trey-k deskontu berezia eman diezaioke Fabrikam-i akordio horretarako.</span><span class="sxs-lookup"><span data-stu-id="0ab13-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="0ab13-116">Kasu honetan, Fabrikam-ek produktuetan oinarritutako kontratu lerro bat sortzen du Arma Robotikoetarako eta kontratu honetarako kostu unitario bat sartzen du Trey Research-eko arma robotikoen kostu estandarretik ezberdina.</span><span class="sxs-lookup"><span data-stu-id="0ab13-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
