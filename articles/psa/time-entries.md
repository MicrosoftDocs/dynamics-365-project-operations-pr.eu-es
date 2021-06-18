---
title: Sortu denbora-sarrerak
description: Gai honek denbora sarrerak sortzeari buruzko informazioa ematen du.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bc8e52fef0aa02505e412c746343ce1410c40ac3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999251"
---
# <a name="create-time-entries"></a><span data-ttu-id="67417-103">Sortu denbora-sarrerak</span><span class="sxs-lookup"><span data-stu-id="67417-103">Create time entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="67417-104">Dynamics 365 Project Service Automation aplikazioaren aurreko bertsioetan, denbora-sarrerak astero idazten ziren.</span><span class="sxs-lookup"><span data-stu-id="67417-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="67417-105">Project Service Automation-en 3. bertsioan, denbora-sarrerak egunero sartzen dira.</span><span class="sxs-lookup"><span data-stu-id="67417-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="67417-106">Hala ere, sarrerak sortu eta denbora gutxira, modu masiboan sortu edo kopiatu ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="67417-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="67417-107">Sortu denbora-sarrera bat</span><span class="sxs-lookup"><span data-stu-id="67417-107">Create a time entry</span></span>

<span data-ttu-id="67417-108">Jarraitu urrats hauei denbora-sarrera sortzeko.</span><span class="sxs-lookup"><span data-stu-id="67417-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="67417-109">**Denbora-sarrerak** orrian, hautatu **Berria**.</span><span class="sxs-lookup"><span data-stu-id="67417-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="67417-110">**Sorrera bizkorra: Denbora-sarrera** elkarrizketa-koadroan, sartu denboraren iraupena minutu, ordu edo egunetan.</span><span class="sxs-lookup"><span data-stu-id="67417-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="67417-111">Iraupena formatu honetan sartu behar da: *x* minutu, *x* ordu edo *x* egun.</span><span class="sxs-lookup"><span data-stu-id="67417-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="67417-112">Orduak eta egunak ere balio hamartarrak erabiliz idatz daitezke, adibidez, *x.x* ordu edo *x.x* egun.</span><span class="sxs-lookup"><span data-stu-id="67417-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="67417-113">Hautatu debora idatziko duzun denbora-sarrera mota eta proiektua.</span><span class="sxs-lookup"><span data-stu-id="67417-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="67417-114">**Proiektuaren zeregina** eremuan, aurkitu zeregina denbora-sarrera honetarako.</span><span class="sxs-lookup"><span data-stu-id="67417-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="67417-115">Erabiltzaile bati esleituta ez dagoen zereginetarako denbora-sarrera bat sortzen ari bazara, **Proiektuaren zeregina** eremuan, hautatu **Bilatu** botoia, hautatu **Aldatu ikuspegia** eta, ondoren, hautatu **Proiektu aktiboko zeregin guztiak** zeregin guztiak zerrendatzeko.</span><span class="sxs-lookup"><span data-stu-id="67417-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View**, and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="67417-116">Idatzi deskribapena, deskribapen bat beharrezkoa bada eta, ondoren, hautatu **Gorde eta itxi**.</span><span class="sxs-lookup"><span data-stu-id="67417-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="67417-117">Denbora-sarrera sortu eta gorde ondoren, denbora-sarreraren saretan editatu ahal izango duzu.</span><span class="sxs-lookup"><span data-stu-id="67417-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="67417-118">Denbora-sarreraren saretak bi formatu onartzen ditu:</span><span class="sxs-lookup"><span data-stu-id="67417-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="67417-119">Denbora-sarrerak **hh: mm** formatuan idatz ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="67417-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="67417-120">Formatu hori ordu eta zatiki bihurtzen da.</span><span class="sxs-lookup"><span data-stu-id="67417-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="67417-121">Orduak eta zatikiak zuzenean idatz ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="67417-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="67417-122">Kontuan izan ordu bateko zatikiak ez direla minutuak.</span><span class="sxs-lookup"><span data-stu-id="67417-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="67417-123">Beraz, 1,5 orduk ordu 1 eta 30 minutu adierazten du.</span><span class="sxs-lookup"><span data-stu-id="67417-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="67417-124">Arau bera aplikatzen zaie egun bateko zatikiei.</span><span class="sxs-lookup"><span data-stu-id="67417-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="67417-125">Egun batek 24 ordu ditu, eta 0,5 egunek 12 ordu.</span><span class="sxs-lookup"><span data-stu-id="67417-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="67417-126">Sortu denbora-sarrerak modu masiboan</span><span class="sxs-lookup"><span data-stu-id="67417-126">Bulk create time entries</span></span>

