---
title: Eguneko dietak
description: Gai honek Gastuen kudeaketan erabiltzen diren dieten arauei buruzko informazioa eskaintzen du.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 70e26a5e0f9a06730a2166318006429195335d4d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276288"
---
# <a name="per-diems"></a><span data-ttu-id="09240-103">Eguneko dietak</span><span class="sxs-lookup"><span data-stu-id="09240-103">Per diems</span></span>

<span data-ttu-id="09240-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="09240-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="09240-105">Eguneko egun bat lanagatik bidaiatzen duen langileari ematen zaion hobaria da.</span><span class="sxs-lookup"><span data-stu-id="09240-105">A per diem is an allowance that is paid to a worker who is traveling for work.</span></span> <span data-ttu-id="09240-106">Gastuen kudeaketan, eguneko arauak sor ditzakezu bidaia-egoera desberdinetarako.</span><span class="sxs-lookup"><span data-stu-id="09240-106">In Expense management, you can create per diem rules for  various travel situations.</span></span> <span data-ttu-id="09240-107">Eguneko tasak urteko garaian, bidaiaren kokapenean edo bietan oinarrituta egon daitezke.</span><span class="sxs-lookup"><span data-stu-id="09240-107">Per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="09240-108">Eguneko araua sortzen duzunean, eguneko tasaren ehuneko bat gordeko dela zehaztu dezakezu langileak osagarriak diren otorduak edo zerbitzuak jasotzen baditu.</span><span class="sxs-lookup"><span data-stu-id="09240-108">When you create a per diem  rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="09240-109">Halaber, eguneko tasak langilearen bidaiari aplikatu ahal izateko gutxieneko eta gehieneko ordu kopurua ere ezar dezakezu.</span><span class="sxs-lookup"><span data-stu-id="09240-109">You can also set a minimum and maximum number of hours that the per diem rate can apply to a worker's travel.</span></span>

## <a name="configuration"></a><span data-ttu-id="09240-110">Konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="09240-110">Configuration</span></span> 

1. <span data-ttu-id="09240-111">Eguneko kokapenak gehitzeko, joan **Konfiguratu** > **Kalkuluak eta kodeak** > **Eguneko esleipenak**.</span><span class="sxs-lookup"><span data-stu-id="09240-111">To add per diem locations, go to **Set up** > **Calculations and codes** > **Per diem locations**.</span></span>
2. <span data-ttu-id="09240-112">Goian gehitutako kokapen bakoitzerako, hautatu eguneko tasa eta dibisa, hotelerako, otorduetarako eta bestelako gastuetarako hasiera eta amaiera data zehatz baten artean balioduna.</span><span class="sxs-lookup"><span data-stu-id="09240-112">For each of the locations added above, select a per diem rate and currency that is valid between a specific start and end date for hotel, meals, and other expenses.</span></span> <span data-ttu-id="09240-113">Eguneko tasak eta monetak konfiguratuta daude **Konfiguratu** > **Kalkuluak eta kodeak** > **Dietak**.</span><span class="sxs-lookup"><span data-stu-id="09240-113">Per diem rates and currencies are configured under **Set up** > **Calculations and codes** > **Per diems**.</span></span>
3. <span data-ttu-id="09240-114">**Eguneko kokapenak** orrialdean, konfiguratu eguneko tasa mailak.</span><span class="sxs-lookup"><span data-stu-id="09240-114">On the **Per diem locations** page, configure per diem rate tiers.</span></span> <span data-ttu-id="09240-115">Eguneko tasa-mailek hoteleko, otorduko eta bestelako gastuetarako eguneko hobari baten ehunekoaren banaketa zehazteko aukera ematen dute.</span><span class="sxs-lookup"><span data-stu-id="09240-115">Per diem rate tiers allow you to define the percentage split of a daily allowance for hotel, meal, and other expenses.</span></span> 
4. <span data-ttu-id="09240-116">Gosarian, bazkarian edo afarian otorduen ehuneko murrizketa zehazteko, eguneratu eremuko **Gastuak kudeatzeko parametroak** orrialdean **Eguneko** fitxa.</span><span class="sxs-lookup"><span data-stu-id="09240-116">To specify the meal percentage reduction for breakfast, lunch, or dinner, update the fields on the **Expense management parameters** page on the **Per diem** tab.</span></span> 
    
## <a name="submit-expenses-using-per-diem"></a><span data-ttu-id="09240-117">Bidali egun bakoitzeko gastuak</span><span class="sxs-lookup"><span data-stu-id="09240-117">Submit expenses using per diem</span></span>
<span data-ttu-id="09240-118">Dietak erabiliz gastuak bidaltzeko, erabili **Eguneko** gastuen kategoria gastuen txostena sortzen duzunean.</span><span class="sxs-lookup"><span data-stu-id="09240-118">To submit expenses utilizing per diems, use the **Per diem** expense category when you create an expense report.</span></span> <span data-ttu-id="09240-119">Sartu **Eguneko egunetik aurrera**, **Eguneko egunerokoa** eta **Eguneko kokapena**.</span><span class="sxs-lookup"><span data-stu-id="09240-119">Enter the **Per diem from date**, **Per diem to date**,  and the **Per diem location**.</span></span> <span data-ttu-id="09240-120">Zenbatekoa hautatutako kokapeneko eguneko tasen arabera kalkulatuko da eta otorduen murrizketa eguneko tasen mailen arabera kalkulatuko da.</span><span class="sxs-lookup"><span data-stu-id="09240-120">The amount will be calculated based on the per diem rates for the selected location and meal reduction will be calculated based on the per diem rate tiers.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]