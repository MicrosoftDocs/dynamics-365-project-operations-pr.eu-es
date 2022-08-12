---
title: Azpikontratuaren lerroak produktuen arabera
description: Artikulu honek produktuen azpikontratazio-lerroak nola erregistratu eta saltzaileen produktuen erosketak erregistratzeko hainbat eremu erabili azaltzen du.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: ff9636f86102fa671a443d7646614070b3e2ee79
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8934351"
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

| Eremua | Deskribapenak | Inpaktu funtzionala|
| ----- | ----------- | ----------- |
| Izena | Identifikazioan laguntzeko azpikontrata lerroaren izena. |Azpikontratazio lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da.
| Deskribapenak | Azpikontratuaren lerroan aginduta dauden produktuen deskribapen laburra. | Batere ez |
| Lerro mota | Eremu honek balioa lehenetsia dauka **Kopuruan oinarrituta**. |Batere ez |
| Fakturazio-metodoa | Hau da aukera multzo Project Operations-ek onartzen dituzten bi kontratazio eredu nagusiak adierazten dituena: **Prezio finkoa** eta **Denbora eta materiala**. | Aukeratutako fakturazio metodoan oinarrituta, Mugarrian oinarritutako faktura egutegia eskuragarri dago Prezio finkoaren fakturazio metodoa duten azpikontratazio lerroetarako. |
| Transakzio-klasea |Eremu honek balioa lehenetsia dauka **Denbora**. Produktuak erosteko azpikontrata lerroak sortzeko, ezarri **Transakzio klasea** eremua **Materiala** gisa.  | Horrek adierazten du azpikontratazio lerroa proiektuetan erabilitako produktuen erosketa erregistratzeko erabiltzen ari dela. |
| Hautatu produktua | Aukeratu erosten ari zaren produktua produktuen katalogoan mantentzen den edo idatzi beharreko produktua den. |Batere ez |
| Produktu | Hautatu produktu aktibo bat katalogoan. Eremu hau eskuragarri dago soilik **Aukeratu produktua** ezarrita dago **Lehendik dagoena**. |**Produktua** eta **Unitatea** balioen konbinazioa lehenetsitako moduan edo azpikontratatutako linearen unitateko prezioaren arabera kalkulatuko da.
| Katalogotik kanpoko produktua | Idatzi izena katalogoz kanpoko produktua. Eremu hau eskuragarri dago soilik **Aukeratu produktua** ezarrita dago **Katalogoz kanpokoa**.  |Erosketa prezioa ez da automatikoki beteko idazketa produktuetarako.|
| Eskatutako entrega-data | Idatzi produktuen beharrezko entrega data.| Data hau azpikontratari atxikitako proiektuen prezioen zerrendetatik proiektuaren prezioen zerrenda hautatzeko ere erabiltzen da. Azpikontratazio linean produktuaren kostua prezio zerrenda horretatik lehenetsita dago. |
| Kontratatutako entrega-data | Idatzi produktuak kontratu bidez entregatzeko hitzarmena adostea.  |Batere ez|
| Eskatutako kopurua | Idatzi saltzaileari erosten zaion produktuaren kopurua.| Hau erabiliko da abisuak erakusteko proiektuaren kudeatzailea kopuru horretatik gora ateratzen denean.|
| Salmenta-unitatea | Balio hau lehenetsita dago katalogoko produktuetan soilik. |Noiz **Produktua** eta **Eskatutako entrega eguna** biak daude hautatuta, sistemak entregatzeko dataren arabera aukeratutako prezioen zerrenda hautatzen du. Lotutako prezioen zerrendako elementuak bat datorren produktuari buruz galdetzen dira. Unitate eta unitate taldearen balioak prezioen zerrendako erregistroaren konfigurazioan lehenetsita daude. |
| Unitatea | Balio horrek lehenespenez egiten du prezioen zerrendako elementuen erregistroan ezarritako unitatea. Beharrezkoa izanez gero, beste unitate batera alda dezakezu.| Produktuaren eta unitatearen konbinazioa lehendik dauden katalogoko produktuen azpikontrata lerroaren unitateko prezioa lehenesteko erabiltzen da. |
| Unitate-prezioa | Prezio unitarioa lehenetsita dago azpikontratazio lerroaren eskatutako entrega datarako aplikagarria den proiektuaren prezio zerrendarekin lotutako produktuen eta unitatearen konbinazioa erabiliz.  |Batere ez |
| Guztizko partziala | Irakurtzeko soilik den eremu hau Kantitatea x Prezio unitario gisa kalkulatzen da bi eremuek balioak sartu badituzte. Bai **Kopurua** zelaia, **Prezio unitarioa** eremua edo biak hutsik daude, eskuz sar dezakezu balio bat.  |Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren balioa. |Batere ez |
| Zenbatekoa guztira | Kalkulatutako eremu honek zergak sartu ondoren azpikontrataren zenbateko lerro osoa erakusten du. Eremu honetako balioa guztizko Azpitotala + Zerga gisa kalkulatzen da. |Batere ez |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]