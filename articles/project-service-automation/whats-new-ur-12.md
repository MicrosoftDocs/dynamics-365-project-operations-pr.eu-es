---
title: Project Service Automation eguneratzea 12, V3 bertsioari buruzko berritasunak
description: Gai honek Project Service Automation eguneratzea 12, V3 bertsioko berritasunei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: af8dbfe3-7ce9-4374-9c03-17b2e1d6ac32
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 758717562c12a72848f1a874fa8b1171139ebb0c
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748865"
---
# <a name="project-service-automation-v3-update-release-12"></a><span data-ttu-id="c7f1f-103">Project Service Automation V3, eguneratzea 12</span><span class="sxs-lookup"><span data-stu-id="c7f1f-103">Project Service Automation V3, Update Release 12</span></span>
<span data-ttu-id="c7f1f-104">Atsegin handiz adierazten dugu Dynamics 365 Project Service Automation (PSA) aplikazioaren azken eguneratzea.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="c7f1f-105">Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="c7f1f-106">Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="c7f1f-107">Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroa eta joan soluzioen orrira eguneratzea instalatzeko.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="c7f1f-108">Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="c7f1f-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="c7f1f-109">Gai honek Project Service Automation V3, 12. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 12.</span></span> <span data-ttu-id="c7f1f-110">Bertsio honek V3.10.2.34 konpilazio-zenbakia du eta, oro har, 2019ko urrian jarriko da erabilgarri automatikoki eguneratzeko moduan.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-110">This version has a build number of V3.10.2.34 and is generally available through a self-update in October 2019.</span></span>

## <a name="update-release-12"></a><span data-ttu-id="c7f1f-111">12. eguneratze-bertsioa</span><span class="sxs-lookup"><span data-stu-id="c7f1f-111">Update Release 12</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="c7f1f-112">Akatsen zuzenketa</span><span class="sxs-lookup"><span data-stu-id="c7f1f-112">Bug fixes</span></span>

- <span data-ttu-id="c7f1f-113">Denbora eta gastua</span><span class="sxs-lookup"><span data-stu-id="c7f1f-113">Time and Expense</span></span>

    - <span data-ttu-id="c7f1f-114">Konponduta: Denbora-sarreraren errore-mezularitza eguneratu egin da testuinguru adierazgarriagoarekin.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-114">Fixed: Time entry error messaging has been updated with more relevant context.</span></span>
    - <span data-ttu-id="c7f1f-115">Konponduta: Denbora-sarreraren sareta eta antolaketa ongi bistaratzen da korritze-barra bertikalean, eskatzean.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-115">Fixed: Time entry grid and schedule correctly displays the vertical scrollbar when required.</span></span>
    - <span data-ttu-id="c7f1f-116">Konponduta: Bidalitako gastua eta denbora-sarrerak onar daitezke.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-116">Fixed: Submitted expense and time entries can be approved.</span></span>
    - <span data-ttu-id="c7f1f-117">Konponduta: Utzi onespenaren berrespenaren elkarrizketa-mezua zuzendu da onespenaren egoera islatzeko **Onartuta** egoeratik **Bidalita** egoerara.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-117">Fixed: Cancel approval confirmation dialog message has been corrected to reflect the status of the approval when changed from **Approved** to **Submitted**.</span></span>
    - <span data-ttu-id="c7f1f-118">Konponduta: **Prezioa**, **Unitatea** eta **Kopurua** eremuak blokeatuta daude Gastuen erregistroan, onartu ondoren.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-118">Fixed: **Price**, **Unit**, and **Quantity** fields are now locked on the Expense record after it is has been approved.</span></span>

- <span data-ttu-id="c7f1f-119">Proiektuen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="c7f1f-119">Project Management</span></span>

    - <span data-ttu-id="c7f1f-120">Konponduta: **Berria** ekintza **Taldekidea** inprimaki nagusitik kendu da.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-120">Fixed: **New** action on **Team member** main form has been removed.</span></span>
    - <span data-ttu-id="c7f1f-121">Konponduta: Baliabideen esleipenak eguneratu egin dira kontura zehatzak ez diren sarrera-erroreengatik, eta horrek zereginen amaiera-data aldatzea eragin du.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-121">Fixed: Resource assignments have been updated to account for inaccurate rounding errors, which lead to a shift in a task’s end date.</span></span>
    - <span data-ttu-id="c7f1f-122">Konponduta: Zereginen sarean, zerbitzariaren aldeko akatsak agertuko zaizkio erabiltzaileari.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-122">Fixed: In the task grid, relevant server-side errors will be surfaced to the user.</span></span>
    - <span data-ttu-id="c7f1f-123">Konponduta: Taldekidearen izenak zereginen pertsonen hautatzailean errendatzen da posizioaren izena beharrean.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-123">Fixed: The team member’s name now renders in the task people picker instead of the position name.</span></span>

- <span data-ttu-id="c7f1f-124">Baliabideen kudeaketa</span><span class="sxs-lookup"><span data-stu-id="c7f1f-124">Resource Management</span></span>

    - <span data-ttu-id="c7f1f-125">Konponduta: Txantiloi batetik sortutako proiektuaren baliabide-eskakizunen xehetasunek proiektuaren egutegia erabiltzen dute orain.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-125">Fixed: Resource requirement details for projects created from a template now use the project calendar.</span></span>
    - <span data-ttu-id="c7f1f-126">Konponduta: Trebetasunak eta gaitasunak lehenetsi egiten dira funtzio nagusitik funtzio horretarako sortutako baliabide-eskakizunera.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-126">Fixed: Skills and competencies now default from role master data to the resource requirement created for that role.</span></span>

- <span data-ttu-id="c7f1f-127">Sales</span><span class="sxs-lookup"><span data-stu-id="c7f1f-127">Sales</span></span>

    - <span data-ttu-id="c7f1f-128">Konponduta: Objektuen ID bikoiztuak aurkitu dira **Kontratu nagusia** inprimakian.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-128">Fixed: Duplicate object IDs found on the **Contract main** form.</span></span>
    - <span data-ttu-id="c7f1f-129">Konponduta: Logika eguneratu egin da **Eskaintzaren azterketa** fitxa ikusgai egiteko, fitxaren metadatuen konfigurazioa bistara dadin.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-129">Fixed: Logic has been updated to make the **Quote Analysis** tab visible so that it displays the metadata setup of the tab.</span></span>
    - <span data-ttu-id="c7f1f-130">Konponduta: Egiazko erregistroan kontabilitate-data denboraren/gastuen sarrera-datatik dator eta ez onespen-datatik.</span><span class="sxs-lookup"><span data-stu-id="c7f1f-130">Fixed: Accounting date on the actual record now comes from the date of the time/expense entry date and not the date of the approval.</span></span>
