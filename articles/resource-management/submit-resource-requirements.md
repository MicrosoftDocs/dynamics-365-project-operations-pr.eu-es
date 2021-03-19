---
title: Bidali baliabide-eskaera bat
description: Sortutako baliabide-eskakizuna baliabide-eskaera gisa bidal dezakezu. Ondoren, eskaera baliabide-kudeatzaile bati bidaliko zaio, bete dezan.
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bc97af1ec90e60417c502eb329a85004e769e05b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279123"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="93b6b-104">Bidali baliabide-eskaera bat</span><span class="sxs-lookup"><span data-stu-id="93b6b-104">Submit a resource request</span></span>

<span data-ttu-id="93b6b-105">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="93b6b-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="93b6b-106">Sortutako baliabide-eskakizuna baliabide-eskaera gisa bidal dezakezu.</span><span class="sxs-lookup"><span data-stu-id="93b6b-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="93b6b-107">Ondoren, eskaera baliabide-kudeatzaile bati bidaliko zaio, bete dezan.</span><span class="sxs-lookup"><span data-stu-id="93b6b-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="93b6b-108">Dynamics 365 Project Operations-en (PSA), **Proiektuak** orrian, hautatu **Taldea** fitxan baliabide erreserbagarrien zerrenda ikusteko.</span><span class="sxs-lookup"><span data-stu-id="93b6b-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="93b6b-109">Hautatu zerrendatik baliabide-eskakizunen bat duen baliabide orokorra eta egin klik **Bidali eskaera** aukeran.</span><span class="sxs-lookup"><span data-stu-id="93b6b-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="93b6b-110">Taldekide orokorraren eskaera-egoerara aldatu egingo da **Bidalita** egoerara.</span><span class="sxs-lookup"><span data-stu-id="93b6b-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="93b6b-111">Eskaera bete ondoren, baliabide orokorra baliabide izendatu batekin ordezkatuko da baliabide-kudeatzaileak eskaera izendatutako baliabidearen erreserba eginez betetzen badu.</span><span class="sxs-lookup"><span data-stu-id="93b6b-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="93b6b-112">Bestela, baliabide-kudeatzaileak izendun baliabide bat proposatzen badu, baliabide orokorra taldean geratuko da eta eskaeraren egoera aldatu egingo da **Berrikusi behar da** egoerara.</span><span class="sxs-lookup"><span data-stu-id="93b6b-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]