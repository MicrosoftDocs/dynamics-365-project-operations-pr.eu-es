---
title: Project Service Automation eguneratzearen 20, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 20. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: 12edae76dbc6de63d3e2d36058c4092f80ede77d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070985"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="61452-103">Project Service Automation 20, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="61452-103">Project Service Automation Update Release 20, V3</span></span>

<span data-ttu-id="61452-104">Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="61452-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="61452-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="61452-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="61452-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="61452-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="61452-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="61452-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="61452-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="61452-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="61452-109">Gai honek Project Service Automation V3, 20. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="61452-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="61452-110">Bertsio honen konpilazio-zenbakia V 3.10.31.37 da eta, oro har, 2020ko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.</span><span class="sxs-lookup"><span data-stu-id="61452-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="61452-111">20. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="61452-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="61452-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="61452-112">Bug fixes</span></span>

<span data-ttu-id="61452-113">**Proiektuen kudeaketa**</span><span class="sxs-lookup"><span data-stu-id="61452-113">**Project Management**</span></span>

<span data-ttu-id="61452-114">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="61452-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="61452-115">Orduak eskatzen dituen esleipen-metodoak dituen proiektuko taldekideak inportatzean garbi geratzen ez den errore-mezu agertzen da zero ordu zehazten direnean.</span><span class="sxs-lookup"><span data-stu-id="61452-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="61452-116">Erabiltzaileek akats okerra jasotzen dute gehieneko karaktere kopurua idatzi dutenean proiektu-zeregin baten **Deskribapena** eremuan.</span><span class="sxs-lookup"><span data-stu-id="61452-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="61452-117">**Microsoft Dynamics 365 Project Service Automation gehigarrien deskarga** orrialdeak ingeleseko deskargen orrialdera birbideratzen du erabiltzailearen hizkuntza-ezarpenak japonieraz ezarrita daudenean.</span><span class="sxs-lookup"><span data-stu-id="61452-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="61452-118">Zerbitzariaren errorea gertatzen denean, **Antolaketa** fitxaren sinkronizazio-etiketa, **Proiektuak** inprimakian, batzuetan geratu egiten da.</span><span class="sxs-lookup"><span data-stu-id="61452-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="61452-119">Beharrezkoak ez diren zeregin-eguneratzeak bidaltzen ari dira zeregin bat aldatzen denean.</span><span class="sxs-lookup"><span data-stu-id="61452-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="61452-120">**Sales**</span><span class="sxs-lookup"><span data-stu-id="61452-120">**Sales**</span></span>

<span data-ttu-id="61452-121">Arazo hauek konpondu dira:</span><span class="sxs-lookup"><span data-stu-id="61452-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="61452-122">**Kontratua** inprimakian, **Sortu faktura** bi aldiz sakatzean, benetako datuen erregistro baten bi faktura sortzen ditu.</span><span class="sxs-lookup"><span data-stu-id="61452-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="61452-123">Internet Explorer 11-n, erabiltzaileek ezin dute sortu gastuen sarrerarik.</span><span class="sxs-lookup"><span data-stu-id="61452-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="61452-124">Kostuen itzulera eta Fakturatu gabeko salmenten benetako datuen itzulketa lotu gabe daude.</span><span class="sxs-lookup"><span data-stu-id="61452-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="61452-125">**Freskatu benetako datuak** botoiak, **Proiektua** inprimakian, ez du freskatzen **Zereginaren benetako ordutegia**.</span><span class="sxs-lookup"><span data-stu-id="61452-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="61452-126">**PreValidateProjectTeamMemberCreate** plug-inak baliabide deskargagarri orokor bikoiztuak sor ditzake **msdyn_isgenericresourceprojectscoped** atributua **Gezurra** gisa ezarrita dagoenean.</span><span class="sxs-lookup"><span data-stu-id="61452-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="61452-127">**Birkalkulatu** eremuak produktuetan oinarritutako eskaintzaren lerroaren xehetasunen eta kontratuaren lerroaren xehetasunen kobra daitezkeen kostuak garbitzen ditu.</span><span class="sxs-lookup"><span data-stu-id="61452-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="61452-128">Egoera zehatzetan, **PostEstimateLineUpdate** pluginak erreferentzia nuluaren salbuespen-errorea erakusten du.</span><span class="sxs-lookup"><span data-stu-id="61452-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="61452-129">**Errentagarritasunaren analisia taulako** denbora-fasearen iraupena ez dator bat eskaintzako kostuen iraupenarekin prezio finkoaren eskaintzaren lerroaren xehetasunean.</span><span class="sxs-lookup"><span data-stu-id="61452-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="61452-130">Unitateko eta unitate-taldeko balioak ez dira behar bezala lehenesten gastu kategorietan **Kontratuaren lerroko xehetasunak** eta **Eskaintzaren lerroaren xehetasunak** inprimakietan.</span><span class="sxs-lookup"><span data-stu-id="61452-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="61452-131">**Erakundearen unitateko kostuaren prezioa** zerrenden baimena gainjarri egiten da data-eraginkortasunean.</span><span class="sxs-lookup"><span data-stu-id="61452-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="61452-132">Erabiltzaileek ez dute **OrgUnit** aldatzeko baimenik eskaera mota ez denean lanean oinarritutakoa, erreferentzia nuluaren salbuespen-errorea sortuko duelako.</span><span class="sxs-lookup"><span data-stu-id="61452-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="61452-133">**Eskaintzaren lerroaren xehetasunak** inprimakitik **Eskaintza** fitxara itzultzen saiatzean, inprimakia freskatu egiten da eta **Laburpena** fitxa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="61452-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>
