---
title: Konfiguratu proiektu-kategoriak
description: Gai honek proiektuaren kategoriak konfiguratzeari buruzko informazioa ematen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b7adf61a82714a0148d9c8b1d2b2b37fd611c1cf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287493"
---
# <a name="configure-project-categories"></a><span data-ttu-id="de1e1-103">Konfiguratu proiektu-kategoriak</span><span class="sxs-lookup"><span data-stu-id="de1e1-103">Configure project categories</span></span>

<span data-ttu-id="de1e1-104">_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_</span><span class="sxs-lookup"><span data-stu-id="de1e1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="de1e1-105">Project Operations-ek gaitasun sendoak eskaintzen dituzte proiektuetako diru-sarrerak eta gastuak sailkatzeko.</span><span class="sxs-lookup"><span data-stu-id="de1e1-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="de1e1-106">Kategoriek proiektuen transakzioen berri emateko eta aztertzeko gaitasuna eskaintzen dute eta liburuak liburu nagusira eramaten dituzte.</span><span class="sxs-lookup"><span data-stu-id="de1e1-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="de1e1-107">Ondorengo diagramak transakzio kategorien, partekatutako kategorien eta proiektuen kategorien arteko korrelazioa erakusten du.</span><span class="sxs-lookup"><span data-stu-id="de1e1-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="de1e1-108">Transakzio kategoriak proiektuen transakzioen oinarrizko taldekatzea dira.</span><span class="sxs-lookup"><span data-stu-id="de1e1-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="de1e1-109">Taldekatze horren barruan, aplikazio eta moduluen artean parteka daitezkeen kategoria partekatuen multzoa dago.</span><span class="sxs-lookup"><span data-stu-id="de1e1-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="de1e1-110">Zehaztasunetan are gehiago sakonduz, proiektuen kategoriak kategorien maila zehatzenak dira.</span><span class="sxs-lookup"><span data-stu-id="de1e1-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="de1e1-111">Proiektuen kategoriak pertsona juridikoei, moduluei eta aplikazioei dagozkie.</span><span class="sxs-lookup"><span data-stu-id="de1e1-111">Project categories are specific to legal entity, module, and application.</span></span>

![Transakzio-kategorien, kategoria partekatuen eta proiektu-kategorien arteko korrelazioa](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="de1e1-113">Transakzio-kategoriak</span><span class="sxs-lookup"><span data-stu-id="de1e1-113">Transaction categories</span></span>

<span data-ttu-id="de1e1-114">Transakzio kategoriek proiektuen transakzioen oinarrizko taldekatzea adierazten dute eta ez dira konpainia edo transakzio motak.</span><span class="sxs-lookup"><span data-stu-id="de1e1-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="de1e1-115">Adibidez, Contoso Robotics-ek Diseinua, Bidaia, Instalazioa eta Zerbitzuen Transakzio kategoriak erabiltzen ditu Proiektuaren transakzioak taldekatzeko.</span><span class="sxs-lookup"><span data-stu-id="de1e1-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="de1e1-116">Transakzio kategoriak Project Operations moduluan definitzen dira.</span><span class="sxs-lookup"><span data-stu-id="de1e1-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="de1e1-117">Joan **Ezarpenak** \> **Transakzio-kategoriak** aukerara, inprimakia irekitzeko.</span><span class="sxs-lookup"><span data-stu-id="de1e1-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="de1e1-118">Sortu transakzioen kategoria berria hautatuta **Berria** edo hautatuz **Inportatu Excel-etik**.</span><span class="sxs-lookup"><span data-stu-id="de1e1-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="de1e1-119">Partekatutako kategoriak</span><span class="sxs-lookup"><span data-stu-id="de1e1-119">Shared categories</span></span>

<span data-ttu-id="de1e1-120">Dynamics 365-ek Shared categories kontzeptua erabiltzen du gastuak aplikazio desberdinetan sailkatzeko, adibidez Dynamics 365 Finance, Dynamics 365 hornikuntza-katea eta Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="de1e1-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="de1e1-121">Sortutako Transakzio-kategoria bakoitzerako, Project Operations-ek erlazionatutako lau kategoria partekatu sortzen dituzte automatikoki: Orduak, Gastuak, Tasak eta Elementua.</span><span class="sxs-lookup"><span data-stu-id="de1e1-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="de1e1-122">Partekatutako kategoriak berrikusi eta doitu ditzakezu hona joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Kategoria partekatuak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="de1e1-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="de1e1-123">Proiektu-kategoriak</span><span class="sxs-lookup"><span data-stu-id="de1e1-123">Project categories</span></span>

<span data-ttu-id="de1e1-124">Proiektuen kategoriek kategoriaren konfigurazio maila zehatzena adierazten dute eta proiektuaren kontulari batek bereizita eta enpresa bakoitzerako konfiguratu behar ditu.</span><span class="sxs-lookup"><span data-stu-id="de1e1-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="de1e1-125">Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Proiektuen kategoriak** aukerara.</span><span class="sxs-lookup"><span data-stu-id="de1e1-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="de1e1-126">Hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="de1e1-126">Select **New**.</span></span>
3. <span data-ttu-id="de1e1-127">Aukeratu **Kategoria IDa** aurreko atalean sortutako Partekatutako kategoriakoa.</span><span class="sxs-lookup"><span data-stu-id="de1e1-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="de1e1-128">Project Operation-en eragiketei esker, transakzio kategoriarekin lotura duten kategoria partekatuak soilik erabil daitezke.</span><span class="sxs-lookup"><span data-stu-id="de1e1-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="de1e1-129">Hautatu kategoria taldea.</span><span class="sxs-lookup"><span data-stu-id="de1e1-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="de1e1-130">Kategoria-taldeak</span><span class="sxs-lookup"><span data-stu-id="de1e1-130">Category groups</span></span>

<span data-ttu-id="de1e1-131">Kategoria-taldeak propietateak partekatzeko erabiltzen dira, batez ere profilak argitaratzeko, erlazionatutako proiektu kategorien artean.</span><span class="sxs-lookup"><span data-stu-id="de1e1-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="de1e1-132">Transakzio mota bakoitzerako gutxienez kategoria talde bat egon behar da eta proiektu kategoria bakoitzari talde bat esleitzen zaio.</span><span class="sxs-lookup"><span data-stu-id="de1e1-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="de1e1-133">Project Operations-en argitaratzeko zehaztapenak proiektuaren kostu eta diru-sarreren profileko arauek, proiektuen kategoriek eta kategoria taldeek definitzen dituzte.</span><span class="sxs-lookup"><span data-stu-id="de1e1-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="de1e1-134">Kategoria taldeak konfigura ditzakezu hona joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Kategoria taldeak**.</span><span class="sxs-lookup"><span data-stu-id="de1e1-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]