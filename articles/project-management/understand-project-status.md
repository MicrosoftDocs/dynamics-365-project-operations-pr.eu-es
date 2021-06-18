---
title: Ulertu proiektuaren egoera
description: Gai honek proiektuetan esleitutako egoerari buruzko informazioa eskaintzen du Dynamics 365 Project Operations-en.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ad8c012b93bc65595dca33df1770562916c557e0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993401"
---
# <a name="understand-project-status"></a><span data-ttu-id="e7528-103">Ulertu proiektuaren egoera</span><span class="sxs-lookup"><span data-stu-id="e7528-103">Understand project status</span></span>

<span data-ttu-id="e7528-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="e7528-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="e7528-105">**Egoera** atala **Proiektuaren entitatea** orrialdeak kostuaren eta esfortzuaren arabera proiektu baten osasunaren laburpena eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="e7528-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="e7528-106">Egoeraren laburpen-eremuak</span><span class="sxs-lookup"><span data-stu-id="e7528-106">Status summary fields</span></span>

- <span data-ttu-id="e7528-107">**Proiektuaren egoera orokorra** eremua editagarria den eremua da, eta proiektuaren egoera orokorra erakusten du.</span><span class="sxs-lookup"><span data-stu-id="e7528-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="e7528-108">Kolore bidezko kodeketa erabiltzen du eremuak, hala nola berdea, horia eta gorria, arriskua handitzen dela adierazteko.</span><span class="sxs-lookup"><span data-stu-id="e7528-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="e7528-109">**Oharrak** eremuak proiektu-kudeatzaileari egoerari buruzko iruzkin zehatzak sartzen uzten dio.</span><span class="sxs-lookup"><span data-stu-id="e7528-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="e7528-110">**Egoeraren eguneratze-data** eremua ez da editagarria.</span><span class="sxs-lookup"><span data-stu-id="e7528-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="e7528-111">Eremu honetako balioa egoera azkenekoz noiz eguneratu zen adierazten duen denbora-marka da.</span><span class="sxs-lookup"><span data-stu-id="e7528-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="e7528-112">**Antolaketaren errendimendua** eta **Kostuen errendimendua** eremuak jarraipen-saretatik ezartzen dira.</span><span class="sxs-lookup"><span data-stu-id="e7528-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="e7528-113">Erro-nodoaren antolaketa eta kostuaren bariantza positiboak direnean **Ahaleginaren jarraipena** ikuspegian, eremu horiek **Aurreratua** gisa egunera ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="e7528-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="e7528-114">Erro-nukleoaren antolaketa eta kostuaren bariantza negatiboak direnean, eremu horiek **Atzeratuta** gisa ezartzen dira.</span><span class="sxs-lookup"><span data-stu-id="e7528-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]