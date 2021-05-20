---
title: Proiektuko faktura-proposamenen errendimendua
description: Gai honek proiektuaren faktura proposamenen errendimendu hobekuntzei buruzko informazioa eskaintzen du.
author: Yowelle
manager: AnnBe
ms.date: 04/20/2021
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 1641d5f731029fdbdc16c4b652cc752a583058c6
ms.sourcegitcommit: 68d52fc983861114e654ffc8d2472b4db9b48981
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/20/2021
ms.locfileid: "5920287"
---
# <a name="project-invoice-proposal-performance"></a><span data-ttu-id="9e919-103">Proiektuko faktura-proposamenen errendimendua</span><span class="sxs-lookup"><span data-stu-id="9e919-103">Project invoice proposal performance</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="9e919-104">Faktura proposamen berri bat sortzen duzunean errendimendu arazoak sor ditzakezu proiektuen eta azpiproiektuen kopurua handitzen den neurrian.</span><span class="sxs-lookup"><span data-stu-id="9e919-104">When you create a new invoice proposal you might encounter performance issues as the number of projects and subprojects increase.</span></span> <span data-ttu-id="9e919-105">Errendimendua hobetzeko, argitaratutako proiektuen transakzioen faktura proposamen berria sortzeko behar den denbora murrizten duen eginbidea dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="9e919-105">To improve performance, a feature is available that reduces the time needed to create a new invoice proposal for posted project transactions.</span></span>

## <a name="enable-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="9e919-106">Gaitu proiektuko faktura-proposamenen errendimenduaren hobekuntza</span><span class="sxs-lookup"><span data-stu-id="9e919-106">Enable project invoice proposal performance enhancement</span></span>
<span data-ttu-id="9e919-107">Proiektuaren faktura proposamenaren errendimendua hobetzeko eginbidea gaitzeko, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="9e919-107">To enable the project invoice proposal performance enhancement feature, complete the following steps.</span></span>

1.  <span data-ttu-id="9e919-108">Joan **Ezaugarrien kudeaketa** > **Guztiak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="9e919-108">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="9e919-109">Ezaugarrien zerrendan, bilatu **Proiektuaren faktura proposamenaren errendimendua hobetzea**.</span><span class="sxs-lookup"><span data-stu-id="9e919-109">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="9e919-110">Hautatu **Gaitu orain**.</span><span class="sxs-lookup"><span data-stu-id="9e919-110">Select **Enable now**.</span></span>
3.  <span data-ttu-id="9e919-111">Freskatu arakatzailea eta sortu faktura proposamen berria.</span><span class="sxs-lookup"><span data-stu-id="9e919-111">Refresh your browser, and then create a new invoice proposal.</span></span>

## <a name="turn-off-project-invoice-proposal-performance-enhancement"></a><span data-ttu-id="9e919-112">Desaktibatu proiektuko faktura-proposamenen errendimenduaren hobekuntza</span><span class="sxs-lookup"><span data-stu-id="9e919-112">Turn off project invoice proposal performance enhancement</span></span>
<span data-ttu-id="9e919-113">Osatu urrats hauek proiektuaren faktura proposamenaren errendimendua hobetzeko eginbidea desaktibatzeko.</span><span class="sxs-lookup"><span data-stu-id="9e919-113">Complete the following steps to turn off the project invoice proposal performance enhancement.</span></span>

1.  <span data-ttu-id="9e919-114">Joan **Ezaugarrien kudeaketa** > **Guztiak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="9e919-114">Go to **Feature management** > **All**.</span></span> <span data-ttu-id="9e919-115">Ezaugarrien zerrendan, bilatu **Proiektuaren faktura proposamenaren errendimendua hobetzea**.</span><span class="sxs-lookup"><span data-stu-id="9e919-115">In the feature list, locate **Project invoice proposal performance enhancement**.</span></span>
2.  <span data-ttu-id="9e919-116">Hautatu **Desgaitu**.</span><span class="sxs-lookup"><span data-stu-id="9e919-116">Select **Disable**.</span></span>
3.  <span data-ttu-id="9e919-117">Freskatu arakatzailea.</span><span class="sxs-lookup"><span data-stu-id="9e919-117">Refresh your browser.</span></span>

> [!NOTE]
> <span data-ttu-id="9e919-118">Faktura proposamenen errendimendua ezin da aplikatu fakturazio arauak gaituta daudenean edo batch prozesuak martxan daudenean.</span><span class="sxs-lookup"><span data-stu-id="9e919-118">Invoice proposal performance can't be applied when billing rules are enabled or batch processes are running.</span></span>
