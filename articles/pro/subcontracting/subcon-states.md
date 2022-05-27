---
title: Azpikontratu bateko egoera-trantsizioak
description: Gai honek Microsoft-en azpikontratu baten egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations azpikontratua sortu, exekutatu eta ixten den heinean.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: c9533d046398c708c55467e6b1a25acf6abade3e
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8579153"
---
# <a name="state-transitions-on-a-subcontract"></a>Azpikontratu bateko egoera-trantsizioak 

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek Microsoft-en azpikontratu baten egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations. Estatu bakoitza zirriborro gisa adierazten da, baieztatuta, itxita edo bertan behera utzita. Hurrengo irudiak egoera-trantsizioak adierazten ditu.

![Azpikontratu egoera eredua](../media/SubconStates.png)  

Ondorengo taulak egoera bakoitzak proiektuaren eragiketetan azpikontratu baten bizi-zikloan adierazten duenaren deskribapena eskaintzen du.

| Egoera | Deskribapenak | Baimendutako trantsizioak |
| --- | --- | --- |
| Zirriborroak | Horrek azpikontratu baten hasierako egoera adierazten du. Saltzailearekin negoziazioak abian dira. Lerroak eta prezioak aldaketak jasan ditzakete. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilerari ere erreferentzia egin daiteke. Egoera honetan dagoen azpikontratua editatu eta ezaba daiteke. | Berretsita |
| Berretsita | Honek azpikontratu baten etapa adierazten du saltzailearekin prezioei eta erosteko lerroko elementuei buruzko negoziazioak amaitu ondoren. Dena den, azpikontratatutako baliabideen bidez materialak eta/edo lanak benetako entregak egiten jarraitzen dute. Egoera honetako azpikontratu bat baliabide eta materialen proiektuen eskakizunak estimatu eta kudeatzeko erabil daiteke. Proiektu batean denbora, gastu eta materialaren erabilerari ere erreferentzia egin daiteke. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. The **Utzi** botoiak berretsitako azpikontratua bertan behera uzteko aukera ematen du. The **Berriro ireki** botoiak azpikontratua berriro irekitzeko aukera ematen du, berriro sartzeko **Zirriborroa** egoera. Erabili **Itxi** botoia baieztatutako azpikontratua ixteko. | Itxita <br> Utzi da <br> Zirriborroak |
| Itxita | Honek azpikontratu baten fasea adierazten du, materialak edo/eta lanak azpikontratatutako baliabideen bidez benetako entrega amaitzen direnean. Egoera honetan dagoen azpikontratua ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta kudeatzeko. Gainera, jada ezin da erreferentzia egin proiektu batean denbora, gastu eta materialaren erabilerari buruz. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. | Batere ez |
| Utzi da | Honek azpikontratu baten fasea adierazten du, materialak edo/eta lanak azpikontratatutako baliabideen bidez entregatu behar ez direnean. Egoera honetan dagoen azpikontratu bat ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta pertsonalizatzeko, ezta proiektu batean denbora, gastu eta materialaren erabilerari erreferentzia egin ere. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. | Batere ez |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
