---
title: Aurreikusi proiektuetan oinarritutako kontratuaren lerroa
description: Gai honek proiektuan oinarritutako kontratu lerroak aurreikusteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cdc8984e080d995e3a0b667fe662291b499235b2
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278493"
---
# <a name="estimate-a-projectbased-contract-line"></a>Aurreikusi proiektuetan oinarritutako kontratuaren lerroa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_ 

Dynamics 365 Project Operations-en, proiektuan oinarritutako kontratu lerroak xehetasunak ditu, kontratu lerroa emateko egindako lanaren kostua eta diru sarrera potentzialak kalkulatzen laguntzen dutenak.

Proiektuetan oinarritutako kontratu lerro bat kalkulatzeko, joan **Kontratu-lerroaren xehetasuna** proiektuan oinarritutako fitxa **Kontratu-lerroa**.  Proiektuan oinarritutako kontratu lerro batean aurrekontua sortzeko bi modu daude:

   - Sortu aurrekontua zuzenean kontratuaren lerroan, kontratuaren lerroaren xehetasunak eskuz gehituz.
   - Sortu proiektu bat eta proiektu plana, eta, ondoren, proiektua eta zereginak proiektuaren kontratu lerroarekin lotu. Horrek proiektuaren planaren aurrekontua kontratu lerroan inportatzeko prozesua ahalbidetzen du kontratu lerroan sartutako osagaietan oinarrituta.

## <a name="create-an-estimate-directly-on-a-projectbased-contract-line"></a>Sortu aurreikuspenak zuzenean proiektuetan oinarritutako kontratuaren lerro batean

1. Joan kontratuaren lerrora eta hautatu **Kontratu-lerroaren xehetasuna** fitxa. Fitxa honetan sortzen dituzun lerroak laburtu eta bistaratzen dira **Kontratatutako balioa** **Kontratuaren lerroa** eremuan. 
2. **Kontratuaren lerroaren xehetasunak** azpisarean, hautatu **+ Kontratu linea berrien xehetasuna**. Bizkor sortzeko graduatzailea irekitzen da. Ondorengo eremuak eskuragarri daude **Kontratu-lerroaren xehetasunak** forma:

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| **Azalpena** | **Sorrera bizkorra** | Aurreikuspen jakin baten azalpena. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Transakzio-klasea** | **Sorrera bizkorra** | Goitibeherako fitxategian sartutako transakzio klaseen zerrenda da **Orokorra** proiektuan oinarritutako kontratu lerroaren fitxa. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Funtzioa** | **Sorrera bizkorra** | Lan hori egiten ari den edo gastu hori eragiten duen pertsonaren papera. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Kategoria** | **Sorrera bizkorra** | Lanaren edo gastuaren kategoria. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Hasiera-data** | **Sorrera bizkorra** | Lanaren hasiera-data. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Amaiera-data** | **Sorrera bizkorra** | Lanaren amaiera-data. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen den kostua. |
| **Baliabideen enpresa** | **Sorrera bizkorra** | Kostu hori jasaten ari den eta bertan lan egiteko baliabidea eskaintzen duen enpresa edo pertsona juridikoa. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. Eremu hau kostuen prezioak berreskuratzeko ere erabiltzen da. |
| **Baliabide-unitatea** | **Sorrera bizkorra** | Kostu hori suposatzen duen eta bertan lan egiteko baliabidea hornitzen duen baliabideen unitatea. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. Eremu hau kostuen prezioak berreskuratzeko ere erabiltzen da. |
| **Unitate-antolaketa** | **Sorrera bizkorra** | Lanaren edo gastuaren unitate taldea. Unitateak unitateen ordutegiari edo unitate talde bati dagozkie. Adibidez, *miliak* eta *kilometroak (km)* distantzia deskribatzen duten unitate multzo bateko kide diren unitateak dira. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Unitatea** | **Sorrera bizkorra** | Lanaren edo gastuaren unitatea. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Kopurua** | **Sorrera bizkorra** | Lanaren edo gastuaren zenbatekoa. | Eremu honek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Unitate-prezioa** | **Sorrera bizkorra** | Lana burutzen duen rolaren faktura-tasa edo gastu-kategoriako salmenta-prezioa. Eremu honek **Denbora** lehenetsia du hasierako datarako eraginkorra den proiektuaren prezioen zerrendako funtzio eta baliabideen konbinazioan oinarrituta. Gastuei dagokienez, eremu honen lehenetsia hasierako datarako eraginkorra den proiektuaren prezioen zerrendako transakzioen kategoriako prezioaren konfiguraziokoa da. Transakzio-kategoriaren prezio-metodoa **unitateko prezioa** ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. | Lana burutzen duen rolaren kostua, edo kostua gastu-kategoriako unitateko kostua. Eremu honek lehenetsitakoa da **Rolean oinarritutako denbora** eta kontratazio unitateari atxikitako kostu prezioen zerrendako eginkizunen prezioen lerroan baliabideen hornikuntza konbinazioa hasiera datarako indarrean dago. Gastuei dagokienez, eremu honen lehenetsia hasierako datarako eraginkorra den kontratu-unitateen zerrendako transakzioen kategoriako prezioaren konfiguraziokoa da. Transakzio-kategoriaren prezio-metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. |
| **Aurreikusitako zerga** | **Sorrera bizkorra** | Lan honen edo gastuaren zerga zenbatetsia erabiltzaileak sartutako moduan. | Lan honen edo gastuaren zerga zenbatetsia erabiltzaileak sartutako moduan. |
| **Zenbatekoa** | **Sorrera bizkorra** | Eremu honetako balio hau erabiltzaileak gehi dezake **Kopurua** eta **Prezioa** eremuak hutsik geratzen dira. **Kopurua** eta **Prezioa** betetzen dira **Zenbatekoa** eremua irakurtzeko soilik da eta honela kalkulatzen da **(Kopurua \*Unitateko prezioa) + Zerga**. | &nbsp; |

