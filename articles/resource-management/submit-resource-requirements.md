---
title: Bidali baliabide-eskaera bat
description: Sortutako baliabide-eskakizuna baliabide-eskaera gisa bidal dezakezu. Ondoren, eskaera baliabide-kudeatzaile bati bidaliko zaio, bete dezan.
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 94cf0f0d88e9be2522936b45122ed0037434d4f3
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070930"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="95e1a-104">Bidali baliabide-eskaera bat</span><span class="sxs-lookup"><span data-stu-id="95e1a-104">Submit a resource request</span></span>

<span data-ttu-id="95e1a-105">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="95e1a-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="95e1a-106">Sortutako baliabide-eskakizuna baliabide-eskaera gisa bidal dezakezu.</span><span class="sxs-lookup"><span data-stu-id="95e1a-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="95e1a-107">Ondoren, eskaera baliabide-kudeatzaile bati bidaliko zaio, bete dezan.</span><span class="sxs-lookup"><span data-stu-id="95e1a-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="95e1a-108">Dynamics 365 Project Operations-en, **Proiektuak** orrian, hautatu **Taldea** fitxan baliabide erreserbagarrien zerrenda ikusteko.</span><span class="sxs-lookup"><span data-stu-id="95e1a-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="95e1a-109">Hautatu zerrendatik baliabide-eskakizunen bat duen baliabide orokorra eta egin klik **Bidali eskaera** aukeran.</span><span class="sxs-lookup"><span data-stu-id="95e1a-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="95e1a-110">Taldekide orokorraren eskaera-egoerara aldatu egingo da **Bidalita** egoerara.</span><span class="sxs-lookup"><span data-stu-id="95e1a-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="95e1a-111">Eskaera bete ondoren, baliabide orokorra baliabide izendatu batekin ordezkatuko da baliabide-kudeatzaileak eskaera izendatutako baliabidearen erreserba eginez betetzen badu.</span><span class="sxs-lookup"><span data-stu-id="95e1a-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="95e1a-112">Bestela, baliabide-kudeatzaileak izendun baliabide bat proposatzen badu, baliabide orokorra taldean geratuko da eta eskaeraren egoera aldatu egingo da **Berrikusi behar da** egoerara.</span><span class="sxs-lookup"><span data-stu-id="95e1a-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>
