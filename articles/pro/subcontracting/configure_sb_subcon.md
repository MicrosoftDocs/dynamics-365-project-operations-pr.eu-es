---
title: Konfiguratu Schedule Board lan-kontratuko langileak eta azpikontratatutako gaitasuna erakusteko
description: Gai honek Microsoft-en Schedule Board nola konfiguratu deskribatzen du Dynamics 365 Project Operations azpikontratatutako baliabideen gaitasuna erakusteko proiektuaren baliabideen eskakizunak betetzean.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: d645dee741a45dcb0219e4e4f58a329b7b873e10
ms.sourcegitcommit: 45893132bd8bfaf944ee0ac855484684dd1ee945
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/09/2021
ms.locfileid: "7902983"
---
# <a name="configure-schedule-board-to-show-contract-workers-and-subcontracted-capacity"></a>Konfiguratu Schedule Board lan-kontratuko langileak eta azpikontratatutako gaitasuna erakusteko 

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Programazio taula Microsoft-en Dynamics 365 Project Operations baliabideak bilatzeko bi modutara erabil daiteke:

- Baliabideen bilaketa orokorra proiektuetan oinarritutako baliabide-eskakizun zehatzen testuingururik gabe.
- Baldintza-baliabide espezifikoen bilaketa non proiektuaren eskakizunak iradokitako baliabideen testuingurua emango duen.

Programazio-batzordeari azpikontratatutako baliabideen gaitasunaren eta lan-kontratuko langileen berri emateko, eguneraketak egin behar dituzu Programazio-taularen ezarpenak. Eguneratze hauek honako hauek dira: 
- Eguneratu Schedule Board ezarpenak baliabideen bilaketa orokorrerako.
- Eguneratu Schedule Board ezarpenak eskakizunetan oinarritutako baliabideen bilaketarako.

## <a name="update-schedule-board-settings-for-general-resource-search"></a>Eguneratu Schedule Board ezarpenak baliabideen bilaketa orokorrerako
### <a name="update-filters-for-general-resource-search"></a>Eguneratu iragazkiak baliabide orokorrak bilatzeko
Baliabide bat bilatzen duzunean, programazio-taulan eskuragarri dauden iragazkiak eguneratu behar dira, kanpoko baliabideak ere bilatu ahal izateko, hauetako bat edo guztiak zehaztuz:
  - Langile mota, erakutsitako baliabideak lan-kontratuko langileak edo langileak izan behar diren.
  - Baliabide bat izan behar duen enpresa saltzailea.
  - Azpikontratu edo azpikontratu lerro zehatz bati dagozkion baliabideak.
    
### <a name="update-retrieve-resource-query"></a>Eguneratu baliabideen kontsulta berreskuratzeko
Bilaketarako erabilitako kontsulta ere eguneratu behar da iragazki-atributu osagarri hauek erabiltzeko. Erabili urrats hauek Schedule Board konfigurazioa eguneratzeko baliabideen bilaketa orokorrerako:  
1. Ireki **Antolatu taularen ezarpenak** Ordutegi Batzorde espezifiko baterako.
2. Ireki **Ezarpen orokorrak** fitxa eta joan hona **Beste ezarpen batzuk**.
3. Atal honetako ezarpenen zerrendan, eguneratu **Iragazkien diseinua** to **Iragazki-diseinu lehenetsia Project Operations Lite-rako**.
4. Eguneratu **Berreskuratu Baliabideen Kontsulta** to **Lehenetsitako Berreskuratu Baliabideen Kontsulta Project Operations Literako**.

![Eguneratu Schedule Board ezarpenak baliabideen bilaketa orokorrerako](../media/BoardSettings.png)  

## <a name="update-schedule-board-settings-for-requirementbased-resource-search"></a>Eguneratu Schedule Board ezarpenak eskakizunetan oinarritutako baliabideen bilaketarako
### <a name="update-filters-for-requirement-specific-resource-search"></a>Eguneratu iragazkiak eskakizunen araberako baliabideen bilaketarako 
Baliabide bat bilatzen duzunean, programazio-taulan eskuragarri dauden iragazkiak eguneratu behar dira, kanpoko baliabideak ere bilatu ahal izateko, hauetako bat edo guztiak zehaztuz:
 - Langile mota, erakutsitako baliabideak lan-kontratuko langileak edo langileak izan behar diren.
 - Baliabide bat izan behar duen enpresa saltzailea.
 - Azpikontratu edo azpikontratu lerro zehatz bati dagozkion baliabideak.

### <a name="update-retrieve-resource-query-for-requirement-specific-resource-search"></a>Eguneratu berreskuratzeko baliabideen kontsulta eskakizunen berariazko baliabideen bilaketarako 
Bilaketarako erabilitako kontsulta ere eguneratu behar da iragazki-atributu osagarri hauek erabiltzeko. Erabili urrats hauek Schedule Board konfigurazioa eskakizunetan oinarritutako baliabideen bilaketa eguneratzeko:

1. Ireki **Antolatu taularen ezarpenak** Ordutegi-taula zehatz baterako eta gero hautatu **Ireki Ezarpen lehenetsiak** eskakizun zehatzen bilaketarako ezarpenak irekitzeko.
2. Ireki **Ezarpen orokorrak** fitxa eta joan hona **Beste ezarpen batzuk**.
3. Atal honetako ezarpenen zerrendan, eguneratu **Iragazkien diseinua** to **Iragazki-diseinu lehenetsia Project Operations Lite-rako**.
4. Eguneratu **Berreskuratu Baliabideen Kontsulta** to **Lehenetsitako Berreskuratu Baliabideen Kontsulta Project Operations Literako**.
5. Ireki **Ordutegi motak** fitxa eta joan **Proiektua**.
6. Ezarpenen azpian **Proiektua**, eguneratu **Programazio Laguntzailea baliabideak berreskuratzeko kontsulta** to **Lehenetsitako Berreskuratu Baliabideen Kontsulta Project Operations Literako** eta eguneratu **Programazio Laguntzailea Berreskuratu Murrizketen Kontsulta** to **Lehenetsitako Berreskuratu Murrizketen Kontsulta Project Operations Literako**.

![Eguneratu Schedule Board ezarpenak eskakizunetan oinarritutako baliabideen bilaketarako](../media/SASettings.png)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
