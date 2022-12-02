---
title: Transferitu proiektuaren aurrekontuak urte fiskalaren amaieran
description: Artikulu honek informazioa ematen du gainerako aurrekontu kopuruak etorkizuneko ekitaldietara nola transferitu eta aurrekontuen erregistroaren xehetasunak sortzeko moduari buruz.
author: Yowelle
ms.date: 03/23/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 5b4e768cb78d6a6cb76b3c338fd76363d5290ebd
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8684029"
---
# <a name="transfer-project-budgets-at-fiscal-year-end"></a>Transferitu proiektuaren aurrekontuak urte fiskalaren amaieran

[!include [banner](../includes/banner.md)]

Urte anitzeko proiektu batean lanean ari zarenean, baliteke gainerako aurrekontua urte fiskal amaitzean. Gainerako aurrekontuaren zenbatekoak hurrengo ekitaldira transferi ditzakezu eta lotutako aurrekontuen erregistroaren xehetasunak sor ditzakezu lotutako liburu nagusiko kontuetan. Gainerako zenbatekoak aurrera eraman aurretik, aztertu eta aztertu gainerako aurrekontuaren zenbatekoak.

## <a name="review-and-analyze-remaining-budget-amounts"></a>Gainerako aurrekontu kopuruak berrikusi eta aztertu

Bete urrats hauek proiektuen urte amaierako aurrekontuaren zenbatekoak berrikusteko, baina ez eraman zenbatekoak aurrera.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Aurrekontuak** > **Egin aurrera aurrekontuak**. 
2. **Proiektuaren aurrekontua aurrera eramateko prozesua** orrialdean, **Urte amaierako aukerak** fitxa, egiaztatu hori **Egin aurrera proiektuaren gainerako aurrekontuaren zenbatekoak** ez dago gaituta.
3. **Parametroak** fitxan, **Proiektuaren aurrekontua** eremuan, hautatu urte fiskal zeinaren gainerako aurrekontu kopurua ikusi nahi duzun. 
4. **Urte fiskalaren hasiera** eremuan, hautatu urte fiskal zeinaren gainerako aurrekontu kopurua ikusi nahi duzun. 
5. **Iragarpen eredutik abiatuta** eremuan, hautatu **Gainerako aurrekontua**. 
6. Aukeratutako irizpideak betetzen dituzten eta gainerako aurrekonturik ez duten proiektuak sartzeko, hautatu **Erakutsi zero geratzen dena**.  
7. **Aukeratu aurrekontuak** fitxan, hautatu **Berreskuratu aurrekontu guztiak** hautatutako irizpideekin bat datozen aurrekontu guztiak kargatzeko eta, ondoren, hautatu **Prozesua**. 
8. Aurrekontu multzo jakin bat panelean kargatzen duen datu basearen kontsulta diseinatzeko, hautatu **Berreskuratu hautatutako aurrekontuak**.

Panelean lerro zehatz bati buruzko informazio gehiago lortzeko, hautatu lerroa eta hautatu **Ikusi aurrekontuaren xehetasunak** edo **Ikusi kontuak**.

## <a name="carry-forward-remaining-budget-amounts"></a>Aurreratu gainerako aurrekontu kopuruak 

