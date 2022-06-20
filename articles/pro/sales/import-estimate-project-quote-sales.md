---
title: Inportatu proiektuaren aurreikuspenak proiektuetan oinarritutako eskaintzaren lerrora - arina
description: Artikulu honetan, proiektu baten zenbatespenak aurrekontu-lerro batera nola inportatu behar den ematen da.
author: rumant
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 820d858fecf70e50a9ce8943db706ff6cac29992
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8917285"
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
