---
title: Erosi izakinik gabeko materialak ordaindu gabeko saltzaileen faktura bat erabiliz
description: Gai honetan azaltzen diren saltzaileen fakturak nola grabatu azaltzen da.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b5e6632d73c8a211b1f0d568be8e10ef47be77e2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993763"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="d7c6a-103">Erosi izakinik gabeko materialak ordaindu gabeko saltzaileen faktura bat erabiliz</span><span class="sxs-lookup"><span data-stu-id="d7c6a-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="d7c6a-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="d7c6a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d7c6a-105">Enpresa batek material baterako material ez hornituak proiektu baterako, kostuak berehala erregistratu daitezke proiektuaren aurka.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="d7c6a-106">Adibidez, Contoso Robotics US ekipoak berritzeko proiektu bat egiten ari da eta software lizentziak behar ditu.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="d7c6a-107">Lizentzia horiek hirugarrenen saltzaile batek eskuratzen ditu.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="d7c6a-108">Dynamics 365 Finance erabiliz, Ordaintzeko kontuetako idazkariak saltzailearen faktura dokumentu bat erregistratzen du eta lizentziaren kostuak ekipamendua berritzeko proiektuari zuzenean egozten dizkio.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="d7c6a-109">Gai honetan azaldutako funtzionalitatea erabili aurretik, berrikusi eta aplikatu beharrezko konfigurazioak.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="d7c6a-110">Informazio gehiagorako, ikusi [Gaitu ez dauden materialak eta saltzailearen faktura pendienteak](configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="d7c6a-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="d7c6a-111">Bidali proiektuari lotutako saltzailearen faktura zain</span><span class="sxs-lookup"><span data-stu-id="d7c6a-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="d7c6a-112">Saltzailearen fakturak zain daude **Saltzailearen fakturak zain** orrialdea (**Ordaintzeko kontuak** > **Fakturak** > **Saltzailearen fakturak zain**).</span><span class="sxs-lookup"><span data-stu-id="d7c6a-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="d7c6a-113">Bete urrats hauek proiektuari lotutako saltzailearen faktura pendiente bat bidaltzeko:</span><span class="sxs-lookup"><span data-stu-id="d7c6a-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="d7c6a-114">Joan **Ordaintzeko kontuak** > **Fakturak** aukerara eta hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="d7c6a-115">**Faktura kontua** eremuan, hautatu saltzailea eta **Zenbakia** eremuan, sartu saltzailearen faktura identifikazioa.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="d7c6a-116">Gehitu lerro bat saltzailearen fakturan eta **Elementuaren zenbakia** eremuan, hautatu saltzailearengandik erositako stockik gabeko elementua.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="d7c6a-117">Kontratazio kategoria batean oinarritutako saltzaileen faktura lerroak ezin dira proiektuaren aurka erregistratu.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="d7c6a-118">Gehitu erositako kantitatea.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-118">Add the quantity purchased.</span></span> <span data-ttu-id="d7c6a-119">Sistemak unitateko prezioa beteko du hornitu gabeko elementuen prezioaren konfigurazioan oinarrituta.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="d7c6a-120">Egiaztatu zenbateko osoa eta beharrezko gainerako xehetasunak linean.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="d7c6a-121">Linearen xehetasunetan, **Proiektua** fitxan, hautatu elementu hau grabatuko den proiektuaren IDa.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="d7c6a-122">Aukeran, hautatu jardueraren zenbakia eta eguneratu proiektuaren kategoria eta lerroaren propietatea.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="d7c6a-123">Bidali zain dagoen saltzailearen faktura.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-123">Post pending vendor invoice.</span></span> <span data-ttu-id="d7c6a-124">Faktura argitaratzen denean, sistemak erregistratzen du:</span><span class="sxs-lookup"><span data-stu-id="d7c6a-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="d7c6a-125">Saltzailearen saldoaren zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="d7c6a-126">Salmenten zergen zenbatekoa.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-126">The sales tax amount.</span></span>
    - <span data-ttu-id="d7c6a-127">Proiektuaren kostua kontratazioen integrazio kontuan erregistratzen da.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="d7c6a-128">Proiektuaren benetako transakzioa Dataverse-n.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="d7c6a-129">Transakzio hau gehiago prozesatzen da [Project Operations integrazio-aldizkaria](../project-accounting/project-operations-integration-journal.md) erabiliz.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="d7c6a-130">Aldizkari hau argitaratzeak zenbatekoa kontratazioen integrazio kontutik proiektuaren kostu kontura mugitzen du.</span><span class="sxs-lookup"><span data-stu-id="d7c6a-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
