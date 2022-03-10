---
title: Azpikontratuaren lerroak gastuen kategorien arabera
description: Gai honetan produktuen azpikontratazio lerroak nola grabatu eta saltzaileek denbora erosketak erregistratzeko eremu desberdinak nola erabili azaltzen da.
author: rumant
ms.date: 08/06/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0c32bf2ac54de98a921d338e436ecd089e68a759
ms.sourcegitcommit: cd4e81f129681a12f2efe63ec2bb14e611cf88ba
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/20/2021
ms.locfileid: "7506084"
---
#  <a name="subcontract-lines-for-expense-categories"></a>Azpikontratuaren lerroak gastuen kategorien arabera

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Urtean azpikontrata Dynamics 365 Project Operations gastuen kategorietarako lerro bat izan dezake. Gastu kategorietarako azpikontratazio lerroei esker, proiektuaren kudeatzaile batek zerbitzu edo produktu kategoriak eros ditzake proiektu batean karga ditzaketen saltzaileei.

Project Operations gastu kategorietarako azpikontratazio lerro bat sortzeko, osatu hurrengo urratsak.

1. Nabigazio panelean, hautatu **Azpikontratak**, eta ireki lan egin nahi duzun azpikontratua.
2. Gainean **Azpikontratatzeko Lineak** fitxa, hautatu **Berria** lerro berri bat sortzeko.
3. Gainean **Sortu bizkor** orrialdean, **Transakzio Klase** eremua, hautatu **Gastua** eta sartu edo hautatu beharrezko edozein eremuko informazioa.

Hurrengo taula hornitu informazioa eremuari buruz **Azpikontrataren lerroa** xehetasunak orria eta **Sortu bizkor** orria.

| **Eremua** | **Azalpena** | **Inpaktu funtzionala** |
| --- | --- | --- |
| Izena | Identifikazioan laguntzeko azpikontrata lerroaren izena. | Azpikontratazio lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da. |
| Deskribapenak | Azpikontratazio lerroan erosten ari diren gastuen kategorien deskribapen laburra. | Batere ez |
|Lerro mota | Eremu honek balioa lehenetsia dauka **Kopuruan oinarrituta**. |Batere ez |
| Fakturazio-metodoa | Hau da aukera multzo Project Operations-ek onartzen dituzten bi kontratazio eredu nagusiak adierazten dituena: **Prezio finkoa** eta **Denbora eta materiala**. | Mugarrian oinarritutako faktura egutegia eskuragarri dago azpikontratazioaren lerroetarako, Prezio finkoaren fakturazio metodoa hautatuta badago. |
| Transakzio-klasea | Eremu honek balioa lehenetsia dauka **Denbora**. Produktuak erosteko azpikontrata lerroak sortzeko ezarri **Transakzio klasea** eremuan **Gastua**.  | Horrek adierazten du azpikontratazio lerroa proiektuetan erabilitako gastuen kategoriaren erosketa erregistratzeko erabiltzen ari dela. |
| Transakzio-kategoria | Sistemako transakzio aktiboen kategorien zerrenda erakusten du. |Batere ez |
| Eskatutako hasiera | Idatzi erosketen kategoriak saltzailearen eskura egon behar duen eguna. | Eskatutako hasiera azpikontratari erantsitako proiektuen prezioen zerrendetatik proiektuaren prezioen zerrenda hautatzeko erabiltzen da. Azpikontratazio linearen kategoriaren kostua prezio zerrenda horretatik dator. |
| Eskatutako amaiera | Idatzi erosketa-kategoriak behar ez diren eguna. | Hau erabiliko da abisuak erakusteko proiektuaren kudeatzaile batek azpikontratazio lerro hau data horretatik aurrera eskatzen diren proiektuaren gastu zehatzen kalkuluekin lotzen duenean. |
| Eskatutako kopurua | Saltzailearengandik erositako kategoriaren kopurua. | Hau erabiliko da abisuak erakusteko proiektuaren kudeatzailea kopuru horretatik gora ateratzen denean.|
| Salmenta-unitatea | Balio lehenetsia hautatutako kategorian konfiguratutako unitate talde lehenetsian oinarritzen da. |Batere ez |
| Unitatea | Lehenetsia hautatutako kategorian konfiguratutako unitate lehenetsian oinarritzen da.  | **Kategoria** eta **Unitatea** balioen konbinazioa lehenetsitako moduan edo azpikontratatutako linearen unitateko prezioaren arabera kalkulatuko da.  |
| Unitate-prezioa | Balio lehenetsiak konbinazioa erabiltzen du **Kategoria** eta **Unitatea** proiektuaren prezioen zerrendarekin lotutako kategoria-preziotik eskatutako hasiera azpikontrata lerroaren data. |Batere ez |
| Guztizko partziala | Irakurtzeko soilik den eremua da Kantitatea X Unitatearen prezioa bezala kalkulatzen dena, bai kantitatearen bai unitateko prezioaren balioak sartzen badira. Eremu biak edo biak hutsik badaude, balio bat sar dezakezu eremu horretan. |Batere ez |
| Salmenten zerga | Idatzi salmenta-zergaren zenbatekoa. |Batere ez |
| Zenbatekoa guztira | Azpikontratuaren lerroaren guztizko kantitatea barne hartutako zergak. Eremu honetan kalkulatuta dago Azpitotala + Salmenten zerga. |Batere ez |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
