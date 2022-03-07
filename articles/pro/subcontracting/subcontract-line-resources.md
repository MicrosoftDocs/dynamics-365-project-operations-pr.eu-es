---
title: Azpikontratatuaren lerroko baliabideak
description: Gai honetan saltzaileak denboraz azpikontratatzeko lerro zehatz baterako eskaintzen dituen baliabide dedikatuak nola zehaztu azaltzen da.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4a929b985a51ab49d3e34ce4a5c277af4c05c216
ms.sourcegitcommit: d507a75a19c992a9421e4f3605162a2faa84a445
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/27/2021
ms.locfileid: "7558442"
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
4. **Azpikontratazioaren lineako baliabide berria** orrian, sartu beharrezko informazioa eta hautatu **Gorde eta itxi**.

Hurrengo taulan azpi-kontratazio lerroaren baliabideak azaltzen dira.

| Eremua | Deskribapenak | Inpaktu funtzionala |
| ----- | ----------- | ----------------- |
| Baliabide erreserbagarria | Aukeratu azpikontratazio lerroan baliabide gisa erabili nahi duzun **Kontratuetako langilea** motako baliabide erreserbagarria.| Kontratatutako langilearentzako erreserbatzeko baliabiderik sortu ez baduzu, utzi eremu hau hutsik. Erregistroa gordetzean erreserbatzeko baliabide bat sortuko da.  |
| Contact | Zure azpikontrata lineako baliabidea sor dezakezu lehendik dagoen kontaktu batetik. Erabili bilaketa sistemako kontaktu aktiboen zerrenda ikusteko. Hautatu azpikontratu honen saltzailearen kontaktu bat. Aukeratu duzun kontaktua azpikontratako saltzailearentzako baliozko kontaktua ez bada, azpikontrataren lineako baliabideen erregistroa ez da gordeko.| Aukeratutako kontaktuarentzako erreserbatzeko baliabiderik ez badago, sistemak hautatutako kontaktuarentzako erreserbagarria den baliabide bat sortzen du azpikontrataren lineako baliabidea sortu aurretik. |
| Erabiltzailea | Azpikontratatzeko lineako baliabide bat sor dezakezu erabiltzaile aktibo bat hautatuta. Erabili bilaketa sistemako erabiltzaile aktiboen zerrenda ikusteko.| Aukeratutako erabiltzailearentzako erreserbatzeko baliabiderik ez badago, sistemak hautatutako erabiltzailearentzako erreserbagarria den baliabide bat sortzen du azpikontrataren lineako baliabidea sortzen da. |
| Hasiera-data | Azpikontratako langilearen esleipena hasiko den eguna.| Baliabide hau data tarte hori baino lehenagokoa den denboraldi baterako erreserbatzen bada, abisua agertuko da. |
| Amaiera-data | Azpikontratako langilearen esleipena amaituko den eguna.| Baliabide hau data tarte horren ostekoa den denboraldi baterako erreserbatzen bada, abisua agertuko da. |
| Ahalegina | Kontratatutako langileak azpikontratazio linea honetan emango dituen ahalegin ordu kopurua.| Baliabide hau azpikontratu honetan ematen den esfortzuaz haratago gordetzen bada, abisua agertuko da. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
