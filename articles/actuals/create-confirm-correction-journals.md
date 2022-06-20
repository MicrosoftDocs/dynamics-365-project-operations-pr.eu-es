---
title: Zuzenketa-egunkariak sortu eta berretsi
description: Artikulu honek zuzenketa aldizkari bat sortzeari eta baieztatzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 70886aa5a3060fa58461ce215e4de3b7286093e3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928049"
---
# <a name="create-and-confirm-correction-journals"></a>Zuzenketa-egunkariak sortu eta berretsi

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Batzuetan, baliteke denbora edo gastuen sarrera gaizki sartzea. Adibidez, aholkulari batek data okerra hauta dezake ordu-sarrera bat sortzen duenean, edo proiektu okerra hauta dezake gastu bat sartzen dutenean. Aholkulari batek ezin baditu bidalitako sarrerak eguneratu, backend-eko administratzaileak zuzenean zuzendu ditzake proiektu baten benetakoak.

## <a name="correct-approved-time-entries"></a>Zuzendu onartutako denbora-sarrerak     

Bete urrats hauek proiektu bateko denbora-sarrera bakarrak edo bat baino gehiago zuzentzeko.

1. **Salmentak** eremuan, hautatu **Transakzioak** eta, ondoren, hautatu **Onartutako ordua**. 

2. **Onartutako ordua** zerrendan, kokatu eta hautatu onartutako denbora-sarrera bat edo gehiago zuzentzeko. Lotutako sarrerak aurkitzeko iragazkia erabil dezakezu. Adibidez, Proiektuaren ID bat iragazi eta Proiektu ID horrekin onartutako denbora-sarrera guztiak hauta ditzakezu.

3. Hautatu **Zuzendu sarrera**. Zuzenketa-aldizkari berri bat sortuko da automatikoki, esleitutako **Denboraren zuzenketa** motarekin. Aukeratutako sarrerak aldizkarian gehituko dira. 

4. **Aldizkari berria** orrian, sartu **Deskribapena** zuzenketa-aldizkarian eta, ondoren, hautatu **Ordu-sarreraren zuzenketak** fitxa.  

5. **Denbora-sarreren balio berriak** atalean, eguneratu eremuak informazio egokiarekin behar ahala. Adibidez, esleitutako proiektua edo baliabide eserbagarria alda dezakezu.

6. Hautatu **Aurrebista**. Elkarrizketa-koadroan, hautatu **Ados**. **Aldizkari-lerroak** fitxan, aldatu eta zuzendu diren hautatutako denbora-sarrerekin lotutako jatorrizko benetako datuen zerrenda ikus dezakezu. Zuzenketa osagarriak egin behar badira, errepikatu 5. eta 6. urratsak. 

    > [!NOTE]
    > Zuzendutako benetako datuek **Denboraren sarrerako balio berriak** sekzioan hautatutako balio berak dituzte.

7. Zuzenketak espero bezala agertzen badira, hautatu **Berretsi**. Elkarrizketa-koadroan, hautatu **Ados**.

8. **Salmentak** eremuan, hautatu **Proiektuak** eta, ondoren, ireki denboraren sarrerak eguneratu dituzun proiektua. 

9. **Proiektuak** orrialdean, **Benetako datuak** fitxan, ikusi egin dituzun aldaketak. 

    > [!NOTE]
    > **Benetako datuak** fitxa ez badago ikusgai, hautatu **Erlazionatutakoak** > **Benetako datuak** aukera.  

10. **Ikuspegiaren erlazionatutako benetako datuak** zerrendan, aldatu den jatorrizko denbora-sarrerak zerrendatuta jarraitzen duela ikus dezakezu, dagozkion zuzendutako sarrerekin batera. 

 
## <a name="correct-approved-expense-entries"></a>Zuzendu onartutako gastuen sarrerak

Bete urrats hauek gastuen sarrera bat edo gehiago zuzentzeko. 

1. **Salmentak** eremuan, ezkerreko nabigazio-panelean, **Transakzioak** aukeraren azpian, hautatu **Onartutako gastuak**.

2. **Onartutako gastuak** zerrendan, hautatu zuzendu nahi duzun proiektua eta hautatu **Zuzendu sarrerak**. Zuzenketa-aldizkari berri bat sortuko da automatikoki esleitutako **Gastuen zuzenketa** motarekin. 

