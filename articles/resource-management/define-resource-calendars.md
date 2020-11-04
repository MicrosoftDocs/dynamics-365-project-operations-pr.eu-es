---
title: Zehaztu baliabide-egutegiak
description: Gai honek Project Operations-en baliabideen lanordu-egutegiak definitzeko moduari buruzko informazioa eskaintzen du.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ab39d7e5dc2d8c01ed49ca0f1a4d1691aaf15637
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070884"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="5c1c0-103">Zehaztu baliabide-egutegiak</span><span class="sxs-lookup"><span data-stu-id="5c1c0-103">Define resource calendars</span></span>

<span data-ttu-id="5c1c0-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="5c1c0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5c1c0-105">Proiektu batean lan egiten duen baliabide erreserbagarri bakoitzak lanorduen egutegia izan behar du erabilgarritasuna zehazteko.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="5c1c0-106">Baliabide baten lan orduak bi eratara defini daitezke:</span><span class="sxs-lookup"><span data-stu-id="5c1c0-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="5c1c0-107">Baliabide baten egutegiaren arau indibidualak definitu</span><span class="sxs-lookup"><span data-stu-id="5c1c0-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="5c1c0-108">Aplikatu lehendik dagoen egutegiaren txantiloia baliabidearentzat</span><span class="sxs-lookup"><span data-stu-id="5c1c0-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="5c1c0-109">Zehaztu baliabidearen lanorduak</span><span class="sxs-lookup"><span data-stu-id="5c1c0-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="5c1c0-110">**Baliabideak** menuan, hautatu **Baliabideak**.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="5c1c0-111">Sareta ikuspegian, hautatu dagokion **Erreserbatzeko Baliabidea**.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="5c1c0-112">**Baliabideen xehetasunak** orrian, hautatu **Lan-orduak** fitxa. Lehenespenez, erreserbatzeko baliabideen egutegiak erakundearentzat definitutako lanordu lehenetsiko txantiloiaren lanorduak lehenetsi ditu.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="5c1c0-113">Laneko ordutegia eguneratzeko, egin klik eskuineko botoiarekin definitu beharreko egutegiaren arau hasierako datan.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="5c1c0-114">Erabili egutegiaren arauen menua egun zehatz baterako, serieko hondarreko edo egutegi osoko egutegi arau bat definitzeko.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="5c1c0-115">Aukera hautatu ondoren, ondoren definitu dezakezu:</span><span class="sxs-lookup"><span data-stu-id="5c1c0-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="5c1c0-116">Laneko ordutegia aplikatuko den asteko eguna.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="5c1c0-117">Egun bakoitzeko lanorduak.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-117">The working times within each day.</span></span>
    - <span data-ttu-id="5c1c0-118">Egutegi-arauaren ordu-zona.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="5c1c0-119">Hala badagokio, lanik gabeko denbora ere zehaztu daiteke araurako.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="5c1c0-120">Egutegiaren txantiloia baliabide bati aplikatzea</span><span class="sxs-lookup"><span data-stu-id="5c1c0-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="5c1c0-121">**Baliabideak** menuan, hautatu **Baliabideak**.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="5c1c0-122">Sareta ikuspegian, hautatu 25 **Erreserbatzeko baliabide** eguneratzeko.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="5c1c0-123">Aukeratu **Ezarri egutegia** eta elkarrizketa-koadro batek erabilgarri dauden lan orduen txantiloien zerrenda eskatuko dizu.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="5c1c0-124">Hautatu erabili nahi duzun txantiloia eta sakatu **Aplikatu**.</span><span class="sxs-lookup"><span data-stu-id="5c1c0-124">Select the template you want to use, and then select **Apply**.</span></span>
