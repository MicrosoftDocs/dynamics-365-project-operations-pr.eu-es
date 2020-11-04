---
title: Erreserbak vs. zereginak
description: Gai honek baliabideen erreserben eta baliabideen esleipenen arteko desberdintasunak eskaintzen ditu.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fa99783e52dbcdeaf80bbfd03df0f458f86b5e99
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070885"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="c6ea9-103">Erreserbak vs. zereginak</span><span class="sxs-lookup"><span data-stu-id="c6ea9-103">Bookings vs assignments</span></span>

<span data-ttu-id="c6ea9-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="c6ea9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c6ea9-105">Erreserbak proiektu batekiko baliabide baten behin behineko edo behin betiko esleipenak dira.</span><span class="sxs-lookup"><span data-stu-id="c6ea9-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="c6ea9-106">Behin betiko erreserbak baliabideen ahalmena kontsumitzen du.</span><span class="sxs-lookup"><span data-stu-id="c6ea9-106">Hard bookings consume a resource's capacity.</span></span> 

<span data-ttu-id="c6ea9-107">Esleipenak proiektuaren antolaketako proiektuaren zereginei esleitutako baliabideen esleipenak dira.</span><span class="sxs-lookup"><span data-stu-id="c6ea9-107">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="c6ea9-108">Baliabideak benetakoak edo orokorrak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="c6ea9-108">The resources can be real or generic.</span></span> 

<span data-ttu-id="c6ea9-109">Egokiena, benetako baliabideetarako, erreserbak eta zereginak ados egotea izango litzateke, ez baitira desberdinak.</span><span class="sxs-lookup"><span data-stu-id="c6ea9-109">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="c6ea9-110">Hala ere, Microsoft Dynamics Project Operations-ek ez du hitzarmen hori betearazten.</span><span class="sxs-lookup"><span data-stu-id="c6ea9-110">However, Microsoft Dynamics Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="c6ea9-111">**Kontziliazioa** ikuspegiak proiektu-kudeatzaileari baliabideen erreserbak eta esleipenak bat ez datozen tokiak erakusten dizkio.</span><span class="sxs-lookup"><span data-stu-id="c6ea9-111">The **Reconciliation** view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>
