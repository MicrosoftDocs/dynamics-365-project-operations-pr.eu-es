---
title: Estatu-trantsizioak azpikontratu batean
description: Gai honek Microsoft-en azpikontratu baten egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations azpikontratua sortu, exekutatu eta ixten den heinean.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: d67f4a3cd834c25462304c2d75c824427fcbd034
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903602"
---
# <a name="state-transitions-on-a-subcontract"></a>Estatu-trantsizioak azpikontratu batean 

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek Microsoft-en azpikontratu baten egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations. Estatu bakoitza zirriborro gisa adierazten da, baieztatuta, itxita edo bertan behera utzita. Hurrengo irudiak egoera-trantsizioak adierazten ditu.

![Azpikontratu egoera eredua](../media/SubconStates.png)  

Ondorengo taulak egoera bakoitzak proiektuaren eragiketetan azpikontratu baten bizi-zikloan adierazten duenaren deskribapena eskaintzen du.

| Egoera | Deskribapenak | Baimendutako trantsizioak |
| --- | --- | --- |
| Zirriborroak | Horrek azpikontratu baten hasierako egoera adierazten du. Saltzailearekin negoziazioak abian dira. Lerroak eta prezioak aldaketak izan ditzakete. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilera ere erreferentzia egin daiteke. Egoera honetan dagoen azpikontratua editatu eta ezaba daiteke. | Berretsita |
| Berretsita | Honek azpikontratu baten etapa adierazten du saltzailearekin prezioei eta erosteko lerroko elementuei buruzko negoziazioak amaitu ondoren. Dena den, azpikontratatutako baliabideen bidez materialak eta/edo lanak benetako entregak egiten jarraitzen dute. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilera ere erreferentzia egin daiteke. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. The **Utzi** botoiak berretsitako azpikontratua bertan behera uzteko aukera ematen du. The **Berriro ireki** botoiak azpikontratua berriro irekitzeko aukera ematen du, berriro sartzeko **Zirriborroa** egoera. Erabili **Itxi** botoia baieztatutako azpikontratua ixteko. | Itxita <br> Utzi da <br> Zirriborroak |
| Itxita | Honek azpikontratu baten fasea adierazten du, materialak edo/eta lanak azpikontratatutako baliabideen bidez benetako entrega amaitzen direnean. Egoera honetan dagoen azpikontratua ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta kudeatzeko. Gainera, jada ezin da erreferentzia egin proiektu batean denbora, gastu eta materialaren erabilerari buruz. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. | Batere ez |
| Utzi da | Honek azpikontratu baten fasea adierazten du, materialak edo/eta lanak azpikontratatutako baliabideen bidez entregatu behar ez direnean. Egoera honetan dagoen azpikontratu bat ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta pertsonalizatzeko, ezta proiektu batean denbora, gastu eta materialaren erabilerari erreferentzia egin ere. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. | Batere ez |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
