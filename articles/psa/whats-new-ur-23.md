---
title: Project Service Automation eguneratzearen 23, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 23. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: eaae9cc62c449695cb2e999be48c57075aadbb21
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070983"
---
# <a name="project-service-automation-update-release-23-v3"></a>Project Service Automation 23, V3 eguneratze-bertsioa

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 23. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.34.30 konpilazio-zenbakia du eta, oro har, 2020ko abuztuan jarriko da erabilgarri automatikoki eguneratzeko moduan.

## <a name="update-release-23"></a>23. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira:
- Kudeatu ertzeko kasua **Proiektuko talde-kidea ezabatzea** eremuan, salbuespen esanguratsua eskaintzeko.
- Esleipenak inportatzean kentzeko pantaila huts bat sortzen da.

**Baliabideen kudeaketa**

Arazo hauek konpondu dira:

- **Baliabideen erabilera-saretaren baliabide-txartela** eremuak datu okerrak erakusten ditu denbora-eskala bost egunetik gorakoa denean.
- Bezeroek erreserbatzeko baliabide bat sortzen dutenean, pluginak tarteka huts egiten du baliabidea automatikoki Microsoft Office 365 talde batean gehitzerakoan.
- **Adiskidetzea** ikuspegiak eskuzko ingeradak gaizki erakusten ditu **Astea** edo **Hilabetea** ikuspegian.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- **RetrieveMultiple for usersettings** entitate kopuru gehiegizkoak errendimendu okerra eragiten ari dira proiektuen onarpenetarako eta bestelako eragiketetarako.
- **Zereginen plangintza** saretaren baliabideen bilaketa proiektu-taldeko bost talde-kideri erakustera mugatuta dago. 
- **Zereginen plangintza** saretaren baliabideen bilaketak ez du iragazten baliabide inaktiborik.
- Eskuzko moduak ez du espero bezala funtzionatzen zereginen xehetasunen egituraren plangintzaren proiektuan.
- **Zereginen plangintza** saretak **Transakzio inaktiboen kategoriak** erakusten ditu.
- **Baliabideen esleipena** saretak gaizki biribiltzen du zeregin batek hainbat zeregin dituenean.
- Biribiltzeko balioak planifikatutako kostuaren eta benetako kostuaren artean desberdinak dira zeregin bakar baterako.

**Sales**

Arazo hauek konpondu dira:

- **Eskuratu transakzio kategoria guztiak** bi aldiz sakatuta lerro anitz sortzen dira.