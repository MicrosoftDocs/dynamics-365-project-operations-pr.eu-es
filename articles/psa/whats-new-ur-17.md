---
title: Project Service Automation eguneratzearen 17, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 17. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: bb93208217972639f91b39b7b6705d9897373ef7
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126783"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="cd8e6-103">Project Service Automation 17, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="cd8e6-103">Project Service Automation Update Release 17, V3</span></span>

<span data-ttu-id="cd8e6-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="cd8e6-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="cd8e6-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="cd8e6-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="cd8e6-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="cd8e6-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="cd8e6-109">Gai honek PSA V3, 17. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="cd8e6-110">Bertsio honek V3.10.6.34 konpilazio-zenbakia du eta, oro har, 2020ko martxoan jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="cd8e6-111">17. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="cd8e6-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="cd8e6-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="cd8e6-112">Bug fixes</span></span>

<span data-ttu-id="cd8e6-113">**Orokorra**</span><span class="sxs-lookup"><span data-stu-id="cd8e6-113">**General**</span></span>

- <span data-ttu-id="cd8e6-114">Konponduta: Project Service Automation eguneratu da Team Member lizentziak betearazteko (Proiektuen baliabide-guneak Taldekidea zerbitzu-planaren 3.x metadatuak ditu)</span><span class="sxs-lookup"><span data-stu-id="cd8e6-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="cd8e6-115">**Denbora eta gastua**</span><span class="sxs-lookup"><span data-stu-id="cd8e6-115">**Time and Expense**</span></span>

- <span data-ttu-id="cd8e6-116">Konponduta: ezin da gastuen aurreikuspen bat aldatu zerotik zero ez den zenbateko batera (0).</span><span class="sxs-lookup"><span data-stu-id="cd8e6-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="cd8e6-117">Aldaketa baztertu egin da.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-117">The change is ignored.</span></span>

<span data-ttu-id="cd8e6-118">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="cd8e6-118">**Project Management**</span></span>

- <span data-ttu-id="cd8e6-119">Konponduta: nuluak ez diren egiaztapenak gehitu dira taldekidearen posizioaren izenean.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="cd8e6-120">Konponduta: **msdyn_userresourceid** eremua zaharkitu egin da **msdyn_resourceassignment** entitatean.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="cd8e6-121">Konponduta: Bertsio berritu 2.x bertsiotik 3.x bertsiora ahalegin hutsalen ingeradak kudeatzeko zereginen esleipenetan.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="cd8e6-122">**Sales**</span><span class="sxs-lookup"><span data-stu-id="cd8e6-122">**Sales**</span></span>

- <span data-ttu-id="cd8e6-123">Konponduta: **Invoice.PreValidateInvoiceUpdate** parametroak berresleitutako erregistroaren jabeak ongi kudeatzen ditu orain.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="cd8e6-124">Konponduta: Transakzioaren klasea **Ordua** denean, **UnitGroup** ezin da editatu erakunde guztietan: **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail** eta **ContractLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-124">Fixed: When the transaction class is **Time**, **UnitGroup** is non-editable for all entities including, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, and **ContractLineDetails**.</span></span> <span data-ttu-id="cd8e6-125">Alabaina, **Unitatea** ez da editagarria **JournalLine** eta **InvoiceLineDetails** parametroetan soilik.</span><span class="sxs-lookup"><span data-stu-id="cd8e6-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>


