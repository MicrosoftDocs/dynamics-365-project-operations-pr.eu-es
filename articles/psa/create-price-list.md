---
title: Sortu prezio-zerrenda
description: Nola sortu prezio-zerrenda Project Service-n
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 32f0cc66d1caa08bd24eb232338444df0388de3f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006046"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="fee8a-103">Sortu prezio-zerrenda (Project Service)</span><span class="sxs-lookup"><span data-stu-id="fee8a-103">Create a price list (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="fee8a-104">Prezio-zerrendek eskaintzak eta proiektuak sortzeko kontu-kudeatzaileek erabil ditzaketen txantiloiak ematen dituzte, eta proiektuaren kostuak ezartzeko balia ditzakete.</span><span class="sxs-lookup"><span data-stu-id="fee8a-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="fee8a-105">Funtzioen eta gastuen lerro-elementuen zerrenda bat ematen dute, baita bakoitzaren prezioa ere.</span><span class="sxs-lookup"><span data-stu-id="fee8a-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="fee8a-106">Prezio-zerrenda ugari sor ditzakezu hainbat bezero-segmentu edo salmenta-kanalen prezio-egitura bereiziak mantendu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="fee8a-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="fee8a-107">Bezeroei kobratuko diezun moneta bakoitzerako prezio-zerrenda bat sortzea gomendatzen da.</span><span class="sxs-lookup"><span data-stu-id="fee8a-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="fee8a-108">Banatuko den lana bakoitzerako gutxi gorabeherako finantza-gastuak sortzeko, ziurtatu proiektu bakoitzak kostu bat eta salmentako prezio-zerrenda bat duela.</span><span class="sxs-lookup"><span data-stu-id="fee8a-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="fee8a-109">Konfiguratu kostuen eta salmenten prezio-zerrenda lehenetsia, zure erakundean sortutako proiektu guztiei aplikatuko zaiena.</span><span class="sxs-lookup"><span data-stu-id="fee8a-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="fee8a-110">Prezio-zerrendak funtzioen eta gastuen kategorietan oinarritzen dira, eta beraz, prezio-zerrenda bat sortu baino lehen, ziurtatu dagoeneko konfiguratu dituzula prezio-zerrenda sortzen ari zaren bitartean erabili nahi dituzun funtzioak eta gastu-kategoriak.</span><span class="sxs-lookup"><span data-stu-id="fee8a-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="fee8a-111">Joan **Project Service > Prezio-zerrendak**.</span><span class="sxs-lookup"><span data-stu-id="fee8a-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="fee8a-112">Sakatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="fee8a-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="fee8a-113">**Testuingurua** aukeran, hautatu prezio-zerrenda **Kostua**, **Erosketa** edo **Salmenta** ekintzarako den.</span><span class="sxs-lookup"><span data-stu-id="fee8a-113">In **Context**, select whether this price list is for **Cost**, **Purchase**, or **Sales**.</span></span>  
  
4.  <span data-ttu-id="fee8a-114">**Izena** aukeran, idatzi prezio-zerrendaren izena.</span><span class="sxs-lookup"><span data-stu-id="fee8a-114">In **Name**, enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="fee8a-115">**Moneta** aukeran, hautatu fakturatzeko edo kostu gisa erabiliko duzun moneta.</span><span class="sxs-lookup"><span data-stu-id="fee8a-115">In **Currency**, select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="fee8a-116">**Denbora-unitatea** aukeran, zehaztu prezioa aplikatzen den denbora-tartea, eguna edo ordua, esaterako.</span><span class="sxs-lookup"><span data-stu-id="fee8a-116">In **Time Unit**, specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="fee8a-117">Bete **Hasiera-data**, **Amaiera-data** eta **Azalpena** eremuak.</span><span class="sxs-lookup"><span data-stu-id="fee8a-117">Fill in the **Start Date**, **End Date**, and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="fee8a-118">Sakatu **Gorde**, erregistroa sortzeko, editatzen jarraitu ahal izateko.</span><span class="sxs-lookup"><span data-stu-id="fee8a-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="fee8a-119">Prezio-zerrendari funtzio-prezio bat gehitzeko, sakatu **+** **Funtzio-prezioak** aukeran.</span><span class="sxs-lookup"><span data-stu-id="fee8a-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="fee8a-120">**Funtzio-prezioa** panelean, bete zehaztasunak eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="fee8a-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="fee8a-121">Jarraitu behar diren funtzio-prezioak gehitzen.</span><span class="sxs-lookup"><span data-stu-id="fee8a-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="fee8a-122">Amaitzean, sakatu **Gorde** pantailaren behe-eskuineko izkinan.</span><span class="sxs-lookup"><span data-stu-id="fee8a-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="fee8a-123">Prezio-zerrendari gastuen kategoriako prezio bat gehitzeko, sakatu **+** **Kategoria-prezioak** aukeran.</span><span class="sxs-lookup"><span data-stu-id="fee8a-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="fee8a-124">**Transakzio-kategoriaren prezioa** panelean, bete zehaztasunak eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="fee8a-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="fee8a-125">Jarraitu behar diren kategoria-prezioak gehitzen.</span><span class="sxs-lookup"><span data-stu-id="fee8a-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="fee8a-126">Amaitzean, sakatu **Gorde** pantailaren behe-eskuineko izkinan.</span><span class="sxs-lookup"><span data-stu-id="fee8a-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="fee8a-127">Prezio-zerrendan prezio-zerrendako elementuak gehitzeko, sakatu **+** **Prezio-zerrendako elementuak** atalean.</span><span class="sxs-lookup"><span data-stu-id="fee8a-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="fee8a-128">**Prezio-zerrendako elementuak** panelean, bete zehaztasunak eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="fee8a-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="fee8a-129">Jarraitu behar diren prezio-zerrendako elementuak gehitzen.</span><span class="sxs-lookup"><span data-stu-id="fee8a-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="fee8a-130">Amaitzean, sakatu **Gorde** pantailaren behe-eskuineko izkinan.</span><span class="sxs-lookup"><span data-stu-id="fee8a-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="fee8a-131">Prezio-zerrendan lurralde-erlazioak gehitzeko, sakatu **+** **Lurralde-erlazioak** aukeran.</span><span class="sxs-lookup"><span data-stu-id="fee8a-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="fee8a-132">**Konexio berria** leihoan, bete zehaztasunak eta, ondoren, sakatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="fee8a-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="fee8a-133">Jarraitu behar diren lurralde-erlazioak gehitzen.</span><span class="sxs-lookup"><span data-stu-id="fee8a-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="fee8a-134">Amaitzean, sakatu **Gorde** pantailaren behe-eskuineko izkinan.</span><span class="sxs-lookup"><span data-stu-id="fee8a-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="fee8a-135">Ikusi baita ere</span><span class="sxs-lookup"><span data-stu-id="fee8a-135">See Also</span></span>  
 [<span data-ttu-id="fee8a-136">Konfiguratu Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="fee8a-136">Configure Project Service Automation</span></span>](../psa/configure.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]