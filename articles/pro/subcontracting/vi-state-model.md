---
title: Saltzailearen faktura bateko egoera-trantsizioak
description: Artikulu honetan Microsoften hornitzaile-faktura baten estatu-trantsizioak azaltzen dira Dynamics 365 Project Operations.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 58b07322fb6480fdeb07eb867a7aabc0eff7b955
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8934305"
---
# <a name="state-transitions-on-a-vendor-invoice"></a>Saltzailearen faktura bateko egoera-trantsizioak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu honetan Microsoften hornitzaile-faktura baten estatu-trantsizioak azaltzen dira Dynamics 365 Project Operations. Honako egoera hauek erabiltzen dira: Zirriborroa, Berrikuspena **,** Baieztatua **,** Itxaronaldia **eta** Kitatua. **·** **·**

Hurrengo ilustrazioetan estatu-trantsizioak erakusten dira.

![Azpikontrato-egoeraren trantsizio-eredua.](../media/VI_State_Model.jpg)

Hurrengo taulan, proiektu-eragiketetako hornitzaile-faktura baten bizi-zikloko egoera bakoitza zer den azaltzen da.

| Egoera | Deskribapenak | Baimendutako trantsizioak |
| --- | --- | --- |
| Zirriborroak | Egoera hori hornitzailearen faktura baten hasierako egoera da. Lineak eta prezioak aldatu egin behar dira. Hornitzailearen faktura bat argitaratu eta ezabatu daiteke egoera honetan. | Prozesuan |
| Berrikusten | Egoera horrek hornitzaile-faktura baten prozesatze-egoera adierazten du. Hornitzailearen faktura-linea batek, gutxienez, en ari-tza **egiaztatzeko egoera du**. | Baieztatuta, Itxaron |
| Berretsita | Egoera hori hornitzaile-faktura baten etapa da, eta aplikazioak kostuen datu errealak sortu ditu hornitzailearen faktura-linea bakoitzerako. Hornitzaileen fakturen lerroekin bat egin zuten kostuen benetako datu guztiak itzuli eta ordeztu egin dira hornitzaileen faktura-linea horien benetako kostuekin. Hornitzailearen faktura bat ezin da editatu, ezta ezabatu ere. Cancelar **botoia erabil** dezakezu baieztatutako hornitzailearen faktura bat ezeztatzeko. Cancelar ekintzak Confirmar ekintzaren eragina iraultzen du. | Utzi da |
| Zain | <p>Egoera hori hornitzailearen faktura baten etapa bat da, non hornitzailearen faktura ezin den mugitu, fakturarekin edo hornitzailearen egoerarekin izandako arazo baten ondorioz. Hornitzailearen faktura bat ezin da baieztatu, ezeztatu, editatu edo ezabatu.</p><p>Hornitzailearen faktura Estatu Borrador **edo** Berrikustean **mugitzeko** erabili dezakezu berriro irekitzea. Hornitzailearen fakturaren linea batek, gutxienez, enkaera edo osatutze-egoera **badu**, hornitzailearen faktura berriz irekiko da berrikuspen-egoeran **·**.**·** Hornitzailearen fakturaren linea guztiek hasi gabeko egiaztapen-egoera **badute, hornitzailearen faktura berriro irekiko da Borrador** estatuan **.**</p> | Zirriborroa, Berrikustean |
| Utzi da | Egoera horrek azpikontratatu baten etapa irudikatzen du, non ez den beharrezkoa materialak eta / edo azpikontratatutako baliabideengatik egindako lana benetako entregatzea. Egoera horretan azpikontratu bat ezin da erabili baliabide eta materialen proiektuaren baldintzak zenbatetsi eta hornitzeko, eta ezin da aipatu proiektu batean materialen denbora, gastuak eta erabilera. Estatu honetako azpikontratu bat ezin da editatu, ezta ezabatu ere. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
