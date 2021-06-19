---
title: Prezio finkoko diru-sarrerak kalkulatzeko proiektuak
description: Gai honek proiektuetako prezio finkoaren diru-sarrerei buruzko informazioa ematen du.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 639c6a104f2a90366a0f477c0d7cf384f19cdd81
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013786"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="80997-103">Prezio finkoko diru-sarrerak kalkulatzeko proiektuak</span><span class="sxs-lookup"><span data-stu-id="80997-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="80997-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="80997-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="80997-105">Urtean proiektuaren kontratu lerro bat sortzen duzunean Dynamics 365 Project Operations Microsoft Dataverse-n, sistemak automatikoki sortzen du prezio finkoko diru-sarreren aurrekontua.</span><span class="sxs-lookup"><span data-stu-id="80997-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="80997-106">Proiektu honetako informazioa honako hauetan oinarrituta dago:</span><span class="sxs-lookup"><span data-stu-id="80997-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="80997-107">Prezio finkoko fakturazio metodoa.</span><span class="sxs-lookup"><span data-stu-id="80997-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="80997-108">Lotutako proiektua.</span><span class="sxs-lookup"><span data-stu-id="80997-108">An associated project.</span></span>
  - <span data-ttu-id="80997-109">Urtean gutxienez mugarri bat zehaztu da **Fakturen egutegia** fitxan **Proiektuaren kontratu lerroa** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="80997-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="80997-110">Berrikusi prezio finkoko diru-sarreren aurreikuspenen proiektuak</span><span class="sxs-lookup"><span data-stu-id="80997-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="80997-111">Prezio finkoen diru-sarreren kalkuluen proiektuak berrikusteko, jarraitu urrats hauek:</span><span class="sxs-lookup"><span data-stu-id="80997-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="80997-112">Dynamics 365 Finance ingurunean, joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Prezio finkoko diru-sarrerak kalkulatzeko proiektuak**.</span><span class="sxs-lookup"><span data-stu-id="80997-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="80997-113">Aukeratu ikusi nahi duzun proiektua eta egin klik bikoitza botoian **Estimatu proiektuaren IDa** erregistroa ireki eta proiektuaren xehetasunak berrikusteko.</span><span class="sxs-lookup"><span data-stu-id="80997-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="80997-114">Zabaldu **Proiektua** fitxa. Proiektuan ikusiko duzu **Aukeratutako proiektuak** sareta.</span><span class="sxs-lookup"><span data-stu-id="80997-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="80997-115">Sistemak proiektu lehenetsi gisa erabiltzen du, proiektuaren kontratu lerroarekin lotutako proiektua delako.</span><span class="sxs-lookup"><span data-stu-id="80997-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="80997-116">Elkartea aldatzeko, hautatu proiektu osagarriak eta gehitu fitxategira **Aukeratutako proiektuak** sareta.</span><span class="sxs-lookup"><span data-stu-id="80997-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="80997-117">Sareta honetan proiektu anitz hautatzen badira, proiektuaren ehunekoaren osaketa eta diru-sarreren kalkuluak batera kalkulatuko dira hautatutako proiektu guztietarako.</span><span class="sxs-lookup"><span data-stu-id="80997-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="80997-118">Proiektuaren kostua, diru-sarreren profila, kostuen txantiloia eta aldiaren kodea eskuz ezar daitezke.</span><span class="sxs-lookup"><span data-stu-id="80997-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="80997-119">Eskuz ezarrita ez badaude, balioek lehenetsitakoak izango dira proiektuaren lehenengo kalkulu kalkuluan proiektuaren kostu eta diru-sarreren profiletarako konfiguratutako arauak erabiliz.</span><span class="sxs-lookup"><span data-stu-id="80997-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]