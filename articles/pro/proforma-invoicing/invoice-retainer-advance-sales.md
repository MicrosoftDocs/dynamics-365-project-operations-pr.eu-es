---
title: Fakturatu atxikipen edo aurrerakin bat
description: Gai honek proiektuaren eragiketetan atxikipena edo aurrerakina fakturatzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c1c53e39a8c6fb27deff5e7a05d5cca3a4215466
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274128"
---
# <a name="invoice-a-retainer-or-an-advance"></a>Fakturatu atxikipen edo aurrerakin bat

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek aurrerakinetan oinarritutako kontratuak eta aldi bateko aurrerakinak onartzen ditu. Proiektuaren kontratuan, atxikitzaileen ordutegia edo behin-behineko aurrerapen bat erregistratu dezakezu. Hala ere, proiektuaren kontratu mailan grabatzeak ez du berehala atxikipena edo aurrerapena erabilgarri egongo. Bezeroari benetan kobratzen duen fakturan atxikipena edo aurrerakina erabiltzeko, lehenik atxikipena edo aurrerakina fakturatu behar da.

Osatu urrats hauek atxikipena edo aurrerakina fakturatzeko.

1. Aukeratu **Salmentak** > **Fakturazioa** > **Atxikitzaileak eta aurrerakinak**. 
2. **Aurrerakinak eta gordailuak** orrialdean, erabili iragazkia atxikitzaile zehatza hautatzeko edo aurreratzeko fakturatzeko eta markatu gisa **Fakturatzeko prest**.
3. Sortu faktura bat eskuz **Proiektuaren kontratua** zerrenda edo xehetasun orria. Atxikipena edo aurrerakina fakturaren zirriborroan agertzen da **Aurrerakinak eta gordailuak** atala **Faktura** orrialdea.
4. Berretsi faktura. Horrek atxikipena edo aurrerapena erabilerarako erabilgarri jarriko ditu. Fakturan egiaztatu dezakezu **Atxikitzaileak eta aurrerakinak** zerrenda orria. Fakturatutako Aurrerapena edo Atxikipena egiteko, eskuragarri dagoen zenbatekoa saretan agertzen da.

## <a name="create-a-retainer-or-advance-from-the-invoice-grid"></a>Sortu atxikipena edo aurreratu Faktura saretik

Atxikimendua edo aurrerakina sor dezakezu zuzenean fakturan.

1. Faktura zirriborro batean, **Aurrerakinak eta gordailuak** azpisarea, hautatu **Berria** atxikipen berria edo aurrerapena sortzeko. 
2. **Sorrera bizkorra** orrialdean, gehitu beharrezko informazioa eta hautatu **Gorde**. Atxikipena edo aurrerakina fakturarekin lotutako proiektuaren kontratuan sortzen da. Aurrerakina eta gordailua automatikoki markatzen da **Fakturatzeko prest** gisa eta, ondoren, **Aurrerakinak eta atxikipenak** azpisaretan gehitzen da **Faktura** orrian.

## <a name="reconcile-an-invoiced-retainer-or-advance"></a>Konpondu fakturatutako atxikipen edo aurrerakin bat

Atxikipena edo aurrerakina fakturatu ondoren, fakturan erabil daitezke edo bateratu daitezke denbora, gastuak, mugarriak edo proiektuetan oinarritutako beste karga batzuekin. Bezeroak fakturaren zenbatekoa murrizten ikusiko du faktura honetan erabilitako atxikipenaren edo aurrerakinaren zenbatekoarekin.

Atxikimenduak edo aurrerakinak fakturatu dituen proiektuaren kontratu batengatik sortzen den faktura guztietan, Project Operations-ek automatikoki atxikipena edo aurrerakina fakturan aplikatzen du.

