---
title: Saltzailearen faktura bateko egoera-trantsizioak
description: Artikulu honek saltzaileen fakturaren egoera-trantsizioak azaltzen ditu Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: e25e4d63d4c9098112a7f40abe60c7184018d582
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9261001"
---
# <a name="state-transitions-on-a-vendor-invoice"></a>Saltzailearen faktura bateko egoera-trantsizioak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu honek saltzaileen fakturaren egoera-trantsizioak azaltzen ditu Microsoft Dynamics 365 Project Operations. Egoera hauek erabiltzen dira: **Zirriborroa**, **Berrikuspenean**, **Baieztatuta**, **Atxikitan**, eta **Bertan behera utzita**.

Ondorengo ilustrazioek egoera-trantsizioak erakusten dituzte.

![Azpikontratatu baten egoera-trantsizio ereduak.](../media/VI_State_Model.jpg)

Hurrengo taulak egoera bakoitzak zer adierazten duen azaltzen du saltzaileen faktura baten bizi-zikloan Project Operations-en.

| Egoera | Deskribapenak | Onartutako trantsizioak |
| --- | --- | --- |
| Zirriborroak | Egoera hori saltzaileen faktura baten hasierako egoera da. Lerroak eta prezioak alda daitezke. Egoeran horretan dauden Saltzailearen fakturak ezin dira editatu edo ezabatu. | Abian |
| Berrikusten | Egoera hori saltzaileen faktura baten prozesatze-egoera da. Gutxienez saltzaileen faktura-lerro batek egiaztapen-egoera du **Abian**. | Berretsita, zain |
| Berretsita | Egoera honek hornitzaileen faktura baten fasea adierazten du, non aplikazioak kostu errealak sortu dituen hornitzaileen faktura-lerro bakoitzeko. Saltzaileen faktura-lerroekin bat etortzen diren estekatutako kostu errealak alderantzikatu dira eta hornitzaileen faktura-lerro horietako kostu errealekin ordeztu dira. Egoeran horretan dauden Saltzailearen fakturak ezin dira editatu edo ezabatu. Erabili dezakezu **Utzi** botoia berretsitako saltzaile-faktura bertan behera uzteko. Utzi ekintzak Berretsi ekintzaren eragina alderantzikatzen du. | Utzi da |
| Zain | <p>Egoera honek hornitzaile-faktura baten fase bat adierazten du, non saltzaile-faktura mugitu ezin den fakturarekin edo saltzailearen egoerarekin arazo bat dagoelako. Egoeran horretan dauden Saltzailearen fakturak ezin dira berretsi, utzi editatu edo ezabatu.</p><p>Berriro ireki ekintza erabil dezakezu hornitzailearen faktura eramateko **Zirriborroa** edo **Berrikuspenean** egoerara. Saltzaileen fakturako gutxienez lerro batek egiaztapen-egoera badu **Abian** edo **Osatu**, saltzaileen faktura berriro irekiko da **Berrikuspenean** egoeran. Saltzaileen fakturako lerro guztiek egiaztapen-egoera badute **Ez da hasi**, saltzaileen faktura berriro irekiko da **Zirriborroa** egoeran.</p> | Zirriborroa, berrikusten |
| Utzi da | Egoera honek azpikontratazio baten fasea adierazten du, non jada beharrezkoa ez den materialak eta/edo lanak azpikontratatutako baliabideen bidez entregatzea. Egoera honetan dagoen azpikontratu bat ezin da erabili baliabide eta materialen proiektuen eskakizunak estimatzeko eta hornitzeko, eta, gainera, ezin da erreferentzia egin proiektu batean denbora, gastu eta materialaren erabilera. Egoeran horretan dauden azpikontratuak ezin dira editatu edo ezabatu. | Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
