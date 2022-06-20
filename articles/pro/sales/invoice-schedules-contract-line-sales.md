---
title: Sortu faktura-antolaketak proiektuetan oinarritutako kontratuaren lerro batean - arina
description: Artikulu honek fakturen egutegiak eta mugarriak sortzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 403b993c3f61ca5f0fb1bac45331aa0613d16439
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921103"
---
# <a name="create-invoice-schedules-on-a-project-based-contract-line---lite"></a>Sortu faktura-antolaketak proiektuetan oinarritutako kontratuaren lerro batean - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Faktura-antolaketa proiektuetan oinarritutako kontratuaren lerro batean atxiki dezakezu. Fakturazioa kontratua irabazi ondoren Proiektuaren kontratua sortzeko soilik onartzen da. Fakturen ordutegiek proiektuetan oinarritutako kontratu lerro baten fakturak zirriborroa automatikoki sortzea ahalbidetzen dute. Beti fakturak eskuz sortzeko asmoa baduzu, proiektuan oinarritutako kontratu lerroan edo kontratu lerro batean faktura ordutegiak sortzeari utz diezaiokezu.

## <a name="create-a-time-and-material-invoice-schedule-for-a-project-based-contract-line"></a>Sortu denboraren eta materialaren faktura-antolaketa proiektuetan oinarritutako kontratuaren lerro batean

Proiektuetan oinarritutako kontratuaren lerro batek denboraren eta materialaren fakturazio-metodoa duenean, datan oinarritutako faktura-antolaketa sor dezakezu. Datan oinarritutako fakturen egitaraua automatikoki sortzeko, jarraitu urrats hauek.

1. Joan **Ezarpenak** > **Fakturen maiztasunak** faktura maiztasuna konfiguratzeko.
2. Ireki proiektuaren kontratua eta **Laburpena** fitxa, zehaztu eskatutako entrega data.
3. Ireki dataren araberako fakturen egutegia sortu nahi duzun kontratuaren denbora eta materiala. 
4. **Fakturen ordutegia** fitxa, hautatu fakturazioaren hasiera data eta fakturazio maiztasuna. 
5. Azpisaretan, hautatu **Sortu faktura-antolaketa**.

    Sistemak fakturaren egutegia sortzen du eremuko informazio honekin:

    - **Faktura exekutatzeko data** fakturazio maiztasunaren arabera ezartzen da.
    - **Transakzioaren amaiera eguna** egunaren aurreko egunean ezartzen da **Faktura exekutatzeko data**.
    - **Exekutatu egoera** automatikoki ezartzen da **Exekutatu gabe**. Faktura automatikoki sortzeko lana **Faktura exekutatzeko data** jakin batean exekutatzen denean, eremu hau eguneratuko du **Exekutatu arrakastaz** edo **Exekutatu huts egin du**.

## <a name="create-a-fixed-price-invoice-schedule-for-a-project-based-contract-line"></a>Sortu prezio finkoko faktura-antolaketa proiektuetan oinarritutako kontratuaren lerro batean

Proiektuetan oinarritutako kontratu lerroak prezio finkoko fakturazio metodoa duenean, mugarrietan oinarritutako faktura egutegia sor dezakezu. Osatu urrats hauek egutegiko aldirako berdin banatzen diren mugarri multzo finko baterako mugarrietan oinarritutako faktura ordutegia automatikoki sortzeko.

1. Joan **Ezarpenak** > **Fakturen maiztasunak** faktura maiztasuna konfiguratzeko.
2. Ireki proiektuaren kontratua eta **Laburpena** fitxa, zehaztu eskatutako entrega data.
3. Ireki mugarriko ordutegia sortu behar duzun prezio finkoko kontratu linea. 
4. **Fakturen ordutegia (fakturazio mugarriak)** fitxa, hautatu fakturazioaren hasiera data eta fakturazio maiztasuna. 
5. Azpisaretan, hautatu **Sortu tartekako mugarriak**.

    Sistemak fakturaren egutegia sortzen du mugirriko informazio honekin:

    - **Mugarriaren izena** fakturazio maiztasunaren arabera diktatutako datan ezartzen da.
    - **Mugarriaren data** fakturazio maiztasunaren arabera diktatutako datan ezartzen da.
    - **Mugarri kopurua** proiektuaren araberako kontratuaren lerroan kontratuaren zenbatekoa maiztasunak, fakturazio-hasierak eta eskatutako entrega-datak agindutako mugarri kopuruaren arabera zatituz kalkulatzen da.
    - Kontratu lerroak balioa badu **Aurreikusitako Zerga Zenbatekoa** eremua, eremu hori mugarri bakoitzera berdin banatzen da aldizkako mugarriak sortzerakoan.

Fakturazio mugarriek proiektuan oinarritutako kontratu lerroaren kontratuaren balioa berdina izan behar dute. Berdinak ez badira, errore bat gertatzen da. Akats hori konpondu dezakezu fakturazio mugarriek lerroaren kontratuaren balioa osatzen dutela egiaztatuz mugarriak sortuz, editatuz edo ezabatuz. Aldaketak egin ondoren, freskatu orria.

### <a name="manually-create-milestones"></a>Sortu eskuz mugarriak

Prezio finkoaren mugarriak eskuz sor daitezke, aldian-aldian banatzen ez direnean. Mugarri bat eskuz sortzeko, jarraitu urrats hauek.

1. Ireki mugarria sortu behar duzun prezio finkoko kontratu linea. 
2. **Fakturen ordutegia** fitxan, azpisarean, hautatu **+ Sortu Kontratu linea mugarri berria**.
3. **Mugarrien sorrera** inprimakia, sartu beharrezko informazioa ondoko taulan oinarrituta. 

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| Mugarriaren izena | Sorrera bizkorra | Mugarriaren izenaren testu eremua. | Eremu hau proiektuaren kontratu lerroaren mugarrian eta fakturan sartzen da. |
| Proiektuaren zeregina | Sorrera bizkorra | Mugarria proiektuaren zeregin bati lotuta badago, erabili erreferentzia hau logika pertsonalizatua gehitzeko eta mugarriaren egoera ezartzeko atazaren egoeran oinarrituta. | Ez dago zeregin bati buruzko erreferentzia horren beherako eraginik. |
| Mugarriaren data | Sorrera bizkorra | Faktura automatikoki sortzeko prozesuak fakturatzeko kontuan hartzeko mugarri horren egoera bilatu behar duen eguna. | Hau proiektuaren kontratu lerroaren mugarrian eta fakturan sartzen da. |
| Fakturaren egoera | Sorrera bizkorra | Mugarria sortzen denean, egoera hau beti ezartzen da **Ez dago fakturatzeko prest** edo **Ez da hasi**. | Hau proiektuaren kontratu lerroaren mugarrian eta fakturan sartzen da. |
| Lerroaren zenbatekoa | Sorrera bizkorra | Bezeroari fakturatuko zaion mugarriaren zenbatekoa edo balioa. | Eremu hau proiektuaren kontratu lerroaren mugarrian eta fakturan sartzen da. |
| Zergak | Sorrera bizkorra | Mugarrian aplikatutako zergaren zenbatekoa. | Hau proiektuaren kontratu lerroaren mugarrian eta fakturan sartzen da. |

4. Hautatu **Gorde eta itxi**.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]