Hori ikus daiteke **Atxikitzaile eta aurrerapen aplikatuak** saretan **Faktura** orrialdea. Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Atxikitzaile eta aurrerapen aplikatuak** sareta **Proiektuaren faktura** orrialdea.

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| Deskribapena | Hori ikus daiteke **Aplikatutako atxikipenak eta aurrerapenak** saretan **Proiektuaren faktura** orrialdean |Irakurtzeko soilik den eremu honek faktura honetan erabilitako atxikipenaren edo aurrerakinaren deskribapena eskaintzen du. Balioa ezin da aldatu fakturan. Balio hau egunkarian azpisarean eguneratu daiteke **Proiektuaren kontratua** orrialdean. | Eremu hau bezeroari bistaratu dakioke inprimatutako fakturan, fakturan zein atxikipen edo aurrerakin aplikatzen den adierazteko. |
| Entrega-data | Hori ikus daiteke **Aplikatutako atxikipenak eta aurrerapenak** saretan **Proiektuaren faktura** orrialdean  | Irakurtzeko soilik den eremu honek faktura honetan erabilitako atxikipenaren edo aurrerakinaren faktura-data eskaintzen du. Balioa ezin da aldatu fakturan. Balio hau egunkarian azpisarean eguneratu daiteke **Proiektuaren kontratua** orrialdean. | Eremu hau bezeroari bistaratu dakioke inprimatutako fakturan, atxikipena edo aurrerakina bezeroari aplikatuko zitzaion data adierazteko. |
| Kopurua | Hori ikus daiteke **Aplikatutako atxikipenak eta aurrerapenak** saretan **Proiektuaren faktura** orrialdean  | Irakurtzeko soilik den eremu honek faktura honetan erabilitako atxikipenaren edo aurrerakinaren zenbatekoa eskaintzen du. Balioa ezin da aldatu fakturan. Balio hau egunkarian azpisarean eguneratu daiteke **Proiektuaren kontratua** orrialdean. | Eremu hau bezeroari bistaratu dakioke inprimatutako fakturan bezeroak ordaindutako atxikipenaren edo aurrerakinaren jatorrizko zenbatekoa adierazteko. |
| Erabilitako zenbatekoa | Hori ikus daiteke **Aplikatutako atxikipenak eta aurrerapenak** saretan **Proiektuaren faktura** orrialdean  | Irakurtzeko soilik den eremu honek atxikipenaren edo aurrerapenaren zenbatekoa erabili den laburbiltzen duen kalkulatutako balioa eskaintzen du. | Eremu hau bezeroari bistaratu dakioke inprimatutako fakturan atxikipen edo aurrerakin honetan jada erabilitako zenbatekoa adierazteko. |
| Zenbateko hedatua | Hori ikus daiteke **Aplikatutako atxikipenak eta aurrerapenak** saretan **Proiektuaren faktura** orrialdean  | Eremu editagarri honek proiektu-faktura honetan erabiltzen ari den atxikipenaren edo aurrerakinaren zenbatekoa eskaintzen du. Kopuru hori ezin da aurrerapenean eskuragarri dagoena baino handiagoa izan. Sistemak automatikoki kalkulatzen du **Zenbatekoa** eta **Erabilitako kopurua** saretako eremuak. Kopuru hori txikiagotu dezakezu erabilgarri dagoena baino gutxiago erabiltzeko, baina ezin duzu kopurua eskuragarri dagoena baino gehiago erabili. | Eremu hau bezeroari bistaratu dakioke inprimatutako fakturan atxikipen edo aurrerakin honetan jada erabiltzen ari den zenbatekoa adierazteko. |
| Aurrerapen zenbatekoaren balantzea. | Hori ikus daiteke **Aplikatutako atxikipenak eta aurrerapenak** saretan **Proiektuaren faktura** orrialdean  | Irakurtzeko soilik den eremu honek faktura baieztatu ondoren atxikipen edo aurrerakinaren zenbatekoa geratuko denaren balioa ematen du. | Eremu hau bezeroari bistaratu dakioke inprimatutako fakturan faktura berretsi eta ordaindu eta gero atxikipen edo aurrerakin honetan jada erabil gabe geratutako zenbatekoa adierazteko. |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]