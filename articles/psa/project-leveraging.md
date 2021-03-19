---
title: Salmenten aurreikuspenak eta proiektuak
description: Gai honek salmenta prozesuko antolaketa eta aurreikuspenak aprobetxatzeari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 87dc72b76ec4f88684ef2c702718e1ab631ff936
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283893"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="5dbbd-103">Salmenten aurreikuspenak eta proiektuak</span><span class="sxs-lookup"><span data-stu-id="5dbbd-103">Sales estimates and projects</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="5dbbd-104">Salmenta prozesuan zehar, salmenten aurreikuspenak sor ditzakezu proiektu bat salmenta-eskaintzari lotuz.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="5dbbd-105">Horrela, salmenta prozesuan aurreikuspen determinista gerta daiteke proiektuen antolaketa eta aurreikuspen gaitasunak aprobetxatzeko.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="5dbbd-106">Salmentak aurrera egiten badu, salmenten aurreikuspena egiteko erabilitako antolaketa erabil daiteke proiektuaren plana berriro finkatzeko oinarri gisa.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="5dbbd-107">Estekatu proiektua eskaintzaren lerro bati</span><span class="sxs-lookup"><span data-stu-id="5dbbd-107">Linking a project to a quote line</span></span>

<span data-ttu-id="5dbbd-108">Proiektuetan oinarritutako eskaintzaren lerroa sortzen duzunean, beste proiektu bat sor dezakezu edo lehendik dagoen proiektu batekin lotu **Eskaintzaren lerroa** orrian.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![Eskaintzaren lerroaren inprimakia](media/project-8.png)
 
<span data-ttu-id="5dbbd-110">Eskaintzaren lerroko xehetasunetatik abiatuta beste proiektu bat sortzen duzunean, proiektuaren txantiloiak aprobetxatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="5dbbd-111">Proiektuaren txantiloiak erakunde baten proiektu tipikoen planak eta finantza-aurreikuspenak adierazten dituzten proiektu ereduak dira.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="5dbbd-112">Aurreko proiektuetako proiektu-planen eta aurreikuspenen kopiak ere irudikatu ahal izango dituzte.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![Eskaintzaren lerroaren xehetasunak](media/project-9.png)
  
<span data-ttu-id="5dbbd-114">Proiektu bat eskaintza batetik sortzean, proiektua automatikoki lotuko da eskaintzaren lerroarekin.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="5dbbd-115">Proiektu bateko aurreikuspenen osagaiak</span><span class="sxs-lookup"><span data-stu-id="5dbbd-115">Components of estimates in a project</span></span>

<span data-ttu-id="5dbbd-116">Antolaketak lana zereginetan banatzen, zereginen hierarkia mantentzen, zereginak burutzeko zer baliabide behar diren zehazten eta zeregin bat burutzeko behar den ahaleginaren aurreikuspena esleitzen laguntzen dizu.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="5dbbd-117">Laneko ahalegina eta antolaketaren aurreikuspenak zehaztu ditzakezu **Antolaketa** fitxako eremuak erabiliz **Proiektua** orrian.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="5dbbd-118">Prezio-zerrenda bat proiektuarekin lotuta dagoenez, finantza-aurreikuspenak kalkulatzen dira prezioen zerrendan zehazten diren kostu eta salmenta prezioak erabiliz.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="5dbbd-119">Inportatu aurreikuspenak proiektu batetik eskaintza batera</span><span class="sxs-lookup"><span data-stu-id="5dbbd-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="5dbbd-120">Proiektuaren aurreikuspenak zehaztu ondoren, eskaintzaren lerrora inporta ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="5dbbd-121">**Eskaintzaren lerroaren xehetasunak** orrian, hautatu **Inportatu kalkuluetatik** aukera zintan proiektuaren aurreikuspenak laburbiltzeko transakzio mota, funtzioa edo zeregin mailaren arabera.</span><span class="sxs-lookup"><span data-stu-id="5dbbd-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]