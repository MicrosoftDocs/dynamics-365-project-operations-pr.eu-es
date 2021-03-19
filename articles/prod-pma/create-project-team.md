---
title: Sortu proiektuaren taldea
description: Gai honek proiektu-taldeak sortzeari eta kudeatzeari buruzko informazioa ematen du.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kdwns
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 121a007d91c2da4f3b9951901781757b8bcca8fe
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270843"
---
# <a name="create-a-project-team"></a><span data-ttu-id="cf1fa-103">Sortu proiektuaren taldea</span><span class="sxs-lookup"><span data-stu-id="cf1fa-103">Create a project team</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="cf1fa-104">Aurretik proiektu batean konfiguratutako eginkizunak erabiltzeko, proiektuaren kudeatzaileak eginkizunak proiektuarekin lotu behar ditu.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-104">To use the roles that were previously set up in a project, a project manager must associate the roles with the project.</span></span> <span data-ttu-id="cf1fa-105">Hainbat eginkizun esleitu daitezke proiektu baterako.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-105">Multiple roles can be assigned for a project.</span></span> <span data-ttu-id="cf1fa-106">Nahasmena ekiditeko, funtzio hauek automatikoki etiketatzen dira erreserbatu bitartean.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-106">To prevent confusion, these roles are automatically labeled during reservation.</span></span> <span data-ttu-id="cf1fa-107">Adibidez, proiektuaren zuzendariak hiru software ingeniari behar baditu, hiru Software ingeniari funtzio betetzen dituzte **software ingeniaria 1**, **software ingeniaria 2**, eta **software ingeniaria 3** haien etiketak automatikoki sortzen baitira.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-107">For example, if the project manager requires three software engineers, three Software engineer roles that have **software engineer 1**, **software engineer 2**, and **software engineer 3** as their labels are automatically generated.</span></span> <span data-ttu-id="cf1fa-108">Aurretik rolaren ezaugarriak rolerako ezarri badira, iragazki gisa aplikatuko dira baliabide bat bilatzerakoan.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-108">If role characteristics were previously set for the role, they are applied as a filter during searches for a resource.</span></span> <span data-ttu-id="cf1fa-109">Ezaugarri osagarriak gehi daitezke, bilaketa gehiago zehazteko beharrezkoak diren moduan.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-109">Additional characteristics can be added as required to further refine the search.</span></span>

<span data-ttu-id="cf1fa-110">Ikuspegi ezarpenak pertsonaliza daitezke, baliabideen erabilgarritasuna hobeto ikusteko.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-110">View settings can also be customized to give a better view of resource availability.</span></span> <span data-ttu-id="cf1fa-111">Ordubeteko, eguneroko, asteko, hileko, hiruhileko eta urteko erabilgarritasuna erakusteko aukerak daude.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-111">There are options to show hourly, daily, weekly, monthly, quarterly, and annual availability.</span></span> <span data-ttu-id="cf1fa-112">Baliabideetan eskuragarri eta geratzen den gaitasuna erakusteko aukera ere badago.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-112">There is also an option to show available and remaining capacity on resources.</span></span> <span data-ttu-id="cf1fa-113">Aukera hau erabilgarria da denbora kudeatzeko, jardueretarako edo baliabideen erabilgarritasunerako denbora librea kalkulatzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-113">This option is useful for time management, when you're estimating available time for activities or resource availability.</span></span>

<span data-ttu-id="cf1fa-114">Proiektuaren kudeatzaileak orrialdeko rol bat hauta dezake eta, gero, eskakizunera egokitzen den baliabide erabilgarri bat badago, hautatu papera betetzeko baliabide bat gordetzea.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-114">The project manager can select a role on the page and then, if there is an available resource that fits the requirement, select to reserve a resource to fill the role.</span></span> <span data-ttu-id="cf1fa-115">Kontuan izan baliabideak ez direla zertan erreserbatu plangintza faseko une honetan.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-115">Note that the resources don't have to be reserved at this point in the planning stage.</span></span> <span data-ttu-id="cf1fa-116">WBS bat sortzen duzunean, eginkizunak proiektuko langileekin ordezkatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-116">When you create a WBS, you can replace roles with staffed resources for the project.</span></span> <span data-ttu-id="cf1fa-117">Rolak WBSn langileekin hornitutako baliabideekin ordezkatzen badira, baliabideen konfigurazioak proiektuaren taldeen zerrenda eta programazioa automatikoki eguneratuko ditu.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-117">If roles are replaced with staffed resources in the WBS, the resource setup automatically updates the project team listing and scheduling.</span></span>

