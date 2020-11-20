---
title: Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko
description: Gai honek prezio-dimentsioetarako plugin atributuak eguneratzeko informazioa eskaintzen du.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: project-operations
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: c42e5fda79d51430f4dedf46037e11c86a38c474
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121833"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="f0a99-103">Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko</span><span class="sxs-lookup"><span data-stu-id="f0a99-103">Update plug-in attributes to include new pricing dimensions</span></span>

> [!NOTE]
> <span data-ttu-id="f0a99-104">Project Service Automation-en (PSA) Aurrekontua eta Kontratazioa eginbidea erabiltzen ari ez bazara, gai hau salta dezakezu.</span><span class="sxs-lookup"><span data-stu-id="f0a99-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="f0a99-105">Gai honek honako gai hauetan azaldutako prozedurak bete dituzula suposatzen du: [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities.md), [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan](field-references.md), eta [Ezarri eremu pertsonalizatuak prezioen dimentsio gisa](set-up-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="f0a99-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="f0a99-106">Prozedura horiek bete ez badituzu, itzuli, bete itzazu eta, ondoren, itzuli gai honetara.</span><span class="sxs-lookup"><span data-stu-id="f0a99-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="f0a99-107">Eskaintzaren lerroaren xehetasunak sortzen direnean **Eskaintzaren lerroa** orrialdean proiektu baten eskaintzaren lerro baterako, sistemak bi estimazio lerro sortzen ditu atzeko planoan: lerro bat kostuen aldeko estimaziorako eta, bestea, salmenten aldeko estimaziorako.</span><span class="sxs-lookup"><span data-stu-id="f0a99-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="f0a99-108">Gauza bera gertatzen da proiektuaren kontratuaren lerroarekin.</span><span class="sxs-lookup"><span data-stu-id="f0a99-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="f0a99-109">Kostuaren aldeko kopuruari edo eremuari aldaketaren bat egiten diozunean, aldaketa hori salmenten aldera hedatzen da.</span><span class="sxs-lookup"><span data-stu-id="f0a99-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="f0a99-110">Jarraian agertzen diren pluginen ondorioz gertatzen da hori, zeina berriro erregistratu behar den prezio-dimentsioei aldaketaren bat egin ondoren.</span><span class="sxs-lookup"><span data-stu-id="f0a99-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="f0a99-111">PreOperationContractLineDetailUpdate - Eguneratzeak **msdyn_orderlinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="f0a99-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="f0a99-112">PreOperationQuoteLineDetailUpdate - Eguneratzeak **msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="f0a99-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="f0a99-113">Hurrengo urratsek pluginak erregistratzeko prozesua azaltzen dute.</span><span class="sxs-lookup"><span data-stu-id="f0a99-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="f0a99-114">Ireki **PluginRegistrationTool** eta konektatu zure lineako instantziara.</span><span class="sxs-lookup"><span data-stu-id="f0a99-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="f0a99-115">Egin klik **Bilatu** aukeran eta bilatu eguneratu behar den plugina.</span><span class="sxs-lookup"><span data-stu-id="f0a99-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![Bilaketa zuhaitzaren pantaila-argazkia](media/PRT-1.png)

3. <span data-ttu-id="f0a99-117">Plugina aurkitu ondoren, hautatu eta egin klik **Hautatu Inprimaki nagusian**.</span><span class="sxs-lookup"><span data-stu-id="f0a99-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="f0a99-118">Hautatu eguneratu beharreko pluginaren urratsa, egin klik eskuineko botoiarekin eta, ondoren, hautatu **Eguneratu**.</span><span class="sxs-lookup"><span data-stu-id="f0a99-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![Eguneratu beharreko pluginaren pantaila-argazkia](media/PRT-2.png)
 
5. <span data-ttu-id="f0a99-120">Eguneratze leihoan, sakatu elipsia (**...**) iragazkiaren atributuetan.</span><span class="sxs-lookup"><span data-stu-id="f0a99-120">In the update window, click the ellipsis (**...**) in the filtering attributes.</span></span>

 ![Eguneratzeko lehendik dagoen urratsaren konfigurazioaren informazioa](media/PRT-3.png)
 
6. <span data-ttu-id="f0a99-122">Hautatu prezioaren atributuaren kontrol-laukiak.</span><span class="sxs-lookup"><span data-stu-id="f0a99-122">Select the pricing attribute check boxes.</span></span>

 ![Prezio-atributuetarako kontrol-laukien hautaketa erakusten duen pantaila-argazkia](media/PRT-4.png)

7. <span data-ttu-id="f0a99-124">Egin klik **Ados** aukeran orria ixteko eta, ondoren, hautatu **Eguneratu urratsa**.</span><span class="sxs-lookup"><span data-stu-id="f0a99-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 !["Eguneratu urratsa" botoia erakusten duen pantaila-argazkia](media/PRT-5.png)
 
8. <span data-ttu-id="f0a99-126">Errepikatu prozesu hori bigarren pluginarekin, **PreOperationQuoteLineDetail - msdyn_quotelinetransaction eguneratzea**.</span><span class="sxs-lookup"><span data-stu-id="f0a99-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="f0a99-127">Itxi plugina erregistratzeko tresna.</span><span class="sxs-lookup"><span data-stu-id="f0a99-127">Close the plug-in registration tool.</span></span>

