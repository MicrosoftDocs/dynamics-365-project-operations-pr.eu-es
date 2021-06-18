---
title: Sinkronizatu baliabideen gaitasuna
description: Gai honetan baliabidearen ahalmena egutegiekin eta proiektuekin sinkronizatzeko moduari buruzko informazioa eskaintzen da.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8bde3c434680f0651293cbce13ecdce945c3a743
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997496"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="08069-103">Sinkronizatu baliabideen gaitasuna</span><span class="sxs-lookup"><span data-stu-id="08069-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="08069-104">Baliabideak sinkronizatzeko prozesuei esker, egutegiaren eta oinarrizko egutegiaren informazioa proiektuaren baliabideen programazioan sartzen da.</span><span class="sxs-lookup"><span data-stu-id="08069-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="08069-105">Egutegia aldatzen bada, prozesuek beharrezko eguneratzeak egiten dituzte proiektuaren baliabideen programazioan.</span><span class="sxs-lookup"><span data-stu-id="08069-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="08069-106">Prozesuek errendimendua hobetzen ere laguntzen dute, egutegiaren baliabideen informazioa aldez aurretik sinkronizatuta dagoelako.</span><span class="sxs-lookup"><span data-stu-id="08069-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="08069-107">Hori dela eta, baliabideak antolatzeko informazioaren eguneratzeak azkarrago gertatzen dira.</span><span class="sxs-lookup"><span data-stu-id="08069-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="08069-108">Prozesuak multzo gisa antolatzea gomendatzen dizugu, aldi berean ordez.</span><span class="sxs-lookup"><span data-stu-id="08069-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="08069-109">Bestela, norbaitek informazioa azkeneko aldiz sinkronizatu zeneko egun biak barne ahazteko arriskua dago.</span><span class="sxs-lookup"><span data-stu-id="08069-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="08069-110">Data inklusiboak erabiltzen ez badira, hutsuneak gerta daitezke data sinkronizatzean.</span><span class="sxs-lookup"><span data-stu-id="08069-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![Egutegiaren sinkronizazioa](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="08069-112">Sinkronizatu baliabide-gaitasuna bateratzea</span><span class="sxs-lookup"><span data-stu-id="08069-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="08069-113">Sinkronizazio prozesua baliabideen egutegiko informazio guztia sinkronizatzeko diseinatuta dago.</span><span class="sxs-lookup"><span data-stu-id="08069-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="08069-114">Informazio honek proiektuaren Baliabideen egutegiaren edukiera taulan egindako aldaketen inguruko oinarrizko egutegiko informazioa biltzen du.</span><span class="sxs-lookup"><span data-stu-id="08069-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="08069-115">Proiektuan baliabide berriak gehitzen badira, sinkronizazioak eguneratutako egutegiko informazioa eskuragarri dagoela bermatzen laguntzen du.</span><span class="sxs-lookup"><span data-stu-id="08069-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="08069-116">Sinkronizazio hau edozein unetan egin daiteke.</span><span class="sxs-lookup"><span data-stu-id="08069-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="08069-117">Gomendatzen dizugu erabiltzea sorta gisa.</span><span class="sxs-lookup"><span data-stu-id="08069-117">We recommend that you use a batch.</span></span> <span data-ttu-id="08069-118">Aukerak eskuragarri daude edukiera erreserbak sinkronizatzean.</span><span class="sxs-lookup"><span data-stu-id="08069-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="08069-119">Aukeratu **Proiektuen kudeaketa eta kontabilitatea** &gt; **Aldizkakoa** &gt; **Edukiera sinkronizatzea** &gt; **Sinkronizatu baliabideen ahalmenak**.</span><span class="sxs-lookup"><span data-stu-id="08069-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="08069-120">Ezarri aukerak ondoko taulan bistaratzen dira.</span><span class="sxs-lookup"><span data-stu-id="08069-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="08069-121">Aukera</span><span class="sxs-lookup"><span data-stu-id="08069-121">Option</span></span>      | <span data-ttu-id="08069-122">Deskribapenak</span><span class="sxs-lookup"><span data-stu-id="08069-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="08069-123">Garai kodea</span><span class="sxs-lookup"><span data-stu-id="08069-123">Period code</span></span> | <span data-ttu-id="08069-124">Aukeran hautatu Liburu nagusiaren data tarte kodea, baliabideen edukiera biltzeko sinkronizazio prozesuaren hasiera eta amaiera datak ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="08069-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="08069-125">Hasiera-data</span><span class="sxs-lookup"><span data-stu-id="08069-125">Start date</span></span>  | <span data-ttu-id="08069-126">Idatzi baliabideen edukiera biltzeko prozesuen sinkronizazio prozesuaren hasiera data.</span><span class="sxs-lookup"><span data-stu-id="08069-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="08069-127">Amaiera-data</span><span class="sxs-lookup"><span data-stu-id="08069-127">End date</span></span>    | <span data-ttu-id="08069-128">Idatzi baliabideen edukiera biltzeko prozesuen sinkronizazio prozesuaren amaiera data.</span><span class="sxs-lookup"><span data-stu-id="08069-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="08069-129">[![Sinkronizazio-prozesua](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="08069-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]