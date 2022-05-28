---
title: Egoera-trantsizioak saltzaile-faktura batean
description: Gai honek Microsoft-en saltzaileen fakturaren egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 7efb52621ee325d5025dfad0b45218d1fe20a063
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8584673"
---
# <a name="state-transitions-on-a-vendor-invoice"></a>Egoera-trantsizioak saltzaile-faktura batean

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek Microsoft-en saltzaileen fakturaren egoera-trantsizioak azaltzen ditu Dynamics 365 Project Operations. Egoera hauek erabiltzen dira: **Zirriborroa**, **·**, **·**, **·**, eta **Bertan behera utzita**.

Ondorengo ilustrazioek egoera-trantsizioak erakusten dituzte.

![Azpikontratazio egoera trantsizio eredua.](../media/VI_State_Model.jpg)

Hurrengo taulak egoera bakoitzak zer adierazten duen azaltzen du saltzaileen faktura baten bizi-zikloan Project Operations-en.

| Egoera | Deskribapenak | Baimendutako trantsizioak |
| --- | --- | --- |
| Zirriborroak | Egoera hori saltzaileen faktura baten hasierako egoera da. Lerroak eta prezioak alda daitezke. Egoera honetan saltzaileen faktura bat editatu eta ezaba daiteke. | Prozesuan |
| Berrikusten | Egoera honek saltzaileen faktura baten prozesatzeko egoera adierazten du. Gutxienez saltzaileen faktura-lerro batek egiaztapen-egoera du **Abian**. | Berretsita, zain |
| Berretsita | Egoera honek hornitzaileen faktura baten fasea adierazten du, non aplikazioak kostu errealak sortu dituen saltzaileen faktura-lerro bakoitzeko. Saltzaileen faktura-lerroekin bat etortzen diren estekatutako kostu errealak alderantzikatu dira eta hornitzaileen faktura-lerro horietako kostu errealekin ordezkatu dira. Egoera honetan dagoen hornitzaile-faktura bat ezin da editatu edo ezabatu. Erabili dezakezu **Utzi** botoia berretsitako saltzaile-faktura bertan behera uzteko. Utzi ekintzak Berretsi ekintzaren eragina alderantzikatzen du. | Utzi da |
| Zain | <p>Egoera honek hornitzaile-faktura baten fase bat adierazten du, non saltzaile-faktura mugitu ezin den fakturarekin edo saltzailearen egoerarekin arazo bat dagoelako. Egoera honetan dagoen hornitzaile-faktura bat ezin da baieztatu, ezeztatu, editatu edo ezabatu.</p><p>Berriro ireki ekintza erabil dezakezu saltzaileen fakturara eramateko **Zirriborroa** edo **Berrikuspenean** Estatu. Saltzaileen fakturako gutxienez lerro batek egiaztapen-egoera badu **Abian** edo **Osatu**, saltzaileen faktura berriro irekiko da **Berrikuspenean** Estatu. Saltzaileen fakturako lerro guztiek egiaztapen-egoera badute **Ez da hasi**, saltzaileen faktura berriro irekiko da **Zirriborroa** Estatu.</p> | Zirriborroa, Berrikuspenean |
| Utzi da | Egoera honek azpikontratu baten fasea adierazten du, non jada beharrezkoa ez den materialak eta/edo lanak azpikontratatutako baliabideen bidez entregatzea. Egoera honetan dagoen azpikontratu bat ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta pertsonalizatzeko, eta, gainera, ezin da erreferentzia egin proiektu batean denbora, gastu eta materialaren erabilera. Egoera honetan dagoen azpikontratua ezin da editatu edo ezabatu. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
