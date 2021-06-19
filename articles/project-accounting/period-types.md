---
title: Aldi motak
description: Gai honek diru-sarreren aurreikuspenen aldi motak konfiguratzeko informazioa ematen du.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 07cc9cde5fab10accb1fd6efede58926918f614c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013471"
---
# <a name="period-types"></a><span data-ttu-id="8dd46-103">Aldi motak</span><span class="sxs-lookup"><span data-stu-id="8dd46-103">Period types</span></span>

<span data-ttu-id="8dd46-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="8dd46-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8dd46-105">Epe mota batek proiektu bateko diru sarrerak zenbatetan kalkulatzen diren definitzen du.</span><span class="sxs-lookup"><span data-stu-id="8dd46-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="8dd46-106">Gai honek diru-sarreren aurreikuspenen aldi motak konfiguratzeko informazioa ematen du.</span><span class="sxs-lookup"><span data-stu-id="8dd46-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="8dd46-107">Aldi motak sortu eta horiekin lan egin</span><span class="sxs-lookup"><span data-stu-id="8dd46-107">Create and work with period types</span></span>
<span data-ttu-id="8dd46-108">Garai motak sortzeko eta lantzeko, jarraitu urrats hauek:</span><span class="sxs-lookup"><span data-stu-id="8dd46-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="8dd46-109">Dynamics 365 Finance ingurunea, joan **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Aurrekontuak** > **Garai motak**.</span><span class="sxs-lookup"><span data-stu-id="8dd46-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="8dd46-110">Hautatu **Berria**, aldi mota berria sortzeko.</span><span class="sxs-lookup"><span data-stu-id="8dd46-110">Select **New** to create new period type.</span></span> <span data-ttu-id="8dd46-111">Idatzi izena eta deskribapena.</span><span class="sxs-lookup"><span data-stu-id="8dd46-111">Enter a name and description.</span></span>
3. <span data-ttu-id="8dd46-112">**Maiztasuna** eremuan, hautatu balio bat:</span><span class="sxs-lookup"><span data-stu-id="8dd46-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="8dd46-113">**Astea**, **Bi astero**, **Hilean behin**, **Hilabetea**, **Eguna**, **Lau hilean behin** edo **Urtea** hautatzen baduzu, egutegia aldiak sortzeko erabiliko da.</span><span class="sxs-lookup"><span data-stu-id="8dd46-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="8dd46-114">Hautatzen baduzu **Liburuaren aldia**, Liburu orokorraren konfigurazioko liburuen aldiak aldiak sortzeko erabiliko dira.</span><span class="sxs-lookup"><span data-stu-id="8dd46-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="8dd46-115">Hautatzen baduzu **Mugagabea**, aldi pertsonalizatuak zehaztu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="8dd46-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="8dd46-116">Hautatu aldi mota erregistroa eta hautatu **Sortu epeak** aldi motarako aldiak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="8dd46-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="8dd46-117">Aukeratu duzun aldiaren maiztasunean oinarrituta, hasiera data edo sortu beharreko aldi kopurua zehazteko aukera izan dezakezu.</span><span class="sxs-lookup"><span data-stu-id="8dd46-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="8dd46-118">Aukeratu **Aldiak** sortutako aldiak berrikusteko.</span><span class="sxs-lookup"><span data-stu-id="8dd46-118">Select **Periods** to review generated periods.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]