---
title: Azpikontratuaren lerroko mugarriak
description: Gai honetan azaltzen da saltzaile batekin azpikontrata egiteko mugarrietan oinarritutako faktura ordutegia nola sortu eta mantendu.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: d1c30f48e0d43aa55e2c1650637f7f102fb200de
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8579107"
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

    | Eremua | Deskribapenak |Inpaktu funtzionala|
    | --- | --- |----------------------|
    | Mugarriaren izena | Mugarriaren izena. |Azpikontratazio lerroen mugarrietan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da. Mugarri horretan oinarrituta sortzen den saltzailearen faktura lerroak azpikontratazio lerro mugarriaren izena ere erabiliko du saltzailearen faktura lerroaren izen lehenetsi gisa.|
    | Deskribapenak | Mugarriaren azalpena. |Mugarri horretan oinarrituta sortzen den saltzailearen faktura lerroak azpikontratazio lerro mugarriaren deskribapena ere erabiliko du saltzailearen faktura lerroaren deskribapen lehenetsi gisa.|
    | Mugarriaren data | Faktura automatikoki sortzeko prozesuak fakturatzeko kontuan hartzeko mugarri horren egoera bilatu behar duen eguna.| Balio hori saltzailearen faktura lerroaren lehenetsitako data gisa erabiliko da azpikontratazio lerro hau fakturatzerakoan. |
    | Kopurua | Bezeroari fakturatuko zaion mugarriaren zenbatekoa edo balioa. |Balio hori saltzailearen faktura lerroaren lehenetsitako zenbateko gisa erabiliko da azpikontratazio lerro hau fakturatzerakoan. |
    | Zergak | Mugarrian aplikatutako zergaren zenbatekoa.| Balio hori saltzailearen faktura lerroaren lehenetsitako zerga-zenbateko gisa erabiliko da azpikontratazio lerro hau fakturatzerakoan. |
    | Zenbatekoa zergaren ondoren | Irakurtzeko soilik den eremu hau Zenbatekoa + Zerga gisa kalkulatzen da.|Balio hori saltzailearen faktura lerroaren lehenetsitako gisa erabiliko da azpikontratazio lerro hau fakturatzerakoan. |
    | Fakturaren egoera | Mugarria sortzen denean, egoera hau beti ezartzen da **Ez dago fakturatzeko prest**.|  Egoera dagoenean **Fakturatzeko prest**, saltzailearen faktura sortzeak mugarri hori biltzen du saltzailearen fakturan. |

5. Hautatu **Gorde eta itxi**.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
