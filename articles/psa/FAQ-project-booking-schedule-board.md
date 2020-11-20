---
title: Sortu proiektu-erreserba bat antolaketa-paneletik
description: Gai honek proiektuaren erreserba egitasmoaren taulan sortzen den informazioa eskaintzen du.
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
ms.openlocfilehash: ccbfedec82b2d9035b51cf1b283ae5c441f1cbcc
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122283"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a>Sortu proiektu-erreserba bat antolaketa-paneletik

Baliabide bat erreseba dezakezu zuzenean **Taldea** fitxan proiektua taldearen proiektuan edo baliabide eskakizun batetik orokorra taldearen kide zeregin bat sortzen eta, ondoren, osatu proiektua taldearen kide honekin sortutako eskakizun hauen artean.

Baliabidearen antolaketa-panelan zuzenean proiektua inprimatu ere erreserbatutako dezakezu. Hiru era daude hau ebazteko:

- **Sortutako baliabide eskakizuna erreserbatu:** baliabideen eskakizuna sor dezakezu baliabide generiko bat sortu eta proiektu baten barruan zereginak esleitu ondoren.

- **Liburua bete beharrekoa:** eskakizun nagusienak Ordutegiaren taulan agertzen dira **Proiektua** fitxa. 

- **Erreserbatu baliabide eskakizun berri batetik:** baliabide eskakizuna hutsetik sor dezakezu eta proiektu batekin lotu. Antolaketa-taulan, baliabide-eskakizunak **Ireki eskakizunak** fitxan agertzen dira.

## <a name="book-from-a-generated-resource-requirement"></a>Erreserbatu sortutako baliabide eskakizun batetik

Baliabide orokorra sortzeko eta zeregin bat edo gehiago proiektua barruan esleitu. Gero, sortu baliabide-eskakizun bat taldeko kide orokor batetik. 

1.  Tresna-barran antolaketa-panelan, baliabide hau erakutsiko tresna-barran, **Ireki Eskakizunak** fitxa. Baliteke erabili behar duzu zutabe iragazkiak saretan hainbat eskakizunak irekita baldin baduzu. 

    ![Ireki Eskakizunak fitxa Antolaketa panelean](media/FAQ-Project-Booking-Schedule-Board-1.png "Taula bookings eta esleipenetan Eginbideei")

2. Hautatu eskakizuna. **Bilaketa erabilgarritasuna** fitxa agertuko da hautatutako errenkada goialdean.
 
3. Fitxan hautatzean, hautatu antolaketa board Antolaketa-panela modua launches eta iragazkiak baliabide eskakizun betetzen dituzten erabilgarri dauden baliabideak. Gero, bertatik baliabide erreserbatutako dezakezu.

4. Arrastatu ataleko eta dezakezu antolaketa board beheko batetik errenkada hautatutako goiko gelaxkan baliabide bat ezabatu. Duenean jareginez da, bertan irekitzen du **Baliabide Booking Sortu** eskuineko panela.

    Hautatu **Liburua** books baliabide talde proiektua inprimatu.

![Sortu baliabide-erreserba panela](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a>Eskakizun Nagusia liburua

Xede proiektuaren Project Service automatikoki sortu Eskakizun Nagusia izeneko baliabide eskakizun sortzen da. Bizkor erreserbatutako baliabide bat antolaketa board gabe eskakizun bat sortzeko erabiltzen den eskakizun hutsik bat da. Eskakizun-hutsik dagoelako datak lehendabizi, guztirako baldintza kopuruak metodoa eta orduak ahal bada zehaztu behar duzu. 

1. Lehen eskakizunarekin baliabide bat erreserbatzeko, antolaketa-taulan, hautatu **Proiektua** fitxa. Baliteke zutabeko irizpidea erabiltzea **Proiektua** zutabean, hainbat proiektu badituzu.

   ![Zutabe-iragazkiak Antolaketa panelean](media/FAQ-Project-Booking-Schedule-Board-2.png "Taula bookings eta esleipenetan Eginbideei")

2. Hautatu eskakizun batek bere izena proiektua izena eta 0-iraupena da.

3. Hautatu **Bilaketa erabilgarritasuna** fitxa, errenkadan agertzen dena. Hori puts antolaketa-panela Antolaketa Laguntzailearen moduan, eta erabilgarri dauden baliabideak proiektuan inprimatu booked daitezke erakusten du.

4. **Eskakizun Nagusia** 0 iraupena batekin eskakizun hutsik bat denez, behar duzu iraupena ezartzen, **Sortu Baliabide Erreserbatu** panela booking baliabide bat eta hautatu.

5. Hautatu antolaketa board behealdean **Proiektua Nagusia Eskakizun** eta arrastatu eta dezakezu, baliabide bat erreserbatutako da ezabatu.
 
    **Eskakizun Nagusia** 0 iraupena batekin eskakizun hutsik bat denez, behar duzu iraupena ezartzen, **Sortu Baliabide Erreserbatu** panela booking baliabide bat eta hautatzen duzunean eta baliabidea erreserbatzen duzunean.
 
    Tresna-barran antolaketa board **Nagusia Eskakizun** bidez baliabide erreserbatutako duzunean gehitzen proiektua taldeari esleitutako edozein gabe.
 
## <a name="book-from-a-new-resource-requirement"></a>Erreserbatu baliabide eskakizun berri batetik
Jarraitu hurrengo pausoak baliabide bat antolaketa paneletik liburu bat biguntzeko. 

1. Joan **Baliabideen Eskakizunak** eta gero hautatu **Berria** baliabide eskakizun berri bat sortzeko.

2. **Proiektua** fitxan, hautatu proiektu bat eskakizuna proiektuarekin lotzeko.
 
    Antolaketa-panelan, hori azkenaldian sortutako eskakizun gisa azalduko **Ireki Eskakizuna** bat egin dezakezu duen board antolaketa atalean.

3. Erreserbatu baliabidea proiektuko taldera gehitzeko.

4. Baliabideari booked, dela orain zereginak eskuz esleitu behar duzu.

