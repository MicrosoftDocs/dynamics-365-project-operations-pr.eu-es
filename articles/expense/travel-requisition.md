---
title: Bidaiatzeko eskakizunak
description: Gai honek bidaia-eskakizunei buruzko informazioa ematen du.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 0261405abb9305d7f6abcde9cb90d9b184868580
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070905"
---
# <a name="travel-requisitions"></a><span data-ttu-id="5e035-103">Bidaiatzeko eskakizunak</span><span class="sxs-lookup"><span data-stu-id="5e035-103">Travel requisitions</span></span>

<span data-ttu-id="5e035-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="5e035-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="5e035-105">Bidaia eskaera batean bidaia egiteko sortuko diren gastuak agertzen dira.</span><span class="sxs-lookup"><span data-stu-id="5e035-105">A travel requisition lists the expenses that will be incurred for the purpose of travel.</span></span> <span data-ttu-id="5e035-106">Bidaia eskaera bat aurkezten da berrikusteko eta gastuak baimentzeko erabil daiteke.</span><span class="sxs-lookup"><span data-stu-id="5e035-106">A travel requisition is submitted for review and can be used to authorize expenses.</span></span>

<span data-ttu-id="5e035-107">Agian erakundeari kobratzen zaizkion gastuak egin aurretik bidaia eskaera aurkeztu beharko duzu.</span><span class="sxs-lookup"><span data-stu-id="5e035-107">You may be required to submit a travel requisition before you incur any expense that is charged to the organization.</span></span> <span data-ttu-id="5e035-108">Betekizun hau aplikatzen da, kreditu-txartel korporatiboari gastuak kobratu, dirua aurreratzeagatik jasotako dirua gastatu edo erakundeak itzuliko dizun poltsikoko gastuak izan.</span><span class="sxs-lookup"><span data-stu-id="5e035-108">This requirement applies, regardless of whether you charge expenses to a corporate credit card, spend cash that you received from a cash advance, or incur out-of-pocket expenses that will be reimbursed by the organization.</span></span>

<span data-ttu-id="5e035-109">Bidaia eskaerak eta gidalerroak erabil daitezke erakundearen gastuak kudeatzen laguntzeko.</span><span class="sxs-lookup"><span data-stu-id="5e035-109">Travel requisitions and policies can be used to help manage organization expenditures.</span></span> <span data-ttu-id="5e035-110">Adibidez, zure erakundeak bidaia behar duen prezio finkoaren proiektuan lan egiten badu, proiektuko taldekideen bidaia gastuak proiektuaren aurrekontuaren barruan sartu behar dira.</span><span class="sxs-lookup"><span data-stu-id="5e035-110">For example, if your organization is working on a fixed-price project that requires travel, the travel expenses of the project's team members must fit within the project budget.</span></span> <span data-ttu-id="5e035-111">Bidaia gastuak onartu baino lehen onartuz gero, erakundeak proiektua aurrekontuaren barruan mantenduko dela ziurtatu dezake.</span><span class="sxs-lookup"><span data-stu-id="5e035-111">By requiring that travel expenses be approved before they are incurred, the organization can help make sure that the project remains within budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="5e035-112">Konfigurazioa</span><span class="sxs-lookup"><span data-stu-id="5e035-112">Configuration</span></span> 

<span data-ttu-id="5e035-113">Bidaia-eskakizunak "derrigorrezko" gisa konfigura daitezke Gastuak kudeatzeko parametroetan "Bidaiaren aurretiazko baimena derrigorrezkoa" parametroa gaituz.</span><span class="sxs-lookup"><span data-stu-id="5e035-113">Travel Requisitions can be configured as "mandatory" by enabling the "Pre-authorization of travel is mandatory" parameter in Expense Management Parameters.</span></span> 

## <a name="create-and-submit-a-travel-requisition"></a><span data-ttu-id="5e035-114">Sortu eta bidali bidaia eskaera</span><span class="sxs-lookup"><span data-stu-id="5e035-114">Create and submit a travel requisition</span></span>

