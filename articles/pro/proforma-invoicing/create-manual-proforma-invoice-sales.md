---
title: Sortu proformako faktura bat eskuz - arina
description: Gai honetan Projec Operations-eko eskuzko proformako fakturak sortzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5a924de6efc377e28a20e038e7deac04616b95aa
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764488"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="429cb-103">Sortu proformako faktura bat eskuz - arina</span><span class="sxs-lookup"><span data-stu-id="429cb-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="429cb-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="429cb-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="429cb-105">Dynamics 365 Project Operations-en, proforma fakturak eskuz sor daitezke beharren arabera.</span><span class="sxs-lookup"><span data-stu-id="429cb-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="429cb-106">Proformako fakturak sortzeko, joan **Proiektuen kontratuak** zerrendako orrialdera **Proiektuen kontratua** xehetasunen orrira.</span><span class="sxs-lookup"><span data-stu-id="429cb-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="429cb-107">Proiektu-kontratuen zerrenda-orria</span><span class="sxs-lookup"><span data-stu-id="429cb-107">Project Contracts list page</span></span>

<span data-ttu-id="429cb-108">**Proiektuen kontratuak** zerrenda-orrian, hautatu proiektuaren kontratu bat edo gehiago eta sortu hautatutako erregistro guztien fakturak.</span><span class="sxs-lookup"><span data-stu-id="429cb-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="429cb-109">Sistemak hautatutako proiektuen kontratuetako batek zein duen egiaztatzen du **Fakturatzeko prest** atzerapena gaurko data baino lehenagokoa.</span><span class="sxs-lookup"><span data-stu-id="429cb-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="429cb-110">Kontratu horietatik sistemak proforma fakturen zirriborroak sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="429cb-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="429cb-111">Proiektuaren kontratu batek bezero ugari baditu, faktore bat sor daiteke bezero bakoitzeko, eta faktura ugari proiektuko kontratu bakoitzeko.</span><span class="sxs-lookup"><span data-stu-id="429cb-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="429cb-112">Sortutako proiektuaren faktura guztiak eskuragarri daude **Faktura** orrialdean **Fakturazioa** ataleko **Salmentak** eremuan.</span><span class="sxs-lookup"><span data-stu-id="429cb-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="429cb-113">Proiektu-kontratuaren xehetasunen orria</span><span class="sxs-lookup"><span data-stu-id="429cb-113">Project Contract details page</span></span>

<span data-ttu-id="429cb-114">Proforma faktura bat ere sor daiteke **Proiektuaren kontratua** xehetasunen orria.</span><span class="sxs-lookup"><span data-stu-id="429cb-114">A proforma invoice can also be created from the **Project Contract** details page.</span></span> <span data-ttu-id="429cb-115">Sistemak proiektuen kontratuak **Fakturatzeko prest** atzerapena gaurko data baino lehenagokoa dela egiaztatzen du.</span><span class="sxs-lookup"><span data-stu-id="429cb-115">The system verifies the project contract has a **Ready to Invoice** backlog dated before today's date.</span></span> <span data-ttu-id="429cb-116">Kontratu horietatik sistemak proforma fakturen zirriborroak sortzen ditu kontratu lerro bakoitzeko bezero kopuruaren arabera.</span><span class="sxs-lookup"><span data-stu-id="429cb-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="429cb-117">Proforma faktura bakarra sortzen denean, **Faktura** orria irekitzen da.</span><span class="sxs-lookup"><span data-stu-id="429cb-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="429cb-118">Proiektuaren kontratu horretarako faktura ugari sortzen badira, **Fakturak** zerrenda orria irekitako sortutako faktura guztiak erakusteko.</span><span class="sxs-lookup"><span data-stu-id="429cb-118">If multiple invoices are created for that project contract, the **Invoices** list page opens to show all of the created invoices.</span></span>
