---
title: Azpikontratuaren lerroak produktuen arabera
description: Gai honetan produktuen azpikontratazio lerroak nola grabatu eta saltzaileek produktuen erosketak erregistratzeko eremu desberdinak nola erabili azaltzen da.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c0ddc39638ae9830eacc57f3e1def75aa36e6553
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323671"
---
# <a name="subcontract-lines-for-products"></a>Azpikontratuaren lerroak produktuen arabera

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Urtean azpikontrata Dynamics 365 Project Operations produktuentzako azpikontratazio lerro bat izan dezake. Lerro hauei esker, proiektuaren kudeatzaile batek produktuen erosketa egin dezake saltzaileei, proiektuko zereginetan erabili ahal izateko.

Bete urrats hauek Project Operations produktuentzako azpikontratazio lerro bat sortzeko.

1. Nabigazio orrian, hautatu **Azpikontratak**, eta ireki lan egin nahi duzun azpikontratua. 
2. Gainean **Azpikontratatzeko Lineak** fitxa, hautatu **+ Berria** azpikontratazio lerro berri bat sortzeko.
3. Gainean **Sortu bizkor** orrialdean, **Transakzio Klase** eremua, hautatu **Materiala** eta sartu edo hautatu beharrezko eremuko informazioa. 
4. Sakatu **Gorde**.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Azpikontratazioaren lerroaren xehetasunak** orrialdea eta **Sortu azkar** orrialdea produktuak erosteko garrantzitsuak direnez.

| Eremua | Deskribapenak |
| ----- | ----------- |
| Izena | Azpikontratuaren lerroaren izena. |
| Deskribapenak | Azpikontratuaren lerroan aginduta dauden produktuen deskribapen laburra. |
| Lerro mota | Eremu honen balioa lehenetsia da **Kopuruan oinarrituta**. |
| Fakturazio-metodoa |  Azpikontratazio lerroaren fakturazio metodoa. Mugarrian oinarritutako fakturen egutegia eskuragarri dago prezio finkoko fakturazio metodoetarako. |
| Transakzio-klasea | Eremu honen balioa lehenetsia da **Denbora**. Produktuak erosteko azpikontrata lerroak sortzeko **Transakzio Klase** eremua hautatu **Materiala**. Aukeraketa honek adierazten du azpikontratazio lerroa proiektuetan erabilitako produktuen erosketa erregistratzeko erabiltzen dela. |
| Hautatu produktua | Aukeratu erosten ari zaren produktua produktuen katalogoan mantentzen den edo idatzi beharreko produktua den. |
| Produktu | Hautatu produktu aktibo bat katalogoan. Eremu hau eskuragarri dago soilik **Aukeratu produktua** ezarrita dago **Lehendik dagoena**. |
| Katalogotik kanpoko produktua | Idatzi izena katalogoz kanpoko produktua. Eremu hau eskuragarri dago soilik **Aukeratu produktua** ezarrita dago **Katalogoz kanpokoa**.  |
| Eskatutako entrega-data | Aukeratu produktuen beharrezko entrega-data. Data hau azpikontratari atxikitako proiektuen prezioen zerrendetatik proiektuaren prezioen zerrenda hautatzeko ere erabiltzen da. Azpikontratazio linean produktuaren kostua prezio zerrenda horretatik lehenetsita dago. |
| Kontratatutako entrega-data | Aukeratu produktuak kontratu bidez entregatzeko adostutako data.  |
| Eskatutako kopurua | Idatzi saltzaileari erosten zaion produktuaren kopurua. Kopuru horretatik Proiektu kudeatzaile batek gainetik ateratzen badu, abisua agertuko da. |
| Salmenta-unitatea | Balio hau lehenetsita dago katalogoko produktuetan soilik. Noiz **Produktua** eta **Eskatutako entrega eguna** biak daude hautatuta, sistemak entregatzeko dataren arabera aukeratutako prezioen zerrenda hautatzen du. Lotutako prezioen zerrendako elementuak bat datorren produktuari buruz galdetzen dira. Unitate eta unitate taldearen balioak prezioen zerrendako erregistroaren konfigurazioan lehenetsita daude. |
| Unitatea | Balio hau lehenetsita dago prezioen zerrendako erregistroan dagoen unitateko konfiguraziora. Beharrezkoa izanez gero, beste unitate batera alda dezakezu. Produktuaren eta unitatearen konbinazioa lehendik dauden katalogoko produktuen azpikontrata lerroaren unitateko prezioa lehenesteko erabiltzen da. |
| Unitate-prezioa | Prezio unitarioa lehenetsita dago azpikontratazio lerroaren eskatutako entrega datarako aplikagarria den proiektuaren prezio zerrendarekin lotutako produktuen eta unitatearen konbinazioa erabiliz.  |
| Guztizko partziala | Irakurtzeko soilik den eremu hau Kantitatea x Prezio unitario gisa kalkulatzen da bi eremuek balioak sartu badituzte. Bai **Kopurua** zelaia, **Prezio unitarioa** eremua edo biak hutsik daude, eskuz sar dezakezu balio bat.  |
| Salmenten zerga | Idatzi salmenta-zergaren balioa. |
| Zenbatekoa guztira | Kalkulatutako eremu honek zergak sartu ondoren azpikontrataren zenbateko lerro osoa erakusten du. Eremu honetako balioa guztizko azpi + zerga gisa kalkulatzen da. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
