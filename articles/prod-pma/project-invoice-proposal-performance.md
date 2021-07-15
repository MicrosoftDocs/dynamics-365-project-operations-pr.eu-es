---
title: Proiektuko faktura-proposamenen errendimendua
description: Gai honek proiektuaren faktura proposamenen errendimendu hobekuntzei buruzko informazioa eskaintzen du.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ''
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 20121-03-05
ms.dyn365.ops.version: 10.0.18
ms.openlocfilehash: 5a14acf51d277b16896d64c4b12ee00bfb326910
ms.sourcegitcommit: 3a4b181be08ef0428104d72b54a3e61ac2782f14
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "6269775"
---
# <a name="project-invoice-proposal-performance"></a><span data-ttu-id="e14d9-103">Proiektuko faktura-proposamenen errendimendua</span><span class="sxs-lookup"><span data-stu-id="e14d9-103">Project invoice proposal performance</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e14d9-104">Faktura proposamen berri bat sortzen duzunean errendimendu arazoak sor ditzakezu proiektuen eta azpiproiektuen kopurua handitzen den neurrian.</span><span class="sxs-lookup"><span data-stu-id="e14d9-104">When you create a new invoice proposal you might encounter performance issues as the number of projects and subprojects increase.</span></span> <span data-ttu-id="e14d9-105">Errendimendua hobetzeko, argitaratutako proiektuen transakzioen faktura proposamen berria sortzeko behar den denbora murrizten duen eginbidea dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="e14d9-105">To improve performance, a feature is available that reduces the time needed to create a new invoice proposal for posted project transactions.</span></span>

## <a name="enable-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="e14d9-106">Gaitu proiektuko faktura-proposamenen errendimenduaren hobekuntza</span><span class="sxs-lookup"><span data-stu-id="e14d9-106">Enable project invoice proposal performance enhancement</span></span>
<span data-ttu-id="e14d9-107">Proiektuaren faktura proposamenaren errendimendua hobetzeko eginbidea gaitzeko, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="e14d9-107">To enable the project invoice proposal performance enhancement feature, complete the following steps.</span></span>

1.  <span data-ttu-id="e14d9-108">Joan **Ezaugarrien kudeaketa** > **Guztiak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="e14d9-108">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="e14d9-109">Ezaugarrien zerrendan, bilatu **Proiektuaren faktura proposamenaren errendimendua hobetzea**.</span><span class="sxs-lookup"><span data-stu-id="e14d9-109">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="e14d9-110">Hautatu **Gaitu orain**.</span><span class="sxs-lookup"><span data-stu-id="e14d9-110">Select **Enable now**.</span></span>
3.  <span data-ttu-id="e14d9-111">Freskatu arakatzailea eta sortu faktura proposamen berria.</span><span class="sxs-lookup"><span data-stu-id="e14d9-111">Refresh your browser, and then create a new invoice proposal.</span></span>

## <a name="turn-off-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="e14d9-112">Desaktibatu proiektuko faktura-proposamenen errendimenduaren hobekuntza</span><span class="sxs-lookup"><span data-stu-id="e14d9-112">Turn off project invoice proposal performance enhancement</span></span>
<span data-ttu-id="e14d9-113">Osatu urrats hauek proiektuaren faktura proposamenaren errendimendua hobetzeko eginbidea desaktibatzeko.</span><span class="sxs-lookup"><span data-stu-id="e14d9-113">Complete the following steps to turn off the project invoice proposal performance enhancement.</span></span>

1.  <span data-ttu-id="e14d9-114">Joan **Ezaugarrien kudeaketa** > **Guztiak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="e14d9-114">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="e14d9-115">Ezaugarrien zerrendan, bilatu **Proiektuaren faktura proposamenaren errendimendua hobetzea**.</span><span class="sxs-lookup"><span data-stu-id="e14d9-115">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="e14d9-116">Hautatu **Desgaitu**.</span><span class="sxs-lookup"><span data-stu-id="e14d9-116">Select **Disable**.</span></span>
3.  <span data-ttu-id="e14d9-117">Freskatu arakatzailea.</span><span class="sxs-lookup"><span data-stu-id="e14d9-117">Refresh your browser.</span></span>

> [!NOTE]
> <span data-ttu-id="e14d9-118">Faktura proposamenen errendimendua ezin da aplikatu fakturazio arauak gaituta daudenean.</span><span class="sxs-lookup"><span data-stu-id="e14d9-118">Invoice proposal performance can't be applied when billing rules are enabled.</span></span>
> 
> <span data-ttu-id="e14d9-119">Faktura proposamenak sortzeko sorta prozesuan zehar, azpi-zereginen kopurua zereginak gehienez banatuko dira fakturagarriak diren transakzioak dituzten kontratu kopuruaren arabera, sartu duzuna kontuan hartu gabe.</span><span class="sxs-lookup"><span data-stu-id="e14d9-119">During the batch process to create invoice proposals, the number of subtasks will split the tasks to a maximum number based on the number of contracts with invoiceable transactions, regardless of what you have entered.</span></span> <span data-ttu-id="e14d9-120">Adibidez, sartzen baduzu **3** faktura proposamenak sortan azpiatazaren kopuruari dagokionez, eta fakturagarriak diren transakzioak dituzten bi kontratu besterik ez daude, bi azpiataza bakarrik sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="e14d9-120">For example, if you enter **3** for the number of subtasks for invoice proposal creation in batch, and there are only two contracts with invoiceable transactions, only two subtasks are created.</span></span>
