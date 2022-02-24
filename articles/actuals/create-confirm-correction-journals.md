---
title: Zuzenketa-egunkariak sortu eta berretsi
description: Gai honek zuzenketa-egunkari bat sortzeari eta hura berresteari buruzko informazioa ematen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 6cc22168cdfefc4ae7b833bea75f68ba37c1ee67
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127728"
---
# <a name="create-and-confirm-correction-journals"></a>Zuzenketa-egunkariak sortu eta berretsi

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Batzuetan, denbora edo gastuen sarrera bat okerra izan daiteke. Adibidez, baliteke aholkulari batek data okerra aukeratzea denbora-sarreran edo baliteke zenbakiekin nahastea gastu bat idaztean. Aholkulari batek ezin badu bidalitako sarreren eguneratzeak egin, administratzaile batek zuzenean zuzendu dezake proiektuko sarrera.

Gai honetako prozedurak betetzeko, Administratzailearen baimenak beharko dituzu.

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

Adibidez, grafiko honetan, bi errenkada-elementu daude, Zenbatekoa zutabean 8,00 zenbatekoko zordunketak zerrendatuta dituenak. Gainera, Zenbatekoa zutabean zordundutako zenbatekoak dituzten -8,00 zenbatekoko bi errenkada daude. Horrela zuzenketarekin zenbatekoa zero da.

 
## <a name="correct-approved-expense-entries"></a>Zuzendu onartutako gastuen sarrerak

Bete urrats hauek gastuen sarrera bat edo gehiago zuzentzeko. 

1. **Salmentak** eremuan, ezkerreko nabigazio-panelean, **Transakzioak** aukeraren azpian, hautatu **Onartutako gastuak**.

2. **Onartutako gastuak** zerrendan, hautatu zuzendu nahi duzun proiektua eta hautatu **Zuzendu sarrerak**. Zuzenketa-aldizkari berri bat sortuko da automatikoki esleitutako **Gastuen zuzenketa** motarekin. 

3. **Aldizkari berria** orrialdean, idatzi zuzenketaren **Deskribapena** eta **Gastuen zuzenketa** fitxan, **Gastuen balio berriak** sekzioan, hautatu hautatutako gastuen zerrenden zuzendu nahi dituzun datu-eremuetan. Adibidez, gastua beste **Proiektu** bati eslei dakiokezu edo **Gastu-kategoria**, **Gastu-data** edo **Erreserbatzeko baliabidea** zuzen dezakezu.

4. Hautatu **Aurrebista**. Elkarrizketa-koadroan, hautatu **Ados**. 

5. Egiaztatu **Aldizkari-lerroak** fitxako zuzenketak. Aldatu eta zuzendu diren hautatutako denbora-sarrerekin lotutako jatorrizko benetako gastuen zerrenda ikus dezakezu.

6. Zuzendutako balioak espero bezala agertzen badira, hautatu **Berretsi**. Elkarrizketa-koadroan, hautatu **Ados**. Balioak ez badira espero bezala erakusten, hautatu **Utzi** **Onartutako gastuak** zerrendara itzultzeko. Errepikatu 2. urratsetik 5. urratsera. 

> [!NOTE]
> Zuzendutako benetako datuek **Gastuen balio berriak** sekzioan hautatutako balio berak dituzte.

7. Zuzenketa-aldizkaria berretsi ondoren, zoaz eguneratu dituzun proiektuetara, aldaketak ikusteko.  

8. Proiektuaren orrian, **Benetako datuak** fitxan, berrikusi **Ikuspegiarekin erlazionatutako benetako datuak**. Jatorrizko sarrerak eta zuzendutako sarrerak zerrendatzen dira. Grafiko hauetan jatorrizko gastuen sarrera-zenbatekoak eta dagozkion zuzendutako gastuen sarrera-zenbatekoak erakusten dira. 


