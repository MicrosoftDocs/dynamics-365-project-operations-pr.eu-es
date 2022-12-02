---
title: Ad hoc aurrerakin bat kontratu batean sortzea
description: Gai honetan beharrezkoa da kontratuaren aurrerakina sortzeari buruzko informazioa.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 3e450a17990c6fc783ddffdb05e1ab5b9429a3c1
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922161"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract"></a>Ad hoc aurrerakin bat kontratu batean sortzea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Microsoft Dynamics 365 Project Operations-ek aurrez ordainketak eta aurrerakinak dakartzan fakturazio-egoerak onartzen ditu. Erabilera prozesua **Aurrerapenak** **Project Operations** antzekoa da **Atxikitzailea** kontratuak. 

Osatu urrats hauek bezeroari aurrerapena fakturatzeko.

1. Joan **Proiektuaren kontratua** eta, ondoren, hautatu **Aurrerakinak eta gordailuak** fitxa.
2. Aurretik erregistratutako aurrerakin eta aurrerakin guztiak zerrendatzen dituen azpisarean, hautatu **+ Proiektu berriaren kontratuaren atxikipena**. 

    **Sorrera bizkorra** inprimakia aurrez ordaintzeko edo aurreratzeko erregistratzeko irekitzen da.
    
3. Beheko taulan aurrerapen bat grabatzeko eremuak eta berriak sortu ahala kontuan hartu beharreko gogoetak agertzen dira:

    | Eremua | Deskribapena | Downstream eragina |
    | --- | --- | --- |
    | **Proiektuaren kontratuaren bezeroa** | Eremu honen adierazten du aurrerakin hori fakturatuko zaion kontratuko bezeroak. | Kontratuan hainbat bezero badituzu eta horietako bakoitzari atxikipen zehatz bat edo aurrerakinaren zenbatekoa fakturatu behar badiozu, sortu faktura bat bezero bakoitzarentzat. |
    | **Azalpena** | Aurrerakinaren xedearen edo denboraren deskribapena aurrerapen hori identifikatzen laguntzeko. | Deskribapen hau aurrerapen horren faktura-lerroan agertzen da. |
    | **Zenbatekoa** | Aurreordainketaren edo aurrerakinaren zenbatekoa. | Zenbateko hau aurrerapen horren faktura-lerroan agertzen da. |
    | **Fakturaren data** | Bezeroari aurrerakin hori fakturatzen zaion eguna. | Hau da faktura automatikoki sortzeko prozesuaren data aurrerapen horretarako faktura lerro bat sortzeko. |
    | **Fakturaren egoera** | Aukera ezarpen bat da, aurrerapen hori bezero honen faktura zirriborroan gehitzen den ala ez adierazten duena. Hauek dira balio posibleak:</br>- **Ez dago prest fakturatzeko**</br>- **Fakturatzeko prest** | Aurrerakina edo aurretiazko ordainketa gisa markatzen denean **Fakturatzeko prest**, fakturaren zirriborroan lerro denbora gisa gehitzen da. Erabat fakturatutako aurrerakina soilik erabil daiteke hurrengo fakturazio aldiko proiektuaren kostuekin bateratzeko. |

4. Aukeratu **Gorde eta itxi** sortu azkar elkarrizketa-koadroan aurrerakina edo aurretiazko ordainketa erregistratzeko.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]