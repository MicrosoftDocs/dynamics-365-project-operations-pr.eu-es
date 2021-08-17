---
title: Kudeatu proiektuen prezio-zerrendak proiektuko kontratuetan
description: Gai honek proiektuan oinarritutako proiektuaren kontratuan proiektuaren prezio-zerrendak kudeatzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 824026d0620de809c0366c86c2d4d13fe83d4d1ddd4c0dc1cc2645ff712705d5
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6996466"
---
# <a name="manage-project-price-lists-on-project-contracts"></a>Kudeatu proiektuen prezio-zerrendak proiektuko kontratuetan

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations proiektuen kontratuak kontratu bateko salmenta prezioen data eraginkorreko hainbat datu onartzeko diseinatuta daude. Project Operations-en, lotutako erakunde berri bat dago **Proiektuen prezioen zerrendak**. Entitate honek bat-bateko eta besteko harremana du proiektuaren kontratuarekin.

Proiektuen prezioen zerrendak proiektu bateko denbora, materiala eta gastuen transakzioak preziatzeko erabiltzen dira. Kontratu batek proiektuen prezio zerrenda bat edo gehiago dituenean, prezio zerrenda hauek denboraren, materialaren, gastuen kalkuluen eta kontratuari loturiko proiektuen kontratuaren bidez lotzen diren proiektuen prezioak egiteko erabiltzen dira.

Proiektuaren kontratu batean proiektuen prezioen zerrendarik ez dagoenean, abisu-mezu bat ikusiko duzu proiektuaren prezioen zerrendarik ez dagoela eta zure aurrekontuak, egiazko proiektuaren lana, materiala eta erregistratutako gastuak ez direla tasatuko. Ez da salmenta balioen preziorik egongo.

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a>Proiektuaren kontratu batean proiektuaren prezioen zerrenda elkartu edo ez lotu

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-material-and-expenses"></a>Sortu edo lotu prezioen zerrenda zehatz bat proiektuan oinarritutako lana, materiala eta gastuak kalkulatzeko

1. Proiektuaren kontratuan, hautatu **Proiektuen prezioen zerrendak** fitxa.
2. Azpi-sarean, hautatu **+ Gehitu proiektu berriaren prezio zerrenda**.
3. Gainean **Sorrera bizkorra** graduatzailea, hautatu prezioen zerrenda. 

  Goitibeherako zerrendan testuingurua ezarrita duten prezio zerrenda guztiak agertzen dira **Salmentak**, non prezio zerrendako moneta bat datorren kontratuarekin bat datorren.
  
4. Idatzi proiektuaren prezioen zerrenda elkartearen deskribapena, hautatu **Gorde**, eta ondoren itxi **Sortu bizkor** graduatzailea.

   Proiektuaren prezio-zerrendaren lotura sortu da.
   
5. Errepikatu 1-4 urratsak proiektuaren prezio zerrenda bat baino gehiago proiektuaren kontratuarekin lotzeko. Sortu proiektuaren prezio zerrenda bat baino gehiago lotutako proiektuaren prezio zerrenda bakoitzean data eraginkortasuna desberdina baduzu.

> [!NOTE]
> Project Operations-en eragiketek ez dute onartzen proiektuaren prezio zerrenden data eraginkortasuna gainjartzea. Data jakin bat duen transakzio batentzako proiektuen prezioen zerrenda bat badago, transakzio horren prezioa zero izango da lehenespenez.

### <a name="remove-a-project-price-list-association"></a>Kendu proiektuen prezio-zerrenden erlazioa

- Aukeratu proiektuaren prezioen zerrenda, eta hautatu **Ezabatu kontratuaren proiektuaren prezioen zerrenda** azpisarean. 

  Prezioen zerrenda kontratuko proiektuaren prezioen zerrendetatik kentzen da. Prezio zerrenda bera ez da ezabatuko. Kontratuaren elkartea soilik ezabatuko da.

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a>Konfiguratu kontratu batean proiektuen prezioen zerrenden lehenespen automatikoak

Proiektuen prezioen zerrenda proiektuaren prezioen zerrenda lehenetsi gisa ezar daiteke. Konfigurazio horri esker, zure erakundeko kontratu guztiak proiektuaren prezio zerrenda estandar batekin hasten dira beti prezio aldi horretarako.

### <a name="set-up-the-organizational-default-for-project-price-lists"></a>Konfiguratu proiektuaren prezio zerrenden antolakuntza lehenetsia

1. Joan **Ezarpenak** > **Orokorra** eta, ondoren, hautatu **Parametroak**.
2. **Parametro aktiboak** zerrendaren orrian, hautatu eta egin klik bikoitza erregistroan irekitzeko. Egin klik bikoitza egin bitartean, ziurtatu hiperesteka den eremu balio batean klik egiten ez duzula. 
3. **Parametro aktiboak** orrian, hautatu **Prezioen zerrenda** fitxa. Azpisare batek prezioen zerrenda lehenetsien zerrenda erakusten du. Hau da kostuen eta salmenta prezioen zerrenda estandarren zerrenda. **Salmentak** saltzen dituzun moneta guztietan hemen lotutako prezioen zerrendak ziurtatzen du salmenten prezioen zerrenda lehenetsi dela moneta horretan jarduten duten bezeroentzat sortzen dituzun kontratuetan.

### <a name="set-up-a-customer-specific-project-price-list"></a>Konfiguratu bezeroarentzako proiektuaren prezioen zerrenda

Bezeroei buruzko proiektuaren prezioen zerrendak ere konfigura ditzakezu zure bezeroekin prezioen akordio nagusia negoziatu duzunean.

1. Joan **Salmentak** > **Bezeroak** atalera.
2. Kontu aktiboen zerrendan, hautatu prezio zerrenda berezia duen bezeroa.
3. Aukeratu bezeroaren erregistroa irekitzeko eta hautatu **Proiektuen prezioen zerrendak** fitxa. Azpisare batek bezero honen berariazko proiektuen prezioen zerrenda erakusten du. 
4. Sortu prezio zerrenda elkarte berria hemen bezero honen proiektuen prezio zerrenda zehatza izan dezazun.

## <a name="custom-pricing-on-a-project-contract"></a>Proiektuaren kontratuaren prezio pertsonalizatuak

Erakundearen eta bezeroaren berariazko proiektuen prezioen zerrenda lehenetsiak izan ondoren, zure proiektuen kontratuak proiektuen prezioen zerrenda elkarte horiekin sortuko dira automatikoki. Hala ere, proiektuaren kontratu bateko proiektuen prezioen zerrendak beti erantsitako data eta kontratuaren izenarekin kopiatzen dira. Kontu eta proiektuen kudeatzaileak kopia hauen prezioen aldaketak egiten has daitezke. Aldatutako prezio hauek proiektuaren kontratu honi soilik aplikatuko zaizkio.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
