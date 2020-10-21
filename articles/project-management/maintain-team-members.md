---
title: Kudeatu taldeko kideak
description: Gai honek proiektu taldeetara izena duten baliabideak erreserbatzeko eta hauek zereginetara esleitzeko informazioa eskaintzen du .
author: ruhercul
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: f5b36628e90896c9fe6570de71c95eab83a44ebd
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961809"
---
# <a name="maintain-team-members"></a><span data-ttu-id="08362-103">Kudeatu taldeko kideak</span><span class="sxs-lookup"><span data-stu-id="08362-103">Maintain team members</span></span>

<span data-ttu-id="08362-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="08362-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="08362-105">Proiektuko taldeari izendatutako baliabide bat gehi diezaiokezu zuzenean taldean erreserbatuz.</span><span class="sxs-lookup"><span data-stu-id="08362-105">You can add a named resource to your project team by booking them directly to the team.</span></span>

1. <span data-ttu-id="08362-106">Dynamics 365 Project Operations-en, joan **Proiektuak** atalera eta ireki erreserba egiten ari zaren proiektua.</span><span class="sxs-lookup"><span data-stu-id="08362-106">In Dynamics 365 Project Operations, go to **Projects**, and select the open the project that you're booking for.</span></span>
2. <span data-ttu-id="08362-107">**Proiektua** orrialdean **Taldea** fitxan, hautatu **Berria** aukeran.</span><span class="sxs-lookup"><span data-stu-id="08362-107">On the **Project** page, on the **Team** tab, select **New**.</span></span> 
3. <span data-ttu-id="08362-108">**Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroan, hautatu erreserbatzeko baliabidea.</span><span class="sxs-lookup"><span data-stu-id="08362-108">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="08362-109">**Funtzioa** eremua baliabidearen lehenetsitako funtzioarekin beteko da esleituta badago.</span><span class="sxs-lookup"><span data-stu-id="08362-109">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="08362-110">Funtzioa alda dezakezu.</span><span class="sxs-lookup"><span data-stu-id="08362-110">You can change the role.</span></span> 
4. <span data-ttu-id="08362-111">Aukeratu baliabidea beharko den hasiera eta amaiera datak eta hautatu baliabidearen ahalmena esleitzeko metodoa.</span><span class="sxs-lookup"><span data-stu-id="08362-111">Select the from and to dates that the resource will be needed, and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="08362-112">**Proiektu onartzailea**eremuan, hautatu **Bai**, taldekidea proiektuaren onartzailea izan dadin nahi baduzu.</span><span class="sxs-lookup"><span data-stu-id="08362-112">In the **Project Approver** field, select **Yes** if you want the team member to be a project approver.</span></span> <span data-ttu-id="08362-113">Taldekideak proiektu honetarako gastuak eta sarrerak onartzea onar dezakeela.</span><span class="sxs-lookup"><span data-stu-id="08362-113">The team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="08362-114">Sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="08362-114">Select **Save**.</span></span>

<span data-ttu-id="08362-115">Erreserbatutako baliabidea proiektuan zereginetara eslei dezakezu.</span><span class="sxs-lookup"><span data-stu-id="08362-115">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="08362-116">**Proiektua** orrialdean, **Antolaketa** fitxan, baliabide berriari zereginak esleitzeko.</span><span class="sxs-lookup"><span data-stu-id="08362-116">On the **Project** page, on the **Schedule** tab, assign tasks to the new resource.</span></span> <span data-ttu-id="08362-117">Zereginen sareko **Baliabideak** eremutik abian jarri den baliabide hautatzaileak hautatu ditzakezu taldekideak erakutsiko ditu.</span><span class="sxs-lookup"><span data-stu-id="08362-117">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>


<span data-ttu-id="08362-118">Project Operations-en, baliabideen erreserbak eta atazen esleipenak ez daude estu lotuta.</span><span class="sxs-lookup"><span data-stu-id="08362-118">In Project Operations, resource bookings and task assignments aren't tightly coupled.</span></span> <span data-ttu-id="08362-119">Baliabideen hautagailua antolaketan erabiltzen duzunean, taldekideei zereginak eslei diezazkiekeela proiektuan egindako erreserbek estaltzen dutena baino ordu gehiago.</span><span class="sxs-lookup"><span data-stu-id="08362-119">When you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>

<span data-ttu-id="08362-120">Taldekideen erreserben eta zereginen arteko desberdintasunak agertzen dira **Taldea** eta **Baliabideen bateratzea** fitxak.</span><span class="sxs-lookup"><span data-stu-id="08362-120">The differences between team member bookings and assignments are shown on the **Team** and **Resource Reconciliation** tabs.</span></span> <span data-ttu-id="08362-121">Baliabideen erreserben eta zereginen arteko aldeak maila zehatzagoan bateratu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="08362-121">You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

<span data-ttu-id="08362-122">Erabili baliabide hautagailua **Antolaketa** fitxan, proiektuko parte ez diren baliabideak bilatu eta hautatzeko.</span><span class="sxs-lookup"><span data-stu-id="08362-122">Use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="08362-123">Baliabide horiek baliabide-hautatzailean agertzen dira **Bestelako baliabideak** moduan.</span><span class="sxs-lookup"><span data-stu-id="08362-123">These resources are shown in the resource picker as **Other Resources**.</span></span>

<span data-ttu-id="08362-124">Hautapena egiten duzunean, baliabidea proiektuko taldeari gehitu eta zereginari esleitzen zaio, baina ez da erreserbarik sortzen.</span><span class="sxs-lookup"><span data-stu-id="08362-124">When you make a selection, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

<span data-ttu-id="08362-125">**Berdinkatzea** fitxaren luzatzeko erreserba gaitasuna erabil dezakezu edo **Antolaketa-panela** aukera baliabidearen gaitasuna proiektua erreserbatzeko.</span><span class="sxs-lookup"><span data-stu-id="08362-125">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

<span data-ttu-id="08362-126">Taldekide bat zure proiektuan erreserbatu ondoren, **Mantendu erreserbak** edo **Antolaketa-panela** erabil dezakezu erreserbak kudeatzeko.</span><span class="sxs-lookup"><span data-stu-id="08362-126">After a team member is booked on your project, you can use **Maintain bookings** or the **Schedule Board** directly to manage their bookings.</span></span>
