---
title: Erreserbak vs. zereginak
description: Gai honek baliabideen erreserben eta baliabideen esleipenen arteko desberdintasunak eskaintzen ditu.
author: ruhercul
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8fe6937dfdfe137f28917c16da1d7dc6155284ae
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130203"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="616fe-103">Erreserbak vs. zereginak</span><span class="sxs-lookup"><span data-stu-id="616fe-103">Bookings vs assignments</span></span>

<span data-ttu-id="616fe-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="616fe-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="616fe-105">Erreserbak proiektu batekiko baliabide baten behin behineko edo behin betiko esleipenak dira.</span><span class="sxs-lookup"><span data-stu-id="616fe-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="616fe-106">Behin betiko erreserbak baliabideen ahalmena kontsumitzen du.</span><span class="sxs-lookup"><span data-stu-id="616fe-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="616fe-107">Erreserbek taldeentzako antolakuntza kontzeptuak adierazten dituzte, baliabideak proiektu desberdinetan nola arituko diren ulertu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="616fe-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="616fe-108">Dynamics 365 Project Operations-ek erreserbak proiektu mailako kontzeptutzat hartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="616fe-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="616fe-109">Erreserbak ez bezala, esleipenak proiektuaren antolaketako proiektuaren zereginei esleitutako baliabideen esleipenak dira.</span><span class="sxs-lookup"><span data-stu-id="616fe-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="616fe-110">Baliabideak izendatu edo generikoak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="616fe-110">The resources can be named or generic.</span></span> 

<span data-ttu-id="616fe-111">Normalean, baliabide baten erreserben baturak baliabideen zereginen batura berdina izango da zeregin batean edo gehiagotan.</span><span class="sxs-lookup"><span data-stu-id="616fe-111">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="616fe-112">Hala ere, Project Operations-ek ez du hitzarmen hori betearazten.</span><span class="sxs-lookup"><span data-stu-id="616fe-112">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="616fe-113">**Kontziliazioa** ikuspegiak proiektu-kudeatzaileari baliabideen erreserbak eta esleipenak bat ez datozen tokiak erakusten dizkio.</span><span class="sxs-lookup"><span data-stu-id="616fe-113">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>
