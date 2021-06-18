---
title: Proiektuko faktura-proposamenen errendimendua
description: Gai honek proiektuaren faktura proposamenen errendimendu hobekuntzei buruzko informazioa eskaintzen du.
author: Yowelle
ms.date: 04/20/2021
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
ms.openlocfilehash: 0e7a9eedc80a88e80b7788be4fe4b2f969be8ba1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999476"
---
# <a name="project-invoice-proposal-performance"></a><span data-ttu-id="0e728-103">Proiektuko faktura-proposamenen errendimendua</span><span class="sxs-lookup"><span data-stu-id="0e728-103">Project invoice proposal performance</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="0e728-104">Faktura proposamen berri bat sortzen duzunean errendimendu arazoak sor ditzakezu proiektuen eta azpiproiektuen kopurua handitzen den neurrian.</span><span class="sxs-lookup"><span data-stu-id="0e728-104">When you create a new invoice proposal you might encounter performance issues as the number of projects and subprojects increase.</span></span> <span data-ttu-id="0e728-105">Errendimendua hobetzeko, argitaratutako proiektuen transakzioen faktura proposamen berria sortzeko behar den denbora murrizten duen eginbidea dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="0e728-105">To improve performance, a feature is available that reduces the time needed to create a new invoice proposal for posted project transactions.</span></span>

## <a name="enable-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="0e728-106">Gaitu proiektuko faktura-proposamenen errendimenduaren hobekuntza</span><span class="sxs-lookup"><span data-stu-id="0e728-106">Enable project invoice proposal performance enhancement</span></span>
<span data-ttu-id="0e728-107">Proiektuaren faktura proposamenaren errendimendua hobetzeko eginbidea gaitzeko, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="0e728-107">To enable the project invoice proposal performance enhancement feature, complete the following steps.</span></span>

1.  <span data-ttu-id="0e728-108">Joan **Ezaugarrien kudeaketa** > **Guztiak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="0e728-108">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="0e728-109">Ezaugarrien zerrendan, bilatu **Proiektuaren faktura proposamenaren errendimendua hobetzea**.</span><span class="sxs-lookup"><span data-stu-id="0e728-109">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="0e728-110">Hautatu **Gaitu orain**.</span><span class="sxs-lookup"><span data-stu-id="0e728-110">Select **Enable now**.</span></span>
3.  <span data-ttu-id="0e728-111">Freskatu arakatzailea eta sortu faktura proposamen berria.</span><span class="sxs-lookup"><span data-stu-id="0e728-111">Refresh your browser, and then create a new invoice proposal.</span></span>

## <a name="turn-off-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="0e728-112">Desaktibatu proiektuko faktura-proposamenen errendimenduaren hobekuntza</span><span class="sxs-lookup"><span data-stu-id="0e728-112">Turn off project invoice proposal performance enhancement</span></span>
<span data-ttu-id="0e728-113">Osatu urrats hauek proiektuaren faktura proposamenaren errendimendua hobetzeko eginbidea desaktibatzeko.</span><span class="sxs-lookup"><span data-stu-id="0e728-113">Complete the following steps to turn off the project invoice proposal performance enhancement.</span></span>

1.  <span data-ttu-id="0e728-114">Joan **Ezaugarrien kudeaketa** > **Guztiak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="0e728-114">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="0e728-115">Ezaugarrien zerrendan, bilatu **Proiektuaren faktura proposamenaren errendimendua hobetzea**.</span><span class="sxs-lookup"><span data-stu-id="0e728-115">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="0e728-116">Hautatu **Desgaitu**.</span><span class="sxs-lookup"><span data-stu-id="0e728-116">Select **Disable**.</span></span>
3.  <span data-ttu-id="0e728-117">Freskatu arakatzailea.</span><span class="sxs-lookup"><span data-stu-id="0e728-117">Refresh your browser.</span></span>

> [!NOTE]
> <span data-ttu-id="0e728-118">Faktura proposamenen errendimendua ezin da aplikatu fakturazio arauak gaituta daudenean edo batch prozesuak martxan daudenean.</span><span class="sxs-lookup"><span data-stu-id="0e728-118">Invoice proposal performance can't be applied when billing rules are enabled or batch processes are running.</span></span>
