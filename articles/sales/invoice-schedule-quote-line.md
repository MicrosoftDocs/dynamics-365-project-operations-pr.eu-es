---
title: Fakturazio-antolaketak proiektuetan oinarritutako eskaintza-lerroetan
description: Gai honek fakturen ordutegiak eta aurrekontu lerroen mugarriak sortzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 506de5217de48814d6b8f03a10c7c8648c575198
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278268"
---
# <a name="invoice-schedules-on-project-based-quote-lines"></a>Fakturazio-antolaketak proiektuetan oinarritutako eskaintza-lerroetan

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuan oinarritutako aurrekontu lerroak faktura egutegia adierazteko gaitasuna ematen du. Aukerakoa da aurrekontuaren fasean, aplikazioak ez baitu onartzen proiektu bat fakturatzea Aurrekontu lerro batera lotuta dagoenean. Fakturazioa aurrekontua irabazi ondoren soilik onartzen da. Aurrekontuaren fasean faktura-egutegia sortzeak dakarren beherako eragin bakarra faktura-egutegi hori proiektuan oinarritutako kontratu-lerroan kopiatzea da. Aurrekontu fasean faktura ordutegirik sortzen ez baduzu, proiektuan oinarritutako kontratu lerroan egin ahal izango duzu.

Orokorrean, fakturen egutegien xedea proiektuetan oinarritutako kontratu lerro baterako fakturen zirriborroak automatikoki sortzea ahalbidetzea da. 

## <a name="create-a-time-and-material-invoice-schedule-for-a-project-based-quote-line"></a>Sortu denbora eta materialen fakturen egutegia proiektuan oinarritutako aurrekontu lerro baterako

Proiektuetan oinarritutako aurrekontu lerro baten fakturazio metodoa Denbora eta materiala denean, sistemak datan oinarritutako faktura ordutegia sortzen du. Datan oinarritutako fakturen egitaraua automatikoki sortzeko, jarraitu urrats hauek.

1. Joan **Ezarpenak** > **fakturazio maiztasunak** eta ezarri faktura maiztasuna.
2. **Eskaintzak** orrian, ireki proiektuaren aurrekontua eta **Laburpena** fitxa, zehaztu eskatutako entrega data.
3. Ireki dataren araberako fakturen ordutegia sortzeko behar duzun denbora eta materialaren aurrekontua. 
4. **Faktura-antolaketa** fitxan, hautatu balioak **Fakturazioaren hasiera** eta **Fakturen maiztasuna** eremuak. 
5. Azpisaretan, hautatu **Sortu faktura-antolaketa**.
6. Aplikazioak fakturaren egutegia sortzen du **Faktura exekutatzeko data**, **Transakzioen ebazpen-data** eta **Exekutatu egoera** eremuak honela ezarrita:

    - **Faktura exekutatzeko data** fakturazio maiztasunaren arabera diktatutako datan ezartzen da.
    - **Transakzioaren amaiera eguna** egunaren aurreko egunean ezartzen da **Faktura exekutatzeko data**.
    - **Exekutatu egoera** automatikoki ezartzen da **Exekutatu gabe**. Faktura automatikoki sortzeko lana faktura exekutatzeko data jakin batean exekutatzen denean, eremu hau bietara eguneratuko du **Exekutatu arrakastaz** edo **Exekutatu huts egin du**.

## <a name="create-a-fixed-price-invoice-schedule-for-a-project-based-quote-line"></a>Sortu Prezio finkoen fakturen egutegia proiektuan oinarritutako aurrekontu lerro baterako

Proiektuan oinarritutako aurrekontu lerroak a duenean **Finkoa** fakturazio-metodoaren arabera, sistemak mugarrietan oinarritutako fakturen egutegia sortzen du. Osatu urrats hauek egutegi aldirako berdin banatzen diren mugarri multzo finko baterako programazio hau automatikoki sortzeko.

1. Joan **Ezarpenak** > **fakturazio maiztasunak** eta ezarri faktura maiztasuna.
2. **Eskaintzak** orrian, ireki proiektuaren aurrekontua eta **Laburpena** fitxa, zehaztu eskatutako entrega data.
3. Ireki mugarrien egitaraua sortzeko behar duzun prezio finkoaren aurrekontua. 
4. **Faktura-antolaketa** fitxan, hautatu balioak **Fakturazioaren hasiera** eta **Fakturen maiztasuna** eremuak. 
5. Azpisaretan, hautatu **Sortu tartekako mugarriak**.
6. Aplikazioak fakturaren egutegia sortzen du mugarri baten izenarekin, datarekin eta zenbatekoarekin.

    - Mugarriaren izena data fakturazio maiztasunaren arabera diktatutako datan ezartzen da.
    - Mugarriaren data fakturazio maiztasunaren arabera diktatutako datan ezartzen da.
    - Mugarrien zenbatekoa proiektuan oinarritutako aurrekontu-lerroan aurrekontuaren zenbatekoa maiztasunaren eta fakturazioaren hasierako eta eskatutako entrega datek agindutako mugarri kopuruaren arabera zatituz kalkulatzen da.
    - Aurrekontuaren lerroak zerga zenbateko estimatua badu ere, balio hori mugarri bakoitzaren artean banatzen da aldian behin mugarriak sortzerakoan.

### <a name="manually-create-milestones"></a>Sortu eskuz mugarriak

Prezio finkoaren mugarriak eskuz ere sor daitezke, aldian-aldian banatzen ez direnean. Mugarriak eskuz sortzeko:

Ireki mugarriak sortzeko behar duzun prezio finkoaren aurrekontua. **Fakturen ordutegia** fitxan, azpisarean, hautatu **+ Sortu aurrekontu lerroaren mugarri berria** eta sartu beharrezko informazioa hurrengo taulan oinarrituta.

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Mugarriaren izena | Sorrera bizkorra | Mugarriaren izena. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da |
| Proiektuaren zeregina | Sorrera bizkorra | Mugarria proiektuaren zereginarekin lotuta badago, erreferentzia hau erabil dezakezu logika pertsonalizatua gehitzeko mugarriaren egoera atazaren egoeran oinarrituta. | Aplikazioak ez du zeregin baterako erreferentzia honen beherako eraginik. |
| Mugarriaren data | Sorrera bizkorra | Ezarri faktura automatikoki sortzeko prozesuak mugarri horren egoera bilatzeko data fakturatzeko kontuan hartzeko. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |
| Fakturaren egoera | Sorrera bizkorra | Mugarri bat sortzen denean, egoera hau beti ezartzen da **Ez dago fakturatzeko prest**. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |
| Lerroaren zenbatekoa | Sorrera bizkorra | Bezeroari fakturatuko zaion mugarriaren zenbatekoa edo balioa. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |
| Zergak | Sorrera bizkorra | Mugarrian aplikatuko den zerga kopurua. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |


[!INCLUDE[footer-include](../includes/footer-banner.md)]