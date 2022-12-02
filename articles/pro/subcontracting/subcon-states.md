---
title: Azpikontratatu baten egoera-trantsizioak
description: Artikulu honek azpikontratu baten egoera-trantsizioak azaltzen ditu Microsoft Dynamics 365 Project Operations azpikontratua sortu, gauzatu eta ixten den heinean.
author: rumant
ms.date: 09/14/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 2804fc30f8dade42dc1093e5fc0f01fa1db22ca3
ms.sourcegitcommit: 08eb3be9eda44e9446c43ed9b6aefd58d77927c5
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/15/2022
ms.locfileid: "9522924"
---
# <a name="state-transitions-on-a-subcontract"></a>Azpikontratatu baten egoera-trantsizioak 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Artikulu honek azpikontratuaren egoera-trantsizioak azaltzen ditu Microsoft Dynamics 365 Project Operations. Estatu bakoitza zirriborro gisa adierazten da, baieztatuta, itxita edo bertan behera utzita. Ondorengo ilustrazioek egoera-trantsizioak erakusten dituzte.

![Azpikontratatu baten egoera-eredua](../media/SubconStates.png)  

Hurrengo taulak egoera bakoitzak zer adierazten duen azaltzen du azpikontratu baten bizi-zikloan Project Operations-en.

| Egoera | Deskribapenak | Onartutako trantsizioak |
| --- | --- | --- |
| Zirriborroak | Horrek azpikontratu baten hasierako egoera adierazten du. Saltzailearekin negoziazioak abian dira. Lerroak eta prezioak alda daitezke. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilera ere erreferentzia egin daiteke. Egoeran horretan dauden azpikontratuak editatu edo ezabatu daitezke. | Berretsita |
| Berretsita | Honek azpikontratu baten etapa adierazten du saltzailearekin prezioei eta erosteko lerroko elementuei buruzko negoziazioak amaitu ondoren. Dena den, azpikontratatutako baliabideen bidez materialak eta/edo lanak egiaz bidaltzen ari dira oraindik. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilera ere erreferentzia egin daiteke. Egoeran horretan dauden azpikontratuak ezin dira editatu edo ezabatu. **Utzi** botoiak berretsitako azpikontratua bertan behera uzteko aukera ematen du. **Berriro ireki** botoiak azpikontratua berriro irekitzeko aukera ematen du, berriro sartzeko **Zirriborroa** egoera. Erabili **Itxi** botoia baieztatutako azpikontratua ixteko. | Itxita <br> Utzi da <br> Zirriborroak |
| Itxita | Honek azpikontratazio baten fasea adierazten du, non osatutako materialak eta/edo lanak azpikontratatutako baliabideen bidez entregatzea. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko ezin da erabili. Proiektu batean denbora, gastu eta materialaren erabilera ere erreferentzia ezin da egin. Egoeran horretan dauden azpikontratuak ezin dira editatu edo ezabatu. | Batere ez |
| Utzi da | Honek azpikontratazio baten fasea adierazten du, non ezin diren materialak eta/edo lanak azpikontratatutako baliabideen bidez entregatu. Egoera honetan dagoen azpikontratu bat ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta hornitzeko, eta, gainera, ezin da erreferentzia egin proiektu batean denbora, gastu eta materialaren erabilera. Egoeran horretan dauden azpikontratuak ezin dira editatu edo ezabatu. | Batere ez |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
