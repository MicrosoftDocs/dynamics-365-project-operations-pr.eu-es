---
title: Produktuetan oinarritutako eskaintzaren lerroen kostuak kudeatzea
description: Gai honek kostuaren prezioa produktuetan oinarritutako eskaintzaren lerroari aplikatzeari buruzko lerroei buruzko informazioa ematen du.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1fa7896e249abfefd3e93cba4bad789e67e14f31
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003436"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="b20aa-103">Produktuetan oinarritutako eskaintzaren lerroen kostuak kudeatzea</span><span class="sxs-lookup"><span data-stu-id="b20aa-103">Costing product-based quote lines</span></span>

<span data-ttu-id="b20aa-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="b20aa-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="b20aa-105">Produktuan oinarritutako aurrekontu lerroak Dynamics 365 Project Operations-en ere **Kostuaren prezioa** eremua dute.</span><span class="sxs-lookup"><span data-stu-id="b20aa-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="b20aa-106">Eremu hau aurrekontuaren lerroan produktuaren kostuaren prezioaren jarraipena egiteko eta beheranzko errentagarritasun kalkuluak egiteko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="b20aa-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="b20aa-107">Katalogoko produktu baterako produktuan oinarritutako aurrekontu lerroa sortzen denean, produktuan oinarritutako aurrekontu lerroaren kostua lehenetsita dago **Kostu estandarra** produktuaren katalogoaren eremua.</span><span class="sxs-lookup"><span data-stu-id="b20aa-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="b20aa-108">Produktuen katalogoan kostu estandarraren eremua Erakundearen oinarrizko monetan konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="b20aa-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="b20aa-109">Produktuan oinarritutako aurrekontu lerroaren unitateko kostu lehenetsia aurrekontuaren salmenten monetara bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="b20aa-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="b20aa-110">Produktuetan oinarritutako eskaintzaren lerroko unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="b20aa-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="b20aa-111">Produktuan oinarritutako aurrekontu lerro batean kostu unitarioa edukitzearen helburua salmenta bakoitzeko produktu baten kostu desberdinak ahalbidetzea da.</span><span class="sxs-lookup"><span data-stu-id="b20aa-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="b20aa-112">Ez da ohiko eszenatokia, baina, batzuetan, produktuaren kostua hornitzaileak deskontatu dezake azken salmentaren bezeroaren arabera.</span><span class="sxs-lookup"><span data-stu-id="b20aa-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="b20aa-113">Adibidez:</span><span class="sxs-lookup"><span data-stu-id="b20aa-113">For example:</span></span>

<span data-ttu-id="b20aa-114">Fabrikam Robotics A Datum Corporation-en muntaia lerroetan beso robotikoak instalatzen ari da.</span><span class="sxs-lookup"><span data-stu-id="b20aa-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="b20aa-115">Fabrikam-ek instalazio zerbitzuak eskaintzen ditu, baina beso robotikoak Trey robotikatik eskuratzen dira.</span><span class="sxs-lookup"><span data-stu-id="b20aa-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="b20aa-116">A Datum Corporation-en beso robotikoak instalatzeak Trey-ren beso robotikoen industria bertikal berria irekitzen badu, Trey-k deskontu berezia eman diezaioke Fabrikam-i akordio horretarako.</span><span class="sxs-lookup"><span data-stu-id="b20aa-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="b20aa-117">Kasu honetan, Fabrikam-ek produktuetan oinarritutako aurrekontu lerroa sortuko du Arma Robotikoetarako eta aurrekontu honetarako unitateko kostu berezia sartuko du.</span><span class="sxs-lookup"><span data-stu-id="b20aa-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="b20aa-118">Kostu hori Trey Robotic Arms-en kostu estandarretik ezberdina da.</span><span class="sxs-lookup"><span data-stu-id="b20aa-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]