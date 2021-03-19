---
title: Kudeatu produktuetan oinarritutako kontratuaren lerroen unitate konplexuak - arina
description: Gai honek harpidetzan oinarritutako produktuen salmentari laguntzeko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 029d2aa4fd20fc036a34ae6136fe12454f3b7703
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273318"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a><span data-ttu-id="655fe-103">Kudeatu produktuetan oinarritutako kontratuaren lerroen unitate konplexuak - arina</span><span class="sxs-lookup"><span data-stu-id="655fe-103">Manage complex units for product-based contract lines - lite</span></span>

<span data-ttu-id="655fe-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="655fe-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="655fe-105">Dynamics 365 Project Operations-ek kantitate faktoreak erabiltzen ditu harpidedun oinarritutako produktuen salmenta sustatzeko.</span><span class="sxs-lookup"><span data-stu-id="655fe-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="655fe-106">Harpidetzetan oinarritutako produktuetarako, kontratuan edo proiektuaren kontratuaren lerroan erabiltzaile-hilabete kopurua adierazten da.</span><span class="sxs-lookup"><span data-stu-id="655fe-106">For subscription-based products, the quantity on the contract or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="655fe-107">Harpidedun softwarearen prezioa katalogoan gordetzen da erabiltzaile bakoitzeko prezio gisa.</span><span class="sxs-lookup"><span data-stu-id="655fe-107">The price of subscription software is stored in the catalog as the price per-user, per-month.</span></span> <span data-ttu-id="655fe-108">Salmenta prozesuan, kontratuaren lerroko prezioa erabiltzaile bakoitzeko, salmentako agentearen bidez negoziatu eta deskontatu zen hileko prezioa izan ohi da.</span><span class="sxs-lookup"><span data-stu-id="655fe-108">During the sales process, the price on the contract line is usually the per-user, per-month price that was negotiated and discounted by the sales agent.</span></span> <span data-ttu-id="655fe-109">Akordio bakoitzak erabiltzaile kopurua eta harpidetza hilabete desberdinak ditu.</span><span class="sxs-lookup"><span data-stu-id="655fe-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="655fe-110">Kontratuaren lerroaren zenbatekoa kalkulatzeko erabiltzen den kantitatea erabiltzaile kopurua eta harpidetza hilabeteen produktua da.</span><span class="sxs-lookup"><span data-stu-id="655fe-110">The quantity used to calculate the amount of the contract line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="655fe-111">Salmenta mota hori onartzeko, Project Operations laguntzak *kantitate faktoreen* kontzeptua sartu zuen.</span><span class="sxs-lookup"><span data-stu-id="655fe-111">To support this type of sale, Project Operations supports the concept of *quantity factors*.</span></span> <span data-ttu-id="655fe-112">Kopuru-faktoreek produktuaren atributuetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="655fe-112">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="655fe-113">Produktu baterako propietate espezifikoak konfiguratzen dituzunean, propietate horien edo propietate guztien azpimultzoa uzten dizu kantitate faktore gisa.</span><span class="sxs-lookup"><span data-stu-id="655fe-113">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="655fe-114">Project Operations-ek balioztatzen du zenbakizko datu mota bat duten zenbakizko propietateak edo produktuaren propietateak kantitate faktore gisa markatzen direla.</span><span class="sxs-lookup"><span data-stu-id="655fe-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="655fe-115">Konfiguratutako kantitate faktoreak dituen produktu bat kontratu lerro bati gehitzen zaionean, **Kopurua** eremua irakurtzeko soilik bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="655fe-115">When a product with configured quantity factors is added to a contract line, the **Quantity** field  becomes read-only.</span></span> <span data-ttu-id="655fe-116">Kantitate faktoreak diren produktuaren propietateen balioak sartu ondoren, Project Operations-ek kontratuaren lerroaren kantitatea kalkulatzen du.</span><span class="sxs-lookup"><span data-stu-id="655fe-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the contract line.</span></span>

