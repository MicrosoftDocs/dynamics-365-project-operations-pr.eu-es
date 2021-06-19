---
title: Antolatu proiektuaren baliabideak
description: Nola antolatu proiektuaren baliabideak Project Service-n
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c67633960bb448d2190ec1bfde4e964f4fcb7969
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6008476"
---
# <a name="schedule-resources-for-a-project-project-service"></a><span data-ttu-id="6facd-103">Antolatu proiektuaren baliabideak (Project Service)</span><span class="sxs-lookup"><span data-stu-id="6facd-103">Schedule resources for a project (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6facd-104">Baliabideen erabilgarritasuna egiazta dezakezu zure baliabideen okupazio-maila oro har ikusteko edo abilezien, taldearen, kokapenaren edo beste aukera batzuen arabera iragaz ditzakezu ikuspegiak.</span><span class="sxs-lookup"><span data-stu-id="6facd-104">You can check resource availability to get an overall view of how booked your resources are, or you can filter the view by skills, team, location, and other options.</span></span>  
  
<span data-ttu-id="6facd-105">Antolatu board erabilgarritasuna beren eta baliabide-zerrenda erakusten du.</span><span class="sxs-lookup"><span data-stu-id="6facd-105">The schedule board shows list of resources and their availability.</span></span> <span data-ttu-id="6facd-106">Erakutsi modu erabilgarritasuna ikuspegia modua **Ordu**, **Eguna**, **Asteko**, edo **Hilabeteko**.</span><span class="sxs-lookup"><span data-stu-id="6facd-106">Select a view mode to show availability by **Hours**, **Day**, **Week**, or **Month**.</span></span>  
  
<span data-ttu-id="6facd-107">Antolaketa-panela erabili aurretik, konfiguratu egin behar da.</span><span class="sxs-lookup"><span data-stu-id="6facd-107">Before you use the schedule board, it’s important to set it up.</span></span> <span data-ttu-id="6facd-108">Informazio gehiago lortzeko, ikusi [Konfiguratu antolaketa-panela (Field Service edo Project Service Automation)](/dynamics365/field-service/configure-schedule-board).</span><span class="sxs-lookup"><span data-stu-id="6facd-108">For more information, see [Configure the schedule board (Field Service or Project Service Automation)](/dynamics365/field-service/configure-schedule-board).</span></span>
  
