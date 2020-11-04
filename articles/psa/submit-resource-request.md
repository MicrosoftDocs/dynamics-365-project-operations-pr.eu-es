---
title: Baliabide-eskaera bat bidaltzen
description: Gai honek proiektuko baliabideen eskaera bidaltzeari buruzko informazioa ematen du.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: bcea3d640d7e9ee2b071c55bff9ade3268edb319
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071129"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="dff4f-103">Baliabide-eskaera bat bidaltzen</span><span class="sxs-lookup"><span data-stu-id="dff4f-103">Submitting a resource request</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="dff4f-104">Sortutako baliabide-eskakizuna baliabide-eskaera gisa bidal dezakezu.</span><span class="sxs-lookup"><span data-stu-id="dff4f-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="dff4f-105">Ondoren, eskaera baliabide-kudeatzaile bati bidaliko zaio, bete dezan.</span><span class="sxs-lookup"><span data-stu-id="dff4f-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="dff4f-106">Project Service Automation-en (PSA), **Proiektuak** orrian, egin klik **Taldea** fitxan baliabide erreserbagarrien zerrenda ikusteko.</span><span class="sxs-lookup"><span data-stu-id="dff4f-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="dff4f-107">Hautatu zerrendatik baliabide-eskakizunen bat duen baliabide orokorra eta egin klik **Bidali eskaera** aukeran.</span><span class="sxs-lookup"><span data-stu-id="dff4f-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![Baliabide-eskaera bat bidaltzen](media/RM-how-to-18.png)

<span data-ttu-id="dff4f-109">Taldekide orokorraren eskaera-egoerara aldatu egingo da **Bidalita** egoerara.</span><span class="sxs-lookup"><span data-stu-id="dff4f-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="dff4f-110">Baliabide-kudeatzaileak eskaera bete ondoren, baliabide orokorra baliabide izendatu batekin ordezkatuko da baliabide-kudeatzaileak eskaera izendatutako baliabidearen erreserba eginez betetzen badu.</span><span class="sxs-lookup"><span data-stu-id="dff4f-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="dff4f-111">Bestela, baliabide orokorra taldean geratuko da eta eskaeraren egoera aldatu egingo da **Berrikusi behar da** egoerara, baliabide-kudeatzaileak izendatutako baliabidea proposatu badu.</span><span class="sxs-lookup"><span data-stu-id="dff4f-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review** , if the resource manager has proposed a named resource.</span></span>
