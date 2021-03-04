---
title: Enpresen arteko gastuak
description: Gai honetan enpresen arteko gastuak langilearen gastuak lana burutu den entitate juridikoari esleitzeko moduari buruzko informazioa ematen da.
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
ms.openlocfilehash: 553ddbe622210169db8de4aa506dcf1ea1e9d5ef
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960817"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="62b29-103">Enpresen arteko gastuak</span><span class="sxs-lookup"><span data-stu-id="62b29-103">Intercompany expenses</span></span>

<span data-ttu-id="62b29-104">Erakunde bateko pertsona juridiko batek lan egiten duen langileak erakunde bereko beste pertsona juridiko baterako lana egin dezake.</span><span class="sxs-lookup"><span data-stu-id="62b29-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="62b29-105">Enpresen arteko gastuak langilearen gastuak lana burutu den entitate juridikoari esleitzeko erabil dezakezu.</span><span class="sxs-lookup"><span data-stu-id="62b29-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="62b29-106">Langilea enplegatzen duen pertsona juridikoari mailegu-pertsona deitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="62b29-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="62b29-107">Langileak gastuak egiten dituen pertsona juridikoari mailegu-pertsona deitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="62b29-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="62b29-108">Langile batek enpresen arteko gastuak sortu eta bidali aurretik, enpresen arteko gastuen lerroak gaitu behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="62b29-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="62b29-109">Pertsona juridiko mailegatzailean **Gastuak kudeatzeko parametroak** orrialdea, hautatu **Onartu enpresen arteko gastu lerroak**.</span><span class="sxs-lookup"><span data-stu-id="62b29-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="62b29-110">Enpresen arteko gastuen zerga argitaratzea</span><span class="sxs-lookup"><span data-stu-id="62b29-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="62b29-111">Mailegu (iturburu) erakunde juridikoarekin lotutako mailegu (destino) entitate juridikoarekin lotutako zerga taldeak erabili aurretik, zure gastuaren txostenean, funtzionalitatea gaitu behar duzu liburu nagusien salmenten gaineko zergaren konfigurazioan.</span><span class="sxs-lookup"><span data-stu-id="62b29-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="62b29-112">**Enpresen arteko zergak argitaratzeko pertsona juridikoa** parametroa ezarrita dagoenean **Iturria** eta **Salmenten gaineko zergaren gaineko zerga arauak aplikatzea** ezarrita dago **Ez**, mailegu-entitate juridikoaren zerga-konbinazioa erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="62b29-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="62b29-113">Parametro bera ezarrita dagoenean **Helmuga**, zorpetutako entitate juridikoaren zerga-konbinazioa erabiliko da.</span><span class="sxs-lookup"><span data-stu-id="62b29-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="62b29-114">Estatu Batuetako pertsona juridikoetarako, parametroa ezarrita dagoenean **Iturria**, **Kobratu beharreko salmenten gaineko zerga** eremua berrian konfiguratu behar da **Liburuak argitaratzeko taldeak** orrialdea.</span><span class="sxs-lookup"><span data-stu-id="62b29-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="62b29-115">Kontabilitate motorrak eremu honetako informazioa erabiliko du zergekin lotutako kontabilitate sarrera egiteko.</span><span class="sxs-lookup"><span data-stu-id="62b29-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="62b29-116">Jokabidea koherentea da proiektuarekin edo proiekturik gabe argitaratutako gastu lerroetan.</span><span class="sxs-lookup"><span data-stu-id="62b29-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
