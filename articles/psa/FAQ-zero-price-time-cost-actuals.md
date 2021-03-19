---
title: Zergatik da prezio lehenetsia zero uneko denbora kostuan?
description: Uneko denboraren kostuan prezio lehenetsia 0 izatea arazoa konpontzeko.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 65f2bc773a376800928cc3746691061d8e290f74
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285783"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a><span data-ttu-id="17686-103">Zergatik da prezio lehenetsia zero uneko denbora kostuan?</span><span class="sxs-lookup"><span data-stu-id="17686-103">Why is the price defaulting to zero on time cost actuals?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="17686-104">Hau ri buruzko FAQ aplikatzen denbora emaitzetan non transakzio heredatzen da denbora eta transakzio mota ez dago Kostua.</span><span class="sxs-lookup"><span data-stu-id="17686-104">This FAQ applies to actuals where the transaction class is set to Time and transaction type is Cost.</span></span> <span data-ttu-id="17686-105">Hurrengo egiaztapenak hiru dira lagun konpontzeko zergatik prezio denbora salmenta benetako zenbatekoak kalkulatu, 0 defaulting da.</span><span class="sxs-lookup"><span data-stu-id="17686-105">The following three checks will help you troubleshoot why the price is defaulting to 0 on time cost actuals.</span></span>
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a><span data-ttu-id="17686-106">1. egiaztatu: Identifikatu kostuaren prezio-zerrenda proiekturako</span><span class="sxs-lookup"><span data-stu-id="17686-106">Check 1: Identify the cost price list for the project</span></span>

<span data-ttu-id="17686-107">Bilaketa proiektua orrira benetako eta deskonektatu proiektua eremu proiektua.</span><span class="sxs-lookup"><span data-stu-id="17686-107">Find the project from the project field of the actual and then go to the project page.</span></span> <span data-ttu-id="17686-108">Sakatu eremuan unitate esteka contracting.</span><span class="sxs-lookup"><span data-stu-id="17686-108">Click on the contracting unit link in the field.</span></span> <span data-ttu-id="17686-109">Unitate Contracting orrian, egiaztatu contracting unitate duela prezio-zerrenda bat Kostua Prezio-Zerrendak saretan.</span><span class="sxs-lookup"><span data-stu-id="17686-109">On the Contracting Unit page, check if the contracting unit has a price list in the Cost Price Lists grid.</span></span>

<span data-ttu-id="17686-110">Prezio-zerrenda bat baino gehiago badago, arazoa isolated izan.</span><span class="sxs-lookup"><span data-stu-id="17686-110">If there is more than one price list, you have isolated the problem.</span></span> <span data-ttu-id="17686-111">Project Service bakarrik onartzen prezio-zerrenda bat bakoitzeko antolakuntza unitatea.</span><span class="sxs-lookup"><span data-stu-id="17686-111">Project Service only supports one price list per organizational unit.</span></span> <span data-ttu-id="17686-112">Kendu prezio-zerrendak entitate honen prezio-zerrenda bakarra Antolakuntza Unitatea-Kostua Prezio-Zerrendak azpisaretan erantsita arte.</span><span class="sxs-lookup"><span data-stu-id="17686-112">Remove all prices lists from this entity until there is only one price list attached in the Cost Price Lists grid of the Organizational Unit.</span></span>

<span data-ttu-id="17686-113">Erantsitako Antolakuntza Unitatea ez dago prezio-zerrendak badira, egin Antolakuntza unitatea moneta-oharra.</span><span class="sxs-lookup"><span data-stu-id="17686-113">If there are no price lists attached to the Organizational Unit, make a note of the currency of the Organizational unit.</span></span> <span data-ttu-id="17686-114">Joan Project Service-ra eta, ondoren, Parametroak eta Prezio-Zerrendak fitxa Kontrol prezio-zerrendak edozein Kostua eta Antolakuntza Unitatea moneta bat datorren moneta-testuinguru badaude, ireki.</span><span class="sxs-lookup"><span data-stu-id="17686-114">Go to the Project Service and then Parameters and open the Price Lists tab. Check if there are any price lists with context set to Cost and currency that matches the currency of the Organizational Unit.</span></span>
 
<span data-ttu-id="17686-115">Horren irizpideekin bat datozen prezio-zerrendak ez badira, arazoak isolated izan.</span><span class="sxs-lookup"><span data-stu-id="17686-115">If there are no price lists that match that criteria, you have isolated the problem.</span></span> <span data-ttu-id="17686-116">Ziurtatu gutxienez prezio-zerrendaren Kostua ezarrita testuinguru kontrolatzen dute eta moneta kontrolatzen Antolakuntza Unitatea moneta bat.</span><span class="sxs-lookup"><span data-stu-id="17686-116">Make sure to have at least one price list whose context is set to Cost and whose currency matches the currency of the Organizational Unit.</span></span>

<span data-ttu-id="17686-117">Horren irizpideekin bat datozen prezio-zerrenda bat baino gehiago badago, jarraitu irakurketa-dokumentuaren egiaztapenak gehiago egiteko.</span><span class="sxs-lookup"><span data-stu-id="17686-117">If there is more than one price list that match that criteria, continue reading this document to make more checks.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a><span data-ttu-id="17686-118">2. egiaztatu: bada beste prezio-zerrendarik identifikatuta zehaztutako datu benetako denbora-kostuan?</span><span class="sxs-lookup"><span data-stu-id="17686-118">Check 2: Are any of the price lists identified above valid for the specific date of the time cost actual?</span></span>

