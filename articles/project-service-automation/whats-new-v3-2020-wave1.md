---
title: Zer den berria edo zer aldatu den Project Service Automation-en 3.x 2020ko 1. bertsioan
description: Gai honek Project Service Automation-en 3 2020ko 1. bertsioan berria denari eta aldatu denari buruzko informazioa eskaintzen du.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 01/24/2020
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x wave 1 2020
author: stsporen
ms.assetid: 48b408c1-11e7-4005-abac-8fd7c0b064b1
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 478080c0570b71188c9f1e12b18b5aadc13903e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748860"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="99756-103">Zer den berria edo zer aldatu den Project Service Automation-en 3 2020ko 1. bertsioan</span><span class="sxs-lookup"><span data-stu-id="99756-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="99756-104">Gai honek Project Service Automation (PSA) 3.x 2020ko 1. bertsioaren bertsio-berritzean kontuan hartu beharreko funtsezko gako batzuk nabarmentzen ditu.</span><span class="sxs-lookup"><span data-stu-id="99756-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="99756-105">Denbora-sarrera</span><span class="sxs-lookup"><span data-stu-id="99756-105">Time entry</span></span>
<span data-ttu-id="99756-106">Ordu-sarreraren esperientzia hedatu da denbora-sarrera hedatzeko gaitasunak bezero-egoera gehiagotara hedatzeko.</span><span class="sxs-lookup"><span data-stu-id="99756-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="99756-107">Barne du sarrera motak gehitzeko gaitasuna, eta orain jokamolde espezifikoak gidatzen ditu **Ordu-sarreraren ezarpenak** izeneko eremu eskema-izenean oinarrituta, **Denbora-iturria** gisa bistaratuta.</span><span class="sxs-lookup"><span data-stu-id="99756-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings**, displayed as **Time Source**.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="99756-108">Bertsio-berritzeko gogoeta</span><span class="sxs-lookup"><span data-stu-id="99756-108">Upgrade consideration</span></span>
<span data-ttu-id="99756-109">Funtzionalitate hau onartzeko, PSA barruko funtzioak eguneratu egin dira pribilegio berriak gehitzeko.</span><span class="sxs-lookup"><span data-stu-id="99756-109">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="99756-110">Pribilegio hauek irakurtzeko baimena ematen diote **Ordu-sarreraren ezarpenak** entitate berriari.</span><span class="sxs-lookup"><span data-stu-id="99756-110">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="99756-111">Denbora erregistratzeko gaitasuna behar duten erabiltzaileei **Ordu-sarreraren erabiltzailea** erabiltzaile-funtzioa eman behar zaie lehendik zituzten funtzioez gain.</span><span class="sxs-lookup"><span data-stu-id="99756-111">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="99756-112">Funtzio honek funtzionalitate berria du eta denbora-sarrerak funtzionatzen jarraituko duela ziurtatzen du.</span><span class="sxs-lookup"><span data-stu-id="99756-112">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="99756-113">Gaur egun hedatutako denbora-sarreraren aldaketak</span><span class="sxs-lookup"><span data-stu-id="99756-113">Currently extended time entry changes</span></span>
<span data-ttu-id="99756-114">Denbora-sarreraren oraingo erabiltzaileen inpaktua gutxitzeko, funtzio-aldaketa hau denbora-sarrera erabiltzen jarraitzeko eskakizun nagusia bakarra da.</span><span class="sxs-lookup"><span data-stu-id="99756-114">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="99756-115">Ikuspegi pertsonalizatuak edo denbora sartzeko esperientzia bereziak sortu badituzu, **Ordu-sarreraren ezarpena** eremuak PSA balio zuzenarekin ezarri behar dituzu.</span><span class="sxs-lookup"><span data-stu-id="99756-115">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
