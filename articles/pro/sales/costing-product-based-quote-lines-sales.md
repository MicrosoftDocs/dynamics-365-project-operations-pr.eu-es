---
title: Produktuetan oinarritutako eskaintzaren lerroen kostuak kudeatzea
description: Gai honek kostuaren prezioa produktuetan oinarritutako eskaintzaren lerroari aplikatzeari buruzko lerroei buruzko informazioa ematen du.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 17b377eab5bcbc1a2327cb3ff87cc75d8de40953
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070939"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="1cae5-103">Produktuetan oinarritutako eskaintzaren lerroen kostuak kudeatzea</span><span class="sxs-lookup"><span data-stu-id="1cae5-103">Costing product-based quote lines</span></span>

<span data-ttu-id="1cae5-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="1cae5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="1cae5-105">Dynamics 365 Project Operations produktuan oinarritutako aurrekontu lerroek ere badute **Kostuaren prezioa** zelaia.</span><span class="sxs-lookup"><span data-stu-id="1cae5-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="1cae5-106">Eremu hau aurrekontuaren lerroan produktuaren kostuaren prezioaren jarraipena egiteko eta beheranzko errentagarritasun kalkuluak egiteko erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="1cae5-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="1cae5-107">Katalogoko produktu baterako produktuan oinarritutako aurrekontu lerroa sortzen denean, produktuan oinarritutako aurrekontu lerroaren kostua lehenetsita dago **Kostu estandarra** produktuaren katalogoaren eremua.</span><span class="sxs-lookup"><span data-stu-id="1cae5-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="1cae5-108">Produktuen katalogoan kostu estandarraren eremua Erakundearen oinarrizko monetan konfiguratzen da.</span><span class="sxs-lookup"><span data-stu-id="1cae5-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="1cae5-109">Produktuan oinarritutako aurrekontu lerroaren unitateko kostu lehenetsia aurrekontuaren salmenten monetara bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="1cae5-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="1cae5-110">Produktuetan oinarritutako eskaintzaren lerroko unitate-kostua</span><span class="sxs-lookup"><span data-stu-id="1cae5-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="1cae5-111">Produktuan oinarritutako aurrekontu lerro batean kostu unitarioa edukitzearen helburua salmenta bakoitzeko produktu baten kostu desberdinak ahalbidetzea da.</span><span class="sxs-lookup"><span data-stu-id="1cae5-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="1cae5-112">Ez da ohiko eszenatokia, baina, batzuetan, produktuaren kostua hornitzaileak deskontatu dezake azken salmentaren bezeroaren arabera.</span><span class="sxs-lookup"><span data-stu-id="1cae5-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="1cae5-113">Adibidez:</span><span class="sxs-lookup"><span data-stu-id="1cae5-113">For example:</span></span>

<span data-ttu-id="1cae5-114">Fabrikam Robotics A Datum Corporation-en muntaia lerroetan beso robotikoak instalatzen ari da.</span><span class="sxs-lookup"><span data-stu-id="1cae5-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="1cae5-115">Fabrikam-ek instalazio zerbitzuak eskaintzen ditu, baina beso robotikoak Trey robotikatik eskuratzen dira.</span><span class="sxs-lookup"><span data-stu-id="1cae5-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="1cae5-116">A Datum Corporation-en beso robotikoak instalatzeak Trey-ren beso robotikoen industria bertikal berria irekitzen badu, Trey-k deskontu berezia eman diezaioke Fabrikam-i akordio horretarako.</span><span class="sxs-lookup"><span data-stu-id="1cae5-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="1cae5-117">Kasu honetan, Fabrikam-ek produktuetan oinarritutako aurrekontu lerroa sortuko du Arma Robotikoetarako eta aurrekontu honetarako unitateko kostu berezia sartuko du.</span><span class="sxs-lookup"><span data-stu-id="1cae5-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="1cae5-118">Kostu hori Trey Robotic Arms-en kostu estandarretik ezberdina da.</span><span class="sxs-lookup"><span data-stu-id="1cae5-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>
