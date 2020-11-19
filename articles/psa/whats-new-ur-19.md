---
title: Project Service Automation eguneratzearen 19, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 19. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: ecc923cccfad21985025ab9d8006aaff16afc25f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070989"
---
# <a name="project-service-automation-update-release-19-v3"></a>Project Service Automation 19, V3 eguneratze-bertsioa

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek PSA V3, 19. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honen konpilazio-zenbakia V3.10.30.41 da eta, oro har, 2020ko maiatzeko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-19"></a>19. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira: 

- Denbora-sarrerak ongi ez agertzetik eratorritako akatsak.
- Denbora-sarreren saretak ez du onartzen **Data soilik** eremuko portaera.
- Project Resources ez dago erabilgarri, proiektu baten gastua sortzeko.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira: 

-  Hirugarren mailako zereginek gutxi gorabeherako ahalegin okerra eragiten du Osatzea (EAC) kalkulatzeko garaian.

**Sales**

Arazo hauek konpondu dira: 

- **Birkalkulatu** ekintzak ez du funtzionatzen gastuen kontratuaren lerroko xehetasunekin edo eskaintzaren lerroko xehetasunekin.
- **Eguneratu prezioak** falta da gutxi gorabeherako gastuetan.
-  Bezeroek ezin dute hautatu kontratuaren egoeraren arrazoi pertsonalizatua **Proiektuaren kontratua** orrian.
- Bezeroek errendimendu degradatua izaten dute eskaintza batetik prezio-zerrenda pertsonalizatua sortzean.
- Bezeroek inkoherentziak dituzte lehenetsitako **unitateekin** **Eskaintzaren lerroko xehetasunak** eta **Kontratuaren lerroko xehetasunak** orrietan.
- Egotz ezin daitekeen transakzioen kategoriako elementuak egotz daitekeen kontratuaren lerro batean gehitzeak ez du errespetatuko transakzio kategoriako **Egotz ezin daitekeena** fakturazio mota.
- Bezeroek ezin dituzte erabili gehitu berri diren funtzioak eta kategoriak aurrez sortutako kontratuetan.
- Bezeroek errendimendu degradatua izaten dute Ezinbesteko berreskuratzea PreValidateProjectTeamMemberUpdate.cs-en
- **Baliabideen kategoriak** zerrendan egotz ezin daitezkeen funtzio gisa konfiguratutako funtzioak **Funtzio egozgarriak** fitxan gehituko dira **Egotz ezin daitezkeenak** gisa proiektuaren kontratuaren lerroan.
- Bezeroek errendimendu degradatua izan dezakete proiektu bat sortzerakoan **GetBookableResourceIdFromUser** parametroak baliabide erreserbagarrien zutabe guztiak berreskuratzen dituelako ID nagusia bakarrik berreskuratu beharrean.
- **TransactionType** entitateari aurre-balioztatzea eguneratzeko plugina falta zaio, erabiltzaileak transakzio motetarako baliozkoak ez diren **Unitateak** eta **UnitGroups** transakzio motetan ez sartzeko.
- **Kendu** urratsak ez du funtzionatzen denbora-sarreren inportaziorako.