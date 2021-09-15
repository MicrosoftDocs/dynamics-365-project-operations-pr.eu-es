---
title: Azpikontratuaren lerroko mugarriak
description: Gai honetan azaltzen da saltzaile batekin azpikontrata egiteko mugarrietan oinarritutako faktura ordutegia nola sortu eta mantendu.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3301e5a627e4842009fcd5e352f1b76fd3053ee3
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323761"
---
# <a name="subcontract-line-milestones"></a>Azpikontratuaren lerroko mugarriak

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Urtean Dynamics 365 Project Operations, prezio finkoko fakturazio metodoarekin azpikontrata lerro batek mugarrian oinarritutako faktura programa zehaztu dezake saltzailearekin.

Saltzailearen fakturaziorako mugarriak automatikoki sor daitezke maiztasun jakin bat erabiliz edo eskuz sor ditzakezu.

## <a name="automatically-create-a-milestone-based-invoice-schedule-for-a-subcontract-line"></a>Sortu automatikoki mugarrian oinarritutako faktura ordutegia azpikontrata lerro baterako

Osatu urrats hauek berdin banatutako mugarri multzo finko baterako mugarrietan oinarritutako faktura ordutegia automatikoki sortzeko.

1. Joan **Ezarpenak** > **Fakturen maiztasunak** eta konfiguratu azpikontratazio lerroen faktura maiztasuna.
2. Ireki **Azpikontratak** orrialdea, ireki lan egin nahi duzun azpikontratua eta, ondoren, ireki mugarriko egitaraua sortuko duzun prezio finkoaren azpikontrata lerroa.
3. Gainean **Azpikontratatzeko Linearen Mugarriak** fitxa, hautatu **Mugarri periodikoak sortu**.
4. Elkarrizketa koadroan, sartu edo hautatu data tartea, mugarri kopurua eta fakturaren maiztasuna. Hasiera data bat hauta dezakezu edo mugarri kopurua eta fakturaren maiztasuna edo hasiera data hauta dezakezu edo amaiera data eta fakturazio maiztasuna hauta ditzakezu. Ezin dituzu amaiera data eta mugarri kopurua hautatu.
Informazio hori erabiliz, sistemak fitxategian agertzen diren mugarriak eta erregistroak sortzen ditu **Mugarriak** sareta.

   - **Mugarriaren izena** - Mugarriaren izena fakturazioaren maiztasunaren arabera mugarriaren datan ezartzen da.
   - **Mugarri Data** - Fakturen maiztasunean oinarritutako data.
   - **Mugarri kopurua** - Azpikontratazio lerroaren zenbateko azpitotala mugarri kopuruaz zatituz kalkulatzen da.

Azpikontratazio lerroak balioa badu **Aurreikusitako Zerga Zenbatekoa** eremuan, balio hori mugarri bakoitzari berdin gehitzen zaio aldizkako mugarriak sortzerakoan.

Azpikontratuaren lerroaren mugarriak pilatzen ditu azpikontratuaren lerroaren baliora berdina izan beharko luke. Berdinak ez badira, errore bat gertatzen da. Akatsa konpondu eta mugarri osoa azpikontrataren lerro balioaren berdina dela egiaztatu dezakezu mugarri eta zerga zenbatekoak sortuz, editatuz edo ezabatuz. Aldaketak egin ondoren, gorde eta freskatu orria akats gehiago ez daudela ziurtatzeko.

## <a name="manually-create-subcontract-line-milestones"></a>Eskuz sortu azpikontratuaren lerroaren mugarriak

Azpikontratazio lerro bateko prezio finkoaren mugarriak eskuz sor daitezke, aldian-aldian banatzen ez direnean. Azpikontratazioaren lerro mugarria eskuz sortzeko, jarraitu urrats hauek.

1. Nabigazio panelean, hautatu **Azpikontratak**, eta ireki lan egin nahi duzun azpikontratua.
2. Ireki mugarri bat sortu nahi duzun prezio finkoaren azpikontrata lerroa.
3. Gainean **Azpikontratazio lerro mugarriak** fitxa, azpi-saretan, hautatu **+ Azpikontrata lerro mugarri berria**.
4. Gainean **Azpikontrata Line Mugarri berria** orrian, sartu beharrezko informazioa ondoko taulan oinarrituta.

    | Eremua | Deskribapenak |
    | --- | --- |
    | Mugarriaren izena | Mugarriaren izena. |
    | Deskribapenak | Mugarriaren azalpena.  |
    | Mugarriaren data | Faktura automatikoki sortzeko prozesuak fakturatzeko kontuan hartzeko mugarri horren egoera bilatu behar duen eguna. Balio hori saltzailearen faktura lerroan sartzen da azpikontratu hori fakturatzerakoan. |
    | Kopurua | Bezeroari fakturatuko zaion mugarriaren zenbatekoa edo balioa. Balio hori saltzailearen faktura lerroan sartzen da azpikontratu hori fakturatzerakoan. |
    | Zergak | Mugarrian aplikatutako zergaren zenbatekoa. Balio hori saltzailearen faktura lerroan sartzen da azpikontratu hori fakturatzerakoan. |
    | Zenbatekoa zergaren ondoren | Zenbatekoa + Zerga gisa kalkulatzen den irakurtzeko soilik den eremu hau. Balio hori saltzailearen faktura lerroan sartzen da azpikontratu hori fakturatzerakoan. |
    | Fakturaren egoera | Mugarria sortzen denean, egoera hau beti ezartzen da **Ez dago fakturatzeko prest**.  Egoera dagoenean **Fakturatzeko prest**, saltzailearen faktura sortzeak mugarri hori biltzen du saltzailearen fakturan. |

5. Hautatu **Gorde eta itxi**.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
