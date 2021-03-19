---
title: Expense estimates
description: Gai honek proiektuan oinarritutako gastuak definitzeko edo kalkulatzeko informazioa eskaintzen du.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3f0429366c69346113003355679c055cd2c74ca3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287043"
---
# <a name="expense-estimates"></a><span data-ttu-id="05906-103">Expense estimates</span><span class="sxs-lookup"><span data-stu-id="05906-103">Expense estimates</span></span>
<span data-ttu-id="05906-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="05906-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="05906-105">Baliabideetan oinarritutako kalkuluak definitzearekin batera, Dynamics 365 Project Operations proiektuen kudeatzaileek proiektu bakoitzeko proiektuetan oinarritutako gastuak definitzeko aukera ematen du.</span><span class="sxs-lookup"><span data-stu-id="05906-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="05906-106">Gastu-elementu bakoitza proiektuko zeregin jakin batekin edo gastu-kategoriarekin lotu daiteke.</span><span class="sxs-lookup"><span data-stu-id="05906-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="05906-107">Gastu kategoriak normalean antolakuntza mailan definitzen dira.</span><span class="sxs-lookup"><span data-stu-id="05906-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="05906-108">Gastu-kategoria bakoitzaren prezioak normalean hierarkia honetan definitzen dira:</span><span class="sxs-lookup"><span data-stu-id="05906-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="05906-109">Erakundea</span><span class="sxs-lookup"><span data-stu-id="05906-109">Organization</span></span>
- <span data-ttu-id="05906-110">Bezeroa</span><span class="sxs-lookup"><span data-stu-id="05906-110">Customer</span></span>
- <span data-ttu-id="05906-111">Eskaintza/Kontratua</span><span class="sxs-lookup"><span data-stu-id="05906-111">Quote/contract</span></span>

<span data-ttu-id="05906-112">Bete urrats hauek proiektuaren gastua ikusi, gehitu edo ezabatzeko.</span><span class="sxs-lookup"><span data-stu-id="05906-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="05906-113">Joan **Proiektuak**, eta hautatu landu nahi duzun proiektua.</span><span class="sxs-lookup"><span data-stu-id="05906-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="05906-114">Aukeratu **Proiektuaren aurrekontuak** fitxa eta ikusi proiektuaren gastuen zerrenda.</span><span class="sxs-lookup"><span data-stu-id="05906-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="05906-115">Aukeratu **Gastu berria** gastu bat gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="05906-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="05906-116">Edo hautatu ezabatzeko gastua eta hautatu **Ezabatu gastua**.</span><span class="sxs-lookup"><span data-stu-id="05906-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="05906-117">Atributu hauek zehazten dira gastu lerro bakoitzerako:</span><span class="sxs-lookup"><span data-stu-id="05906-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="05906-118">**Kategoria**: Proiektu batean sortutako gastu guztiak deskribatzeko erabiltzen diren talde komunak.</span><span class="sxs-lookup"><span data-stu-id="05906-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="05906-119">**Hasiera data**: Gastua sortuko dela aurreikusten den eguna.</span><span class="sxs-lookup"><span data-stu-id="05906-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="05906-120">**Kopurua**: Kategoria jakin baterako gastuen elementu kopurua.</span><span class="sxs-lookup"><span data-stu-id="05906-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="05906-121">**Unitatearen kostuaren prezioa**: Gastuaren kostua kalkulatzeko erabilitako unitateko prezioa.</span><span class="sxs-lookup"><span data-stu-id="05906-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="05906-122">**Unitatearen salmentaren prezioa**: Salmenta-prezioen kostua kalkulatzeko erabilitako unitateko prezioa.</span><span class="sxs-lookup"><span data-stu-id="05906-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]