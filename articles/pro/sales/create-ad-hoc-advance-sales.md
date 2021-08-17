---
title: Ad hoc aurrerakin bat kontratu batean sortzea
description: Gai honetan beharrezkoa da kontratuaren aurrerakina sortzeari buruzko informazioa.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: bceed1372dbaf523426a4c34da7152d77fe108240c8c3e4e1390c43b1cf536a4
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6999121"
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