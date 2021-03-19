---
title: Sortu faktura-antolaketa proiektuetan oinarritutako kontratuaren lerro batean
description: Gai honek fakturen ordutegiak eta kontratuaren lerroen mugarriak sortzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/17/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b0da3b3f8f14ecf9a4c4f057cd26c0ca9eb5ec2f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278223"
---
# <a name="create-an-invoice-schedule-on-a-project-based-contract-line"></a>Sortu faktura-antolaketa proiektuetan oinarritutako kontratuaren lerro batean 

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Faktura-antolaketa proiektuetan oinarritutako kontratuaren lerro batean sor dezakezu. Fakturazioa kontratua irabazi eta proiektuaren kontratua sortzen ari zarenean bakarrik onartzen da. Fakturen egutegi batek proiektuan oinarritutako kontratu lerro baten fakturak zirriborroa automatikoki sortzea ahalbidetzen du. Hala ere, fakturak eskuz soilik sortzen badituzu, kontratu-lerroetan fakturen ordutegiak sortzeari utz diezaiokezu.

## <a name="create-a-time-and-material-invoice-schedule-for-a-contract-line"></a>Sortu denbora eta materialen fakturen egutegia kontratuaren lerro baterako

Proiektuetan oinarritutako kontratuaren lerro batek denboraren eta materialaren fakturazio-metodoa duenean, datan oinarritutako faktura-antolaketa sor dezakezu. Datan oinarritutako fakturen egitaraua automatikoki sortzeko, jarraitu urrats hauek.

1. Joan **Ezarpenak** > **Fakturazio maiztasunak** eta ezarri faktura maiztasuna.
2. Joan proiektuaren kontratuaren erregistroa eta **Laburpena** fitxan, **Eskatutako entrega-data** eremuan, hautatu data.
3. Ireki Dataren araberako fakturen ordutegia sortzeko behar duzun **Denbora eta materiala** kontratuaren lerroa. 
4. **Faktura-antolaketa** fitxan, hautatu fakturazioaren hasiera-data eta fakturen maiztasuna.
5. Azpisaretan, hautatu **Sortu faktura-antolaketa**. Fakturaren egutegia sortzen da **Faktura exekutatzeko data**, **Transakzioen ebazpen-data** eta **Exekutatu egoera** eremuak honela ezarrita:

    - **Faktura exekutatzeko data**: fakturazio maiztasunaren arabera diktatutako datan ezartzen da.
    - **Transakzioaren amaiera-eguna**: faktura exekutatu baino egun bat lehenago.
    - **Exekutatu egoera**: automatikoki ezartzen da **Exekutatu gabe**. Faktura automatikoki sortzeko lana faktura exekutatzeko data jakin batean exekutatzen denean, eremu hau eguneratuko du **Exekutatu arrakastaz** edo **Exekutatu huts egin du**.

## <a name="create-a-fixed-price-invoice-schedule-for-a-contract-line"></a>Sortu prezio finkoen fakturen egutegia kontratuaren lerro baterako

Kontratuaren lerroak fakturazio-metodo finkoa duenean, mugarrietan oinarritutako fakturen egutegia sortzen du. 

> [!NOTE]
> Mugarriak ezin dira kontratu-lerro batean sortu, baldin eta kontratu-lerroarekin mapatutako proiekturik ez badago.

Osatu urrats hauek egutegi aldirako berdin banatzen diren mugarrietan oinarritutako fakturazio-programazio hau automatikoki sortzeko.

1. Joan **Ezarpenak** > **Fakturazio maiztasunak** eta ezarri faktura maiztasuna.
2. Joan proiektuaren kontratuaren erregistroa eta **Laburpena** fitxan, **Eskatutako entrega-data** eremuan, hautatu data.
3. Ireki **Prezio finkoa** kontratuaren lerroa, mugarrien egitaraua sortzeko erabiltzen ari zarena. **Fakturazio-mugarriak** fitxan, hautatu fakturazioaren hasiera-data eta fakturen maiztasuna. 
4. Azpisaretan, hautatu **Sortu tartekako mugarriak**. Fakturen egutegia fitxategiarekin sortzen da **Mugarriaren izena**, **Mugarri Data** eta **Mugarri kopurua** eremuak honela ezartzen dira:

    - **Mugarriaren izena**: Izen hori fakturaren maiztasunak agintzen du.
    - **Mugarriaren data**: fakturazio maiztasunaren arabera diktatutako datan ezartzen da.
    - **Mugarriaren zenbatekoa**: zenbatekoa kalkulatzeko kontratuaren lerroan kontratuaren zenbatekoa maiztasunaren eta fakturazioaren hasierako eta eskatutako entrega datek agindutako mugarri kopuruaren arabera zatituz kalkulatzen da.

    Kontratu lerroak balioa badu **Zergaren zenbateko estimatua** eremua, orduan eremu hori mugarri bakoitzera berdin banatzen da aldizkako mugarriak sortzerakoan.

Fakturazio mugarriek kontratuaren linearen kontratuaren balioa berdina izan behar dute. Hala egiten ez badute, errore bat jasoko duzu **Kontratu-lerroa** orrialdea. Akatsa konpondu dezakezu fakturazio mugarriek lerroaren kontratuaren balioa osatzen dutela egiaztatuz mugarriak sortuz, editatuz edo ezabatuz. Aldaketak egin ondoren, freskatu orria errorea ezabatzeko.

### <a name="manually-create-milestones"></a>Sortu eskuz mugarriak

Prezio finkoaren mugarriak eskuz sor ditzakezu, aldian-aldian banatzen ez direnean. Osatu urrats hauek mugarriak eskuz sortzeko.

1. Ireki mugarri bat sortzen ari zaren prezio finkoko kontratu linea eta **Fakturen Ordutegia** fitxa, azpisarean, hautatu **+ Sortu Contract line mugarri berria**. 
2. **Mugarrien sorrera** orrian, sartu beharrezko informazioa ondoko taulan oinarrituta.

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| Mugarriaren izena | Sorrera bizkorra | Mugarriaren izenaren testu eremua. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |
| Proiektuaren zeregina | Sorrera bizkorra | Mugarria proiektuaren zereginarekin lotuta badago, erreferentzia hau erabil dezakezu logika pertsonalizatua gehitzeko mugarriaren egoera atazaren egoeran oinarrituta. | Aplikazioak ez du zeregin baterako erreferentzia honen beherako eraginik. |
| Mugarriaren data | Sorrera bizkorra | Ezarri faktura automatikoki sortzeko prozesuak mugarri horren egoera bilatzeko data fakturatzeko kontuan hartzeko. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |
| Fakturaren egoera | Sorrera bizkorra | Mugarri bat sortzen denean, egoera hau beti ezartzen da **Ez dago fakturatzeko prest** edo **Hasi gabe**. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |
| Lerroaren zenbatekoa | Sorrera bizkorra | Bezeroari fakturatuko zaion mugarriaren zenbatekoa edo balioa. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |
| Zergak | Sorrera bizkorra | Mugarrian aplikatutako zergaren zenbatekoa. | Hori proiektuaren kontratu-lerroaren mugarrira eta fakturara hedatzen da. |

3. Hautatu **Gorde eta itxi**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]