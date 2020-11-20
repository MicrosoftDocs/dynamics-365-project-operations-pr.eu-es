---
title: Inplementatu Project Operations - arina
description: Gai honek Project Operations lite hedapena instalatzeko moduari buruzko informazioa eskaintzen du. Aurre egin fakturazio proformari.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0633585fcef91d9218d6140764addb7cf96ab31d
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175651"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="94db9-103">Inplementatu Project Operations - arina</span><span class="sxs-lookup"><span data-stu-id="94db9-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="94db9-104">_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_</span><span class="sxs-lookup"><span data-stu-id="94db9-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="94db9-105">Project Operations-ek inplementazio eredu ugari onartzen ditu.</span><span class="sxs-lookup"><span data-stu-id="94db9-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="94db9-106">Inplementazio eredu onena zehazteko, ikusi [Inplementazio motak](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="94db9-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="94db9-107">Inplementazio honek, Lite inplementazioa - proformaren fakturazioari aurre egiten dio **Common Data Service -Project Operations-en inplementazioa soilik**.</span><span class="sxs-lookup"><span data-stu-id="94db9-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="94db9-108">Instalatu Project Operations CDS ingurune berrian</span><span class="sxs-lookup"><span data-stu-id="94db9-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="94db9-109">Instalatu lehendik dagoen CDS ingurune batean</span><span class="sxs-lookup"><span data-stu-id="94db9-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="94db9-110">Instalatu Project Operations CDS ingurune berri batean</span><span class="sxs-lookup"><span data-stu-id="94db9-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="94db9-111">[Globala edo Power Platform Administratzailea](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) Project Operations lizentziarekin, sortu CDS ingurune berria [PowerPlatform administrazio-zentroan](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="94db9-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="94db9-112">Ziurtatu **CDS datu-basea** eta **Dynamics 365 aplikazioak** gaituta daudela.</span><span class="sxs-lookup"><span data-stu-id="94db9-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="94db9-113">Informazio gehiago lortzeko, ikusi [Sortu eta kudeatu inguruneak Power Platform administrazio-zentroan](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="94db9-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="94db9-114">Aukeratu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen inplementazio-zerrendatik.</span><span class="sxs-lookup"><span data-stu-id="94db9-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="94db9-115">Instalatu Project Operations lehendik dagoen CDS ingurune batean</span><span class="sxs-lookup"><span data-stu-id="94db9-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="94db9-116">[Orokorra edo Power Platform Administratzaile](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) gisa Project Operations lizentziarekin, kokatu ingurunea [PowerPlatform administrazio-zentroa](https://admin.powerplatform.com) Project Operations instalatu nahi dituzunean.</span><span class="sxs-lookup"><span data-stu-id="94db9-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="94db9-117">Instalatu **Microsoft Dynamics 365 Project Operations** Dynamics 365 aplikazioen inplementazio-zerrendatik.</span><span class="sxs-lookup"><span data-stu-id="94db9-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="94db9-118">Informazio gehiago eskuratzeko, irakurri [Kudeatu Dynamics 365 aplikazioak](https://docs.microsoft.com/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="94db9-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>


