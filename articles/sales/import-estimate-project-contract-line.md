---
title: Inportatu aurreikuspen bat proiektuetan oinarritutako kontratuaren lerro batera
description: Gai honek proiektu batetik kontratuaren lerro batera aurreikuspenak inportatzeari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f2b9cbb4cce1691f262c85d95849e01f1a812d51
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/20/2020
ms.locfileid: "4071271"
---
# <a name="import-an-estimate-to-a-project-based-contract-line"></a>Inportatu aurreikuspen bat proiektuetan oinarritutako kontratuaren lerro batera

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Dynamics 365 Project Operations-en, kalkuluak proiektu batetik inporta ditzakezu proiektuan oinarritutako kontratu lerro batera.

1. Egiaztatu **Proiektua** proiektuan oinarritutako kontratu lerroaren eremua betetzen da.
2. **Kontratu-lerroaren xehetasunak** fitxan, azpisarean, hautatu **Inportatu proiektuaren zenbatespenetik**. Laburpen aukerak dituen elkarrizketa-orria irekiko da. Eskuragarri dauden laburpen aukerak hauek dira: **Transakzio klasea** , **Kategoria** , **Rola** eta **Proiektuaren zeregina**. Laburpenen hautapenetan oinarritatuta, kontratuaren lerro honetan sartutako transakzio klase guztietarako proiektuaren aurrekontua kopiatzen da. 
3. Zein transakzio klase sartzen diren egiaztatzeko, hautatu kontratuaren lerroko **Orokorra** fitxan eta egiaztatu balioak **Sartu denbora** , **Sartu gastuak** eta **Sartu Tasak**.

Aurrekontuak inportatzerakoan, aplikazioak sistemak kontratuak lehenetsiko ditu aurrekontuari erantsitako proiektuen prezioen zerrendetan eta proiektuan oinarritutako aurrekontu lerroan ezarritako fakturazio motaren arabera. Proiektuan oinarritutako kontratuaren lerroan eginkizun edo kategoria ez-kargagarritzat konfiguratzen bada, rolaren edo kategoriaren inportatutako estimazio lerroa ez-kargagarritzat ezarriko eta ez da kontratuaren lerroaren balio batuketara gehituko.

Kontratuaren lerroak lerroaren xehetasunak dituenean, **Kontratuaren balioa** eta **Aurreikusitako zerga** kontratuaren lerroan eremuak laburbilduta daude eta ezin dira editatu.

Sistema-aukera anitzak hautatzen direnean, laburpena hautatutako aukera guztien arabera laburbiltzen saiatzen da. Laburpenaren irteerak inportatutako kontratu lerro gehiago lortzen ditu laburpen aukera bakarra hautatzen baduzu baino.

Adibidez, proiektuak gastuen aurrekontu lerro hauek baditu:

| Ataza | Kategoria | Data | Kantitatea | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| A zeregina | Hegazkin-txartelak | 2020/01/10 | 4 | 400 | 1600 |
| B zeregina | Hotela | 2020/01/10 | 4 | 200 | 800 |
| C zeregina | Hotela | 2020/11/01 | 2 | 200 | 400 |

Erabiltzaileak **Transakzio klasearen** arabera laburbiltzea hautatzen duenean, informazio hau inportatuko da:

| Ataza | Kategoria | Data | Kantitatea | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| &nbsp;  | &nbsp;  | 2020/01/10 | 3.34 | 840 | 2800 |

Erabiltzaileak **Transakzio klasea** eta **Kategoria** arabera laburbiltzea hautatzen duenean, informazio hau inportatuko da:

| Ataza | Kategoria | Data | Kantitatea | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| A zeregina | Hegazkin-txartelak | 2020/01/10 | 4 | 400 | 1600 |
| &nbsp;  | Hotela | 2020/01/10 | 6 | 200 | 1200 |

Erabiltzaileak **Transakzio klasearen** , **Kategoriaren** eta **Hosto-nodoaren zereginaren** arabera laburbiltzea hautatzen duenean, hau inportatuko da. Ohartu emaitza hau proiektuan zegoenaren berdina dela:

| Ataza | Kategoria | Data | Kantitatea | Unitate-prezioa | Kopurua |
| --- | --- | --- | --- | --- | --- |
| A zeregina | Hegazkin-txartelak | 2020/01/10 | 4 | 400 | 1600 |
| B zeregina | Hotela | 2020/01/10 | 4 | 200 | 800 |
| C zeregina | Hotela | 2020/11/01 | 2 | 200 | 400 |
