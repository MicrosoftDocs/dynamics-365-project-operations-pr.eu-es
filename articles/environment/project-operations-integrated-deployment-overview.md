---
title: Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen inplementazio orokorraren Project Operations
description: Gai honek inplementazio motari buruzko informazioa eskaintzen du, baliabidean / pilatu gabeko egoeretako Project Operations-en eragiketak.
author: rumant
ms.date: 11/02/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 3648bf6c5e00fe701f309392bd09819f84bf574d
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368686"
---
# <a name="project-operations-for-resourcenon-stocked-based-scenarios-deployment-overview"></a><span data-ttu-id="2984f-103">Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen inplementazio orokorraren Project Operations</span><span class="sxs-lookup"><span data-stu-id="2984f-103">Project Operations for resource/non-stocked based scenarios deployment overview</span></span>

<span data-ttu-id="2984f-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="2984f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2984f-105">Inplementazio motak, Dynamics 365 Project Operations baliabideetarako / stockean oinarritutako eszenatokietarako, gaitasun hauek ditu proiektuetan oinarritutako enpresentzat:</span><span class="sxs-lookup"><span data-stu-id="2984f-105">The deployment type, Dynamics 365 Project Operations for resource/non-stocked based scenarios has the following capabilities for project-based companies:</span></span>

- <span data-ttu-id="2984f-106">Proiektuaren plangintza Microsoft Project weberako</span><span class="sxs-lookup"><span data-stu-id="2984f-106">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="2984f-107">Lan-baliabideen dimentsio anitzeko prezioak eta kostuak</span><span class="sxs-lookup"><span data-stu-id="2984f-107">Multi-dimensional pricing and costing for labor resources</span></span>
- <span data-ttu-id="2984f-108">Gastuen kategorien arabera oinarritutako prezioak</span><span class="sxs-lookup"><span data-stu-id="2984f-108">Category-based pricing for expense categories</span></span>
- <span data-ttu-id="2984f-109">Proiektuetan oinarritutako salmenten kudeaketa Dynamics 365 Sales gaitasunak erabiliz</span><span class="sxs-lookup"><span data-stu-id="2984f-109">Project-based sales management using Dynamics 365 Sales capabilities</span></span>
- <span data-ttu-id="2984f-110">Universal Resource Scheduling, hala nola beste aplikazio batzuekin bateratzen dena Dynamics 365 Field Service eta Dynamics 365 Customer Service, esaterako</span><span class="sxs-lookup"><span data-stu-id="2984f-110">Universal resource scheduling that integrates with other applications such as Dynamics 365 Field Service and Dynamics 365 Customer Service</span></span>
- <span data-ttu-id="2984f-111">Proiektuaren aurrerapena eta denboraren jarraipena</span><span class="sxs-lookup"><span data-stu-id="2984f-111">Project progress and Time Tracking</span></span>
- <span data-ttu-id="2984f-112">Proiektuak eta proiektuak ez diren oinarrizko gastuak eta gastu guztiak kudeatzeko esperientziak, ordainagiriak jasotzeko OCR gaitasunak erabiliz</span><span class="sxs-lookup"><span data-stu-id="2984f-112">Basic and full Expense management experiences for project and non-project expenses including receipt capture using OCR capabilities</span></span>
- <span data-ttu-id="2984f-113">Proformatik bezeroari begiratzen dion fakturazioa eta enpresa mailako salmenten gaineko zerga eta data eraginkorra den truke-tasaren sistema babesten dituena.</span><span class="sxs-lookup"><span data-stu-id="2984f-113">Invoicing that extends from proforma to customer-facing and is backed by an enterprise-class sales tax and date-effective exchange rate system.</span></span>
- <span data-ttu-id="2984f-114">Proiektuaren kostu konfiguragarria, diru-sarreren profilak eta lanean ari diren (WIP) kontabilitate eta sortzapen arauak</span><span class="sxs-lookup"><span data-stu-id="2984f-114">Configurable project cost, revenue profiles, and rules for work in progress (WIP) accounting and accruals</span></span>
- <span data-ttu-id="2984f-115">Proiektuaren diru-sarreren aitorpena</span><span class="sxs-lookup"><span data-stu-id="2984f-115">Project revenue recognition</span></span>
- <span data-ttu-id="2984f-116">Hedagarritasuna Power Platform bidez</span><span class="sxs-lookup"><span data-stu-id="2984f-116">Extensibility through the Power Platform</span></span>

<span data-ttu-id="2984f-117">Inplementazio mota honek Dynamics 365 Finance eta Dynamics 365 Supply Chain Management aplikazioak.</span><span class="sxs-lookup"><span data-stu-id="2984f-117">This deployment type provides an extension to the functionality provided by Dynamics 365 Finance and Dynamics 365 Supply Chain Management applications.</span></span>

<span data-ttu-id="2984f-118">Inplementazio hau aukeratu beharko litzateke proiektuaren eragiketen itxaropena proiektuaren bizi-ziklo osoa erabiltzea, baldintza hauek biltzen dituena:</span><span class="sxs-lookup"><span data-stu-id="2984f-118">This deployment should be chosen the expectation of Project Operations is to use the full project lifecycle that includes the following requirements:</span></span>

- <span data-ttu-id="2984f-119">Salmenta aplikazioko gaitasunak erabiliz proiektuan oinarritutako salmentak beste salmenta mota batzuekin kudeatzeko gaitasuna.</span><span class="sxs-lookup"><span data-stu-id="2984f-119">Ability to manage project-based sales with other types of sales using the capabilities in the Sales application.</span></span>
- <span data-ttu-id="2984f-120">Proiektuak kudeatzeko sistema integratua, proiektuen salmentetatik hasi eta kontabilitaterako barne programak eta fakturagarriak kudeatzen dituena.</span><span class="sxs-lookup"><span data-stu-id="2984f-120">An integrated project management system that manages internal and billable projects for schedules and financials from project sales to accounting.</span></span>
- <span data-ttu-id="2984f-121">Gastuak kudeatzeko sistema, proiektuak eta proiektuak ez diren gastuen jarraipena egiteko politikak betearaztea eta itzultzea barne.</span><span class="sxs-lookup"><span data-stu-id="2984f-121">An expense management system that includes policy enforcements and reimbursements for tracking project and non-project expenses.</span></span>
- <span data-ttu-id="2984f-122">Enpresa mailako salmenten gaineko zergaren eta truke tasaren motor aberatsa behar du, proiektuetarako bezeroei begira fakturak sortzeko.</span><span class="sxs-lookup"><span data-stu-id="2984f-122">Require a rich, enterprise-class sales tax and exchange rate engine to generate customer-facing invoices for projects.</span></span>
- <span data-ttu-id="2984f-123">Nazioarteko Financial Reporting Arauak (IFRS) bateragarriak diren proiektuen kontabilitate eta diru sarrerak ezagutzeko sistema.</span><span class="sxs-lookup"><span data-stu-id="2984f-123">An International Financial Reporting Standards(IFRS)-compliant project accounting and revenue recognition system.</span></span>
- <span data-ttu-id="2984f-124">Finance edo Supply Chain Management aplikazioak eta proiektuetan oinarritutako transakzioen integrazioa.</span><span class="sxs-lookup"><span data-stu-id="2984f-124">Finance or Supply Chain Management applications and integration of project-based transactions.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]