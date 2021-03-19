---
title: Plugin-atributuak prezio-dimentsio berriak gehitzeko eguneratzen
description: Gai honek prezio-dimentsioetarako plugin atributuak eguneratzeko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7999c003a0cf670d586ebf4445901e106fbee39f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274668"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="eacd2-103">Eguneratu plugin-atributuak prezio-dimentsio berriak gehitzeko</span><span class="sxs-lookup"><span data-stu-id="eacd2-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="eacd2-104">Gai honek prezio-dimentsioetarako plugin atributuak eguneratzeko informazioa eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="eacd2-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="eacd2-105">Gai hau aurrekontuaren eta kontratuaren ezaugarriei soilik aplikatzen zaie Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="eacd2-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eacd2-106">Aurrebaldintzak</span><span class="sxs-lookup"><span data-stu-id="eacd2-106">Prerequisites</span></span>
<span data-ttu-id="eacd2-107">Gai honetako pausoak bete aurretik, gai hauetako prozedurak bete beharko dituzu:</span><span class="sxs-lookup"><span data-stu-id="eacd2-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="eacd2-108">Sortu eremu eta entitate pertsonalizatuak</span><span class="sxs-lookup"><span data-stu-id="eacd2-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="eacd2-109">Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan </span><span class="sxs-lookup"><span data-stu-id="eacd2-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="eacd2-110">[Konfiguratu eremu pertsonalizatuak prezio-dimentsio gisa](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="eacd2-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="eacd2-111">Prozedura horiek bete ez badituzu, bete itzazu eta, ondoren, itzuli gai honetara.</span><span class="sxs-lookup"><span data-stu-id="eacd2-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="eacd2-112">Erregistratu plugina</span><span class="sxs-lookup"><span data-stu-id="eacd2-112">Register a plug-in</span></span>
<span data-ttu-id="eacd2-113">Aurrekontuaren lerroaren xehetasuna sortzen denean **Aipatu lerroa** proiektuaren aurrekontu lerroaren orrialdea, sistemak bi estimazio lerro sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="eacd2-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="eacd2-114">Lerro bat aurrekontuaren kostuaren aldekoa da eta beste lerroa salmenten aldekoa.</span><span class="sxs-lookup"><span data-stu-id="eacd2-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="eacd2-115">Gauza bera gertatzen da proiektuaren kontratuaren lerroarekin.</span><span class="sxs-lookup"><span data-stu-id="eacd2-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="eacd2-116">Kostuaren aldeko kopuruari edo eremuari aldaketaren bat egiten diozunean, aldaketa hori salmenten aldean ere egiten da.</span><span class="sxs-lookup"><span data-stu-id="eacd2-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="eacd2-117">Hori posible da, Quotelinedetaileko eta kontratatutako xehetasun entitateetako PreOperation plug-inek kostu aldetik atributu espezifikoak transakzioaren salmenten aldera konektatzen dituztelako.</span><span class="sxs-lookup"><span data-stu-id="eacd2-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="eacd2-118">Salmenten aldetik prezioen dimentsio balioetan egindako aldaketak kostuaren aldetik ere egin behar badituzu, honako plug-in hauek berriro erregistratu beharko dira prezioen dimentsioan aldaketak egin ondoren.</span><span class="sxs-lookup"><span data-stu-id="eacd2-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="eacd2-119">Hauek dira eguneratzeko eta berriro erregistratzeko pluginak:</span><span class="sxs-lookup"><span data-stu-id="eacd2-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="eacd2-120">PreOperationContractLineDetailUpdate - **Eguneratu msdyn_orderlinetransaction**</span><span class="sxs-lookup"><span data-stu-id="eacd2-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="eacd2-121">PreOperationQuoteLineDetailUpdate - **msdyn_quotelinetransaction eguneratzen du**.</span><span class="sxs-lookup"><span data-stu-id="eacd2-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="eacd2-122">Osatu urrats hauek pluginak eguneratzeko eta berriro erregistratzeko.</span><span class="sxs-lookup"><span data-stu-id="eacd2-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="eacd2-123">Ireki **PluginRegistrationTool** eta konektatu zure Project Operations-en Dataverse ingurunea.</span><span class="sxs-lookup"><span data-stu-id="eacd2-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="eacd2-124">Aukeratu **Bilatu**, eta idatzi eguneratu beharreko pluginaren lehen hizkiak.</span><span class="sxs-lookup"><span data-stu-id="eacd2-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="eacd2-125">Plugina aurkitu ondoren, hautatu eta hautatu **Hautatu Inprimaki nagusian**.</span><span class="sxs-lookup"><span data-stu-id="eacd2-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="eacd2-126">Hautatu **Eguneratu msdyn_orderlinetransaction** urratsa, egin klik eskuineko botoiarekin eta, ondoren, hautatu **Eguneratu**.</span><span class="sxs-lookup"><span data-stu-id="eacd2-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="eacd2-127">**Eguneratu** elkarrizketa-leihoan, sakatu elipsia (**...**) iragazkiaren atributuetan.</span><span class="sxs-lookup"><span data-stu-id="eacd2-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="eacd2-128">Iragazteko atributuak leihoa ireki eta entitatearen atributu guztien zerrenda eta prezioen dimentsioak eskaintzen ditu.</span><span class="sxs-lookup"><span data-stu-id="eacd2-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="eacd2-129">Hautatu prezioen dimentsio atributuen kontrol laukiak.</span><span class="sxs-lookup"><span data-stu-id="eacd2-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="eacd2-130">Hautatu **Ados** aukeran orria ixteko eta, ondoren, hautatu **Eguneratu urratsa**.</span><span class="sxs-lookup"><span data-stu-id="eacd2-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="eacd2-131">Errepikatu 2-7. urratsak bigarren pluginerako, **PreOperationQuoteLineDetail**.</span><span class="sxs-lookup"><span data-stu-id="eacd2-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="eacd2-132">Plugin honetarako, **Eguneratu msdyn_quotelinetransaction** urratsa eguneratu behar duzu.</span><span class="sxs-lookup"><span data-stu-id="eacd2-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="eacd2-133">Itxi **PluginRegistrationTool**.</span><span class="sxs-lookup"><span data-stu-id="eacd2-133">Close **PluginRegistrationTool**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]