---
title: Benetako datuen zuzenketa masiboak onartutako denboraren eta gastuen sarrerek arabera
description: Gai honetan administratzaile batek aurrez onartutako orduaren edo gastuen sarreran zuzenketa bat edo masibo bat nola egin dezakeen azaltzen da, fakturazioa osatu gabe badago.
author: rumant
manager: AnnBe
ms.date: 04/02/2020
ms.topic: article
ms.service: dynamics-ax-applications
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
search.app:
- ProjectOperations
ms.openlocfilehash: 063c4d017f5904f09c3c239bfa432a128872e4d7
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144938"
---
# <a name="bulk-corrections-of-actuals-created-by-approved-time-and-expense-entries"></a>Benetako datuen zuzenketa masiboak onartutako denboraren eta gastuen sarrerek arabera

[!include [banner](../includes/psa-now-project-operations.md)]

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

![Benetako datuekin erlazionatutako ikuspegi-zerrenda](https://github.com/MicrosoftDocs/dynamics-365-customer-engagement-pr/blob/bulk-corrections-actuals-created-by-approved-time-expense-entries.md/time-actuals.png)
 
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

![Gastuen benetako datuak](https://user-images.githubusercontent.com/60806505/77122219-4cd52900-69fa-11ea-8349-ccd2ffebf640.png)
