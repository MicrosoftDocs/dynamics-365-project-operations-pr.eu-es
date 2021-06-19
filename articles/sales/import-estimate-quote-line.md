---
title: Inportatu proiektuaren aurreikuspenak proiektuetako eskaintzaren lerrora
description: Gai honek proiektu batetik proiektuaren eskaintzaren lerro batera aurreikuspenak inportatzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ae491495575ce2a5e4aaf0d8f22a14ea4b5e72de
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010186"
---
# <a name="import-estimates-for-a-project-to-a-project-quote-line"></a>Inportatu proiektuaren aurreikuspenak proiektuetako eskaintzaren lerrora

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Salmenta aurreko fasean proiektu bat sortzen bada, proiektuaren finantza-aurrekontua proiektuan oinarritutako aurrekontu-lerrora inportatzea hauta dezakezu.

1. Ziurtatu proiektuan oinarritutako aurrekontu lerroak proiektuaren informazioa duela **Proiektua** eremua.
2. **Eskaintza-lerroaren xehetasunak** fitxan, hautatu **Inportatu proiektuaren aurreikuspenak**.
3. Irekitzen den elkarrizketa-orrian, hautatu laburtzeko aukera hauetako bat:

  - **Transakzio-klasea**
  - **Kategoria**
  - **Funtzioa** 
  - **Proiektuaren zeregina**

Aukeratutakoan oinarrituta, aurrekontu lerro honetan sartutako transakzio klase guztietarako proiektuaren aurrekontua kopiatzen da. Zein transakzio klase sartzen diren egiaztatzeko, hautatu **Orokorra** proiektuan oinarritutako aurrekontu lerroan fitxa eta egiaztatu balioak **Sartu denbora**, **Sartu gastuak** eta **Sartu Tasak**.

Aurrekontuak inportatzerakoan, sistemak aurrekontuak lehenetsiko ditu aurrekontuari erantsitako proiektuen prezioen zerrendetan eta proiektuan oinarritutako aurrekontu lerroan ezarritako fakturazio motaren arabera. Proiektuan oinarritutako aurrekontu lerroan eginkizun edo kategoria ez bada kargagarritzat konfiguratzen bada, inportatutako estimazio lerroa ez da kargagarritzat ezarriko eta ez da aurrekontu lerroaren balio batuketara gehituko.

Aurrekontuaren lerroak lerroaren xehetasunak dituenean, **Aipatu balioa** eta **Aurreikusitako zerga** aurrekontuaren lerroan eremuak laburbilduta daude eta ezin dira editatu.

Sistema-aukera anitzak hautatzen direnean, laburpena hautatutako aukera guztien arabera laburbiltzen saiatzen da. Emaitza da inportatutako aurrekontu lerroen irteera laburpen aukera bakarra hautatuz gero baino gehiago izango dela.

Adibidez, proiektuak gastuen aurrekontu lerro hauek baditu.

| Ataza | Kategoria | Data | Kopurua | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| A zeregina | Hegazkin-txartelak | 2020/01/10 | 4 | 400 | 1600 |
| B zeregina | Hotela | 2020/01/10 | 4 | 200 | 800 |
| C zeregina | Hotela | 2020/11/01 | 2 | 200 | 400 |

Erabiltzaileak Transakzio klasearen arabera laburbiltzea hautatzen duenean, informazio hau inportatuko da.

| Ataza | Kategoria | Data | Kopurua | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| | | 2020/01/10 | 3.34 | 840 | 2800 |

Erabiltzaileak Transakzio klasearen eta Kategoriaren arabera laburbiltzea hautatzen duenean, informazio hau inportatuko da.

| Ataza | Kategoria | Data | Kopurua | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| A zeregina | Hegazkin-txartelak | 2020/01/10 | 4 | 400 | 1600 |
| | Hotela | 2020/01/10 | 6 | 200 | 1200 |

Erabiltzaileak Transakzio klasearen, Kategoriaren eta Hosto-nodoaren zereginaren arabera laburbiltzea hautatzen duenean, informazio hau inportatuko da. Ohartu emaitza hau proiektuan zegoenaren berdina dela.

| Ataza | Kategoria | Data | Kopurua | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| A zeregina | Hegazkin-txartelak | 2020/01/10 | 4 | 400 | 1600 |
| B zeregina | Hotela | 2020/01/10 | 4 | 200 | 800 |
| C zeregina | Hotela | 2020/11/01 | 2 | 200 | 400 |


[!INCLUDE[footer-include](../includes/footer-banner.md)]