Gainerako aurrekontuaren zenbatekoak prozesatzen dituzunean, liburu nagusian transakzioak sor ditzakezu aurreratzen ari zaren zenbatekoetarako. Liburu handiko transakzioak sortzeko, osatu ataleko urratsak, [Aurreratu aurrekontuaren zenbatekoak eta liburu handien transakzioak sortu](#carry-forward). 

> [!NOTE]
> Aurreratzen diren aurrekontu kopuruak aukeran aurreikusitako eredura transferitzen dira **Iragarpen ereduak** orria aurreratze iragarpen eredu gisa.  

## <a name="carry-forward-budget-amounts-and-create-general-ledger-transactions"></a><a name="carry-forward"></a>Aurreratu aurrekontuaren zenbatekoak eta liburu handien transakzioak sortu

1.  Hautatu **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Aurrekontuak** > **Egin aurrera aurrekontuak**. 
2. **Proiektuaren aurrekontua aurrera eramateko prozesua** orrialdean, hautatu **Urte amaiera**, eta, ondoren, gaitu **Egin aurrera proiektuaren gainerako aurrekontuaren zenbatekoak** eta **Sortu aurrekontuen erregistroaren sarrerak liburu nagusian**. 
3. **Parametroak** fitxan, **Proiektuaren parametroak** eremuen taldea, hautatu hau:

   - **Proiektuaren urteko aurrekontua**: Hautatu urte fiskalaren hasiera zeinaren gainerako aurrekontu kopurua ikusi nahi duzun. 
   - **Irabaziak eta galerak**: Emaitza eta irabazien transakzioak liburu nagusian sortzea. 
   -  **WIP**: Sortu Work in Progress (WIP) transakzioak liburu nagusian.
   -  **Nominak**: Nominak esleitzeko transakzioak liburu nagusian sortu. 

5. **Liburu nagusi orokorra** eremu taldean, eman honako informazio hau: 

   - **Urte fiskalaren hasiera** eremuan, hautatu urte fiskal zeinaren proiektuen gainerako aurrekontu kopuruak transferitu nahi duzun. Lehenetsitako balioa urteko balioaren ondorengoa da **Proiektuaren aurrekontua** eremua.
   -  **Aurreratzeko epea** eremuan, hautatu aurrekontuen erregistroaren xehetasunak liburu nagusian sortu nahi dituzun aldiak. Normalean hasierako urte fiskal lehen aldia izaten da.

6. **Kopiatu hemendik/hona** eremu taldean, eman honako informazio hau:

   - **Iragarpen eredutik abiatuta** eremuan, hautatu proiektuetarako transferitu nahi dituzun gainerako aurrekontu kopuruekin lotutako proiektuaren aurrekontuaren aurreikuspen eredua. 
   - **Liburu nagusiaren aurrekontuko eredura** eremuan, hautatu liburu nagusirako transferitu nahi dituzun liburu nagusi orokorreko kopuruekin lotutako proiektuaren aurrekontuaren aurreikuspen eredua. 
   -  Aukeratu **Salmenten moneta transferitu** proiektuaren salmenten moneta erabiltzeko proiektuetarako aurrekontuko zenbatekoak transferitzen dituzunean sortzen diren liburu handien transakzioetarako. Aukera hautatzen ez denean, transakzioek kontabilitate moneta erabiltzen dute. 
   -  Aukeratu **Erakutsi zero geratzen dena** gainerako aurrekontu kopururik ez duten baina beheko panelean bistaratutako proiektuetan hautatutako beste irizpideak betetzen dituzten proiektuak sartzeko.

7. **Hautatu aurrekontuak** fitxan, hautatu **Berreskuratu aurrekontu guztiak** hautatutako irizpideekin bat datozen aurrekontu guztiak kargatzeko. Proiektuaren aurrekontu multzo jakin bat panelean kargatzen duen datu basearen kontsulta diseinatzea nahiago baduzu, hautatu **Berreskuratu hautatutako aurrekontuak**.
8. Prozesatu nahi duzun proiektu bakoitzerako, hautatu proiektuaren lerroaren hasieran dagoen aukera.

    > [!TIP]
    > Proiektu guztiak edo gehienak hautatzeko, hautatu marka goiko ezkerreko izkinan. Edozein proiektu izapidetzea baztertzeko, garbitu proiektu horren kontrol-marka.

9. Aukeratutako proiektuen gainerako aurrekontu kopuruak hautatutako urte fiskal-era transferitzeko eta aurrekontuen erregistroaren xehetasunak liburu nagusian sortzeko, hautatu **Prozesua**.

## <a name="carry-forward-budget-amounts-without-creating-general-ledger-transactions"></a>Aurreratu aurrekontuaren zenbatekoak liburu handien transakzioak sortu gabe

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Aurrekontuak** > **Egin aurrera aurrekontuak**.
2. **Proiektuaren aurrekontua aurrera eramateko prozesua** orrialdean, **Urte amaierako aukerak** eremuan, hautatu **Egin aurrera proiektuaren gainerako aurrekontuaren zenbatekoak**.
3. **Parametroak** taldean, **Proiektuaren aurrekontua** eremuan, hautatu urte fiskal zeinaren gainerako aurrekontu kopurua ikusi nahi duzun.
4. **Kopiatu hemendik/hona** taldean, eman honako informazio hau:

   - **Iragarpen eredutik abiatuta** eremuan, hautatu proiektuetarako transferitu nahi dituzun gainerako aurrekontu kopuruekin lotutako proiektuaren aurrekontuaren aurreikuspen eredua. 
   - Hautatu **Erakutsi geratzen den zero** aurrekontu zenbatekorik geratzen ez zaien baina hautatu dituzun irizpideak betetzen dituzten proiektuak gehitzeko.
   - **Hautatu aurrekontuak** taldean, hautatu **Berreskuratu aurrekontu guztiak** hautatutako irizpideekin bat datozen aurrekontu guztiak kargatzeko. Proiektuaren aurrekontu multzo jakin bat panelean kargatzen duen datu basearen kontsulta diseinatzeko, hautatu **Berreskuratu hautatutako aurrekontuak**.

5. Prozesatu nahi duzun proiektu bakoitzerako, hautatu proiektuaren lerroaren hasieran dagoen aukera. 
6. Aukeratu **Prozesua** hautatutako proiektuen gainerako aurrekontu kopuruak hautatutako urte fiskalera transferitzeko.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
