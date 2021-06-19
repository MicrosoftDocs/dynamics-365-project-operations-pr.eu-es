---
title: Finantza-dimentsio lehenetsiak
description: Gai honek dimentsio finantzarioaren lehenespenak konfiguratzeko moduari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d2509f74d34ac3dce4c6915ca860283750eb50b1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013291"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="1cd35-103">Finantza-dimentsio lehenetsiak</span><span class="sxs-lookup"><span data-stu-id="1cd35-103">Financial dimension defaults</span></span>

<span data-ttu-id="1cd35-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="1cd35-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="1cd35-105">Dynamics 365 Project Operations-ek erabiltzen du [Finantza-dimentsioak](/dynamics365/finance/general-ledger/financial-dimensions) esparrua Dynamics 365 Finance proiektu gehigarrien eta liburu nagusien transakzioen inguruko informazio osagarria eskaintzeko.</span><span class="sxs-lookup"><span data-stu-id="1cd35-105">Dynamics 365 Project Operations uses the [Financial dimensions](/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="1cd35-106">Finantza dimentsio lehenetsiak bezero, proiektuaren finantzaketa iturri, mugarri, proiektu kontratu lerro edo proiektu batean ezar daitezke.</span><span class="sxs-lookup"><span data-stu-id="1cd35-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="1cd35-107">Definitu bezeroarentzako lehenetsitako finantza dimentsioak</span><span class="sxs-lookup"><span data-stu-id="1cd35-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="1cd35-108">Bezeroen dimentsio lehenetsiak Finantzan zehazten dira.</span><span class="sxs-lookup"><span data-stu-id="1cd35-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="1cd35-109">Osatu urrats hauek dimentsioaren balio lehenetsiak ezartzeko.</span><span class="sxs-lookup"><span data-stu-id="1cd35-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="1cd35-110">Joan **Kobratu beharreko kontuak** > **Bezeroak** > **Bezero guztiak**.</span><span class="sxs-lookup"><span data-stu-id="1cd35-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="1cd35-111">**Bezeroak** orrialdean, **Finantza dimentsioak** fitxa, ezarri bezero zehatzentzako finantza dimentsioaren balioak.</span><span class="sxs-lookup"><span data-stu-id="1cd35-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="1cd35-112">Definitu proiektu-kontratuen lehenetsitako finantza dimentsioak</span><span class="sxs-lookup"><span data-stu-id="1cd35-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="1cd35-113">Proiektuen kontratuak urtean sortu eta mantentzen dira Common Data Service (CDS).</span><span class="sxs-lookup"><span data-stu-id="1cd35-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="1cd35-114">Proiektuen kontratuen kontabilitate atributuak **Proiektuen kudeaketa eta kontabilitatea** modulua Finantzetan.</span><span class="sxs-lookup"><span data-stu-id="1cd35-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="1cd35-115">Ezarri proiektuaren finantzaketa iturriaren dimentsio ekonomikoak</span><span class="sxs-lookup"><span data-stu-id="1cd35-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="1cd35-116">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu-kontratuak**.</span><span class="sxs-lookup"><span data-stu-id="1cd35-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="1cd35-117">Hautatu eguneratu nahi duzun erregistroa eta **Proiektuaren kontratua** fitxa, hautatu **Erakutsi lehenetsitako kontabilitatea**.</span><span class="sxs-lookup"><span data-stu-id="1cd35-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="1cd35-118">Zabaldu **Lotutako informazioa** eta hautatu **Finantzaketa iturriak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="1cd35-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="1cd35-119">Ezarri finantza-dimentsio lehenetsiak.</span><span class="sxs-lookup"><span data-stu-id="1cd35-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="1cd35-120">Kontuan izan finantza dimentsioak bezeroaren kontutik lehenetsita daudela.</span><span class="sxs-lookup"><span data-stu-id="1cd35-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="1cd35-121">Ezarri proiektuaren kontratuaren lerroaren dimentsio ekonomikoak</span><span class="sxs-lookup"><span data-stu-id="1cd35-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="1cd35-122">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu-kontratuak**.</span><span class="sxs-lookup"><span data-stu-id="1cd35-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="1cd35-123">Hautatu eguneratu nahi duzun erregistroa eta **Proiektuaren kontratua** fitxa, hautatu **Erakutsi lehenetsitako kontabilitatea**.</span><span class="sxs-lookup"><span data-stu-id="1cd35-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="1cd35-124">Zabaldu **Lotutako informazioa** eta hautatu **Kontratuaren lerroak** fitxa.</span><span class="sxs-lookup"><span data-stu-id="1cd35-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="1cd35-125">Ezarri finantza-dimentsio lehenetsiak.</span><span class="sxs-lookup"><span data-stu-id="1cd35-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="1cd35-126">Finantza dimentsioaren lehenespenak aplikagarriak dira eta prezio finkoaren (mugarria) kontratu lerroekin bakarrik erabil daitezke.</span><span class="sxs-lookup"><span data-stu-id="1cd35-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="1cd35-127">Lehenespen horiek erlazionatutako proiektuaren kontuko transakzioetan eta faktura lerroetan erabiltzen dira.</span><span class="sxs-lookup"><span data-stu-id="1cd35-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="1cd35-128">Definitu proiektuen lehenetsitako finantza dimentsioak</span><span class="sxs-lookup"><span data-stu-id="1cd35-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="1cd35-129">Proiektuak CDS-n sortu eta mantentzen dira.</span><span class="sxs-lookup"><span data-stu-id="1cd35-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="1cd35-130">Proiektuen kontabilitate atributuak **Proiektuen kudeaketa eta kontabilitatea** modulua Finantzetan.</span><span class="sxs-lookup"><span data-stu-id="1cd35-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="1cd35-131">Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu guztiak**.</span><span class="sxs-lookup"><span data-stu-id="1cd35-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="1cd35-132">Hautatu eguneratu nahi duzun erregistroa eta **Proiektua** fitxa, hautatu **Erakutsi lehenetsitako kontabilitatea**.</span><span class="sxs-lookup"><span data-stu-id="1cd35-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="1cd35-133">Zabaldu **Lotutako informazioa** eta hautatu **Konfiguratu** fitxa.</span><span class="sxs-lookup"><span data-stu-id="1cd35-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="1cd35-134">Ezarri finantza-dimentsio lehenetsiak.</span><span class="sxs-lookup"><span data-stu-id="1cd35-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="1cd35-135">Kontuan izan finantza dimentsioak bezeroaren kontutik lehenetsita daudela.</span><span class="sxs-lookup"><span data-stu-id="1cd35-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="1cd35-136">Proiektua proiektu kontratuko bezero anitzekin kontratu lerro batekin lotzen bada, bezero nagusia lehenetsitako finantza dimentsioetarako erabiltzen da.</span><span class="sxs-lookup"><span data-stu-id="1cd35-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="1cd35-137">Proiektuaren lehenetsitako finantza dimentsioak egunkariaren lerroaren lehenespenak ezartzeko erabiltzen dira denbora, gastu eta kuoten transakzioetarako **Project Operations Integration Journal** eta lotutako proiektuen faktura-lerroetan.</span><span class="sxs-lookup"><span data-stu-id="1cd35-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]