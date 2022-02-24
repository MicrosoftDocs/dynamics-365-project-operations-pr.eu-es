---
title: Project Service Automation eguneratzearen 23, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 23. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 87f89828aeff22d9b473539e294d5cf04d46a203
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150023"
---
# <a name="project-service-automation-update-release-23-v3"></a>Project Service Automation 23, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

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
