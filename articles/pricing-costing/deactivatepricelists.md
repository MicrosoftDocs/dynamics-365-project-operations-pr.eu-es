---
title: Desaktibatu prezio-zerrendak
description: Gai honetan erabiltzen ez diren edo zaharrak diren prezioen zerrendak nola desaktibatu edo ezabatu azaltzen da.
author: rumant
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d5d6cf6b4b097c08edca5a3235ed1b438a0eae2d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001321"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="35841-103">Desaktibatu prezio-zerrendak</span><span class="sxs-lookup"><span data-stu-id="35841-103">Deactivate price lists</span></span> 

<span data-ttu-id="35841-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="35841-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="35841-105">Erabilitako edo erabili gabeko prezioen zerrendak kentzeko Dynamics 365 Project Operations, bi urrats bete behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="35841-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="35841-106">Kendu edo ezabatu orri zehatzetako prezioen zerrenda.</span><span class="sxs-lookup"><span data-stu-id="35841-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="35841-107">Desaktibatu edo ezabatu prezioen zerrenda Prezio aktiboen zerrendetatik **Prezio zerrendak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="35841-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="35841-108">Bi urratsak bete behar dituzu prezio zerrenda guztiz kentzeko.</span><span class="sxs-lookup"><span data-stu-id="35841-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="35841-109">Prezio zerrenda aktiboen ikuspegitik prezioen zerrenda zuzenean ezabatzea edo desaktibatzea da 2. urratsa egitea ez da nahikoa.</span><span class="sxs-lookup"><span data-stu-id="35841-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="35841-110">1. urratsean aipatutako leku guztietatik prezio zerrenda honen elkartea ere ezabatu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="35841-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="35841-111">Ezabatu orri zehatzetako prezioen zerrenda</span><span class="sxs-lookup"><span data-stu-id="35841-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="35841-112">Project Operations-etatik prezio zerrenda ezabatzeko, joan orrialde hauetara:</span><span class="sxs-lookup"><span data-stu-id="35841-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="35841-113">**Proiektuen parametroak** orria > **Prezio-zerrendak** fitxa</span><span class="sxs-lookup"><span data-stu-id="35841-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="35841-114">**Antolakuntza unitatea** orrialdea > **Prezio zerrendak** sareta</span><span class="sxs-lookup"><span data-stu-id="35841-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="35841-115">**Kontua** orria > **Proiektuen prezio-zerrendak** sareta</span><span class="sxs-lookup"><span data-stu-id="35841-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="35841-116">**Proiektuaren aurrekontuak** orrialdea > **Proiektuen prezioen zerrendak** sareta: hau proiektu aktiboen aurrekontu guztiei aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="35841-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="35841-117">**Proiektuaren kontratuak** orrialdea > **Proiektuen prezioen zerrendak** sareta: hau proiektu aktiboen kontratu guztiei aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="35841-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="35841-118">Orrialde bakoitzerako, ezabatu nahi duzun prezio zerrenda hautatu behar duzu eta, ondoren, hautatu **Ezabatu**.</span><span class="sxs-lookup"><span data-stu-id="35841-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="35841-119">Ezabatu edo desaktibatu prezioen zerrenda Prezio zerrendak orrialdetik</span><span class="sxs-lookup"><span data-stu-id="35841-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="35841-120">Prezio zerrenda aktiboen zerrendetatik ezabatzeko, joan hona: **Salmentak** > **Bezeroak** > **Prezio zerrendak**.</span><span class="sxs-lookup"><span data-stu-id="35841-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="35841-121">Hautatu ezabatu nahi duzun prezio zerrenda eta, ondoren, hautatu **Ezabatu**.</span><span class="sxs-lookup"><span data-stu-id="35841-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="35841-122">Lehendik dauden transakzioetan prezioen zerrenda aipatzen bada, ezin izango duzu ezabatu.</span><span class="sxs-lookup"><span data-stu-id="35841-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="35841-123">Hori gertatzen bada, prezioen zerrenda desaktiba dezakezu inongo ikuspegitan ager ez dadin.</span><span class="sxs-lookup"><span data-stu-id="35841-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="35841-124">Prezioen zerrenda desaktibatzeko, hautatu berriro prezioen zerrenda, eta hautatu **Desaktibatu**.</span><span class="sxs-lookup"><span data-stu-id="35841-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