<span data-ttu-id="17686-119">Project Service hartu prezio defaulting prezio-zerrenda bat, prezio-zerrenda horren behar da aplikagarria salmentak denbora-kostua benetako data.</span><span class="sxs-lookup"><span data-stu-id="17686-119">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the time cost actual.</span></span> <span data-ttu-id="17686-120">Egiaztatu hauek ikus gaineko identifikatutako prezio-zerrendak aplikagarria dira:</span><span class="sxs-lookup"><span data-stu-id="17686-120">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="17686-121">Egiaztatu hasiera- eta amaiera-datak orokorra fitxan erantsita prezio-zerrendak hutsik ez.</span><span class="sxs-lookup"><span data-stu-id="17686-121">Check if the start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="17686-122">Hasiera eta amaiera-datak prezioa zerrendak gaineko identifikatu dira hutsik, arazoa isolated izan.</span><span class="sxs-lookup"><span data-stu-id="17686-122">If the start and end dates on price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="17686-123">Egin ohar bat denbora-kostuaren hasiera-data eremua benetako eta egiaztatu identifikatutako prezio-zerrendak-da aplikagarria data.</span><span class="sxs-lookup"><span data-stu-id="17686-123">Make a note of the start date field on your time cost actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="17686-124">Adibidez, benetako denbora-kostuaren data behar daude hasiera-data eta amaiera-data ere prezio-zerrendan.</span><span class="sxs-lookup"><span data-stu-id="17686-124">For example, the date of the time cost actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="17686-125">Horri buruzko eremu zehatzera salmentak denbora-kostuaren benetako data horren prezio-zerrendarik ez badago, arazoa isolated izan.</span><span class="sxs-lookup"><span data-stu-id="17686-125">If there is no price list that covers that date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="17686-126">Aldatu, hasiera- eta amaiera-datak prezio-zerrenda, prezio-zerrenda benetako denbora-kostuaren data estaltzen dela ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="17686-126">Modify the start and end dates of the price list to ensure that the price list covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="17686-127">Benetako denbora-kostuko data estaltzen duen prezio-zerrenda bat baino gehiago badaude, arazo bakan bat duzu.</span><span class="sxs-lookup"><span data-stu-id="17686-127">If there is more than one price list that covers the date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="17686-128">Konpondu arazoa editatu hasiera- eta amaiera-datetan prezio-zerrendak-horri buruzko eremu zehatzera benetako denbora-kostuaren prezio-zerrenda bakarra dago daitezen.</span><span class="sxs-lookup"><span data-stu-id="17686-128">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="17686-129">Horri buruzko eremu zehatzera kostuaren ordua benetako data prezio-zerrenda bat badago, mugitu begiratu hurrengo dokumentua.</span><span class="sxs-lookup"><span data-stu-id="17686-129">If there is only one price list that covers that date of the time cost actual, move to the next check in the document.</span></span>
<span data-ttu-id="17686-130">Beharrezko konponketez egin ditzakezu, baina denbora-sarrera sortu berriro, onartu da eta egiaztatu fakturatu gabeko denbora-kostuaren prezio baliogabea.</span><span class="sxs-lookup"><span data-stu-id="17686-130">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a><span data-ttu-id="17686-131">3. egiaztatu: Badago prezio bat prezio-zerrendaren, prezioen neurriak dira ordua kostuaren benetako?</span><span class="sxs-lookup"><span data-stu-id="17686-131">Check 3: Is there a price in the price list for the pricing dimensions on the time cost actual?</span></span>

<span data-ttu-id="17686-132">Behar bezala osatu Egiaztatu 1 eta 2 Egiaztatu, baduzu orain koadrorako proiektua prezio-zerrenda bakarra denbora-kostua benetako data honetan aplikagarria den.</span><span class="sxs-lookup"><span data-stu-id="17686-132">If you have successfully completed Check 1 and Check 2, you should now have only one price list that is applicable for the date of the time cost actual.</span></span> <span data-ttu-id="17686-133">Ireki Prezio-zerrenda eta joan Funtzio-prezioak fitxara. Ziurtatu errenkada bat dagoela prezio-dimentsioaren saretan benetako denbora-kostuan.</span><span class="sxs-lookup"><span data-stu-id="17686-133">Open this Price List and go to the Role Prices tab. Make sure that there is a row in the grid for the pricing dimensions on the time cost actual.</span></span>

<span data-ttu-id="17686-134">Badago errenkada ez dago prezio-prezioen neurriak dira ordua kostuaren-saretan funtzioa benetako, ondoren, duzu izan isolated arazoa.</span><span class="sxs-lookup"><span data-stu-id="17686-134">If there is no row in the role price grid for the pricing dimensions on the time cost actual, then you have isolated the problem.</span></span> <span data-ttu-id="17686-135">Sortu errenkada bat Funtzioa prezioak saretan, prezioen neurriak dira ordua zure kostuaren-benetako.</span><span class="sxs-lookup"><span data-stu-id="17686-135">Create a row in the Role prices grid for the pricing dimensions on your time cost actual.</span></span> <span data-ttu-id="17686-136">Amaieran, beharrezko konponketez egin ditzakezu, baina denbora-sarrera sortu berriro, onartu da eta egiaztatu balio-kostua fakturatu gabeko prezio baliogabea.</span><span class="sxs-lookup"><span data-stu-id="17686-136">Once this is done, recreate time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>
 
<span data-ttu-id="17686-137">Oraindik ikusten ez baduzu baliozko denbora-kostua benetako atalean egiten egiaztapenak hiru goiko ondoren, itxaron saioa laguntza tiketa, gertaera bat.</span><span class="sxs-lookup"><span data-stu-id="17686-137">If you still don't see a valid price on your time cost actual after you’ve done the three checks above, please log a support ticket.</span></span>





[!INCLUDE[footer-include](../includes/footer-banner.md)]