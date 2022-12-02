---
title: Konfiguratu kontratudun langileak eta azpikontratatutako ahalmena erakusteko Antolaketa-panela
description: Artikulu honek Schedule Board nola konfiguratu deskribatzen du Microsoft Dynamics 365 Project Operations azpikontratatutako baliabideen gaitasuna erakusteko proiektuaren baliabideen eskakizunak betetzean.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 355691b63f437de789afab499369afcdf87e6d3d
ms.sourcegitcommit: b2224d1f3c0bd4925d647e6ca3960db81a209521
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/11/2022
ms.locfileid: "9262201"
---
# <a name="configure-schedule-board-to-show-contract-workers-and-subcontracted-capacity"></a>Konfiguratu kontratudun langileak eta azpikontratatutako ahalmena erakusteko Antolaketa-panela 

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Programazio taula Microsoft-en Dynamics 365 Project Operations baliabideak bilatzeko bi modutara erabil daiteke:

- Baliabideen bilaketa orokorra proiektuetan oinarritutako baliabide-eskakizun zehatzen testuingururik gabe.
- Baldintza-baliabide espezifikoen bilaketa non proiektuaren eskakizunak iradokitako baliabideen testuingurua emango duen.

Programazio-batzordeari azpikontratatutako baliabideen gaitasunaren eta lan-kontratuko langileen berri emateko, eguneraketak egin behar dituzu Programazio-taularen ezarpenak. Eguneratze horiek barne hartzen dute: 
- Eguneratu programazio taularen ezarpenak baliabideen bilaketa orokorrerako.
- Eguneratu programazio taularen ezarpenak baliabideen bilaketa eskakizunetan oinarritutakoa.

## <a name="update-schedule-board-settings-for-general-resource-search"></a>Eguneratu programazio taularen ezarpenak baliabideen bilaketa orokorrerako
### <a name="update-filters-for-general-resource-search"></a>Eguneratu iragazkiak baliabide orokorrak bilatzeko
Baliabide bat bilatzen duzunean, programazio-taulan eskuragarri dauden iragazkiak eguneratu behar dira, kanpoko baliabideak ere bilatu ahal izateko, hauetako bat edo guztiak zehaztuz:
  - Langile mota, erakutsitako baliabideak lan-kontratuko langileak edo langileak izan behar diren.
  - Baliabidea dagokion enpresa saltzailea.
  - Azpikontratu edo azpikontratazio lerro zehatz bati dagozkion baliabideak.
    
### <a name="update-retrieve-resource-query"></a>Eguneratu eskuratu baliabide-kontsulta
Bilaketarako erabilitako kontsulta ere eguneratu behar da iragazki-atributu osagarri hauek erabiltzeko. Erabili urrats hauek programazioaren antolaketa konfigurazioa eguneratzeko baliabideen bilaketa orokorrerako:  
1. Ireki **Antolatu taularen ezarpenak** Ordutegi Batzorde espezifiko baterako.
2. Ireki **Ezarpen orokorrak** fitxa eta joan hona **Beste ezarpen batzuk**.
3. Atal honetako ezarpenen zerrendan, eguneratu **Iragazkien diseinua** hona: **Iragazki-diseinu lehenetsia Project Operations Lite-rako**.
4. Eguneratu **Berreskuratu Baliabideen Kontsulta** hona: **Project Operations Lite-rako baliabideen kontsulta lehenetsia**.

![Eguneratu programazio taularen ezarpenak baliabideen bilaketa orokorrerako](../media/BoardSettings.png)  

## <a name="update-schedule-board-settings-for-requirementbased-resource-search"></a>Eguneratu programazio taularen ezarpenak baliabideen bilaketa eskakizunetan oinarritutakoa
### <a name="update-filters-for-requirement-specific-resource-search"></a>Eguneratu iragazkiak eskakizunen berariazko baliabideak bilatzeko 
Baliabide bat bilatzen duzunean, programazio-taulan eskuragarri dauden iragazkiak eguneratu behar dira, kanpoko baliabideak ere bilatu ahal izateko, hauetako bat edo guztiak zehaztuz:
 - Langile mota, erakutsitako baliabideak lan-kontratuko langileak edo langileak izan behar diren.
 - Baliabidea dagokion enpresa saltzailea.
 - Azpikontratu edo azpikontratazio lerro zehatz bati dagozkion baliabideak.

### <a name="update-retrieve-resource-query-for-requirement-specific-resource-search"></a>Eguneratu berreskuratzeko baliabideen kontsulta eskakizunen berariazko baliabideen bilaketarako 
Bilaketarako erabilitako kontsulta ere eguneratu behar da iragazki-atributu osagarri hauek erabiltzeko. Erabili urrats hauek programazioaren antolaketa konfigurazioa eguneratzeko eskakizunetan oinarritutako baliabideen bilaketarako:

1. Ireki **Antolatu taularen ezarpenak** Ordutegi-taula zehatz baterako eta gero hautatu **Ireki Ezarpen lehenetsiak** eskakizun zehatzen bilaketarako ezarpenak irekitzeko.
2. Ireki **Ezarpen orokorrak** fitxa eta joan hona **Beste ezarpen batzuk**.
3. Atal honetako ezarpenen zerrendan, eguneratu **Iragazkien diseinua** hona: **Iragazki-diseinu lehenetsia Project Operations Lite-rako**.
4. Eguneratu **Berreskuratu Baliabideen Kontsulta** hona: **Project Operations Lite-rako baliabideen kontsulta lehenetsia**.
5. Ireki **Ordutegi motak** fitxa eta joan **Proiektua**.
6. Ezarpenen azpian **Proiektua**, eguneratu **Programazio Laguntzailea baliabideak berreskuratzeko kontsulta** hona **Proiektu Operations Literako baliabideen kontsulta lehenetsia** eta eguneratu **Programazio Laguntzailea Berreskuratu Murrizketen Kontsulta** hona **Lehenetsitako Berreskuratu Murrizketen Kontsulta Project Operations Literako**.

![Eguneratu programazio taularen ezarpenak baliabideen bilaketa eskakizunetan oinarritutakoa](../media/SASettings.png)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
