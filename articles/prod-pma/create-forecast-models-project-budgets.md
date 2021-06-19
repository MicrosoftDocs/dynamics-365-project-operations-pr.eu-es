---
title: Sortu proiektuaren aurrekontuen aurreikuspen ereduak
description: Gai honetan gainerako aurrekontuetarako aurreikuspen eredua nola sortu deskribatzen da.
author: Yowelle
ms.date: 04/24/2020
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
ms.openlocfilehash: 3549b41fce72b44230ab27de081dade15a912266
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006271"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="b8278-103">Sortu proiektuaren aurrekontuen aurreikuspen ereduak</span><span class="sxs-lookup"><span data-stu-id="b8278-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b8278-104">Gai honetan gainerako aurrekontuetarako aurreikuspen eredua nola sortu deskribatzen da.</span><span class="sxs-lookup"><span data-stu-id="b8278-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="b8278-105">Aurrekontuen kontrolpean dagoen proiektuak bi aurrekontu mota erabiltzen ditu: jatorrizkoak eta gainerakoak.</span><span class="sxs-lookup"><span data-stu-id="b8278-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="b8278-106">Proiektuaren aurrekontua sortzen duzunean, jatorrizko eta gainerako aurrekontuen aurreikuspen ereduak zehaztu behar dituzu **Iragarpen ereduak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="b8278-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="b8278-107">Zehaztutako ereduetan oinarritutako proiektuen aurrekontuak proiektuaren aurrekontua konprometitzen duzunean sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="b8278-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="b8278-108">Aurrekontuen kontrolerako erabiltzen den iragarpen ereduak ezin du azpimodelarik izan edo azpimodel gisa erabili.</span><span class="sxs-lookup"><span data-stu-id="b8278-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="b8278-109">Aukeratu **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Iragarpenak**  > **Iragarpen ereduak**.</span><span class="sxs-lookup"><span data-stu-id="b8278-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="b8278-110">Aukeratu **Berria** iragarpen eredu berria sortzeko eta, ondoren, idatzi modelo berriaren ID zenbakia eta izena.</span><span class="sxs-lookup"><span data-stu-id="b8278-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="b8278-111">Ezarri **Geldituta** aukera **Bai** iragarpen-ereduaren iragarpen-lerroetan aldaketarik gerta ez dadin.</span><span class="sxs-lookup"><span data-stu-id="b8278-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="b8278-112">Eredua lotzen den iragarpen-lerroek kutxa-fluxuen aurreikuspenak sortu behar badituzte liburu nagusian, hautatu **Diru fluxuen aurreikuspenetan sartu** aukeran **Bai**.</span><span class="sxs-lookup"><span data-stu-id="b8278-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="b8278-113">Proiektuaren data faktura-data gisa erabiltzeko, hautatu **Iragarpenaren faktura-data** aukeran **Bai**.</span><span class="sxs-lookup"><span data-stu-id="b8278-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="b8278-114">**Aurrekontu mota** eremuan, hautatu eredu mota hauetako bat:</span><span class="sxs-lookup"><span data-stu-id="b8278-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="b8278-115">**Jatorrizko aurrekontua**: Hasierako aurrekontua sortu eta onartzen denean konprometitutako jatorrizko aurrekontuaren zenbatekoak erabili.</span><span class="sxs-lookup"><span data-stu-id="b8278-115">**Original budget**: Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="b8278-116">**Gainerako aurrekontua**: Erabili gainerako aurrekontuaren zenbatekoak proiektuaren bizitzan zehar.</span><span class="sxs-lookup"><span data-stu-id="b8278-116">**Remaining budget**: Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="b8278-117">Aurreikuspen eredu honetako saldoak benetako transakzioen bidez murrizten dira eta aurrekontuen berrikuspenen arabera handitzen edo murrizten dira.</span><span class="sxs-lookup"><span data-stu-id="b8278-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="b8278-118">**Aurrera eraman**: Erabili proiektuaren aurrekontuaren zenbatekoak.</span><span class="sxs-lookup"><span data-stu-id="b8278-118">**Carry-forward**: Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="b8278-119">Aurreratzea aukerako prozesua da, erabili gabeko aurrekontu kopuruak urte fiskal batetik bestera transferitzeko exekutatu daitekeena.</span><span class="sxs-lookup"><span data-stu-id="b8278-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="b8278-120">Ezarri ondoko aukerak behar ahala:</span><span class="sxs-lookup"><span data-stu-id="b8278-120">Set the following options as required:</span></span>

   - <span data-ttu-id="b8278-121">Gaitu **Iragarpenaren faktura-data** proiektuaren data faktura-data gisa erabiltzeko.</span><span class="sxs-lookup"><span data-stu-id="b8278-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="b8278-122">Gaitu **Iragarpena WIPekin** Aurreikusteko egiten ari den lanaren arabera (WIP), eta gero hautatu WIP mota.</span><span class="sxs-lookup"><span data-stu-id="b8278-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="b8278-123">Lehenespenez **Aurrekontu mota** **Bat ere ez** gisa utz dezakezu edo idatzi mota berri bat.</span><span class="sxs-lookup"><span data-stu-id="b8278-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="b8278-124">Aurrekontu mota ezin da aldatu erregistro bat aldatu ondoren.</span><span class="sxs-lookup"><span data-stu-id="b8278-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="b8278-125">Aurrekontu mota lehenetsia aldatzen baduzu, gainerako aukera guztiak ez dira erabilgarri egongo eguneratzeetarako, eta ezin duzu iragarpen eredu hau berrerabili.</span><span class="sxs-lookup"><span data-stu-id="b8278-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]