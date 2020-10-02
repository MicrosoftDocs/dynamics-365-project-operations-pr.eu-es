---
title: Konfiguratu fakturak automatikoko sortzeko aukera
description: Gai honek beroari buruzko informazioa eskaintzen du, fakturak automatikoki sortzeko sistema konfiguratzeko.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898111"
---
# <a name="configure-automated-invoice-creation"></a><span data-ttu-id="bf976-103">Konfiguratu fakturak automatikoko sortzeko aukera</span><span class="sxs-lookup"><span data-stu-id="bf976-103">Configure automated invoice creation</span></span>

<span data-ttu-id="bf976-104">_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_</span><span class="sxs-lookup"><span data-stu-id="bf976-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bf976-105">Bete urrats hauek Project eragiketetan faktura automatikoa exekutatzeko.</span><span class="sxs-lookup"><span data-stu-id="bf976-105">Complete the following steps to configure an automated invoice run in Project operations.</span></span>

1. <span data-ttu-id="bf976-106">Joan **Ezarpenak** \> **Lan sortak** atalera.</span><span class="sxs-lookup"><span data-stu-id="bf976-106">Go to **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="bf976-107">Sortu lan-sortat eta eman izen hau: **Project eragiketek fakturak sortzea**.</span><span class="sxs-lookup"><span data-stu-id="bf976-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="bf976-108">Lan-sortaren izenak "Sortu fakturak" terminoa izan behar du.</span><span class="sxs-lookup"><span data-stu-id="bf976-108">The name of the batch job must include the term "create invoices."</span></span>
3. <span data-ttu-id="bf976-109">**Lan mota** eremuan, hautatu **Bat ere ez** aukera.</span><span class="sxs-lookup"><span data-stu-id="bf976-109">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="bf976-110">Berez, **Maiztasuna egunero** eta **Aktibatuta dago** aukerak ezarrita daude **Bai** aukerarekin.</span><span class="sxs-lookup"><span data-stu-id="bf976-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="bf976-111">Hautatu **Lan-fluxua exekutatu**.</span><span class="sxs-lookup"><span data-stu-id="bf976-111">Select **Run Workflow**.</span></span> <span data-ttu-id="bf976-112">**Begiratu erregistroa** elkarrizketa-koadroan, hiru lan-fluxu ikusiko dituzu:</span><span class="sxs-lookup"><span data-stu-id="bf976-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="bf976-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="bf976-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="bf976-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="bf976-114">ProcessRunner</span></span>
    - <span data-ttu-id="bf976-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="bf976-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="bf976-116">Hautatu **ProcessRunCaller** eta gero hautatu **Gehitu**.</span><span class="sxs-lookup"><span data-stu-id="bf976-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="bf976-117">Berrespenaren hurrengo elkarrizketa-koadroan, hautatu **Ados**.</span><span class="sxs-lookup"><span data-stu-id="bf976-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="bf976-118">**Lo** lan-fluxuaren ondoren dator **Prozesua** lan-fluxua.</span><span class="sxs-lookup"><span data-stu-id="bf976-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="bf976-119">Aukeratu ere egin dezakezu **ProcessRunner** 5. urratsean.</span><span class="sxs-lookup"><span data-stu-id="bf976-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="bf976-120">Ondoren, hautatzen duzunean **Ados** aukera, **Prozesua** lan-fluxuaren ondoren dator **Lo** lan-fluxua.</span><span class="sxs-lookup"><span data-stu-id="bf976-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="bf976-121">**ProcessRunCaller** eta **ProcessRunner** lan-fluxuek fakturak sortzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="bf976-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="bf976-122">**ProcessRunCaller** lan-fluxuak **ProcessRunner** lan-fluxuari deitzen dio.</span><span class="sxs-lookup"><span data-stu-id="bf976-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="bf976-123">**ProcessRunner** fakturak benetan sortzen dituen lan-fluxua da.</span><span class="sxs-lookup"><span data-stu-id="bf976-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="bf976-124">Fakturak sortu behar diren kontraturen lerro guztietatik igarotzen da eta fakturak sortzen ditu lerro horietarako.</span><span class="sxs-lookup"><span data-stu-id="bf976-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="bf976-125">Fakturak eratu behar diren kontratuaren lerroak zehazteko, lanpostuak kontratuaren lerroen fakturazio datak aztertzen ditu.</span><span class="sxs-lookup"><span data-stu-id="bf976-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="bf976-126">Kontratu bakarreko kontratuaren lerroek fakturaren iraupen-data bera badute, transakzioak bi faktura-lerro dituen faktura batean elkartzen dira.</span><span class="sxs-lookup"><span data-stu-id="bf976-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="bf976-127">Fakturak sortzeko transakziorik ez badago, lanak fakturaren sorrera saltatzen du.</span><span class="sxs-lookup"><span data-stu-id="bf976-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="bf976-128">**ProcessRunner** exekutatzen amaitu denean, **ProcessRunCaller** lan-fluxuari deitzen dio, amaiera-ordua ematen du eta itxita dago.</span><span class="sxs-lookup"><span data-stu-id="bf976-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="bf976-129">**ProcessRunCaller** lan-fluxuak, ondoren, zehaztutako amaiera-ordutik 24 orduz iraungo duen tenporizadorea hasten du.</span><span class="sxs-lookup"><span data-stu-id="bf976-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="bf976-130">Tenporizadorearen amaieran, **ProcessRunCaller** lan-fluxua itxita dago.</span><span class="sxs-lookup"><span data-stu-id="bf976-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="bf976-131">Lan-sortaren prozesua lan errepikaria da.</span><span class="sxs-lookup"><span data-stu-id="bf976-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="bf976-132">Prozesu-sorta hau askotan exekutatzen bada, lanaren zenbait kasu sortzen dira eta akatsak sor daitezke.</span><span class="sxs-lookup"><span data-stu-id="bf976-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="bf976-133">Hori dela eta, prozesu-sorta behin bakarrik hasi beharko zenuke eta exekutatzen gelditzen bada bakarrik berrabiarazi beharko zenuke.</span><span class="sxs-lookup"><span data-stu-id="bf976-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="bf976-134">Sortako fakturazioa fakturen egutegien arabera konfiguratutako proiektuen kontratu lerroetarako bakarrik exekutatzen da.</span><span class="sxs-lookup"><span data-stu-id="bf976-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="bf976-135">Prezio finkoko fakturazio metodoa duen kontratu-lerroak mugarriak konfiguratu behar ditu.</span><span class="sxs-lookup"><span data-stu-id="bf976-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="bf976-136">Ordua eta materiala fakturatzeko metodoa duen proiektu-kontratuen lerroak fakturen egitaraua finkatuko du.</span><span class="sxs-lookup"><span data-stu-id="bf976-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="bf976-137">Gauza bera gertatzen da proiektuan oinarritutako kontratu lerroan.</span><span class="sxs-lookup"><span data-stu-id="bf976-137">The same applies to a project-based contract line.</span></span>     
