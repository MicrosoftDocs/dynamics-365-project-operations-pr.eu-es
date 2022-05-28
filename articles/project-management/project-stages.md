---
title: Proiektuaren faseak
description: Gai honek eskuragarri dauden proiektuen etapei buruzko informazioa eskaintzen du Microsoft Dynamics Project Operations-en.
author: ruhercul
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: a25f32badd8776c89ad6eb56ad77ff61ad0cccae
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8586191"
---
# <a name="project-stages"></a>Proiektuaren faseak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuaren faseak diseinatu egiten dira proiektuaren egoera aurrera doan heinean. Pertsonalizazioak faseak automatikoki eguneratzeko erabil daitezke negozio prozesuen fluxuekin, Power Automate edo plug-in luzapenak.

Hurrengo fase hauek negozio-prozesuaren fluxu lehenetsian zehazten dira:

- Berria
- Eskaintza
- Plana
- Entregatu
- Osoa
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



[!INCLUDE[footer-include](../includes/footer-banner.md)]