<span data-ttu-id="655fe-117">Adibidez, Dynamics 365 Sales-ek propietate hauek izan ditzake:</span><span class="sxs-lookup"><span data-stu-id="655fe-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="655fe-118">**Erabiltzaile kop**: erabiltzaile kopurua.</span><span class="sxs-lookup"><span data-stu-id="655fe-118">**No of users**: The number of users.</span></span>
- <span data-ttu-id="655fe-119">**Hilabete kop**: harpidetza-hilabete kopurua.</span><span class="sxs-lookup"><span data-stu-id="655fe-119">**No of Months**: The number of subscription months.</span></span>
- <span data-ttu-id="655fe-120">**Produktuaren SKUa** : Produktuaren stock unitatea (SKU).</span><span class="sxs-lookup"><span data-stu-id="655fe-120">**Product SKU**: The stock keeping unit (SKU) for the product.</span></span>

<span data-ttu-id="655fe-121">**Erabiltzaile kop** eta **Hilabete kop** propietateak kantitate faktore gisa markatu daitezke produktuaren lerroko propietateak editatzean.</span><span class="sxs-lookup"><span data-stu-id="655fe-121">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="655fe-122">Produktuaren propietateetatik kantitate faktoreak sortzeko, jarraitu urrats hauek.</span><span class="sxs-lookup"><span data-stu-id="655fe-122">To create quantity factors from product properties, complete the following steps.</span></span>

1. <span data-ttu-id="655fe-123">**Project Operations** aukeran, hautatu **Salmenta-produktuak**.</span><span class="sxs-lookup"><span data-stu-id="655fe-123">On the **Project Operations**, select **Sales-Products**.</span></span>
2. <span data-ttu-id="655fe-124">Ireki kantitate faktoreak ezarri behar dituzun produktua.</span><span class="sxs-lookup"><span data-stu-id="655fe-124">Open the product for which you need to set up quantity factors.</span></span> <span data-ttu-id="655fe-125">Ziurtatu produktuak dagoeneko konfiguratutako propietateak dituela.</span><span class="sxs-lookup"><span data-stu-id="655fe-125">Make sure that the product has properties already set up.</span></span>
3. <span data-ttu-id="655fe-126">**Proiektuaren informazioa** orrian, hautatu **Zenbatekoaren faktoreak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="655fe-126">On the **Project Information** page, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="655fe-127">Azpisaretan, hautatu **+ Eremu berriaren konputazioa**.</span><span class="sxs-lookup"><span data-stu-id="655fe-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="655fe-128">Idatzi **Kopuru faktorea** eremuaren izena eta hautatu eremuaren kalkuluarekin mapatzen den propietate balioa.</span><span class="sxs-lookup"><span data-stu-id="655fe-128">Enter the name of the **Quantity Factor** and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="655fe-129">Gorde eta itxi inprimakia.</span><span class="sxs-lookup"><span data-stu-id="655fe-129">Save and close the form.</span></span>
7. <span data-ttu-id="655fe-130">Errepikatu 2-6 urratsak batera produktuan oinarritutako kontratu linearen kopurua osatuko duten propietate guztientzat.</span><span class="sxs-lookup"><span data-stu-id="655fe-130">Repeat steps 2-6 for all the properties that together will make up the quantity for the product-based contract line.</span></span>

<span data-ttu-id="655fe-131">Kopuru faktoreak konfiguratuta, erabiltzaileak produktu honetarako kontratu lerro bat sortzen duenean, kontratu lerroaren kopurua blokeatuta dago.</span><span class="sxs-lookup"><span data-stu-id="655fe-131">With quantity factors set up, when the user creates a contract line for this product, the quantity of the contract line is locked.</span></span> <span data-ttu-id="655fe-132">Kopurua kontratu lerro horretako jabetza balioen produktu gisa kalkulatzen da.</span><span class="sxs-lookup"><span data-stu-id="655fe-132">The quantity is then calculated as a product of the property values for that contract line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]