<span data-ttu-id="67417-127">Denbora-sarrera sortu eta minutu batzuk geroago, kopiatu egin ditzakezu denbora-sarrera gehigarriak gehitzeko modu masiboan.</span><span class="sxs-lookup"><span data-stu-id="67417-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="67417-128">**Denbora-sarrerak** orrian, hautatu **Kopiatu astea**.</span><span class="sxs-lookup"><span data-stu-id="67417-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="67417-129">**Aldi honetatik** talde-eremuan, **Hasiera data** eta **Amaiera Data** eremuetan, zehaztu denbora-sarrerak kopiatu behar diren data-tartea.</span><span class="sxs-lookup"><span data-stu-id="67417-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="67417-130">**Aldira** talde-eremuan, **Hasiera data** eremuan, zehaztu zein datarako sortu nahi dituzun sarrerak.</span><span class="sxs-lookup"><span data-stu-id="67417-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="67417-131">Hautatu **Kopiatu** aukera **Epea** eremu-taldean zehaztutako astearen egunari dagozkion denbora-sarreren kopia bat sortzeko.</span><span class="sxs-lookup"><span data-stu-id="67417-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="67417-132">Adibidez, pasa den asteko astelehenerako denbora-sarrera **Epea** eremuko taldean zehaztutako aste honetako astelehenean kopiatzen da.</span><span class="sxs-lookup"><span data-stu-id="67417-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="67417-133">Inportatu datuak denbora-sarreretarako</span><span class="sxs-lookup"><span data-stu-id="67417-133">Import data for time entries</span></span>

<span data-ttu-id="67417-134">Proiektuen erreserbetatik eta zereginetatik inportatu ditzakezu datuak.</span><span class="sxs-lookup"><span data-stu-id="67417-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="67417-135">Datuak inportatzean, inportatu nahi dituzun erreserben data zehaztu dezakezu eta, ondoren, modu esplizituan hautatu behar dira **Zirriborroa** denbora-sarrerak gisa sortu behar diren erreserbak.</span><span class="sxs-lookup"><span data-stu-id="67417-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="67417-136">Taldekatu, ordenatu, bilatu eta iragazi gaitasunak</span><span class="sxs-lookup"><span data-stu-id="67417-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="67417-137">Denbora-sarrerak zutabeetan zehaztutako neurrien arabera multzokatu eta iragazi ditzakezu.</span><span class="sxs-lookup"><span data-stu-id="67417-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="67417-138">**Taldekatu honela** eremuan, hautatu denbora-sarrerak iragazteko erabili beharreko neurria.</span><span class="sxs-lookup"><span data-stu-id="67417-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="67417-139">Denbora-sarreraren erregistroak goranzko edo beheranzko ordenan ordenatu ditzakezu zutabeetako izenburuak ordenatzeko gezia erabilita.</span><span class="sxs-lookup"><span data-stu-id="67417-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="67417-140">Gainera, sarrerak erakutsi edo ezkutatu ditzakezu zutabearen goiburuko **Iragazkia** botoia hautatua eta, ondoren, **Bilatu** laukian, proiektuaren izenaren, proiektuaren ataza, denbora-sarreraren edo baliabidearen arabera denbora-sarrerak bilatzeko erabili behar den testua idatziz.</span><span class="sxs-lookup"><span data-stu-id="67417-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]