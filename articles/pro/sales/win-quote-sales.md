---
title: Itxi eskaintza bat - arina
description: Gai honek Project Operations-eko eskaintzak ixteari buruzko informazioa ematen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5ad206232d616cdbdc83e2a17b9177cfb98ffda9
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175696"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="5d0a2-103">Itxi eskaintza bat - arina</span><span class="sxs-lookup"><span data-stu-id="5d0a2-103">Close a quote - lite</span></span>

<span data-ttu-id="5d0a2-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="5d0a2-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5d0a2-105">Proiektuaren eskaintzak Irabazi edo Galdu bezala itxi daitezke.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="5d0a2-106">Eskaintzetako Aktibatu eta Berrikusi eragiketak ez dira onartzen Microsoft Dynamics 365 Project Operations-en; beraz, zirriborroko eskaintza itxi daiteke.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="5d0a2-107">Itxi eskaintza Irabazita gisa</span><span class="sxs-lookup"><span data-stu-id="5d0a2-107">Close a quote as Won</span></span>

<span data-ttu-id="5d0a2-108">Irabazitako proiektuaren eskaintza ixtean eskaintza itxi egingo da egoera itxita eta egoeraren arrazoi Irabazitako moduan.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="5d0a2-109">Eskaintza ixten baduzu, proiektuaren irakurketa soilik irakurtzen da eta eskaintzaren informazioa jasotzen duen proiektuaren zirriborroko eskaintza sortzen da.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="5d0a2-110">Eskaintza itxia ezin denez berriro ireki, baieztapen elkarrizketa-koadroa Baieztapen elkarrizketa-koadroa dago aldaketak egin aurretik, eskaintza itxia ezin baita berriro ireki eta aldaketak atzeraezinak dira.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="5d0a2-111">Aurrekontua aukera bati atxikita badago, aukeraren inguruko beste edozein proiektu automatikoki galduko da itxita.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="5d0a2-112">Aurrekontua Irabazitako moduan ixteak duen eragin ekonomikoa</span><span class="sxs-lookup"><span data-stu-id="5d0a2-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="5d0a2-113">Aurrekontu zirriborro bati atxikita dagoen bitartean proiektu batean erregistratutako denboraren berri eman bada, denboraren edo gastuaren kostua bakarrik erregistratuko da.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="5d0a2-114">Aurrekontua Irabazi ahala itxi ondoren, aplikazioak kostuak berregokituko ditu kostu zaharrenak alderantzikatuz eta kostu erreal berriak berriro sortuz.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="5d0a2-115">Aplikazioak kostu erreal hauek prozesatuko ditu lotutako proiektuaren kontratu lerroaren Fakturazio metodoan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="5d0a2-116">Kostuen fakturak denbora eta material kontratu lerro bati erreferentzia egiten badio, sistemak automatikoki sortuko ditu fakturatu gabeko salmenten fakturak, aurrekontua itxi eta proiektuaren kontratua sortzen denean.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="5d0a2-117">Kostuen prezioak prezio finkoko kontratu lerro bati erreferentzia egiten badio, aplikazioak kostuaren fakturak berriro prozesatzeari utziko dio proiektuaren kontratuko bezeroen fakturazio arau zatituetan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="5d0a2-118">Eskaintza galdu bezala itxi:</span><span class="sxs-lookup"><span data-stu-id="5d0a2-118">Closing a quote as lost:</span></span>

<span data-ttu-id="5d0a2-119">Galdutako proiektuaren eskaintza ixtean egoera ezarriko da Itxita eta egoeraren arrazoia Galdua izango da.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="5d0a2-120">Eskaintza ixteak proiektuaren eskaintza irakurtzeko soilik bihurtzen du.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="5d0a2-121">Aurrekontu itxia ezin denez berriro ireki eta, aurrekontua itxi aurretik, berrespen-elkarrizketa-koadro batek zure aldaketak baieztatuko ditu.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="5d0a2-122">Galduta gisa itxita dagoen proiektuaren aurrekontuak bere lerroetako batean proiektu bat badu erreferentzia, proiektu hori Itxita gisa markatzen da eta egun horretatik aurrerako baliabideen erreserbak bertan behera geratzen dira.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="5d0a2-123">Project Operations-en, aurrekontua Irabazita edo Galduta gisa ixteak ez du Aukeraren egoera horretan eragingo, irekita egongo da eskuz itxi arte.</span><span class="sxs-lookup"><span data-stu-id="5d0a2-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
