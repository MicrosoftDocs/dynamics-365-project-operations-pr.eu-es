---
title: Project Service Automation eguneratzearen 13, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation eguneratzea 13, V3 bertsioko berritasunei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: 435b70255dd0053a496362c9ced9e742cfcca843
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070996"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="54a35-103">Project Service Automation 13, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="54a35-103">Project Service Automation Update Release 13, V3</span></span>
<span data-ttu-id="54a35-104">Atsegin handiz adierazten dugu Dynamics 365 Project Service Automation (PSA) aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="54a35-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="54a35-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="54a35-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="54a35-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="54a35-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="54a35-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroa eta joan soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="54a35-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="54a35-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="54a35-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="54a35-109">Gai honek Project Service Automation V3, 13. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="54a35-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="54a35-110">Bertsio honek V3.10.3.18 konpilazio-zenbakia du eta antolaketa honetan dago erabilgarri:</span><span class="sxs-lookup"><span data-stu-id="54a35-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="54a35-111">**Erabilgarritasun orokorra (auto-eguneratzea):** 2019ko azaroa</span><span class="sxs-lookup"><span data-stu-id="54a35-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="54a35-112">**Eguneratze automatikoa:** 2019ko abendua</span><span class="sxs-lookup"><span data-stu-id="54a35-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="54a35-113">13. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="54a35-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="54a35-114">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="54a35-114">Bug fixes</span></span>

- <span data-ttu-id="54a35-115">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="54a35-115">Time and Expense</span></span>

     - <span data-ttu-id="54a35-116">Konponduta: **Gastuen onarpena** orrialdeko Bilaketaren funtzionalitateak ez du funtzionatzen gastuen xedea bilatzean.</span><span class="sxs-lookup"><span data-stu-id="54a35-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="54a35-117">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="54a35-117">Resource Management</span></span>

     - <span data-ttu-id="54a35-118">Konponduta: Bateratzeko zenbakiak justifikatu ostean eguneratu dira.</span><span class="sxs-lookup"><span data-stu-id="54a35-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="54a35-119">Konponduta: Izena duten baliabideak ezin zaizkie esleitu zereginei **Antolaketa** fitxaren bidez.</span><span class="sxs-lookup"><span data-stu-id="54a35-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="54a35-120">Proiektuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="54a35-120">Project Management</span></span>

     - <span data-ttu-id="54a35-121">Konponduta: Erreferentzia-salbuespen nulu taldekidea esleitzean **TransactionType** eremuari **Unitatea** eta **DefaultGroup** eremuen konfigurazio-informazioa falta denean.</span><span class="sxs-lookup"><span data-stu-id="54a35-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="54a35-122">Sales</span><span class="sxs-lookup"><span data-stu-id="54a35-122">Sales</span></span>

     - <span data-ttu-id="54a35-123">Konponduta: Transakzio motako erregistro bikoiztuek errorea itzultzen dute funtzio-prezioen erregistroak sortzen direnean.</span><span class="sxs-lookup"><span data-stu-id="54a35-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="54a35-124">Konponduta: **Aukera berria** , **Eskaintza** , **Eskaera-lerroa** eta **Gehitu produktua** eremuen botoi osagarriak ikusgai daudenean Aukerak, Abaguneak, Eskaera-produktuak eta proiektuan oinarritutako Lerroak azpisareta aukeren komandoetan.</span><span class="sxs-lookup"><span data-stu-id="54a35-124">Fixed: Extra buttons for **New Opportunity** , **Quote** , **Order Line** , and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines sub-grid.</span></span>


