---
title: Proiektuaren faseak
description: Gai honek proiektuaren faseei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 983c25a0-ed21-4151-a109-b385a88285fa
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 70aa057e127df7ba925e84f5d056a06a4cc8833e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748839"
---
# <a name="project-stages"></a>Proiektuaren faseak 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuaren faseak eguneratu egiten dira proiektuaren egoera aurrera doan heinean. Negozio-prozesuaren fluxu lehenetsiak automatikoki eguneratzen ditu proiektuaren fase batzuk, eta beste batzuk proiektu-kudeatzaileak eguneratzen ditu eskuz. 

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
