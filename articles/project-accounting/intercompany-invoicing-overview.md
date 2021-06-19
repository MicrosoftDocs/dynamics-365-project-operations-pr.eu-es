---
title: Enpresen arteko fakturazioaren informazio orokorra
description: Gai honek enpresen arteko fakturazioa proiektuen inguruko informazioa eta adibideak eskaintzen ditu.
author: sigitac
ms.date: 11/19/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42af89105f8325f1c94df6d2133d2c329facf2b3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002626"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="f7da9-103">Enpresen arteko fakturazioaren informazio orokorra</span><span class="sxs-lookup"><span data-stu-id="f7da9-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="f7da9-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="f7da9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f7da9-105">Zure erakundeak dibisio, filial eta beste pertsona juridiko ugari izan ditzake produktuak eta zerbitzuak elkarri proiektuetarako transferitzen dituztenak.</span><span class="sxs-lookup"><span data-stu-id="f7da9-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="f7da9-106">Zerbitzua edo produktua eskaintzen duen pertsona juridikoari deitzen zaio *pertsona juridiko mailegu-emailea*.</span><span class="sxs-lookup"><span data-stu-id="f7da9-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="f7da9-107">Zerbitzua edo produktua jasotzen duen pertsona juridikoari deitzen zaio *pertsona juridiko mailegu-hartzailea*.</span><span class="sxs-lookup"><span data-stu-id="f7da9-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="f7da9-108">Ondorengo ilustrazioak bi pertsona juridiko, esate baterako, agertoki tipikoa erakusten du. Contoso Robotics USA (maileguan dagoen pertsona juridikoa) eta Contoso Robotics UK-k (mailegu-entitate juridikoa) baliabideak partekatzen ditu abentura lanak bezeroarentzako proiektu bat emateko.</span><span class="sxs-lookup"><span data-stu-id="f7da9-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="f7da9-109">Eszenatoki honetarako, Contoso Robotics USA-k kontratua du lana Adventure Works-i entregatzeko.</span><span class="sxs-lookup"><span data-stu-id="f7da9-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![Enpresen arteko fakturazioa](./media/IntercompanyScenario.png) 

<span data-ttu-id="f7da9-111">Dynamics 365 Project Operations fluxua erabiltzen du enpresen arteko transakzioak prozesatzeko:</span><span class="sxs-lookup"><span data-stu-id="f7da9-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="f7da9-112">Mailegu-entitate juridikoaren baliabideek konpainien arteko denbora edo gastuen transakzioak erregistratzen dituzte, denbora eta gastuak erreserbatuz mailegu-entitate juridikoan proiektuen aurka.</span><span class="sxs-lookup"><span data-stu-id="f7da9-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="f7da9-113">Denbora eta gastuen kostuak mailegu-enpresan erregistratzen dira mailegu-hartzailearen konpainiaren unitateko kostuen prezioen zerrenda erabiliz.</span><span class="sxs-lookup"><span data-stu-id="f7da9-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="f7da9-114">Enpresa arteko fakturatu gabeko salmenta-transakzioak mailegu-enpresan erregistratzen dira mailegu-hartzailearen konpainiaren unitateko kostuen prezioen zerrenda erabiliz.</span><span class="sxs-lookup"><span data-stu-id="f7da9-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="f7da9-115">Fakturatu gabeko diru-sarrerak mailegu-enpresan erregistratzen dira proiektuaren kontratuaren salmenta prezioen zerrenda erabiliz.</span><span class="sxs-lookup"><span data-stu-id="f7da9-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="f7da9-116">Bezeroari faktura daiteke fakturatu gabeko diru sarrerak erregistratzen direnean.</span><span class="sxs-lookup"><span data-stu-id="f7da9-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="f7da9-117">Bezeroak ez du itxaron behar enpresen arteko fakturak prozesatu arte.</span><span class="sxs-lookup"><span data-stu-id="f7da9-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="f7da9-118">Enpresen arteko bezeroen fakturak aldian behin sortzen dira mailegu-enpresan.</span><span class="sxs-lookup"><span data-stu-id="f7da9-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="f7da9-119">Fakturak eskuz edo aldian aldiko prozesu automatizatu bat erabiliz sortzen dira.</span><span class="sxs-lookup"><span data-stu-id="f7da9-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="f7da9-120">Mailegu-entitate juridiko bakoitzeko faktura bakarra sor daiteke edo proiektuaren arabera faktura desberdinak sor daitezke.</span><span class="sxs-lookup"><span data-stu-id="f7da9-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="f7da9-121">Enpresa arteko saltzaileen faktura emailearen legezko entitatean argitaratzen denean, dagokion zain dagoen saltzaile-faktura legezko entitate-hartzailean sortuko da.</span><span class="sxs-lookup"><span data-stu-id="f7da9-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="f7da9-122">Saltzaileen fakturaren zain dauden kostuak faktura argitaratzen denean proiektuaren azpiegituran erregistratuko dira.</span><span class="sxs-lookup"><span data-stu-id="f7da9-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="f7da9-123">Ondorengo diagramak enpresen arteko fakturazioa erakusten du kontabilitateko gertaerekin eta liburu nagusian espero diren bidalketekin erlazionatuta.</span><span class="sxs-lookup"><span data-stu-id="f7da9-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![Enpresen arteko fluxua](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="f7da9-125">Baliabide gehigarriak</span><span class="sxs-lookup"><span data-stu-id="f7da9-125">Additional resources</span></span>

- [<span data-ttu-id="f7da9-126">Konfiguratu enpresen arteko fakturazioa</span><span class="sxs-lookup"><span data-stu-id="f7da9-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="f7da9-127">Grabatu enpresen arteko transakzioak</span><span class="sxs-lookup"><span data-stu-id="f7da9-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="f7da9-128">Sortu enpresen arteko bezeroa eta saltzaileen fakturak</span><span class="sxs-lookup"><span data-stu-id="f7da9-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]