---
title: Proformako faktura bat eskuz sortzea
description: Gai honetan Projec Operations-eko eskuzko proformako fakturak sortzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5e93206737507bf6698a9746815c790d3dfc904
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/20/2020
ms.locfileid: "4071265"
---
# <a name="creating-a-manual-proforma-invoice"></a><span data-ttu-id="0a340-103">Proformako faktura bat eskuz sortzea</span><span class="sxs-lookup"><span data-stu-id="0a340-103">Creating a manual proforma invoice</span></span>

<span data-ttu-id="0a340-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="0a340-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0a340-105">Dynamics 365 Project Operations-en, proforma fakturak eskuz sor daitezke beharren arabera.</span><span class="sxs-lookup"><span data-stu-id="0a340-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="0a340-106">Proformako fakturak sortzeko, joan **Proiektuen kontratuak** zerrendako orrialdera **Proiektuen kontratua** xehetasunen orrira.</span><span class="sxs-lookup"><span data-stu-id="0a340-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="0a340-107">Proiektu-kontratuen zerrenda-orria</span><span class="sxs-lookup"><span data-stu-id="0a340-107">Project Contracts list page</span></span>

<span data-ttu-id="0a340-108">**Proiektuen kontratuak** zerrenda-orrian, hautatu proiektuaren kontratu bat edo gehiago eta sortu hautatutako erregistro guztien fakturak.</span><span class="sxs-lookup"><span data-stu-id="0a340-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="0a340-109">Sistemak hautatutako proiektuen kontratuetako batek zein duen egiaztatzen du **Fakturatzeko prest** atzerapena gaurko data baino lehenagokoa.</span><span class="sxs-lookup"><span data-stu-id="0a340-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="0a340-110">Kontratu horietatik sistemak proforma fakturen zirriborroak sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="0a340-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="0a340-111">Proiektuaren kontratu batek bezero ugari baditu, faktore bat sor daiteke bezero bakoitzeko, eta faktura ugari proiektuko kontratu bakoitzeko.</span><span class="sxs-lookup"><span data-stu-id="0a340-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="0a340-112">Sortutako proiektuaren faktura guztiak eskuragarri daude **Faktura** orrialdean **Fakturazioa** ataleko **Salmentak** eremuan.</span><span class="sxs-lookup"><span data-stu-id="0a340-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="0a340-113">Proiektu-kontratuaren xehetasunen orria</span><span class="sxs-lookup"><span data-stu-id="0a340-113">Project Contract details page</span></span>

<span data-ttu-id="0a340-114">Proforma faktura bat ere sor daiteke **Proiektuaren kontratua** xehetasunen orria, proiektuaren kontratu zehatz horren faktura sortzen duena.</span><span class="sxs-lookup"><span data-stu-id="0a340-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="0a340-115">Sistemak proiektuaren kontratua egiaztatzen du, **Fakturatzeko prest** atzerapena gaurko data baino lehenagokoa.</span><span class="sxs-lookup"><span data-stu-id="0a340-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="0a340-116">Kontratu horietatik sistemak proforma fakturen zirriborroak sortzen ditu kontratu lerro bakoitzeko bezero kopuruaren arabera.</span><span class="sxs-lookup"><span data-stu-id="0a340-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="0a340-117">Proforma faktura bakarra sortzen denean, **Faktura** orria irekitzen da.</span><span class="sxs-lookup"><span data-stu-id="0a340-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="0a340-118">Proiektuaren kontratu horretarako faktura ugari sortu badira, **Fakturak** zerrenda orria irekitako sortutako faktura guztiak erakusteko.</span><span class="sxs-lookup"><span data-stu-id="0a340-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
