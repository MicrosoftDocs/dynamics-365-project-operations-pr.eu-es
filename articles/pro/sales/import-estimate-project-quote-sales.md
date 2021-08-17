---
title: Inportatu proiektuaren aurreikuspenak proiektuetan oinarritutako eskaintzaren lerrora - arina
description: Gai honek proiektu batetik eskaintzaren lerro batera aurreikuspenak inportatzeari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a5ac7827f3499aafb63f6bc0b8580ca52e883f272464532bd353170a12b3ae55
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986116"
---
# <a name="import-estimates-for-a-project-to-a-project-based-quote-line"></a>Inportatu proiektuaren aurreikuspenak proiektuetan oinarritutako eskaintzaren lerrora 

_**Honetarako aplikatzen da:** inplementazio arina - mahukatik proformako fakturaziora, Baliabideen / stockean oinarritutako eszenatokien Project Operations_

Salmenta aurreko fasean proiektu bat sortzen bada, proiektuaren finantza-aurrekontua proiektuan oinarritutako aurrekontu-lerrora inportatzea hauta dezakezu.

1. Ziurtatu proiektuan oinarritutako aurrekontu lerroak proiektuaren informazioa duela **Proiektua** eremua.
2. **Eskaintza-lerroaren xehetasunak** fitxan, hautatu **Inportatu proiektuaren aurreikuspenak**.
3. Irekitzen den elkarrizketa-orrian, hautatu laburtzeko aukera hauetako bat.

  - **Transakzio-klasea**
  - **Kategoria**
  - **Funtzioa** 
  - **Proiektuaren zeregina**

Aukeratutakoan oinarrituta, aurrekontu lerro honetan sartutako transakzio klase guztietarako proiektuaren aurrekontua kopiatzen da. Zein transakzio klase sartzen diren egiaztatzeko, hautatu **Orokorra** proiektuan oinarritutako aurrekontu lerroan fitxa eta egiaztatu balioak **Sartu denbora**, **Sartu gastuak**, **Sartu materialak** eta **Sartu Tasak**.  Zein zeregin sartzen diren egiaztatzeko, hautatu **Zeregin kargagarriak** aurrekontuaren lerroan fitxa.

Lotutako zereginen eta sartutako transakzio klaseen arabera, ataza eta transakzio klase konbinazio horien kalkuluak aurrekontuaren lerroan inportatzen dira.

Aurrekontuak inportatzerakoan, sistemak aurrekontuak lehenetsiko ditu aurrekontuari erantsitako proiektuen prezioen zerrendetan eta proiektuan oinarritutako aurrekontu lerroan ezarritako fakturazio motaren arabera. Proiektuan oinarritutako aurrekontu lerroan eginkizun, funtzio edo kategoria ez bada kargagarritzat konfiguratzen bada, inportatutako estimazio lerroa ez da kargagarritzat ezarriko eta ez da aurrekontu lerroaren balio batuketara gehituko.

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
|||2020/01/10 | 3.34 | 840 | 2800 |

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


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
