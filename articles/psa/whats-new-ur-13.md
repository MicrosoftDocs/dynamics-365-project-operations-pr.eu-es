---
title: Project Service Automation eguneratzearen 13, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation eguneratzea 13, V3 bertsioko berritasunei buruzko informazioa ematen du.
author: ruhercul
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
ms.openlocfilehash: c328821064065e19938406856d327f690f577e7a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000286"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="eb37a-103">Project Service Automation 13, V3 eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="eb37a-103">Project Service Automation Update Release 13, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="eb37a-104">Atsegin handiz adierazten dugu Dynamics 365 Project Service Automation (PSA) aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="eb37a-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="eb37a-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="eb37a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="eb37a-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="eb37a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="eb37a-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroa eta joan soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="eb37a-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="eb37a-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="eb37a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="eb37a-109">Gai honek Project Service Automation V3, 13. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="eb37a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="eb37a-110">Bertsio honek V3.10.3.18 konpilazio-zenbakia du eta antolaketa honetan dago erabilgarri:</span><span class="sxs-lookup"><span data-stu-id="eb37a-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="eb37a-111">**Erabilgarritasun orokorra (auto-eguneratzea):** 2019ko azaroa</span><span class="sxs-lookup"><span data-stu-id="eb37a-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="eb37a-112">**Eguneratze automatikoa:** 2019ko abendua</span><span class="sxs-lookup"><span data-stu-id="eb37a-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="eb37a-113">13. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="eb37a-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="eb37a-114">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="eb37a-114">Bug fixes</span></span>

- <span data-ttu-id="eb37a-115">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="eb37a-115">Time and Expense</span></span>

     - <span data-ttu-id="eb37a-116">Konponduta: **Gastuen onarpena** orrialdeko Bilaketaren funtzionalitateak ez du funtzionatzen gastuen xedea bilatzean.</span><span class="sxs-lookup"><span data-stu-id="eb37a-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="eb37a-117">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="eb37a-117">Resource Management</span></span>

     - <span data-ttu-id="eb37a-118">Konponduta: Bateratzeko zenbakiak justifikatu ostean eguneratu dira.</span><span class="sxs-lookup"><span data-stu-id="eb37a-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="eb37a-119">Konponduta: Izena duten baliabideak ezin zaizkie esleitu zereginei **Antolaketa** fitxaren bidez.</span><span class="sxs-lookup"><span data-stu-id="eb37a-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="eb37a-120">Proiektuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="eb37a-120">Project Management</span></span>

     - <span data-ttu-id="eb37a-121">Konponduta: Erreferentzia-salbuespen nulu taldekidea esleitzean **TransactionType** eremuari **Unitatea** eta **DefaultGroup** eremuen konfigurazio-informazioa falta denean.</span><span class="sxs-lookup"><span data-stu-id="eb37a-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="eb37a-122">Sales</span><span class="sxs-lookup"><span data-stu-id="eb37a-122">Sales</span></span>

     - <span data-ttu-id="eb37a-123">Konponduta: Transakzio motako erregistro bikoiztuek errorea itzultzen dute funtzio-prezioen erregistroak sortzen direnean.</span><span class="sxs-lookup"><span data-stu-id="eb37a-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="eb37a-124">Konponduta: botoiak gehitzeko **Aukera berria**, **Aurrekontua**, **Eskaera lerroa** eta **Gehitu produktua** aukerak, aurrekontuak, eskaerak produktuak eta proiektuetan oinarritutako lerroen azpisarea aginduetan daude ikusgai.</span><span class="sxs-lookup"><span data-stu-id="eb37a-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines subgrid.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]