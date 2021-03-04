---
title: Gastuen txosteneko gastu pertsonalak
description: Gai honek langile baten gastu pertsonalak kudeatzeko bi metodo azaltzen ditu Microsoft Dynamics 365 Finance-n.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d6b9d4fa0f69b4b0fe4bd1786958d22e5580a321
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960862"
---
# <a name="personal-expenses-on-an-expense-report"></a><span data-ttu-id="9b10d-103">Gastuen txosteneko gastu pertsonalak</span><span class="sxs-lookup"><span data-stu-id="9b10d-103">Personal expenses on an expense report</span></span>

<span data-ttu-id="9b10d-104">Negozio bidaietan zehar, langileek zenbaitetan gastu pertsonalak kobratu ditzakete korporazioko kreditu txarteletan.</span><span class="sxs-lookup"><span data-stu-id="9b10d-104">During business travel, workers might sometimes charge personal expenses to their corporate credit cards.</span></span> <span data-ttu-id="9b10d-105">Gastu pertsonalak kudeatzeko prozesurik zehazten ez baduzu, baliteke gastuen txostenen onarpen prozesua etetea langileek beren gastuen txosten zehatzak aurkezten dituztenean.</span><span class="sxs-lookup"><span data-stu-id="9b10d-105">If you don't define a process for handling personal expenses, the approval process for expense reports might be disrupted when workers submit their itemized expense reports.</span></span> 

<span data-ttu-id="9b10d-106">Langilearen gastu pertsonalak kudeatzeko bi metodo daude:</span><span class="sxs-lookup"><span data-stu-id="9b10d-106">There are two methods for handling a worker's personal expenses:</span></span>

- <span data-ttu-id="9b10d-107">**Langileak ordainduta**: Zure erakundeak ez ditu ordaintzen korporazioko kreditu txartelaren fakturan agertzen diren gastu pertsonalak.</span><span class="sxs-lookup"><span data-stu-id="9b10d-107">**Paid by employee** – Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="9b10d-108">Horren ordez, gastu pertsonalak eta korporazioko kreditu txartelean kargatutako korporazio gastuak erakusten dituen txostena sortzen du.</span><span class="sxs-lookup"><span data-stu-id="9b10d-108">Instead, it creates a report that shows personal expenses together with the corporate expenses that were charged to the corporate credit card.</span></span>
- <span data-ttu-id="9b10d-109">**Enpresak ordainduta**: Zure erakundeak korporazioko kreditu txartelaren faktura osoa ordaintzen du eta gero langilearen kontua gastu pertsonalengatik kargatzen du.</span><span class="sxs-lookup"><span data-stu-id="9b10d-109">**Paid by company** – Your organization pays the whole bill for the corporate credit card and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="9b10d-110">Zure erakundeak erabiltzen duen metodoa hauta dezakezu **Gastuak kudeatzeko parametroak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="9b10d-110">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>
