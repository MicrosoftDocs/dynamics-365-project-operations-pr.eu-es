---
title: Zereginen xehetasunen egiturari buruzko gogoeta eguneratuak
description: Gai honek zereginen xehetasunen egitura Project Service Automation-en 2.x-tik 3.x-ra bertsio-berritzeari buruzko informazioa ematen du.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: 169dc24f0d1ae151ea5927123fb738221de88250
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071118"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a>Zereginen xehetasunen egiturari buruzko gogoeta eguneratuak
Gai honek zereginen xehetasunen egitura Project Service Automation-en 2.x-tik 3.x-ra bertsio-berritzeari buruzko informazioa ematen du. Gai honek Project Service Automation-eko (PSA) proiektu baten egoera osasuntsua definitzen du, bertsio-berritzea ondo egin dadin beharrezkoa dena. Bertsio-berritzeak huts egitea eragiten duten blokeo baldintza arruntei buruzko informazioa ere badago. Proiektuen zereginak eta haien funtzioak proiektuaren antolaketan zehazteari buruzko informazio gehiago lortzeko, ikusi [Proiektuen antolaketa](project-creating.md).

## <a name="key-entities"></a>Entitate gakoak
Jada baliabidez kargatutako zereginen xehetasunen egitura zehatza lortzeko, erakunde hauek behar dira:

- [Proiektua](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [Proiektu-taldea](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [Proiektuaren zeregina](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [Baliabide-esleipenak](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [Proiektuaren zereginen mendekotasuna](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [Baliabide erreserbagarriak](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

Baliabideek kargatutako zereginen xehetasunen egitura zehazteko, urrats hauei jarraitu behar diezu:

1. Sortu proiektu berria. Proiektu berria sortzeari buruzko informazio gehiago lortzeko, ikusi [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).
2. Sortu zeregin bat edo gehiago. Zeregin bat sortzeari buruzko informazio gehiago lortzeko, ikusi [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).
3. Zehaztu zereginaren mendekotasunak. Informazio gehiago lortzeko, ikusi [Proiektuaren zereginen mendekotasuna](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).
4. Esleitu proiektuko taldekideak proiektuari. Informazio gehiago lortzeko, ikus [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).
5. Esleitu proiektuko taldekideak zereginei. Informazio gehiago lortzeko, ikus [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).

## <a name="project-team-relationships"></a>Proiektu-taldeko erlazioak

Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:
- Proiektuko taldekide guztiek baliabide erreserbagarri bati esleituta egon behar dute.
- Proiektuko taldekide guztiek proiektu berari esleituta egon behar dute. 

## <a name="project-task-relationships"></a>Proiektuaren zereginen erlazioak
Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:

- Proiektu berarekin erlazionatutako edozein zeregin esleituta egon behar dira.
- Lerroko zeregin guztiek zeregin nagusia izan behar dute.
- Lerroko zeregin guztiek proiektu nagusi bat izan behar dute.

### <a name="valid-conditions"></a>Baliozko baldintzak

- Zereginen iraupen guztiak ordu bat baino handiagoa edo berdina (> =) eta 1.800.000 minutu baino gutxiagokoa (1.250 egun) izan behar du. *
- Zeregin guztien hasierako data hau baino lehenagokoa izan behar da: 2000/01/01.*
- Zeregin guztien hasierako data ezin da izan gaur egun baino 17 urte baino lehenagokoa.*
- Zeregin guztiek hasierako data amaierako dataren berdina edo lehenagokoa izan behar da.
- Sailkapenen transakzio mota guztiek (gastua, materiala, zerga eta denbora) balioak izan behar dituzte **Lehenespeneko unitatea** eta **Salmenta-unitatea** aukeretarako.
- Letrak dituzten data formatuak ekidin behar dira.

### <a name="potential-mitigation-steps"></a>Balizko urrats aringarriak
- Erabili Bilatu aurreratua Proiektuaren IDrik ez duten Proiektuen zereginak identifikatzeko.
- Erabili Bilaketa aurreratua Proiektuaren zereginak identifikatzeko iraupena > 1.800.000 baino handiagoa denean.
- Datu-aldaketak egin aurretik, datuak egoera txarrean izatera eraman dituen entitatearekin lotutako pertsonalizazio guztiak aztertu beharko zenituzke. Pertsonalizazio horiek datuekin lotutako eguneratzeekin jarraitu aurretik zuzendu beharko lirateke.
- Umezurtz geratu diren identifikatutako zereginetarako, pentsatu zeregin horiek ezabatzea beharrezkoak ez badira edo proiektu nagusi egokiarekin lotu behar badira.
- Iraupena 1.250 egun baino handiagoa den edozein zereginetarako, iraupen totala adieraziko duten zeregin ugari gehitzea gomendatzen da, bideragarria bada.

> [!NOTE]
> Izartxo batekin (\*) aipatutako elementuek mugak dituzte bezero-erlazioen kudeaketak (CRM) 7.320 errepikapen-hedapen bakarrik onartzen dituelako. Muga horren azpitik egon behar duzu.

## <a name="resource-assignment-relationships"></a>Baliabide-esleipenaren erlazioak
Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:

- Zereginen xehetasunen egiturako baliabideen esleipen guztiek proiektu berari lotuta egon behar dute.
- Zereginen xehetasunen egiturako baliabideen esleipen guztiek proiektu bereko proiektu-taldekide berari esleituta egon behar dute.

### <a name="potential-mitigation-steps"></a>Balizko urrats aringarriak
- Identifikatu goian azaldutako baldintzetatik kanpo dauden zeregin guztiak.  
- Dagoeneko balio ez duten baliabide-esleipenak ezabatu egin beharko lirateke.

## <a name="project-task-dependency-relationships"></a>Proiektuaren zereginaren mendekotasunaren erlazioak
Bertsio-berritze arrakastatsua ziurtatzeko, harreman hauek ongi mantendu behar dira:

- Proiektuaren zereginen mendekotasun guztiak proiektu berarekin lotuta egon behar dute.
- Zeregin batek ezin dio erreferentzia egin mendekotasun berari behin baino gehiagotan.
