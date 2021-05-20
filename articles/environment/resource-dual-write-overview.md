---
title: Project Operations idazketa dualeko integrazioa
description: Gai honek Project Operations idazketa bikoitzeko integrazioaren ikuspegi orokorra eskaintzen du.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d9d6a7c367872219b4aca32aecb15d6837ebe296
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955643"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="adaab-103">Project Operations idazketa dualeko integrazioaren ikuspegi orokorra</span><span class="sxs-lookup"><span data-stu-id="adaab-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="adaab-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="adaab-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="adaab-105">Project Operations-en erabilerak [idazketa bikoitzeko gaitasunak](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) datuak zehar sinkronizatzeko Microsoft Dataverse eta Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="adaab-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="adaab-106">Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak arteko integrazio horren zati gisa Dataverse eta Finance artean.</span><span class="sxs-lookup"><span data-stu-id="adaab-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![Project Operations-en datu-fluxuen ikuspegi orokorra](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="adaab-108">Project Operations Dataverse-n Erabiltzaile interfaze modernoa (UI) eta koderik gabeko / kode baxuko hedapen erraza erabiltzen ditu Power Platform gaitasunak.</span><span class="sxs-lookup"><span data-stu-id="adaab-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="adaab-109">Proiektuen kudeatzaileek, baliabideen kudeatzaileek, proiektuko taldekideek eta lehen lerroko beste pertsona batzuek Project Operations-en egiten dituzte jarduerak Dataverse-n.</span><span class="sxs-lookup"><span data-stu-id="adaab-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="adaab-110">Project Operations Finance-n proiektuen kontabilitatea eta diru-sarrerak ezagutzeko laguntza eskaintzen du.</span><span class="sxs-lookup"><span data-stu-id="adaab-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="adaab-111">Project Operations Finance finantza esparruan sartzen dira salmenten gaineko zerga kalkulatzeko, moneta truke tasak, finantza dimentsioen berri emateko eta beste.</span><span class="sxs-lookup"><span data-stu-id="adaab-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="adaab-112">Proiektuaren kontularien esperientziak gehienbat Finantzetan oinarritzen dira.</span><span class="sxs-lookup"><span data-stu-id="adaab-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="adaab-113">Project Operations-en integrazioa osagai hau osatzen dute:</span><span class="sxs-lookup"><span data-stu-id="adaab-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="adaab-114">Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa</span><span class="sxs-lookup"><span data-stu-id="adaab-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="adaab-115">Proiektuaren kalkuluak eta benetako datuak</span><span class="sxs-lookup"><span data-stu-id="adaab-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="adaab-116">Proiektuaren fakturak</span><span class="sxs-lookup"><span data-stu-id="adaab-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="adaab-117">Gastuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="adaab-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="adaab-118">Saltzailearen faktura</span><span class="sxs-lookup"><span data-stu-id="adaab-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
