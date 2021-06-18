---
title: Unitateak eta salmenta-unitateak
description: Gai honek Dynamics 365 Project Operations-en unitateak eta salmenta-taldeak nola sortu jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 646e20189efb4aab56972f01a52b1bff19f2e79f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996056"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="789cd-103">Unitateak eta salmenta-unitateak</span><span class="sxs-lookup"><span data-stu-id="789cd-103">Units and unit groups</span></span>

<span data-ttu-id="789cd-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="789cd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="789cd-105">Unitateak produktuak edo zerbitzuak saltzen dituzun kantitateak edo neurketak dira.</span><span class="sxs-lookup"><span data-stu-id="789cd-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="789cd-106">Adibidez, lorategirako hornigaiak saltzen badituzu, baliteke haziak paketetan, kaxetan eta paletetan saltzea.</span><span class="sxs-lookup"><span data-stu-id="789cd-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="789cd-107">Salmenta-unitateko unitate beste horietako da.</span><span class="sxs-lookup"><span data-stu-id="789cd-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="789cd-108">Gai honetako urratsak osatzeko, ziurtatu Sistema administratzailea edo Sales Professional Manager kudeatzailea esleitu zaizula edo baimen baliokideak dituzula.</span><span class="sxs-lookup"><span data-stu-id="789cd-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="789cd-109">Salmenta-unitateak sortu</span><span class="sxs-lookup"><span data-stu-id="789cd-109">Create a unit group</span></span>

1. <span data-ttu-id="789cd-110">Gunearen mapan, hautatu **Unitateak**.</span><span class="sxs-lookup"><span data-stu-id="789cd-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="789cd-111">Aukeratu **Berria**, eta **Sortu Unitate Taldea** elkarrizketa-koadroa, idatzi unitatearen izena.</span><span class="sxs-lookup"><span data-stu-id="789cd-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="789cd-112">**Unitate nagusia** eremuan, idatzi produktua salduko den neurri-unitate txikiena.</span><span class="sxs-lookup"><span data-stu-id="789cd-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="789cd-113">Adibidez, "pieza" edo "ontza" sar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="789cd-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="789cd-114">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="789cd-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="789cd-115">Gehitu unitateak unitate-taldean</span><span class="sxs-lookup"><span data-stu-id="789cd-115">Add units to a unit group</span></span>

1. <span data-ttu-id="789cd-116">Ireki unitate talde bat eta **Erlazionatua** fitxa, hautatu **Unitateak**.</span><span class="sxs-lookup"><span data-stu-id="789cd-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="789cd-117">Ikusiko duzu unitate nagusi dagoeneko gehitzen da.</span><span class="sxs-lookup"><span data-stu-id="789cd-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="789cd-118">Aukeratu **Gehitu unitate berria**, eta **Sorrera azkarra: Unitatea** orrialdean, **Izena** eremuan, sartu unitatearen izena.</span><span class="sxs-lookup"><span data-stu-id="789cd-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="789cd-119">**Kopurua** eremuan, sartu unitateak izango duen kantitatea.</span><span class="sxs-lookup"><span data-stu-id="789cd-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="789cd-120">Adibidez, kutxa batek bi pieza baditu, idatzi "2".</span><span class="sxs-lookup"><span data-stu-id="789cd-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="789cd-121">**Oinarrizko unitatea** eremuan, hautatu oinarrizko unitate bat unitatearen neurketa-unitate baxuena ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="789cd-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="789cd-122">Adibidez, "Pieza" hautatu dezakezu.</span><span class="sxs-lookup"><span data-stu-id="789cd-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="789cd-123">Sakatu **Gorde**:</span><span class="sxs-lookup"><span data-stu-id="789cd-123">Select **Save**:</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]