1. <span data-ttu-id="5e035-115">Joan **Nire gastuak: Bidaia eskatzea** , eta hautatu **Bidaia eskakizun berria**.</span><span class="sxs-lookup"><span data-stu-id="5e035-115">Go to **My expenses: Travel Requisition** , and select **New travel Requisition**.</span></span>
2. <span data-ttu-id="5e035-116">Sartu eskaeraren xedea eta helmuga.</span><span class="sxs-lookup"><span data-stu-id="5e035-116">Enter a purpose and destination for the requisition.</span></span>
3. <span data-ttu-id="5e035-117">**Bidaiaren deskribapena** eremuan, sartu informazio osagarria.</span><span class="sxs-lookup"><span data-stu-id="5e035-117">In the  **Travel description** field, enter any additional information.</span></span> 
4. <span data-ttu-id="5e035-118">Aurreikusitako gastu bakoitzerako, hala nola Hegaldia, otorduak edo autoen alokairua, sortu gastuko lineako elementu bat.</span><span class="sxs-lookup"><span data-stu-id="5e035-118">For each of the expected expenses, such as Flight, meals, or car rental, create an expense line item.</span></span> <span data-ttu-id="5e035-119">Sartu gastu bakoitzerako zenbatetsitako data, zenbatetsitako zenbatekoa eta moneta.</span><span class="sxs-lookup"><span data-stu-id="5e035-119">Include the estimated date, estimated amount, and the currency for each expense.</span></span> 
5. <span data-ttu-id="5e035-120">Aurreikusitako gastuak gehitzen amaitutakoan, hautatu **Gorde**.</span><span class="sxs-lookup"><span data-stu-id="5e035-120">When you have finished adding the expected expenses, select **Save**.</span></span>
6. <span data-ttu-id="5e035-121">Bidaiaren eskaera aurkezteko prest zaudenean, hautatu **Lan-fluxua** > **Bidali**.</span><span class="sxs-lookup"><span data-stu-id="5e035-121">When you are ready to submit the travel requisition, select **Workflow** > **Submit**.</span></span>

<span data-ttu-id="5e035-122">Onartutako bidaia eskaerak hemen ikus ditzakezu **Nire gastuak: bidaia-eskakizuna**.</span><span class="sxs-lookup"><span data-stu-id="5e035-122">You can view your approved travel requisitions under **My Expenses: Travel Requisition**.</span></span> 

## <a name="view-available-travel-requisitions"></a><span data-ttu-id="5e035-123">Ikusi eskuragarri dauden bidaia eskaerak</span><span class="sxs-lookup"><span data-stu-id="5e035-123">View available travel requisitions</span></span>

<span data-ttu-id="5e035-124">Bidaia-eskakizun guztiak ikus ditzakezu **Nire gastuak: bidaia-eskakizunak** aukeran.</span><span class="sxs-lookup"><span data-stu-id="5e035-124">You can view all of your travel requisitions under **My Expenses: Travel Requisitions**.</span></span>

## <a name="approve-travel-requisitions"></a><span data-ttu-id="5e035-125">Onartu bidaiatzeko eskakizunak</span><span class="sxs-lookup"><span data-stu-id="5e035-125">Approve travel requisitions</span></span>

<span data-ttu-id="5e035-126">Aukeratu onartu nahi duzun bidaia-eskaera, eta hautatu **Lan-fluxua** > **Onartu**.</span><span class="sxs-lookup"><span data-stu-id="5e035-126">Select the travel requisition that you want to approve, and then select **Workflow** > **Approve**.</span></span>  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a><span data-ttu-id="5e035-127">Bidali gastuen txostena onartutako bidaia eskaera erabiliz</span><span class="sxs-lookup"><span data-stu-id="5e035-127">Submit an expense report using your approved travel requisition</span></span>

1. <span data-ttu-id="5e035-128">Sortu gastu-txosten berria eta gastuen txostenaren goiburuan eta, onartutako bidaia-eskaeren zerrendan, hautatu **Esleitu bidaiatzeko eskatzeko**.</span><span class="sxs-lookup"><span data-stu-id="5e035-128">Create a new expense report and in the expense report header, and from the list of approved travel requisitions, select **Map to Travel requisition**.</span></span>
2. <span data-ttu-id="5e035-129">**Bidaia eskatzeko zenbatekoa** eremua automatikoki eguneratzen da gastuen txostenaren goiburuan.</span><span class="sxs-lookup"><span data-stu-id="5e035-129">The **Travel requisition amount** field is automatically updated in the expense report header.</span></span>
3. <span data-ttu-id="5e035-130">Gehitu bidaiarako sortutako gastu bakoitza.</span><span class="sxs-lookup"><span data-stu-id="5e035-130">Add each expense incurred for the trip.</span></span> <span data-ttu-id="5e035-131">**Aurrez baimenduta** eremua gaituta badago, bateratutako zenbatekoa eta baimendutako kopurua berariazko gastu-kategoriarako eguneratuko dira.</span><span class="sxs-lookup"><span data-stu-id="5e035-131">If the **Pre-authorized** field is enabled, the reconciled amount and authorized amount for the specific expense category will be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="5e035-132">Gastu-txostena onartutako bidaia-eskaera batera lotzen duzunean, transakzioaren zenbatekoa ezin da baimendutakoa baino handiagoa izan.</span><span class="sxs-lookup"><span data-stu-id="5e035-132">When you map an expense report to an approved travel requisition, the transaction amount can't be greater than the authorized amount.</span></span> 
