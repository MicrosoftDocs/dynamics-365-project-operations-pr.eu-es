---
title: Azpikontratatuaren lerroko baliabideak
description: Gai honetan saltzaileak denboraz azpikontratatzeko lerro zehatz baterako eskaintzen dituen baliabide dedikatuak nola zehaztu azaltzen da.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 48440f82170bde7f0a0a45f8f9849d688b232949
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323356"
---
# <a name="subcontract-line-resources"></a>Azpikontratatuaren lerroko baliabideak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Urtean Dynamics 365 Project Operations, saltzaile batek azpikontratazio lerroan denbora batez erosten ari den baliabide gaitasuna hornitzeko erabiliko diren baliabideak zehaztu ditzake.

## <a name="create-subcontract-line-resources"></a>Sortu azpikontratuaren lerroaren baliabideak

Azpikontratuaren lerroaren baliabideak sortzeko, osatu hurrengo urratsak.

1. Nabigazio panelean, hautatu **Azpikontratak**, eta ireki lan egin nahi duzun azpikontratua.
2. Ireki azpikontratazio lerroa saltzailearen baliabideak zehaztu nahi dituzun denborarako.
3. Hurrengoan **Azpikontratuaren lerroaren baliabideak** fitxa, azpisaretan, hautatu **+ Azpikontratuaren lerroaren baliabide berria**.
4. Hurrengoan **Azpikontratuaren lerroaren mugarri berria** orria, idatzi eskatutako informazioa eta gero hautatu **Gorde eta itxi**.

Hurrengo taulan azpi-kontratazio lerroaren baliabideak azaltzen dira.

| Eremua |  Deskribapenak |
| ----- | ------------ |
| Baliabide erreserbagarria | Aukeratu azpikontratazio lerroan baliabide gisa erabili nahi duzun "Kontratuetako langilea" motako baliabide erreserbagarria. Oraindik itunpeko langilearentzako erreserbatzeko baliabiderik sortu ez baduzu, utzi eremu hau hutsik. Erregistroa gordetzean erreserbatzeko baliabide bat sortzen da.  |
| Contact | Bada **Erreserbatzeko Baliabidea** eremua hutsik dago, azpikontratatutako lineako baliabidea sor dezakezu lehendik dagoen kontaktu batetik. Erabili bilaketa sistemako kontaktu aktiboen zerrenda ikusteko. Hautatu azpikontratu honen saltzailearen kontaktu bat. Erregistroa gordetzean hautatzen duzun kontaktua balioztatzen da. Aukeratu duzun kontaktua baliozko kontaktua ez bada, zure erregistroa ez da gordeko. Aukeratutako kontaktuarentzako erreserbatzeko baliabiderik ez badago, sistemak hautatutako kontaktuarentzako erreserbagarria den baliabide bat sortzen du azpikontrataren lineako baliabidea sortu aurretik. |
| Erabiltzailea | Bada **Erreserbatzeko Baliabidea** eremua hutsik dago, azpikontratatutako lineako baliabidea hautatuz erabiltzaile aktibo bat. Erabili bilaketa sistemako erabiltzaile aktiboen zerrenda ikusteko. Aukeratutako erabiltzailearentzako erreserbatzeko baliabiderik ez badago, sistemak hautatutako erabiltzailearentzako erreserbagarria den baliabide bat sortzen du azpikontrataren lineako baliabidea sortzen da. |
| Hasiera-data | Azpikontratako langilearen esleipena hasiko den eguna. Baliabide hau data tarte hori baino lehenagokoa den denboraldi baterako erreserbatzen bada, abisua agertuko da. |
| Amaiera-data | Azpikontratako langilearen esleipena amaituko den eguna. Baliabide hau data tarte horren ostekoa den denboraldi baterako erreserbatzen bada, abisua agertuko da. |
| Ahalegina | Azpikontratetako langileak azpikontratazio lerro honetan emango dituen ahalegin kopurua. Baliabide hau azpikontrata honetan bideratzen duten esfortzutik harago gordetzen bada, abisua agertuko da. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