## <a name="update-prices-on-contract-line-details"></a>Eguneratu prezioak kontratuaren lineako xehetasunetan

Kontratuarekin bat datorren proiektuaren prezioen zerrendan edo kontratazio unitatearen kostuen prezioen zerrendan prezioak aldatzen badituzu, kontratua banakako lerroaren xehetasunetan berritu ditzakezu aldaketa islatzeko. **Kontratua** orrian, hautatu **Kalkulatu berriro**. Abisu bat irekiko da kontratu honetako linea guztietako prezioak berrezarriko direla jakinarazteko. Aukeratu **Bai** salmenten zein kostuen kontratuaren lerroaren xehetasunak berritzeko.

## <a name="access-contract-line-details-for-cost"></a>Sarbidea kontratuaren lineako xehetasunak kostuaren truke

**Kontratuaren lerroaren xehetasunak** fitxa, hautatu lerro bat saretan azpi-sarearen tresna-barran ekintzak bistaratzeko. Azpi-sarearen tresna-barran lehenengo ekintza da **Ireki kostuaren xehetasuna**. Kontratu-lerro honen xehetasunekin lotutako kostu-tasa eta zenbatekoa ikusteko, hautatu **Ireki kostuaren xehetasuna**. 

> [!NOTE]
> Baliabideen enpresa, baliabideen unitatea, kantitatea, datak, eginkizuna edo kategoriako balioak aldatzea kontratuaren lerroaren xehetasunetarako **Kostua** kontratuaren lerroaren xehetasunari dagozkion balioak aldatzen ditu **Salmentak**.

## <a name="currency-on-contract-line-details-for-cost-and-sales"></a>Kontratuaren lineako xehetasunen kostua eta salmenten xehetasunak

Kontratuaren lerroaren xehetasuna **Salmentak** kontratuaren lerroaren xehetasunaren hasierako datan eraginkorra den proiektuaren prezioen zerrendako moneta lehenetsia ezartzen du.

Kontratuaren lerroaren xehetasuna **Kostua** kontratuaren lerroaren xehetasunaren hasierako datan eraginkorra den kontratuaren kontratazio-unitatearen prezioen zerrendako moneta lehenetsia ezartzen du **Kostua** parametrorako.

Errentagarritasunaren kalkuluek kontratuaren lerroaren xehetasunen zenbatekoak bihurtzen dituzte **Kostua** eta **Salmentak** inguruneko oinarrizko monetara kontratuan benetako eta aurreikusitako marjina orokorrak jakinarazteko.

> [!NOTE]
> Moneta biribiltzeko akatsak eta aldatutako marjinak gerta litezke data truke-tasa eraginkorrik ez dagoelako. Erabili kalkulu horiek proiektuen kontratuetan gutxi gorabeherako gisa eta ez estatistikako benetako txostenetarako edo biribiltzeko zehaztasun handiagoa behar dutenak eta truke-tasen dataren eraginkortasuna ezagutzea.


[!INCLUDE[footer-include](../includes/footer-banner.md)]