<span data-ttu-id="cf1fa-118">[![Eginkizunak eta benetako baliabideak biltzen dituen proiektu taldeen zerrenda](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span><span class="sxs-lookup"><span data-stu-id="cf1fa-118">[![Project team listing that includes both roles and actual resources](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span></span> 

<span data-ttu-id="cf1fa-119">Proiektuaren kudeatzaileak proiektu baterako baliabide bat erreserbatzeko hainbat aukera ditu, adibidez **Gainerako gaitasuna**, **Edukiera osoa**, **Edukiera ehunekoa**, eta **Zehaztu orduak**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-119">The project manager has various options for booking a resource for a project, such as **Remaining capacity**, **Full capacity**, **Capacity percentage**, and **Specify hours**.</span></span> <span data-ttu-id="cf1fa-120">Erreserba aukera hauek edozein unetan bertan behera utzi daitezke baliabideen esleipenak aldatzen badira.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-120">These booking options can be canceled at any time if resource assignments change.</span></span> <span data-ttu-id="cf1fa-121">Bi erreserba mota onartzen dira:</span><span class="sxs-lookup"><span data-stu-id="cf1fa-121">Two types of booking are supported:</span></span>

- <span data-ttu-id="cf1fa-122">**Liburu gogorra** - Baliabideen erreserba onartu eta baieztatu zen konpromisoan zehaztutako iraupenean lan egiteko.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-122">**Hard Book** – The resource reservation was approved and confirmed to work on the engagement for the specified duration.</span></span>
- <span data-ttu-id="cf1fa-123">**Behin behineko erreserba** - Baliabideen erreserbak behin-behinean zen konpromisoan zehaztutako iraupenean lan egiteko.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-123">**Soft book** – The resource reservations was tentatively set to work on the engagement for the specified duration.</span></span>

<span data-ttu-id="cf1fa-124">Prozedura honetan azaltzen nola proiektuaren taldea sortu:</span><span class="sxs-lookup"><span data-stu-id="cf1fa-124">The following procedure explains how to create a project team.</span></span>

## <a name="create-a-project-team"></a><span data-ttu-id="cf1fa-125">Sortu proiektuaren taldea</span><span class="sxs-lookup"><span data-stu-id="cf1fa-125">Create a project team</span></span>

1. <span data-ttu-id="cf1fa-126">Gainean **Proiektu guztiak** zerrendaren orria, hautatu proiektu bat eta, ondoren, hautatu **Editatu**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-126">On the **All projects** list page, select a project, and then select **Edit**.</span></span>
2. <span data-ttu-id="cf1fa-127">Gainean **Proiektu taldea eta programazioa** fitxan, **Egitarauaren amaiera data** eremuan, sartu programazioaren hasiera data gehi hilabete bat.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-127">On the **Project team and scheduling** tab, in the **Schedule end date** field, enter the schedule start date plus one month.</span></span> <span data-ttu-id="cf1fa-128">Adibidez, ordutegia hasteko data 2017ko ekainaren 24a bada (2017/06/24), sartu **2017/07/24**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-128">For example, if the schedule start date is June 24, 2017 (24/06/2017), enter **24/07/2017**.</span></span>
3. <span data-ttu-id="cf1fa-129">Hautatu **Gehitu**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-129">Select **Add**.</span></span>
4. <span data-ttu-id="cf1fa-130">**Gehitu eginkizunak proiektuari** panelean, **Rola** eremua, hautatu **Proiektu zuzendari nagusia**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-130">In the **Add roles to the project** pane, in the **Role** field, select **Senior Project Manager**.</span></span>
5. <span data-ttu-id="cf1fa-131">Aukeratu **Eskatutako gaitasunak**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-131">Select **Required competencies**.</span></span>
6. <span data-ttu-id="cf1fa-132">Gainean **Aukeratu ezaugarriak** orrialdean, lehenago zuzendari nagusiaren eginkizunerako zehaztutako ezaugarriak lehenespenez hautatzen dira.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-132">On the **Choose characteristics** page, the characteristics that you previously set for the Senior project manager role are selected by default.</span></span> <span data-ttu-id="cf1fa-133">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-133">Select **OK**.</span></span>
7. <span data-ttu-id="cf1fa-134">Gainean **Gehitu rolak proiektuari** orrialdean, **Baliabide kopurua** eremua, sartu **1**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-134">On the **Add roles to project** page, in the **Number of resources** field, enter **1**.</span></span>
8. <span data-ttu-id="cf1fa-135">**Baliabidea** eremuan, bilaketak beharrezko gaitasunak dituzten baliabide guztiak erakusten ditu.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-135">In the **Resource** field, the lookup shows all resources that have the required competencies.</span></span> <span data-ttu-id="cf1fa-136">Aukeratu **Daniel Goldschmidt** eta, ondoren, hautatu **Sortu**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-136">Select **Daniel Goldschmidt**, and then select **Create**.</span></span>
9. <span data-ttu-id="cf1fa-137">**Proiektua** orrian, hautatu **Gehitu**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-137">On the **Project** page, select **Add**.</span></span>
10. <span data-ttu-id="cf1fa-138">**Gehitu eginkizunak proiektuari** panelean, **Rola** eremua, hautatu **Taldekidea**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-138">In the **Add roles to the project** pane, in the **Role** field, select **Team member**.</span></span> <span data-ttu-id="cf1fa-139">**Baliabide-kopurua** eremua, sartu **5**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-139">In the **Number of resources** field, enter **5**.</span></span>
11. <span data-ttu-id="cf1fa-140">Hautatu **Sortu**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-140">Select **Create**.</span></span>
12. <span data-ttu-id="cf1fa-141">Gainean **Proiektuak** orrialdea, hautatu **Baliabidea bete**.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-141">On the **Projects** page, select **Fulfill resource**.</span></span>

## <a name="monitor-project-teams"></a><span data-ttu-id="cf1fa-142">Proiektu taldeak kontrolatu</span><span class="sxs-lookup"><span data-stu-id="cf1fa-142">Monitor project teams</span></span>
1. <span data-ttu-id="cf1fa-143">**Proiektu guztiak** orria, hautatu **Proiektuaren ID-a** esteka **XYZ Bertsio berritu fasea 2** proiektua.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-143">On the **All projects** page, select the **Project ID** link for the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="cf1fa-144">Gainean **Proiektu taldea eta programazioa** FastTab, egiaztatu zerrendan agertzen diren proiektuaren baliabideak zuzenak direla.</span><span class="sxs-lookup"><span data-stu-id="cf1fa-144">On the **Project team and scheduling** FastTab, verify that the project resources that are listed are correct.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]