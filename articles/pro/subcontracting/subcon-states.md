---
title: Azpikontratatu baten egoera-trantsizioak
description: Artikulu honek Microsoft-en azpikontratu baten egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations azpikontratua sortu, gauzatu eta ixten den heinean.
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

Artikulu honek Microsoft-en azpikontratu baten egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations. Estatu bakoitza zirriborro gisa adierazten da, baieztatuta, itxita edo bertan behera utzita. Hurrengo irudiak egoera-trantsizioak adierazten ditu.

![Azpikontratazio egoera eredua](../media/SubconStates.png)  

Ondorengo taulak egoera bakoitzak proiektuaren eragiketetan azpikontratu baten bizi-zikloan adierazten duenaren deskribapena eskaintzen du.

| Egoera | Deskribapenak | Baimendutako trantsizioak |
| --- | --- | --- |
| Zirriborroak | Horrek azpikontratu baten hasierako egoera adierazten du. Saltzailearekin negoziazioak abian dira. Lerroak eta prezioak aldaketen menpe daude. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilera ere erreferentzia egin daiteke. Egoera honetan dagoen azpikontratua editatu eta ezaba daiteke. | Berretsita |
| Berretsita | Honek azpikontratu baten etapa adierazten du saltzailearekin prezioei eta erosteko lerroko elementuei buruzko negoziazioak amaitu ondoren. Dena den, azpikontratatutako baliabideen bidez materialak eta/edo lanak egiaz bidaltzen ari dira oraindik. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilera ere erreferentzia egin daiteke. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. The **Utzi** botoiak berretsitako azpikontratua bertan behera uzteko aukera ematen du. The **Berriro ireki** botoiak azpikontratua berriro irekitzeko aukera ematen du, berriro sartzeko **Zirriborroa** egoera. Erabili **Itxi** botoia baieztatutako azpikontratua ixteko. | Itxita <br> Utzi da <br> Zirriborroak |
| Itxita | Honek azpikontratazioaren fasea adierazten du, materialak eta/edo lanak azpikontratatutako baliabideen bidez benetako entrega egiten denean. Egoera honetan dagoen azpikontratua ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta kudeatzeko. Gainera, jada ezin da erreferentzia egin proiektu batean denbora, gastu eta materialaren erabilerari buruz. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. | Batere ez |
| Utzi da | Honek azpikontratazioaren fasea adierazten du, materialak edo/eta lanak azpikontratatutako baliabideen bidez entregatu behar ez direnean. Egoera honetan dagoen azpikontratu bat ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta pertsonalizatzeko, ezta proiektu batean denbora, gastu eta materialaren erabilerari erreferentzia egin ere. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. | Batere ez |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
