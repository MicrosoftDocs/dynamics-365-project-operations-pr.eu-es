---
title: Zer den berria edo zer aldatu den Project Service Automation-en 3.x 2020ko 1. bertsioan
description: Gai honek Project Service Automation-en 3 2020ko 1. bertsioan berria denari eta aldatu denari buruzko informazioa eskaintzen du.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/15/2020
ms.topic: article
author: stsporen
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 16b51995f863d9ee54172625dacbf081c51c8556
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070982"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="f85f2-103">Zer den berria edo zer aldatu den Project Service Automation-en 3 2020ko 1. bertsioan</span><span class="sxs-lookup"><span data-stu-id="f85f2-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="f85f2-104">Gai honek Project Service Automation (PSA) 3.x 2020ko 1. bertsioaren bertsio-berritzean kontuan hartu beharreko funtsezko gako batzuk nabarmentzen ditu.</span><span class="sxs-lookup"><span data-stu-id="f85f2-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="f85f2-105">Denbora-sarrera</span><span class="sxs-lookup"><span data-stu-id="f85f2-105">Time entry</span></span>
<span data-ttu-id="f85f2-106">Ordu-sarreraren esperientzia hedatu da denbora-sarrera hedatzeko gaitasunak bezero-egoera gehiagotara hedatzeko.</span><span class="sxs-lookup"><span data-stu-id="f85f2-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="f85f2-107">Barne du sarrera motak gehitzeko gaitasuna, eta orain jokamolde espezifikoak gidatzen ditu **Ordu-sarreraren ezarpenak** izeneko eremu eskema-izenean oinarrituta, **Denbora-iturria** gisa bistaratuta.</span><span class="sxs-lookup"><span data-stu-id="f85f2-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings** , displayed as **Time Source**.</span></span> <span data-ttu-id="f85f2-108">Denbora, Gastuak eta Onespenak (TESA) izeneko soluzio berria gehitu da, funtzionalitateari laguntzeko.</span><span class="sxs-lookup"><span data-stu-id="f85f2-108">A new solution, called Time, Expense, Statusing, and Approvals (TESA) has been added to support this functionality.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="f85f2-109">Bertsio-berritzeko gogoeta</span><span class="sxs-lookup"><span data-stu-id="f85f2-109">Upgrade consideration</span></span>
<span data-ttu-id="f85f2-110">Funtzionalitate hau onartzeko, PSA barruko funtzioak eguneratu egin dira pribilegio berriak gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="f85f2-110">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="f85f2-111">Pribilegio hauek irakurtzeko baimena ematen diote **Ordu-sarreraren ezarpenak** entitate berriari.</span><span class="sxs-lookup"><span data-stu-id="f85f2-111">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="f85f2-112">Denbora erregistratzeko gaitasuna behar duten erabiltzaileei **Ordu-sarreraren erabiltzailea** erabiltzaile-funtzioa eman behar zaie lehendik zituzten funtzioez gain.</span><span class="sxs-lookup"><span data-stu-id="f85f2-112">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="f85f2-113">Funtzio honek funtzionalitate berria du eta denbora-sarrerak funtzionatzen jarraituko duela ziurtatzen du.</span><span class="sxs-lookup"><span data-stu-id="f85f2-113">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

<span data-ttu-id="f85f2-114">Gainera, denbora-sarreren entitatearen inprimaki guztiak dituzten aplikazio-modulu pertsonalizaturik baduzu, **TESA denbora idazteko inprimaki bizkorra** modulutik kentzeko eskatuko zaizu.</span><span class="sxs-lookup"><span data-stu-id="f85f2-114">Additionally, if you have any custom app modules that include all forms for the time entry entity, you will be required to remove the **TESA time Entry Quick Create Form** from the module.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="f85f2-115">Gaur egun hedatutako denbora-sarreraren aldaketak</span><span class="sxs-lookup"><span data-stu-id="f85f2-115">Currently extended time entry changes</span></span>
<span data-ttu-id="f85f2-116">Denbora-sarreraren oraingo erabiltzaileen inpaktua gutxitzeko, funtzio-aldaketa hau denbora-sarrera erabiltzen jarraitzeko eskakizun nagusia bakarra da.</span><span class="sxs-lookup"><span data-stu-id="f85f2-116">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="f85f2-117">Ikuspegi pertsonalizatuak edo denbora sartzeko esperientzia bereziak sortu badituzu, **Ordu-sarreraren ezarpena** eremuak PSA balio zuzenarekin ezarri behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="f85f2-117">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
