---
title: Ikusi baliabideen erabilera kargagarria
description: Gai honek baliabideen erabilerari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: b07af573bc8d312c45ee4aef50c95942401294fa
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285918"
---
# <a name="view-chargeable-utilization-for-resources"></a>Ikusi baliabideen erabilera kargagarria

[!include [banner](../includes/psa-now-project-operations.md)]
 
**Erabileraren ikuspegia** **Project Service-en baliabideen erabilera** orrialdean erreserbagarria den baliabidearen erabilera kargagarria erakusten da. Ikuspegia antolaketan oinarrituta dagoenez aurkituko dituzu funtzio berdin asko.

> ![Ikuspegi Utilization Eginbideei](media/FAQ-utilization-1.png)
 

Kalkuluak chargeable utilization funtzionatzen duela honela:

   Chargeable utilization = (benetako ordu kargagarriak) / (baliabidearen ahalmena).

Gelaxkek kalkulatutako erabilera kargagarria adierazten dute hautatutako aldirako (egunak, asteak edo hilabeteak).

Erakutsi beren helburuko chargeable utilization as compared to baliabide chargeable utilization gelaxka bakoitzak koloreak. 

Helburuko erabilera ezar daiteke edozer baliabideen funtzio lehenetsia edo baliabide taldeetan horri berari. Kalkuluak begiratzen dio helburuko pertsonria lehenik eta behin, eta ondoren, baliabide-funtzio lehenetsiari.

## <a name="set-target-on-a-resource"></a>Ezarri xedea baliabide batean

1. Joan **Baliabideak** \> **Baliabideak** atalera. 
2. Hautatu baliabide bat erregistroa irekitzeko. 
3. **Project Service** fitxan, helburuko erabilera ere ezar dezakezu baliabiderako.

> ![Eginbideei erabiltzearen arriskua helburuko utilization ezartzeko Project Service fitxan aurki daiteke](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a>Ezarri xedeen erabilera funtzio batean

1. Joan **Baliabideak** \> **Baliabidea funtzioak** atalera. 
2. Hautatu funtzio bat erregistroa irekitzeko. 
3. Ezarri helburuko erabilera funtziorako.

> ![Eginbideei erabiltzearen arriskua helburuko utilization ezartzeko Project Service fitxan aurki daiteke](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a>Kalkulatu baliabideen erabilera kargagarria

Baliabide erabilera kargagarria kalkulatzeko aurrebaldintza batzuk bete beharko dituzu. 

### <a name="set-default-role-for-individual-resource"></a>Ezarri funtzio lehenetsia baliabide indibidualetarako

Lehenik, helburuko erabilera ezar daiteke banako baliabidean edo baliabide-funtzioetan. Helburuak baliabide-funtzioak erabiltzen ari bazara, baliabide taldeetan izan behar du funtzio lehenetsia. 

1. Hau ezartzeko, joan **Baliabideak** \> **Baliabideak** atalera. 
2. Aukeratu baliabide bat, ireki erregistroa eta, ondoren, hautatu **Project Service** fitxa. 
3. **Baliabideen funtzioa** saretan, ziurtatu funtzio bat dagoela baliabiderako eta **Lehenespenezkoa da** ezarrita dagoela **Bai** aukeran.
 
### <a name="change-billing-type-for-resource-role"></a>Aldatu baliabide-funtzio honen fakturazio mota.

Baliabide-funtzioak izan fakturazio mota **Kargagarria** ezarri behar da. 

1. Joan **Baliabideak** \> **Baliabidea funtzioak** atalera. 
2. Ireki eguneratu nahi duzun erregistro bat irekitzeko eta, ondoren, ezarri **Kargagarria** mota lehenetsia fakturazio-funtzio bat.

### <a name="set-working-hours-for-resource-role"></a>Ezarri baliabide funtzioetarako lanorduak
 
Baliabidearen ahalmena kalkuluak lanorduak izan behar du. 

1. Joan **Baliabideak** \> **Baliabideak** atalera. 
2. Hautatu baliabidea erregistroa irekitzeko eta hautatu **Erakutsi lanorduak**. 
3. Baliabideen zerrenda eguneratu dezakezu **Lanordu txantiloia** aplikatuz **Baliabide zerrenda** ikuspegitik.

## <a name="troubleshooting-chargeable-actual-hours"></a>Kargatzeko benetako orduak konpontzeko arazoak

Bertan, entitate kargagarria **Benetako datuak** entitatetik hartzen da. Fakturazio-mota dute **Kargagarria** batekin kalkuluetan agertzen dena eta horregatik izan behar duzu projects non sartuko den benetako zenbatekoak kalkulatu direnak chargeable.

Ez chargeable utilization ikusten ari zara, baduzu hona hemen zenbait gauza dezakezu:

- Baliabideak gaitasunerako lanorduak ditu definituta.
- Baliabidea ditu edozer bat zehaztutako banaka utilization helburuko edo da funtzio lehenetsia esleitu bertan. Funtzioa baliozkorik definituta horretarako utilization helburuko ditu.
- Benetako zenbatekoak Kalkulatu fakturazio mota **Kargagarria** izan bat utilization kalkulatzeko expecting dira aldi baterako. Egiaztatu ikusten ari zarela benetakoak baino beste benetako zenbatekoak kalkulatu fakturazio duen erregistro mota:

  - Erabilitako benetakoa funtzioa fakturazio-zerbait beste chargeable baino mota lehenetsia da.
  - Funtzioa proiektua kontratu-lineak proiektuan backing konfiguratu da. ez-chargeable.
  - Proiektuak ez du erlazionatutako kontratuaren lerrorik.



[!INCLUDE[footer-include](../includes/footer-banner.md)]