---
title: Enpresen arteko gastuak
description: Erakunde bateko pertsona juridiko batek lan egiten duen langileak erakunde bereko beste pertsona juridiko baterako lana egin dezake. Egoera horretan, enpresen arteko gastuen eginbidea erabil dezakezu langilearen gastuak lana egin duen pertsona juridikoari esleitzeko.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071187"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="5a582-104">Enpresen arteko gastuak</span><span class="sxs-lookup"><span data-stu-id="5a582-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="5a582-105">Erakunde bateko pertsona juridiko batek lan egiten duen langileak erakunde bereko beste pertsona juridiko baterako lana egin dezake.</span><span class="sxs-lookup"><span data-stu-id="5a582-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="5a582-106">Egoera horretan, enpresen arteko gastuen eginbidea erabil dezakezu langilearen gastuak lana egin duen pertsona juridikoari esleitzeko.</span><span class="sxs-lookup"><span data-stu-id="5a582-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="5a582-107">Langilea enplegatzen duen pertsona juridikoari mailegu-pertsona deitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="5a582-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="5a582-108">Langileak gastuak egiten dituen pertsona juridikoari mailegu-pertsona deitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="5a582-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="5a582-109">Langile batek beste pertsona juridiko batentzat egiten duen lanaren gastuak sortu eta aurkeztu ahal izango ditu aurretik, maileguan dagoen pertsona juridikoan, **Gastuak kudeatzeko parametroak** orria, hautatu **Onartu enpresen arteko gastu lerroak** aukera.</span><span class="sxs-lookup"><span data-stu-id="5a582-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="5a582-110">Enpresen arteko gastuen zerga argitaratzea</span><span class="sxs-lookup"><span data-stu-id="5a582-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="5a582-111">Mailegu (iturburu) pertsona juridikoarekin lotura duten zerga taldeak erabili behar badituzu zure gastuen txostenean maileguarekin (helmuga) duen pertsona juridikoarekin ordez, hau konfiguratu beharko duzu liburu nagusiko salmenten gaineko zerga konfiguratuta.</span><span class="sxs-lookup"><span data-stu-id="5a582-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="5a582-112">Liburu nagusiaren parametroa denean, **Enpresen arteko zergak argitaratzeko pertsona juridikoa** ezarrita dago **Iturria** eta **Salmenten gaineko zergaren gaineko zerga arauak aplikatzea** ezarrita dago **Ez** , mailegu-entitate juridikoaren zerga-konbinazioa erabiliko da.</span><span class="sxs-lookup"><span data-stu-id="5a582-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="5a582-113">Parametro bera ezarrita dagoenean **Helmuga** , zorpetutako entitate juridikoaren zerga-konbinazioa erabiliko da.</span><span class="sxs-lookup"><span data-stu-id="5a582-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="5a582-114">Estatu Batuetako pertsona juridikoetarako, parametroa ezarrita dagoenean **Iturria** , **Kobratu beharreko salmenten gaineko zerga** eremua berrian konfiguratu behar da **Liburuak argitaratzeko taldeak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="5a582-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="5a582-115">Kontabilitate motorrak eremu honetako informazioa erabiliko du zergekin lotutako kontabilitate sarrera egiteko.</span><span class="sxs-lookup"><span data-stu-id="5a582-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="5a582-116">Jokabidea koherentea da proiektuarekin edo proiekturik gabe argitaratutako gastu lerroetan.</span><span class="sxs-lookup"><span data-stu-id="5a582-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
