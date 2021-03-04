---
title: Behin behineko erreserba-eskakizunak
description: Gai honek baliabide-eskakizunak behin behineko erreserbak egiteari buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 09f7acb95be014034cc03d7eed9d37363d430601
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147368"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="b9124-103">Behin behineko erreserba-eskakizunak</span><span class="sxs-lookup"><span data-stu-id="b9124-103">Soft-book requirements</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b9124-104">Baldiabide-eskaera bat behin betiko erreserbatu daiteke</span><span class="sxs-lookup"><span data-stu-id="b9124-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="b9124-105">Behin betiko erreserbak baliabideen ahalmena kontsumitzen duen proposamena sortzen du.</span><span class="sxs-lookup"><span data-stu-id="b9124-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="b9124-106">Proposamena eskatzaileari igortzen zaio onar dezan.</span><span class="sxs-lookup"><span data-stu-id="b9124-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="b9124-107">Behin behineko erreserba batek baliabidea gehitzen du proiektu-taldean eta egoera desberdina du antolaketa-panelean, baina ez du baliabidearen ahalmena kontsumitzen.</span><span class="sxs-lookup"><span data-stu-id="b9124-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="b9124-108">Antolaketa-paneletik baliabide baten behin behineko erreserba egiteko, ezarri **Erreserbaren egoera** eremua **Behin behinekoa** gisa.</span><span class="sxs-lookup"><span data-stu-id="b9124-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

![Erreserbaren egoera "behin behineko" gisa ezarrita dago](media/Resource-Management-image77.png)

<span data-ttu-id="b9124-110">**Taldea** fitxa **Taldekide izendatuak** ikuspegian dagoenean, baliabidea bertan agertzen da.</span><span class="sxs-lookup"><span data-stu-id="b9124-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="b9124-111">Behin-behinean erreserbatutako orduak **Behin-behinean erreserbatutako orduak** zutabean agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="b9124-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

![Behin-behinean erreserbatutako orduak izendatutako taldekideen ikuspegian](media/Resource-Management-image78.png)

<span data-ttu-id="b9124-113">Behin-behinean erreserbatutako taldekideak zereginetara esleitu daitezke.</span><span class="sxs-lookup"><span data-stu-id="b9124-113">Soft-booked team members can be assigned to tasks.</span></span>

![Behin-behinean erreserbatutako taldekideak zereginetara esleitu dira.](media/Resource-Management-image79.png)

<span data-ttu-id="b9124-115">**Kontziliazioa** fitxan, ez da erreserbarik irakurtzen behin behinean erreserbatutako baliabidetarako, izan ere, **Kontziliazioa** fitxak behin betiko erreserbak baino ez ditu hartzen.</span><span class="sxs-lookup"><span data-stu-id="b9124-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![Erreserbarik ez duten behin behinean erreserbatutako baliabideak Kontziliazioa fitxan](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="b9124-117">Ezin duzu taldike orokor batetik sortutako eskakizun bateko baliabide bat behin behinean erreserbatu.</span><span class="sxs-lookup"><span data-stu-id="b9124-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="b9124-118">Antolaketa-panelean, kolore ezberdina erabiltzen da baliabideen behin behineko erreserbetarako.</span><span class="sxs-lookup"><span data-stu-id="b9124-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![Behin behineko erreserbak antolaketa-panelean](media/Resource-Management-image81.png)

<span data-ttu-id="b9124-120">Behin behineko erreserba behin betiko erreserba bihurtzeko, antolaketa-panelean egin klik eskuineko botoiarekin behin behineko erreserban, eta hautatu **Aldatu egoera** \> **Behin betiko erreserba** \> **Behin betikoa**.</span><span class="sxs-lookup"><span data-stu-id="b9124-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![Erreserba egoera behin betikora aldatzea](media/Resource-Management-image82.png)

<span data-ttu-id="b9124-122">Erreserba aldatzean, egoera aldatu egingo da antolaketa-panelean.</span><span class="sxs-lookup"><span data-stu-id="b9124-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="b9124-123">Erreserbaren egoera orain **Behin betikoa** denez, baliabidea erreserbatuta agertzen da, eta haren ahalmena eta erabilgarritasuna egokitu egiten dira.</span><span class="sxs-lookup"><span data-stu-id="b9124-123">Because the booking status is now **Hard**, the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="b9124-124">Behin betiko erreserba edo behin behineko erreserba bertan behera uzteko metodo bera erabil dezakezu antolaketa-paneletik.</span><span class="sxs-lookup"><span data-stu-id="b9124-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="b9124-125">Proiektuaren **Taldea** fitxan dagoen baliabide bat behin behineko erreserba behin betiko bihurtzeko, hautatu baliabidea eta, ondoren, hautatu **Berretsi**.</span><span class="sxs-lookup"><span data-stu-id="b9124-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![Berretsi komandoa](media/Resource-Management-image83.png)