3. **Aldizkari berria** orrialdean, idatzi zuzenketaren **Deskribapena** eta **Gastuen zuzenketa** fitxan, **Gastuen balio berriak** sekzioan, hautatu hautatutako gastuen zerrenden zuzendu nahi dituzun datu-eremuetan. Adibidez, gastua beste **Proiektu** bati eslei dakiokezu edo **Gastu-kategoria**, **Gastu-data** edo **Erreserbatzeko baliabidea** zuzen dezakezu.

4. Hautatu **Aurrebista**. Elkarrizketa-koadroan, hautatu **Ados**. 

5. Egiaztatu **Aldizkari-lerroak** fitxako zuzenketak. Aldatu eta zuzendu diren hautatutako denbora-sarrerekin lotutako jatorrizko benetako gastuen zerrenda ikus dezakezu.

6. Zuzendutako balioak espero bezala agertzen badira, hautatu **Berretsi**. Elkarrizketa-koadroan, hautatu **Ados**. Balioak ez badira espero bezala erakusten, hautatu **Utzi** **Onartutako gastuak** zerrendara itzultzeko. Errepikatu 2. urratsetik 5. urratsera. 

7. Zuzenketa aldizkaria berretsi ondoren, itzuli eguneratu dituzun proiektura edo proiektuetara aldaketak ikusteko.

8. Proiektuaren orrian, gunean **Benetakoak** fitxa, berrikusi **Benetako Lotutako Ikuspegia** zerrenda. Jatorrizko sarrerak eta zuzendutako sarrerak zerrendatzen dira.


## <a name="correct-approved-material-usage-logs"></a>Onartutako materialaren erabileraren erregistroak zuzentzea

Bete urrats hauek materialaren erabileraren erregistroko sarrera bat edo gehiago zuzentzeko.

1. urtean **Salmentak** eremua, ezkerreko nabigazio-panelean, azpian **Transakzioak**, hautatu **Benetakoak**.

2. urtean **Benetakoak** zerrenda, erabili zutabe-iragazkiak hautatzeko **Materiala** transakzio-klasea, materialen errealak soilik erakusten dira. Erabili beste zutabe-iragazkiak erakusten diren benetakoak gehiago mugatzeko. Nahi duzun benetako multzoa aurkitu ondoren, hautatu benetakoak eta, ondoren, hautatu **Sarrera zuzenak**. Zuzenketa aldizkari berri bat automatikoki sortzen da, eta **Materialaren zuzenketa** mota esleitzen zaio.

3. Gainean **Aldizkari Berria** orrialdean, in **Deskribapena** eremuan, idatzi zuzenketaren deskribapena. Ondoren, gainean **Material Zuzenketa** fitxan, **Materialentzako balio berriak** atalean, hautatu hautatutako material-lerroetarako zuzentzeko datu-eremuak. Adibidez, materiala beste proiektu bati esleitu diezaiokezu, edo produktua, materialaren data edo azpikontratua zuzendu.

4. Hautatu **Aurrebista**. Ondoren, elkarrizketa-koadroan, hautatu **Ados**.

5. Gainean **Aldizkariaren lerroak** fitxa, egiaztatu zuzenketak. Alderantzikatu diren hautatutako material-sarrerekin eta sortu diren dagozkien lerro zuzenduekin erlazionatutako jatorrizko benetakoen zerrenda ikus dezakezu.

6. Zuzendutako balioak espero bezala agertzen badira, hautatu **Berretsi**. Ondoren, elkarrizketa-koadroan, hautatu **Ados**. Balioak espero zirenak ez badira, hautatu **Utzi** itzultzeko **Benetakoak** zerrenda. Ondoren, errepikatu 2tik 5era bitarteko urratsak.

7. Zuzenketa aldizkaria berretsi ondoren, itzuli eguneratu dituzun proiektura edo proiektuetara aldaketak ikusteko.

8. Proiektuaren orrian, gunean **Benetakoak** fitxa, berrikusi **Benetako Lotutako Ikuspegia** zerrenda. Jatorrizko sarrerak eta zuzendutako sarrerak zerrendatzen dira.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
