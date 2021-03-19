---
title: Baliabide-eskakizun orokorrak betetzea
description: Gai honek baliabide generikoen eskakizunetarako izendatutako baliabideei buruzko informazioa eskaintzen du.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fef896ae12c196d5566ad54f3e15373020e4e28a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279573"
---
# <a name="generic-resource-requirement-fulfillment"></a><span data-ttu-id="ffb5f-103">Baliabide-eskakizun orokorrak betetzea</span><span class="sxs-lookup"><span data-stu-id="ffb5f-103">Generic resource requirement fulfillment</span></span>

<span data-ttu-id="ffb5f-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="ffb5f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ffb5f-105">Izena duen baliabide bat erreserbatu dezakezu baliabide.eskakizuna duten baliabide generikoak ordezkatzeko.baliabide</span><span class="sxs-lookup"><span data-stu-id="ffb5f-105">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="ffb5f-106">**Proiektuak** orrian, hautatu **Taldea** fitxa.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-106">On the **Projects** page, select the **Team** tab.</span></span>
2. <span data-ttu-id="ffb5f-107">Hautatu zerrendatik baliabide-eskakizunen bat duen baliabide orokorra eta hautatu **Erreserbatu** aukeran.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-107">Select the generic resource that has a resource requirement from the list, and then select **Book**.</span></span> <span data-ttu-id="ffb5f-108">Edo ireki baliabide-eskakizuna eta hautatu **Erreserbatu** aukeran.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-108">Or, open the resource requirement and then select **Book**.</span></span>
3. <span data-ttu-id="ffb5f-109">**Antolaketa-laguntzailea** orrialdean, hautatu izena duen baliabidea proiektu taldean erreserbatzeko eta hautatu **Erreserbatu** aukeran.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then select **Book**.</span></span>

<span data-ttu-id="ffb5f-110">Erreserba izena duen baliabide batek osatu eta betetzen duenean, baliabide generikoa izena duen baliabidearen bidez ordezkatuko da.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-110">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

<span data-ttu-id="ffb5f-111">Antolaketako zereginak izena duen baliabidearekin ere eguneratzen dira.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-111">The assignments on the schedule are updated with the named resource as well.</span></span>

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="ffb5f-112">Bete baliabide generikoa izena duten hainbat baliabiderekin</span><span class="sxs-lookup"><span data-stu-id="ffb5f-112">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="ffb5f-113">Baliabide generiko baten eskakizuna izena duten hainbat baliabiderekin betetzea, izena duen baliabide bakarra esleitzearen antzekoa da.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-113">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="ffb5f-114">Adibidez, bost eguneko eta 120 orduko iraupena duen zeregina dago.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-114">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="ffb5f-115">Zeregin hau ezin du bost eguneko astean zehar zortzi orduko lanordu tipikoa lantzen duen baliabide batek osatu.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-115">This task can't be completed by one resource that works a typical eight-hour day over a five-day week.</span></span> 

<span data-ttu-id="ffb5f-116">Eskakizuna 120 egunetan robotikako ingeniaritza bost egunetan zehar egiteko da, hau da, eguneko 24 ordukoa.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-116">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

<span data-ttu-id="ffb5f-117">Izena duten hainbat baliabide behar direnean eskaera generiko bat betetzeko adibidea.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-117">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="ffb5f-118">Baliabide ugari erreserbatu beharko dituzu baldintza betetzeko.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-118">You will need to book multiple resources to fulfill the requirement.</span></span>

<span data-ttu-id="ffb5f-119">Gertaera honen alderik nagusia baliabide generikoa zereginari esleitutako taldean geratzen dela da, eta erreserbatutako izena duten taldekideak ez dira karguaren zati gisa esleitzen.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-119">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="ffb5f-120">Proiektuaren zuzendariak lana izena duten baliabideei egoki eman diezaieke.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-120">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="ffb5f-121">The **Kontziliazioa** ikuspegiak lagun diezaioke proiektuaren kudeatzaileari zereginak burutzeko baliabide ugaritan erreserbak hausten.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-121">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="ffb5f-122">Hori ez da automatikoki egiten, aurreko adibide soilak baino konplikatuagoa den edozein agertokitan, esaterako, eskakizuna osatzen duen zeregin-sorta bat daukazunean edo sistemak proiektuak bere gain hartu nahi duen asmoa.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-122">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement or the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="ffb5f-123">Sistemak ezin duenez ulertu helburua, posible da suposizioak aurreikusitakoengandik desberdinak izatea eta aurreikusitako emaitza okerra edo aurreikusi ezin dena gertatuko dela.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-123">Because the system can't understand intent, it's likely that the assumptions will be different than intended and an incorrect or unpredictable result will occur.</span></span> <span data-ttu-id="ffb5f-124">Aurreikus daitekeen emaitza baliabide generikoa esleituta mantentzen dela da proiektuaren kudeatzaileak nahitaez zereginak sortu arte, programaren **Kontziliazioa** ikuspegiaren laguntzarekin.</span><span class="sxs-lookup"><span data-stu-id="ffb5f-124">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]