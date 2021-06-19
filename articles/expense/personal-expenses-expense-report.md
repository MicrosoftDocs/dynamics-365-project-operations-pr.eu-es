---
title: Egin lan gastuen txosteneko gastu pertsonalekin
description: Gai honetan langileek negozioetarako bidaiatzean langileek sortutako gastu pertsonalekin lan egiteko moduari buruzko informazioa ematen da.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025669"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="12d7a-103">Egin lan gastuen txosteneko gastu pertsonalekin</span><span class="sxs-lookup"><span data-stu-id="12d7a-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="12d7a-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="12d7a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="12d7a-105">Negozio bidaietan zehar, langile batek gastu pertsonalak kobra ditzake bere korporazio kreditu txartelean.</span><span class="sxs-lookup"><span data-stu-id="12d7a-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="12d7a-106">Gastu pertsonalak kudeatzeko prozesurik zehaztu ez bada, baliteke gastuen txostena onartzeko prozesua etetea langileak bere gastuen txosten zehatza aurkezten duenean.</span><span class="sxs-lookup"><span data-stu-id="12d7a-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="12d7a-107">Langilearen gastu pertsonalekin lan egiteko erabil ditzakezun bi metodo daude:</span><span class="sxs-lookup"><span data-stu-id="12d7a-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="12d7a-108">**Langileak ordainduta**: Zure erakundeak ez ditu ordaintzen korporazioko kreditu txartelaren fakturan agertzen diren gastu pertsonalak.</span><span class="sxs-lookup"><span data-stu-id="12d7a-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="12d7a-109">Horren ordez, langileak kreditu txartelen saltzaileari zuzenean ordaintzen dizkio gastuak.</span><span class="sxs-lookup"><span data-stu-id="12d7a-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="12d7a-110">**Enpresak ordainduta**: Zure erakundeak korporazioko kreditu txartelaren faktura osoa ordaintzen du, eta gero langilearen kontua gastu pertsonalengatik kargatzen du.</span><span class="sxs-lookup"><span data-stu-id="12d7a-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="12d7a-111">Zure erakundeak erabiltzen duen metodoa hauta dezakezu **Gastuak kudeatzeko parametroak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="12d7a-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="12d7a-112">Gaitu zatitutako gastuen funtzioa zenbateko pertsonalaren eremuak balioa definitzen duenean</span><span class="sxs-lookup"><span data-stu-id="12d7a-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="12d7a-113">Ezaugarria **Gaitu zatitutako gastuen funtzioa zenbateko pertsonalaren eremuak balioa definitzen duenean** lerro mailako lan-fluxua erabiliz onartzen diren gastuen txostenei soilik aplikatzen zaie.</span><span class="sxs-lookup"><span data-stu-id="12d7a-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="12d7a-114">Txostenak hona joanda onartzen dira **Gastuen txostenak prozesatu** > **Niri esleitutako gastuen txostenak** > **Gastu irekien txostena**.</span><span class="sxs-lookup"><span data-stu-id="12d7a-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="12d7a-115">Funtzio hau gaitzeko, joan hona: **Lan eremuak** > **Ezaugarrien kudeaketa**, hautatu **Gaitu zatitutako gastuen funtzioa zenbateko pertsonalaren eremuak balioa definitzen duenean**, eta hautatu **Gaitu orain**.</span><span class="sxs-lookup"><span data-stu-id="12d7a-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="12d7a-116">Ezaugarria gaituta dagoenean, funtzionalitate hori erabiltzen duten gastu-lerroek bi lerro sortzen dituzte txostena aurkeztean.</span><span class="sxs-lookup"><span data-stu-id="12d7a-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="12d7a-117">Bi lerro sortzen dira onartzaileak lerro bakoitza bere aldetik onar dezan.</span><span class="sxs-lookup"><span data-stu-id="12d7a-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
