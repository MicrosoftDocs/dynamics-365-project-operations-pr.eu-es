---
title: Sortu eta aplikatu saltzailearen ordainketa atxikitzeko baldintzak
description: Gai honetan saltzailearen ordainketetarako atxikipen baldintzak konfiguratzeko eta mantentzeko moduari buruzko informazioa ematen da.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 1970a24a5073de6af43db1f1c068332c9ba9c8fe
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071173"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="c8f9c-103">Sortu eta aplikatu saltzailearen ordainketa atxikitzeko baldintzak</span><span class="sxs-lookup"><span data-stu-id="c8f9c-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="c8f9c-104">Saltzaileari ordainketa atxikitzeko baldintzak konfiguratzea proiektu baterako erabilgarria da zure erakundeak saltzaile bati egindako ordainketen zati bat gorde nahi duenean.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="c8f9c-105">Adibidez, saltzaile bati ordainketa egin nahi diozunean entregatutako produktuek zure itxaropenak bete arte.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="c8f9c-106">Saltzailearen ordainketa atxikitzeko baldintzak zehaztu daitezke saltzailearen kontratua negoziatzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="c8f9c-107">Sortu saltzailearen ordainketa atxikitzeko baldintzak</span><span class="sxs-lookup"><span data-stu-id="c8f9c-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="c8f9c-108">Atxikitzeko saltzailearen ordainketaren portzentajea eta aurrez gordetako zenbatekoen zenbatekoa sartu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="c8f9c-109">Kopuruak automatikoki gordetzen dira saltzailearen fakturetan, kontratua zehaztutako amaierako egoerara iritsi arte.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="c8f9c-110">Atxikitzeko baldintzak konfiguratu ondoren, saltzaile horrentzako edozein proiektutan aplika ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="c8f9c-111">Erabili urrats hauek saltzailearen ordainketetarako atxikipen baldintzak konfiguratzeko eta mantentzeko.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="c8f9c-112">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Atxikipena** > **Saltzailearen ordainketa atxikitzeko baldintzak**.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="c8f9c-113">Aukeratu **Berria** saltzailearen atxikipen epe berria gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="c8f9c-114">**Arauaren IDa** termino berriaren balioa automatikoki sartzen da.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="c8f9c-115">Idatzi deskribapen laburra fitxategian **Deskribapena** eremuan eta **Baldintzak** FastTab-en, hautatu **Gehitu lerroa** hauetarako terminoen balioak sartzeko:</span><span class="sxs-lookup"><span data-stu-id="c8f9c-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="c8f9c-116">**Entregatutako unitateen ehunekoa** : Idatzi epea osatzearen ehunekoa.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-116">**Percentage of units delivered** : Enter a percentage of completion for the term.</span></span> <span data-ttu-id="c8f9c-117">Kopuruak automatikoki gordetzen dira saltzailearen fakturetan, proiektuaren osatze-fasea eta zehaztutako ehunekoa bera den arte.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="c8f9c-118">Adibidez, 50,00 idazten baduzu, zenbatekoak mantenduko dira proiektua ehuneko 50 arte osatu arte.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="c8f9c-119">**Atxikitzeko ehunekoa** : Sartu nahi den saltzailearen fakturaren zenbatekoaren ehunekoa.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-119">**Percentage to retain** : Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="c8f9c-120">Adibidez, 10,00 idazten baduzu, saltzailearen fakturaren zenbatekoaren ehuneko 10 mantenduko da, proiektuak atalean ezarritako amaierako ehunekoa lortu arte **Emandako eremuen ehunekoa**.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="c8f9c-121">**Askatzeko ehunekoa** : Aukeratu **Gehitu lerroa** hautatutako proiektuaren amaierarako askatu beharreko zenbatekoen ehunekoa sartzeko.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-121">**Percentage to release** : Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="c8f9c-122">Proiektua osatzeko maila desberdinetarako mugarri bat baino gehiago badituzu, idatzi saltzailearen atxikipen epe lerro bereizi atxikipen arau bakoitzerako.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="c8f9c-123">Lerro bakoitzak atxikipen portzentaje desberdina eta askapen portzentaje desberdina zehaztu dezake proiektuaren amaierako maila bakoitzerako.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="c8f9c-124">Saltzailearen atxikitzeko baldintzak sortu ondoren, saltzaile horrentzako edozein proiektutan aplika ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="c8f9c-125">Aplikatu saltzaileari atxikitzeko baldintzak proiektu bati</span><span class="sxs-lookup"><span data-stu-id="c8f9c-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="c8f9c-126">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu guztiak** eta ireki proiektu bat proiektuen zerrendatik.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="c8f9c-127">**Saltzaileen akordioak** FastTab-en, hautatu **Gehitu lerroa**.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="c8f9c-128">**Kontuaren kodeaeremuan** , hautatu aukera hauetako bat:</span><span class="sxs-lookup"><span data-stu-id="c8f9c-128">In the **Account code field** , select one of the following options:</span></span> 

   - <span data-ttu-id="c8f9c-129">**Taula** : Saltzailearen atxikitze-baldintzak saltzaile bakar bati aplikatzen zaizkio.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-129">**Table** : The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="c8f9c-130">**Taldea** : Saltzailearen atxikitze-baldintzak saltzaile talde bateko saltzaile guztiei aplikatzen zaizkie.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-130">**Group** : The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="c8f9c-131">**Guztia** : Saltzailearen atxikitze-baldintzak saltzaile guztiei aplikatzen zaizkie.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-131">**All** : The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="c8f9c-132">**Saltzailea/Saltzaile taldearen eremuan** , hautatu saltzailea edo saltzaile taldea zein saltzaileren atxikitze baldintzak aplikatzen diren.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-132">In the **Vendor/Vendor group field** , select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="c8f9c-133">Aukeratu baduzu **Guztiak** aurreko urratsean, eremu hau ez dago erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="c8f9c-134">**Saltzailearen atxikitze baldintzak** eremuan, hautatu aurreko prozeduran sortutako atxikitze terminoak.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="c8f9c-135">Proiektuak saltzailearentzako ordaindutako ordainketa (PWP) baldintzak ere baditu, sartu proiektuaren atalase portzentajea **PWP atalasearen ehunekoa** eremua.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="c8f9c-136">Saltzaileari atxikitzeko baldintzak saltzailearentzat sortzen dituzun erosketa-eskaeretan ere agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="c8f9c-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>
