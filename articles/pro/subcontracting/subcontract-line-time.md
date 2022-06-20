---
title: Azpikontratuaren lerroak denboraren arabera
description: Artikulu honek denboraren azpikontratazio lerroak nola erregistratu eta saltzaileei denbora erostea nola erregistratu azaltzen du.
author: rumant
ms.date: 08/05/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 0295ddd1b36eef9289110c4fe7b51397d81320d6
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925933"
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

| **Eremua** | **Azalpena** | **Inpaktu funtzionala** |
| --- | --- | --- |
| Izena | Identifikazioan laguntzeko azpikontrata lerroaren izena. | Azpikontratazio lerroetan oinarritutako bilaketa guztietan lehen zutabe gisa erakutsiko da. |
| Deskribapenak | Azpikontratuaren lerroan erosita dauden zerbitzuen deskribapen laburra. |Batere ez |
| Lerro mota |   Eremu honek balioa lehenetsia dauka **Kopuruan oinarrituta**.| Batere ez |
| Fakturazio-metodoa | Hau da aukera multzo Project Operations-ek onartzen dituzten bi kontratazio eredu nagusiak adierazten dituena: **Prezio finkoa** eta **Denbora eta materiala**. | Aukeratutako fakturazio metodoan oinarrituta, Mugarrian oinarritutako faktura egutegia eskuragarri dago Prezio finkoaren fakturazio metodoa duten azpikontratazio lerroetarako. |
| Transakzio-klasea | Balio lehenetsia **Denbora** da. | Horrek adierazten du azpikontratazio lerroa azpikontratisten denboraren erosketa erregistratzeko erabiltzen ari dela. |
| Funtzioa | Aukeratu denbora erosten ari diren azpikontratazio baliabideen eginkizuna. | Azpikontratazioko baliabideek betetzen duten eginkizunak erosketaren kostua zehazten du. |
| Eskatutako hasiera | Sartu data kontratisten baliabideak behar direnean lanean hasteko. | Azpikontratari erantsitako proiektuen prezioen zerrendetatik proiektuaren prezioen zerrenda hautatzeko erabiltzen da. Azpikontratazio linearen rolaren kostua prezio zerrenda horretatik dator. |
| Eskatutako amaiera | Idatzi azpikontratisten baliabidearen esleipena amaitzen den data. | Hau erabiliko da abisuak erakusteko proiektuaren kudeatzailea data horretatik aurrera gertatzen diren baliabide eskakizunetarako gaitasunetik ateratzen denean. |
| Eskatutako kopurua | Idatzi saltzaileari erosi beharreko rolaren ordu kopurua. | Hau erabiliko da abisuak erakusteko proiektuaren kudeatzailea baliabide-eskakizunetarako gaitasun horretatik gora ateratzen denean. |
| Salmenta-unitatea | Lehenetsitako balioa **Denboraren salmenta-unitatea** da, aldatu ezin dena. | Batere ez|
| Unitatea | Eremu honen lehenetsia ordutik oinarrizko ordu unitatea **Denboraren salmenta-unitatea** da. Balio hau alda dezakezu **Denboraren salmenta-unitateko** edozein unitate erosteko, hala nola eguna edo astea. | **Funtzioa** eta **Unitatea** balioen konbinazioa lehenetsitako moduan edo azpikontratatutako linearen unitateko prezioaren arabera kalkulatuko da. |
| Unitate-prezioa | Unitateko prezio lehenetsiak konbinazioa erabiltzen du **Funtzioa** eta **Unitatea** proiektuaren prezioen zerrendatik **Eskatutako hasiera** azpikontrata lerroaren data. | Aplikagarria den proiektuaren prezioen zerrendak azpikontratazio linearen unitatea ez den beste unitate batean ezarrita duenean, sistemak unitate bihurketa erabiltzen du prezio unitarioa kalkulatzeko. |
| Guztizko partziala |    Irakurtzeko soilik den eremua da Kantitatea x Unitatearen prezioa bezala kalkulatzen dena, bai kantitatearen bai unitateko prezioaren balioak sartzen badira. Kantitatea, prezio-unitatea, edo biak hutsik badaude, idatzi balioa eremuan. | Batere ez|
| Salmenten zerga |   Idatzi salmenta-zergaren zenbatekoa. |Batere ez |
| Zenbatekoa guztira | Azpikontratuaren lerroaren guztizko kantitatea barne hartutako zergak. Eremu honetan kalkulatuta dago Azpitotala + Salmenten zerga.|Batere ez |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
