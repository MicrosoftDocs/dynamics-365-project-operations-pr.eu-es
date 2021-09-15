---
title: Azpikontratuaren lerroak denboraren arabera
description: Gai honetan azaltzen da nola kontratatu lerroak denboran grabatzeko eta saltzaileek denbora erostea erregistratzeko.
author: rumant
ms.date: 08/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 10ebe0fcc86b4652ac01e28108361df1f768b61d
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323851"
---
# <a name="subcontract-lines-for-time"></a>Azpikontratuaren lerroak denboraren arabera

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Urtean azpikontrata Dynamics 365 Project Operations denborarako azpikontratazio lerro bat izan dezake. Denboraz azpikontratatzeko lerroek proiektuaren kudeatzaileari saltzailearen baliabideen denbora erostea ahalbidetzen die proiektuaren zereginak eta baliabideen eskakizunak langileei.

Project Operations produktuentzako azpikontratazio lerro bat sortzeko, osatu hurrengo urratsak.

1. Nabigazio panelean, hautatu **Azpikontratak**, eta ireki azpikontrata.
2. Gainean **Azpikontratatzeko Lineak** fitxa, hautatu **Berria** azpikontratazio lerro berri bat sortzeko.
3. Gainean **Sortu bizkor** orrialdean, **Transakzio Klase** eremua, hautatu **Denbora**.
4. Idatzi geratzen den eremuaren informazioa eta gero hautatu **Gorde**.

  Hurrengo taula hornitu informazioa eremuari buruz **Azpikontrataren lerroa** orria eta **Sortu bizkor** orria.

| **Eremua** | **Azalpena** |
| --- | --- |
| Izena | Azpikontratuaren lerroaren izena. |
| Deskribapenak | Azpikontratuaren lerroan erosita dauden zerbitzuen deskribapen laburra. | 
| Lerro mota | Eremu hori lehenetsitako balioa.  |
| Fakturazio-metodoa | Hautatu fakturazio metodoa. Aipatutako azpikontratazio lerroaren fakturazio metodoan oinarrituta, Mugarrian oinarritutako fakturen egutegia eskuragarri dago Prezio finkoaren fakturazio metodoarentzat. |
| Transakzio-klasea | Eremu hau azpikontratazio lerroa azpikontratazioaren denbora erosteko erregistratzeko erabiltzen den adierazten duen balio lehenetsia da. |
| Funtzioa | Denbora erosten ari diren azpikontratatutako baliabideen eginkizuna. Azpikontratazioko baliabideei esleitutako eginkizunak erosketaren kostua zehazten du. |
| Eskatutako hasiera | Azpikontratazioko baliabideak lanean hasteko eguna. Eskatutako hasiera azpikontratari atxikitako proiektuen prezioen zerrendetatik proiektuaren prezioen zerrenda hautatzeko ere erabiltzen da. Azpikontratazio linean funtzioaren kostua prezio zerrenda horretatik lehenetsita dago. |
| Eskatutako amaiera | Azpikontratisten baliabideen esleipena amaitzen den eguna. Data hau abisuak erakusteko proiektuaren kudeatzaile bat data horretatik aurrera gertatzen diren baliabide eskakizunetarako gaitasun horretatik ateratzen ari denean. |
| Eskatutako kopurua | Saltzaileari erosten zaizkion rol ordu kopurua. Balio hau abisuak erakusteko proiektuaren kudeatzaile bat gertatzen diren baliabide eskakizunetarako gaitasun horretatik ateratzen ari denean. |
| Salmenta-unitatea | Eremu balio honek denbora unitate taldea du lehenetsita eta ezin da aldatu.  |
| Unitatea | Eremu honek denbora-unitateko oinarrizko ordu-unitatea da lehenespenez. Balio hau alda dezakezu Denbora unitate taldeko edozein unitate erosteko, hala nola eguna edo astea. Konbinazioa Funtzioa eta Unitatea erabilita kalkulatzeko unitate-prezioa azpikontratuaren lerroa. |
| Unitate-prezioa | Prezio unitarioa lehenetsita dago azpikontratazio lerroaren eskatutako entrega datarako aplikagarria den proiektuaren prezio zerrendarekin lotutako funtzioa eta unitatearen konbinazioa erabiliz. Aplikagarria den proiektuaren prezioen zerrendak azpikontratazio linearen unitatea ez den beste unitate batean ezarrita duenean, sistemak unitate bihurketa erabiltzen du prezio unitarioa kalkulatzeko. |
| Guztizko partziala | Irakurtzeko soilik den eremua da automatikoki honela kalkulatzen dena **Kopurua x Unitateko prezioa** kantitatea eta prezio unitarioaren balioak sartzen badira. Kantitatea, prezio-unitatea, edo biak hutsik badaude, idatzi balioa eremuan. |
| Salmenten zerga |  Idatzi salmenta-zergaren zenbatekoa. |
| Zenbatekoa guztira | Zergak sartu ondoren azpikontrataren lerroaren zenbateko osoa erakusten du. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
