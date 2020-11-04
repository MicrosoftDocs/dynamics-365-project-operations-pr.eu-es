---
title: Proiektuaren fase motak
description: Gai honek proiektuaren faseei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: 521bf4b3090473a603626a99fded53906b644a7a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071087"
---
# <a name="project-stage-types"></a>Proiektuaren fase motak 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuaren faseak diseinatu egiten dira proiektuaren egoera aurrera doan heinean. Pertsonalizazioak faseak automatikoki eguneratzeko erabil daitezke negozio prozesuen fluxuekin, Power Automate edo plug-in luzapenak.

Hurrengo fase hauek BPF lehenetsian zehazten dira:

- Berria
- Eskaintza
- Plana
- Entregatu
- Osatu
- Itxi 

## <a name="new"></a>Berria

Proiektu bat sortzen duzunean, proiektu fasea **Berria** gisa ezartzen da. Proiektua txantiloi batetik sortu bada, baliteke antolaketa, estimazioa eta taldeko datuak izatea. Bestela esanda, proiektuaren eskema besterik ez da, eta gainerako osagaiak sartu behar dira.

## <a name="quote"></a>Eskaintza

Proiektu bat eskaintza bati esleitzean edo proiektua eskaintza batetik sortzean, proiektuaren fasea **Eskaintza** gisa ezartzen da, eta estimatutako hasiera- eta amaiera-datak eguneratzen dira. Proiektua **Eskaintza** fasean dagoen bitartean, **Proiektuaren entitatea** orriko **Salmentak** fitxak eskaintzaren xehetasunak erakusten ditu.

## <a name="plan"></a>Plana

Proiektu bati erlazionatuta dagoen eskaintza bat irabaztean, eta proiektua **Kontratuta** fasera mugitu bada, proiektuaren fasea **Antolatu** fasera eguneratzen da. Proiektua **Antolatu** fasean dagoen bitartean, **Proiektuaren entitatea** orriak kontratuaren xehetasunak erakusten ditu.

## <a name="deliver"></a>Entregatu

Proiektuaren plana amaitutakoan eta proiektua hasteko prest zaudenean, proiektu-kudeatzaileak proiektuaren fasea eguneratu beharko luke **Entregatu** fasera proiektua hasi dela erakusteko.

## <a name="complete"></a>Osatu 

Proiektuko lanak amaitutakoan, proiektu-kudeatzaileak fasea eguneratu dezake **Osatuta** fasera. Proiektuaren fasea **Osatuta** fasera eguneratuz gero, proiektu-kudeatzaileak lana ehuneko 100ean amaitu dela adierazi du, baina proiektua irekita mantentzen dela, zain dauden denbora- edo gastu-sarrerak erregistratu ahal izateko.

## <a name="close"></a>Itxi

Proeikturako trantsakzio guztiak erregistratu direnean, proiektu-kudeatzaileak fasea eguneratu dezake **Itxi** fasera. Puntu horretan, ezin da transakziorik erregistratu, eta proiektua irakurtzeko soilik egongo da.
