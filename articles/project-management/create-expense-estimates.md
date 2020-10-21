---
title: Expense estimates
description: Gai honek proiektuan oinarritutako gastuak definitzeko edo kalkulatzeko informazioa eskaintzen du.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2afe4ff2f84fc5426c409e6314da73b11a4de281
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907834"
---
# <a name="expense-estimates"></a><span data-ttu-id="bd68d-103">Expense estimates</span><span class="sxs-lookup"><span data-stu-id="bd68d-103">Expense estimates</span></span>
<span data-ttu-id="bd68d-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="bd68d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bd68d-105">Baliabideetan oinarritutako kalkuluak definitzearekin batera, Dynamics 365 Project Operations proiektuetako kudeatzaileek proiektu bakoitzerako proiektuetan oinarritutako gastuak definitzeko aukera ematen du.</span><span class="sxs-lookup"><span data-stu-id="bd68d-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="bd68d-106">Gastu-elementu bakoitza proiektuko zeregin jakin batekin edo gastu-kategoriarekin lotu daiteke.</span><span class="sxs-lookup"><span data-stu-id="bd68d-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="bd68d-107">Gastu kategoriak normalean antolakuntza mailan definitzen dira.</span><span class="sxs-lookup"><span data-stu-id="bd68d-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="bd68d-108">Gastu-kategoria bakoitzaren prezioak normalean hierarkia honetan definitzen dira:</span><span class="sxs-lookup"><span data-stu-id="bd68d-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="bd68d-109">Erakundea</span><span class="sxs-lookup"><span data-stu-id="bd68d-109">Organization</span></span>
- <span data-ttu-id="bd68d-110">Bezeroa</span><span class="sxs-lookup"><span data-stu-id="bd68d-110">Customer</span></span>
- <span data-ttu-id="bd68d-111">Eskaintza/Kontratua</span><span class="sxs-lookup"><span data-stu-id="bd68d-111">Quote/contract</span></span>

<span data-ttu-id="bd68d-112">Bete urrats hauek proiektuaren gastua ikusi, gehitu edo ezabatzeko.</span><span class="sxs-lookup"><span data-stu-id="bd68d-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="bd68d-113">Joan **Proiektuak**, eta hautatu landu nahi duzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="bd68d-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="bd68d-114">Aukeratu **Proiektuaren aurrekontuak** fitxa eta ikusi proiektuaren gastuen zerrenda.</span><span class="sxs-lookup"><span data-stu-id="bd68d-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="bd68d-115">Aukeratu **Gastu berria** gastu bat gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="bd68d-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="bd68d-116">Edo hautatu ezabatzeko gastua eta hautatu **Ezabatu gastua**.</span><span class="sxs-lookup"><span data-stu-id="bd68d-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="bd68d-117">Atributu hauek zehazten dira gastu lerro bakoitzerako:</span><span class="sxs-lookup"><span data-stu-id="bd68d-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="bd68d-118">**Kategoria**: Proiektu batean sortutako gastu guztiak deskribatzeko erabiltzen diren talde komunak.</span><span class="sxs-lookup"><span data-stu-id="bd68d-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="bd68d-119">**Hasiera data**: Gastua sortuko dela aurreikusten den eguna.</span><span class="sxs-lookup"><span data-stu-id="bd68d-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="bd68d-120">**Kopurua**: Kategoria jakin baterako gastuen elementu kopurua.</span><span class="sxs-lookup"><span data-stu-id="bd68d-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="bd68d-121">**Unitatearen kostuaren prezioa**: Gastuaren kostua kalkulatzeko erabilitako unitateko prezioa.</span><span class="sxs-lookup"><span data-stu-id="bd68d-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="bd68d-122">**Unitatearen salmentaren prezioa**: Salmenta-prezioen kostua kalkulatzeko erabilitako unitateko prezioa.</span><span class="sxs-lookup"><span data-stu-id="bd68d-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>

