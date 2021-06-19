---
title: Erreserbak vs. zereginak
description: Gai honek baliabideen erreserben eta baliabideen esleipenen arteko desberdintasunak eskaintzen ditu.
author: ruhercul
ms.date: 01/08/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3c1a1003af0b23c4be44fefac0b3c4ea725f96b2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012751"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="da1b3-103">Erreserbak vs. zereginak</span><span class="sxs-lookup"><span data-stu-id="da1b3-103">Bookings vs assignments</span></span>

<span data-ttu-id="da1b3-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="da1b3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="da1b3-105">Erreserbak proiektu batekiko baliabide baten behin behineko edo behin betiko esleipenak dira.</span><span class="sxs-lookup"><span data-stu-id="da1b3-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="da1b3-106">Behin betiko erreserbak baliabideen ahalmena kontsumitzen du.</span><span class="sxs-lookup"><span data-stu-id="da1b3-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="da1b3-107">Erreserbek taldeentzako antolakuntza kontzeptuak adierazten dituzte, baliabideak proiektu desberdinetan nola arituko diren ulertu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="da1b3-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="da1b3-108">Dynamics 365 Project Operations erreserbak proiektu mailako kontzeptutzat jotzen ditu.</span><span class="sxs-lookup"><span data-stu-id="da1b3-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="da1b3-109">Erreserbak ez bezala, esleipenak proiektuaren antolaketako proiektuaren zereginei esleitutako baliabideen esleipenak dira.</span><span class="sxs-lookup"><span data-stu-id="da1b3-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="da1b3-110">Baliabideak izendatu edo generikoak izan daitezke.</span><span class="sxs-lookup"><span data-stu-id="da1b3-110">The resources can be named or generic.</span></span>  <span data-ttu-id="da1b3-111">Proiektuaren zereginen esleipenetatik baliabide eskakizuna eratortzen denean, Project Operations-ek baliabideak esleitzeko ahaleginaren ingurunea erabiltzen dute baliabide eskakizunen xehetasunak eraikitzeko.</span><span class="sxs-lookup"><span data-stu-id="da1b3-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="da1b3-112">Hala ere, ez da baliabideen esleipenen erreferentzia mantentzen.</span><span class="sxs-lookup"><span data-stu-id="da1b3-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="da1b3-113">Baliabideen eskakizunetik eratorritako erreserben eguneratzeek ez dituzte baliabideen esleipenak eguneratzen.</span><span class="sxs-lookup"><span data-stu-id="da1b3-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="da1b3-114">Normalean, baliabide baten erreserben baturak baliabideen zereginen batura berdina izango da zeregin batean edo gehiagotan.</span><span class="sxs-lookup"><span data-stu-id="da1b3-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="da1b3-115">Hala ere, Project Operations-ek ez du hitzarmen hori betearazten.</span><span class="sxs-lookup"><span data-stu-id="da1b3-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="da1b3-116">**Kontziliazioa** ikuspegiak proiektu-kudeatzaileari baliabideen erreserbak eta esleipenak bat ez datozen tokiak erakusten dizkio.</span><span class="sxs-lookup"><span data-stu-id="da1b3-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]