<span data-ttu-id="6facd-109">Bertsio zahar bat erabiltzen ari bazara, baliabide erabilgarritasuna jakiteko, ikusi [Ikusi baliabideen erabilgarritasuna](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="6facd-109">If you are using an older version, for resource availability, see [View resource availability](../psa/view-resource-availability.md).</span></span>  

> [!IMPORTANT]
>  <span data-ttu-id="6facd-110">Antolaketa board erreserbatu funtzioa, geocoding eta kokaleku-zerbitzuak erabili behar duzu esleipenak aktibatu.</span><span class="sxs-lookup"><span data-stu-id="6facd-110">To use the schedule board booking functionality, geocoding, and location services, you need to turn on maps.</span></span>  
> 
> 1. <span data-ttu-id="6facd-111">Menu nagusian, hautatu **Baliabideen antolaketa** > **Administrazioa**.</span><span class="sxs-lookup"><span data-stu-id="6facd-111">On the main menu, select **Resource Scheduling** > **Administration**.</span></span>  
> 2. <span data-ttu-id="6facd-112">Sakatu **Antolaketa-parametroak**.</span><span class="sxs-lookup"><span data-stu-id="6facd-112">Click **Scheduling parameters**.</span></span>  
> 3. <span data-ttu-id="6facd-113">Ireki erregistroa eta joan behera **Resource Scheduling Optimization** atalean.</span><span class="sxs-lookup"><span data-stu-id="6facd-113">Open record and scroll down to the **Resource Scheduling Optimization** section.</span></span>  
> 4. <span data-ttu-id="6facd-114">**Mapetara konektatu** eremuan, aukeratu **Bai**.</span><span class="sxs-lookup"><span data-stu-id="6facd-114">On the **Connect to Maps** field, choose **Yes**.</span></span>  
> 5. <span data-ttu-id="6facd-115">Onartu baldintzak eta gorde erregistroa.</span><span class="sxs-lookup"><span data-stu-id="6facd-115">Accept terms and save the record.</span></span>  
> 6. <span data-ttu-id="6facd-116">Menu nagusian, hautatu **Project Service** > **Antolaketa-taula**.</span><span class="sxs-lookup"><span data-stu-id="6facd-116">On the main menu, select **Project Service** > **Schedule board**.</span></span> <span data-ttu-id="6facd-117">Han, erreserba-eskaera eskuz antolatzeko era ugari daude.</span><span class="sxs-lookup"><span data-stu-id="6facd-117">From here, there are several ways to manually schedule a booking requirement.</span></span> <span data-ttu-id="6facd-118">Aukeratu hoberen datorkizun metodoa.</span><span class="sxs-lookup"><span data-stu-id="6facd-118">Choose the method that works for you.</span></span>
  
## <a name="find-available-resources"></a><span data-ttu-id="6facd-119">Bilatu erabilgarri dauden baliabideak</span><span class="sxs-lookup"><span data-stu-id="6facd-119">Find available resources</span></span>

1.  <span data-ttu-id="6facd-120">**Erreserba-eskakizunak** zerrendan, sakatu eskuineko botoiarekin antolatu gabeko erreserba eta aukeratu aukera hauetako bat:</span><span class="sxs-lookup"><span data-stu-id="6facd-120">From the **Booking Requirement** list, right-click an unscheduled booking and choose one of the following:</span></span>  
  
- <span data-ttu-id="6facd-121">Aukeratu **Aurkitu erabilgarritasuna - Uneko baliabideak** erabilgarri dauden baliabideak aurkitzeko antolaketa-panelean erabilgarri dauden zerrendatik.</span><span class="sxs-lookup"><span data-stu-id="6facd-121">Choose **Find availability - Current Resources** to find an available resource from the list on the schedule board.</span></span>  
- <span data-ttu-id="6facd-122">Aukeratu **Aurkitu erabilgarritasuna - Uneko baliabideak** erabilgarri dauden baliabideak aurkitzeko sistemako baliabideetatik.</span><span class="sxs-lookup"><span data-stu-id="6facd-122">Choose **Find availability - All Resources**, to find an available resource from resources in the system</span></span>  
   > [!NOTE]
   >  <span data-ttu-id="6facd-123">Hori egitean, iragazkiek hautatutako erreserba-eskakizunen aukerak erakutsiko dira.</span><span class="sxs-lookup"><span data-stu-id="6facd-123">When you do this, the filters will show options for the selected booking requirement.</span></span>  
  
2. <span data-ttu-id="6facd-124">Libre dagoen tarte bat ikusten duzunean, sakatu eskuineko botoiarekin denbora-tartea antolaketa-panelean eta aukeratu **Erreserbatu hau**.</span><span class="sxs-lookup"><span data-stu-id="6facd-124">When you see an available slot, right-click the time slot on the schedule board and choose **Book Here**.</span></span> <span data-ttu-id="6facd-125">Bestela, arrastatu eta utzi erreserba-eskakizuna erabilgarri dagoen denbora-tartean.</span><span class="sxs-lookup"><span data-stu-id="6facd-125">Or, drag and drop the booking requirement to the available time slot.</span></span>  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a><span data-ttu-id="6facd-126">Eguneroko ikuspegia erabiliz baliabide erreserbatutako eta atalean-erreserbatuta dago zuen bilaketa</span><span class="sxs-lookup"><span data-stu-id="6facd-126">Book a resource using the daily view and find who’s under-booked</span></span>
  
1.  <span data-ttu-id="6facd-127">Antolaketat-taulan, hautatu **Ikuspegi modua** eta hautatu **Egunak**.</span><span class="sxs-lookup"><span data-stu-id="6facd-127">On the schedule board, select **View Mode** and select **Days**.</span></span>  
  
    <span data-ttu-id="6facd-128">Sareta-ikuspegia bat baliabideari eguna eta zein egunetan dira doako bakoitzeko booked ordu kopurua erakusten du.</span><span class="sxs-lookup"><span data-stu-id="6facd-128">This shows a grid view of how many hours a resource is booked per day and which days they are free.</span></span>  
  
2.  <span data-ttu-id="6facd-129">Sakatu erreserbatu nahi duzun baliabidearen izena eta hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="6facd-129">Click the name of the resource you want to book, and then select **Book**.</span></span>  
  
3.  <span data-ttu-id="6facd-130">**Baliabidearen erreserba (sortu)** elkarrizketa-koadroan, aukeratu erreserbatu nahi duzun proiektua, erreserba-metodoa eta hasiera- eta amaiera-orduak.</span><span class="sxs-lookup"><span data-stu-id="6facd-130">On the **Resource booking (create)** dialog box, choose the project that you want to book the resource for along with booking method and start and end times.</span></span>  
  
4.  <span data-ttu-id="6facd-131">Amaitutakoan, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="6facd-131">When you’re done, select **Book**.</span></span>  
  
## <a name="view-to-the-schedule-board"></a><span data-ttu-id="6facd-132">Ikusi antolaketa-taulan</span><span class="sxs-lookup"><span data-stu-id="6facd-132">View to the schedule board</span></span>
  
1.  <span data-ttu-id="6facd-133">Hautatu antolatu gabeko erreserba-eskaera beheko zerrendatik.</span><span class="sxs-lookup"><span data-stu-id="6facd-133">Select an unscheduled booking requirement from the list at the bottom.</span></span>  
  
2.  <span data-ttu-id="6facd-134">Arrastatu erreserba-eskaera erabilgarri dagoen antolaketa-taulako baliabide edo denbora-tarte batera.</span><span class="sxs-lookup"><span data-stu-id="6facd-134">Drag the booking requirement to an available resource/time slot on the schedule board.</span></span>  
  
3.  <span data-ttu-id="6facd-135">Amaitutakoan, hautatu **Erreserbatu**.</span><span class="sxs-lookup"><span data-stu-id="6facd-135">When you're done, select **Book**.</span></span>  
  
### <a name="additional-resources"></a><span data-ttu-id="6facd-136">Baliabide gehigarriak</span><span class="sxs-lookup"><span data-stu-id="6facd-136">Additional resources</span></span>  
 [<span data-ttu-id="6facd-137">Baliabide-kudeatzailearen gida</span><span class="sxs-lookup"><span data-stu-id="6facd-137">Resource manager guide</span></span>](../psa/resource-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]