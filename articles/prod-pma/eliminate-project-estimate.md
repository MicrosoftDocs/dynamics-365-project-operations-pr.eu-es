---
title: Ezabatu proiektuaren aurreikuspena
description: Gai honek proiektuaren estimazioa ezabatzeari buruzko informazioa eskaintzen du amaitu ondoren.
author: Yowelle
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: a4ad06bef7ed66a626c6d2ad7ef01ba5b99d1c0f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006901"
---
# <a name="eliminate-a-project-estimate"></a><span data-ttu-id="254b1-103">Ezabatu proiektuaren aurreikuspena</span><span class="sxs-lookup"><span data-stu-id="254b1-103">Eliminate a project estimate</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="254b1-104">Proiektuaren aurreikuspenek proiektuaren antolaketan aurreikusitako eta lanaren finantza ikuspegia eskaintzen dute.</span><span class="sxs-lookup"><span data-stu-id="254b1-104">Project estimates provide the financial view for work that is estimated and scheduled for a project.</span></span> <span data-ttu-id="254b1-105">Proiektu baten aurrekontuekin lan egiteko, proiektua aurrekontu proiektu batera erantsi behar duzu.</span><span class="sxs-lookup"><span data-stu-id="254b1-105">To work with estimates for a project, you must attach the project to an estimate project.</span></span> <span data-ttu-id="254b1-106">Aurreikusitako proiektua lehendik dagoen proiektu batean oinarritzen da beti, baina proiektu anitzek aurrekontu proiektu bakarra aipa dezakete.</span><span class="sxs-lookup"><span data-stu-id="254b1-106">An estimate project is always based on an existing project, however multiple projects can refer to a single estimate project.</span></span> <span data-ttu-id="254b1-107">Prezio finkoak eta inbertsio proiektuak bakarrik erantsi daitezke proiektuak kalkulatzeko, eta proiektu horiek aurrekontuaren proiektuaren talde berekoak izan behar dute.</span><span class="sxs-lookup"><span data-stu-id="254b1-107">Only fixed-price and investment projects can be attached to estimate projects, and those projects must belong to the same project group as the estimate project.</span></span>

<span data-ttu-id="254b1-108">Aurrekontuen proiektua ezabatzeko, osatuta egon behar du.</span><span class="sxs-lookup"><span data-stu-id="254b1-108">To eliminate an estimate project, it must be complete.</span></span> <span data-ttu-id="254b1-109">Ondorengo urratsetan kalkulua nola ezabatu azaltzen da.</span><span class="sxs-lookup"><span data-stu-id="254b1-109">The following steps explain how to eliminate an estimate.</span></span>

