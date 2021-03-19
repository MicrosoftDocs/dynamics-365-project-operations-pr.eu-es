---
title: Itxi eskaintza bat - arina
description: Gai honek Project Operations-eko eskaintzak ixteari buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6214e1b5bec5c9173a6b6e69578de14654da633e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272250"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="971cc-103">Itxi eskaintza bat - arina</span><span class="sxs-lookup"><span data-stu-id="971cc-103">Close a quote - lite</span></span>

<span data-ttu-id="971cc-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="971cc-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="971cc-105">Proiektuaren eskaintzak Irabazi edo Galdu bezala itxi daitezke.</span><span class="sxs-lookup"><span data-stu-id="971cc-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="971cc-106">Aurrekontuaren zirriborroa itxi daiteke Aktibatu eta Berrikusi komatxoen eragiketak Microsoft Dynamics 365 Project Operations ez direlako onartzen.</span><span class="sxs-lookup"><span data-stu-id="971cc-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="971cc-107">Itxi eskaintza Irabazita gisa</span><span class="sxs-lookup"><span data-stu-id="971cc-107">Close a quote as Won</span></span>

<span data-ttu-id="971cc-108">Proiektuaren aurrekontua Irabazitako moduan ixten duzunean, egoera Itxia da eta egoeraren arrazoi Irabazita dago.</span><span class="sxs-lookup"><span data-stu-id="971cc-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="971cc-109">Eskaintza ixten baduzu, proiektuaren irakurketa soilik irakurtzen da eta eskaintzaren informazioa jasotzen duen proiektuaren zirriborroko eskaintza sortzen da.</span><span class="sxs-lookup"><span data-stu-id="971cc-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="971cc-110">Aurrekontu itxia ezin denez berriro ireki, berrespen-elkarrizketa-koadro batek aldaketak baieztatuko ditu.</span><span class="sxs-lookup"><span data-stu-id="971cc-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="971cc-111">Aurrekontua aukera bati atxikita badago, aukeraren inguruko beste edozein proiektu automatikoki galduko da itxita.</span><span class="sxs-lookup"><span data-stu-id="971cc-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="971cc-112">Aurrekontua Irabazitako moduan ixteak duen eragin ekonomikoa</span><span class="sxs-lookup"><span data-stu-id="971cc-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="971cc-113">Aurrekontu zirriborro bati atxikita dagoen bitartean proiektu batean denborari buruzko datuak egiazkoak badira, denboraren edo gastuaren kostua bakarrik erregistratuko da.</span><span class="sxs-lookup"><span data-stu-id="971cc-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="971cc-114">Aurrekontua Irabazi ahala itxi ondoren, aplikazioak kostuak berregokituko ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak berriro sortuz.</span><span class="sxs-lookup"><span data-stu-id="971cc-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="971cc-115">Aplikazioak kostu erreal hauek prozesatuko ditu lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="971cc-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="971cc-116">Kostuen fakturak denbora eta material kontratu lerro bati erreferentzia egiten bazaio, fakturatu gabeko salmenta errealak sortzen dira aurrekontua itxi eta proiektuaren kontratua sortzen denean.</span><span class="sxs-lookup"><span data-stu-id="971cc-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="971cc-117">Kostuen prezioak prezio finkoko kontratu lerro bati erreferentzia egiten badio, aplikazioak proiektuaren kontratuaren bezeroentzako fakturazio arau zatituetan oinarritutako kostuen fakturak berriro prozesatzeari utziko dio.</span><span class="sxs-lookup"><span data-stu-id="971cc-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="971cc-118">Eskaintza galdu bezala itxi:</span><span class="sxs-lookup"><span data-stu-id="971cc-118">Closing a quote as lost:</span></span>

<span data-ttu-id="971cc-119">Proiektuaren aurrekontua Galdutako moduan ixten duzunean, egoera Itxia da eta egoeraren arrazoi Galduta dago.</span><span class="sxs-lookup"><span data-stu-id="971cc-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="971cc-120">Eskaintza ixteak proiektuaren eskaintza irakurtzeko soilik bihurtzen du.</span><span class="sxs-lookup"><span data-stu-id="971cc-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="971cc-121">Aurrekontu itxia ezin denez berriro ireki eta, aurrekontua itxi aurretik, berrespen-elkarrizketa-koadro batek zure aldaketak baieztatuko ditu.</span><span class="sxs-lookup"><span data-stu-id="971cc-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="971cc-122">Galdutako itxita dagoen proiektuaren aurrekontuak bere lerroetako edozein proiektu aipatzen badu, proiektu hori itxita dagoela ere markatuko da.</span><span class="sxs-lookup"><span data-stu-id="971cc-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="971cc-123">Egun horretatik aurrera edozein baliabide erreserba bertan behera geratzen da.</span><span class="sxs-lookup"><span data-stu-id="971cc-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="971cc-124">Project Operations-en, aurrekontua Irabazita edo Galduta gisa ixteak ez du Aukeraren egoera horretan eragingo, irekita egongo da eskuz itxi arte.</span><span class="sxs-lookup"><span data-stu-id="971cc-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]