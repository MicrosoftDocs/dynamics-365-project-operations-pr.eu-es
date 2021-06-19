---
title: Onarpen multzoak
description: Gai honek onarpen multzoari, eskaerei eta eragiketa horien azpimultzoei buruzko informazioa eskaintzen du.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116856"
---
# <a name="approval-sets"></a><span data-ttu-id="362ea-103">Onarpen multzoak</span><span class="sxs-lookup"><span data-stu-id="362ea-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="362ea-104">Onarpenak taldearen onarpen eskaerak eragiketa azpimultzo txikiagoetan biltzen ditu.</span><span class="sxs-lookup"><span data-stu-id="362ea-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="362ea-105">Taldekatze honek Proiektuaren arabera onar ditzake onarpenak eta berriro saiatzea eta sekuentziatzea ahalbidetzen du.</span><span class="sxs-lookup"><span data-stu-id="362ea-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="362ea-106">Multzokatzeak homologazioen prozesuen fidagarritasuna eta trazabilitatea hobetzen ditu homologazio kopuru handietan.</span><span class="sxs-lookup"><span data-stu-id="362ea-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="362ea-107">Onarpen multzoek erlazionatutako erregistroen prozesatze egoera orokorra adierazten dute.</span><span class="sxs-lookup"><span data-stu-id="362ea-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="362ea-108">Onarpen erregistroa onarpen multzo bat erabiliz prozesatzen denean, erregistroa mugitzen da **Bidalita** aukeratik **Onartuta** aukerara, eta onarpen multzoarekin lotu gabe dago.</span><span class="sxs-lookup"><span data-stu-id="362ea-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="362ea-109">Erregistro batek huts egiten badu onarpenera aurkezten denean, erregistroa egoera berean geratzen da **Bidalita** eta onarpen multzoa huts egin duela markatzen da.</span><span class="sxs-lookup"><span data-stu-id="362ea-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="362ea-110">Onarpen multzoak hutsaren errore mezua erregistratzen du.</span><span class="sxs-lookup"><span data-stu-id="362ea-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="362ea-111">Onarpenak eta onarpen multzoak prozesatzea</span><span class="sxs-lookup"><span data-stu-id="362ea-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="362ea-112">Fitxategian prozesatzeko ilaran dauden onarpenak ikusgai daude **Onarpenak prozesatzen** ikuspegia.</span><span class="sxs-lookup"><span data-stu-id="362ea-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="362ea-113">Sistema sarrera guztiak hainbat aldiz modu asinkronoan prozesatzen saiatzen da, aurreko saiakerak huts egiten badu baimena berriro saiatzea barne.</span><span class="sxs-lookup"><span data-stu-id="362ea-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="362ea-114">**Onarpena ezarri Bizitza** eremuak multzoa prozesatzeko geratzen den saiakera kopurua erregistratzen du huts egin duela markatu aurretik.</span><span class="sxs-lookup"><span data-stu-id="362ea-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="362ea-115">Ezin izan dira ezarri onarpenak eta onarpen multzoak</span><span class="sxs-lookup"><span data-stu-id="362ea-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="362ea-116">**Hutsegitea onartu da** ikuspegia erabiltzailearen esku-hartzea behar duten onarpen guztiak zerrendatzen ditu.</span><span class="sxs-lookup"><span data-stu-id="362ea-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="362ea-117">Ireki lotutako onarpen multzoen erregistroak porrotaren zergatia identifikatzeko.</span><span class="sxs-lookup"><span data-stu-id="362ea-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="362ea-118">**Saiatu berriro** hautatuz gero onarpen multzoari bizitza osoko zenbaketa gehitzen dio, onarpen multzoa berriro egoera batera eramaten du **Prozesamendua**, eta gainerako erregistroak prozesatzen saiatzen da.</span><span class="sxs-lookup"><span data-stu-id="362ea-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="362ea-119">Konfiguratu onarpen multzoak</span><span class="sxs-lookup"><span data-stu-id="362ea-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="362ea-120">Gaitu Onarpen multzoen eginbidea</span><span class="sxs-lookup"><span data-stu-id="362ea-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="362ea-121">Onarpen multzoa eginbidea gaitu aurretik, egiaztatu ez dagoela prozesatzen ari diren onarpenik.</span><span class="sxs-lookup"><span data-stu-id="362ea-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="362ea-122">Joan **Proiektuaren parametroak** orrialdera eta hautatu **Ezaugarrien kontrola** > **Gaitu onarpen modernoak**.</span><span class="sxs-lookup"><span data-stu-id="362ea-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="362ea-123">Desaktibatu Onarpen multzoen eginbidea</span><span class="sxs-lookup"><span data-stu-id="362ea-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="362ea-124">Onarpen multzoa eginbidea desaktibatu aurretik, egiaztatu ez dagoela prozesatzen ari diren onarpenik.</span><span class="sxs-lookup"><span data-stu-id="362ea-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="362ea-125">Joan **Proiektuaren parametroak** orrialdera eta hautatu **Ezaugarrien kontrola** > **Desgaitu onarpen modernoak**.</span><span class="sxs-lookup"><span data-stu-id="362ea-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="362ea-126">Atalasea sinkronoa konfiguratzea</span><span class="sxs-lookup"><span data-stu-id="362ea-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="362ea-127">Onarpen multzoak sortzen direnean, prozesamendua bigarren plano batera pasatzen da onartutako hautatutako erregistro kopurua adierazitako atalasea gainditzen duenean.</span><span class="sxs-lookup"><span data-stu-id="362ea-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="362ea-128">Erabili **Atalasea asinkronoa** onarpen prozesamendua sinkronikoki edo asinkronikoki exekutatu behar denean konfiguratzeko eremua.</span><span class="sxs-lookup"><span data-stu-id="362ea-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="362ea-129">Baliozko balioak dira:</span><span class="sxs-lookup"><span data-stu-id="362ea-129">Valid values are:</span></span>

  - <span data-ttu-id="362ea-130">Zero: eskaera guztiak modu asinkronoan prozesatu beharko lirateke.</span><span class="sxs-lookup"><span data-stu-id="362ea-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="362ea-131">Zero baino handiagoak diren zenbakiak: onartutakoak modu asinkronoan prozesatzen dira aurkeztutako onarpen kopuruak balio hori gainditzen duenean.</span><span class="sxs-lookup"><span data-stu-id="362ea-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