1. <span data-ttu-id="254b1-110">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** aukerara, eta ireki proiektua.</span><span class="sxs-lookup"><span data-stu-id="254b1-110">Go to **Project management and accounting** > **All Projects** and open the project.</span></span> 
2. <span data-ttu-id="254b1-111">**Kudeatu** fitxan, hautatu **Aurrekontuak** eta **Estimazioa** orrian hautatu **Ezabatu**.</span><span class="sxs-lookup"><span data-stu-id="254b1-111">On the **Manage** tab, select **Estimates**, and on the **Estimate** page select **Eliminate**.</span></span>
3. <span data-ttu-id="254b1-112">**Ezabatu aurrekontua** orrialdean **Orokorra** fitxa, ezarri aukera hauek:</span><span class="sxs-lookup"><span data-stu-id="254b1-112">On the **Eliminate estimate** page on the **General** tab, set the following options:</span></span>

   - <span data-ttu-id="254b1-113">**Garai kodea**: Aukeratu epearen kodea aurrekontu proiektu egokiak aukeratzeko.</span><span class="sxs-lookup"><span data-stu-id="254b1-113">**Period code**: Select the period code to choose the appropriate estimate projects.</span></span> 
   - <span data-ttu-id="254b1-114">**Aurreikusitako data**: Aukeratu ezabatzeko data egokia.</span><span class="sxs-lookup"><span data-stu-id="254b1-114">**Estimate date**: Select the appropriate estimate date for elimination.</span></span>
   - <span data-ttu-id="254b1-115">**Ezabatu WIP abisuekin**: Gaitu aukera hau jakinarazpenak bidaltzeko egiten ari diren lanekin (WIP) lotutako estimazioa ezabatzen denean.</span><span class="sxs-lookup"><span data-stu-id="254b1-115">**Eliminate with WIP warnings**: Enable this option to provide notification when an estimate that is associated with a work in progress (WIP) will be eliminated.</span></span> <span data-ttu-id="254b1-116">Aukera hau gaituta ez dagoenean, ezabatzeak ezin du jarraitu estimatu gabeko transakziorik baldin badago.</span><span class="sxs-lookup"><span data-stu-id="254b1-116">When this option is not enabled, elimination can’t continue if any non-estimated transactions exist.</span></span> 
   > [!NOTE]
   > <span data-ttu-id="254b1-117">Aukera hau aurrekontu proiektu bati ezabatzea aplikatzen zaionean bakarrik dago erabilgarri.</span><span class="sxs-lookup"><span data-stu-id="254b1-117">This option is available only when elimination is applied to an estimate project.</span></span> <span data-ttu-id="254b1-118">Ez dago erabilgarri aldizkako mezuak erabiltzen ari bazara.</span><span class="sxs-lookup"><span data-stu-id="254b1-118">It is not available if you are using periodic postings.</span></span> <span data-ttu-id="254b1-119">Ezarpen honek ezarpenekin funtzionatzen du **Estimazioa** fitxan **Proiektuaren parametroak** orrialdean, **Baimendu ezabatzea kalkulatu gabeko transakzioak daudenean** zelai taldea.</span><span class="sxs-lookup"><span data-stu-id="254b1-119">This setting works with the settings on the **Estimate** tab on the **Project parameters** page, in the **Allow elimination when non-estimated transactions exist** field group.</span></span>
   - <span data-ttu-id="254b1-120">**Ezarri etapa amaituta**: Gaitu aukera hau aurrekontuaren proiektuaren etapa zehazteko **Amaituta** kanporaketa exekutatu ondoren.</span><span class="sxs-lookup"><span data-stu-id="254b1-120">**Set stage to Finished**: Enable this option to set the estimate project’s stage to **Finished** after you run the elimination.</span></span>
   - <span data-ttu-id="254b1-121">**Inprimatu aurrekontuen zerrenda**: Hautatu aurrekontuen zerrenda inprimatzean sartu beharreko informazioa.</span><span class="sxs-lookup"><span data-stu-id="254b1-121">**Print estimate list**: Select the information to be included when the estimate list is printed.</span></span>
   - <span data-ttu-id="254b1-122">**Erakutsi Infolog**: Gaitu aukera hau Infolog bistaratzeko.</span><span class="sxs-lookup"><span data-stu-id="254b1-122">**Show Infolog**: Enable this option to display the Infolog.</span></span>
   - <span data-ttu-id="254b1-123">**Bidalketa data**: Aukeratu aurrekontuaren liburutegiaren data.</span><span class="sxs-lookup"><span data-stu-id="254b1-123">**Posting date**: Choose the ledger posting date of the estimate.</span></span>

4.  <span data-ttu-id="254b1-124">Hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="254b1-124">Select **OK**.</span></span>
5. <span data-ttu-id="254b1-125">Ezabatze prozesua amaitu ondoren, ezabatutako estimazio proiektua balio negatiboarekin bistaratuko da.</span><span class="sxs-lookup"><span data-stu-id="254b1-125">After the elimination process is complete, the eliminated estimate project is displayed with a negative value.</span></span> 

<span data-ttu-id="254b1-126">Estimazio bat ezabatzeko asmorik ez baduzu, ezabatutako aurrekontua hauta dezakezu eta hautatu **Alderantzizko kanporaketa**.</span><span class="sxs-lookup"><span data-stu-id="254b1-126">If you did not intend to eliminate an estimate, you can select the eliminated estimate and select **Reverse elimination**.</span></span>   


[!INCLUDE[footer-include](../includes/footer-banner.md)]