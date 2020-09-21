---
title: Konfiguratu baliabide-funtzioak
description: Nola konfiguratu baliabideen funtzioak Project Service-n
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0a180069-17d9-40fd-b4af-9b8d50f373ea
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 6a32ec4380e847b897931b6691fa8f9784d0cee7
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748829"
---
# <a name="configure-resource-roles-project-service"></a><span data-ttu-id="ca754-103">Konfiguratu baliabideen funtzioak (Project Service)</span><span class="sxs-lookup"><span data-stu-id="ca754-103">Configure resource roles (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="ca754-104">Funtzioak garrantzitsu dira proiektuen plangintza egitean, baliabideen eskakizunak edo proiektuen kostuak zehaztean.</span><span class="sxs-lookup"><span data-stu-id="ca754-104">Roles play an important part in project planning, when determining resource requirements or costs of a project.</span></span> <span data-ttu-id="ca754-105">Zure proiektuek behar dituzten funtzio bakoitzerako, baliabide-funtzio bat sortu eta abileziak eta gaitasunak lotu behar dizkiozu funtzio horri.</span><span class="sxs-lookup"><span data-stu-id="ca754-105">For each role your projects require, you need to create a resource role and associate skills and proficiencies to that role.</span></span> <span data-ttu-id="ca754-106">Adibidez, baliteke funtzioak sortu nahi izatea garatzailerako, proiektu-kudeatzailerako edo joko-probatzailerako.</span><span class="sxs-lookup"><span data-stu-id="ca754-106">For example, you might want to create roles for developer, project manager, or game tester.</span></span> <span data-ttu-id="ca754-107">Funtzio horretarako abilezia- eta gaitasun-mailak ere ezarriko dituzu.</span><span class="sxs-lookup"><span data-stu-id="ca754-107">You’ll also set the skills and proficiency levels required for the role.</span></span>  
  
 <span data-ttu-id="ca754-108">Konfiguratu baliabide-funtzioak, zure erakundearen gutxi goraberako proiektuaren eragina ziurtatzeko.</span><span class="sxs-lookup"><span data-stu-id="ca754-108">Configure resource roles to ensure effective project estimation for your organization.</span></span>  <span data-ttu-id="ca754-109">Gainera, ziurtatu zehatz ezartzen duzula fakturazio mota.</span><span class="sxs-lookup"><span data-stu-id="ca754-109">Also make sure you accurately set the billing type.</span></span> <span data-ttu-id="ca754-110">Kobratzen ez den fakturazio mota gisa ezarritako elementuak ez dira erakutsiko kontratuaren edo eskaintzaren lineetan.</span><span class="sxs-lookup"><span data-stu-id="ca754-110">An item set with a non-chargeable billing type doesn’t show up on contract or quote lines.</span></span>  
  
 <span data-ttu-id="ca754-111">Baliabide-funtzioak konfiguratu ostean, kostu- eta salmenta-prezioak konfigura ditzakezu prezio-zerrendarekin.</span><span class="sxs-lookup"><span data-stu-id="ca754-111">Once you’ve set up resource roles, you can set up cost and sales prices with a price list.</span></span>  
  
 <span data-ttu-id="ca754-112">Gehitu nahi duzun funtzio bakoitzerako, egin hau:</span><span class="sxs-lookup"><span data-stu-id="ca754-112">For each role you want to add, do the following:</span></span>  
  
1.  <span data-ttu-id="ca754-113">Joan **Project Service > Baliabideen funtzioak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="ca754-113">Go to **Project Service > Resource Roles**.</span></span>  
  
2.  <span data-ttu-id="ca754-114">Sakatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="ca754-114">Click **New**.</span></span>  
  
3.  <span data-ttu-id="ca754-115">**Orokorra** eremuan, adierazi funtzioaren izena **Izena** eremuan eta, ondoren, bete gainerako eremuak, behar diren bezala.</span><span class="sxs-lookup"><span data-stu-id="ca754-115">In the **General** area, enter a name for the role in **Name**, and then fill in the other fields as necessary.</span></span>  
  
4.  <span data-ttu-id="ca754-116">Sakatu **Gorde**, erregistroa sortzeko, editatzen jarraitu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="ca754-116">Click **Save** to create the record so you can continue editing it.</span></span>  
  
5.  <span data-ttu-id="ca754-117">**Abileziak** sekzioak, sakatu **+** abilezia gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="ca754-117">In the **Skills** area, click **+** to add a skill.</span></span>  
  
6.  <span data-ttu-id="ca754-118">**Funtzio-lehiakortasunaren eskakizuna** panelean, sakatu- **Trebezia** eremua, sakatu  **Bilaketa** botoia eta, ondoren, hautatu trebezia bat.</span><span class="sxs-lookup"><span data-stu-id="ca754-118">In the **Role competency requirement** pane, click in the **Skill** field, click the **Search** button, and then select a skill.</span></span>  
  
7.  <span data-ttu-id="ca754-119">Hautatu trebezia horren gaitasun bat eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="ca754-119">Select a proficiency for that skill, and then click **Save**.</span></span>  
  
8.  <span data-ttu-id="ca754-120">Jarraitu behar diren trebezia guztiak gehitzen.</span><span class="sxs-lookup"><span data-stu-id="ca754-120">Continue adding skills as necessary.</span></span> <span data-ttu-id="ca754-121">Amaitzean, sakatu **Gorde** pantailaren behe-eskuineko izkinan.</span><span class="sxs-lookup"><span data-stu-id="ca754-121">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
9. <span data-ttu-id="ca754-122">Baliabide-funtzio hau erabilgarri egiteko proiektuetarako, sakatu **Aktibatu**.</span><span class="sxs-lookup"><span data-stu-id="ca754-122">To make this resource role available for projects to use, click **Activate**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="ca754-123">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="ca754-123">See Also</span></span>  
 [<span data-ttu-id="ca754-124">Baliabideak konfiguratu</span><span class="sxs-lookup"><span data-stu-id="ca754-124">Set up resources</span></span>](../project-service/set-up-resources.md)
