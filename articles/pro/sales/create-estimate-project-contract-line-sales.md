---
title: Aurreikusi proiektuetan oinarritutako kontratuaren lerroa - arina
description: Gai honek proiektuan oinarritutako kontratu lerroak aurreikusteari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 8b4379cc5822d08b55623f0f3d4d49791af90927
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914387"
---
# <a name="estimate-a-projectbased-contract-line---lite"></a>Aurreikusi proiektuetan oinarritutako kontratuaren lerroa - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Dynamics 365 Project Operations-en, proiektuan oinarritutako kontratu lerroak xehetasunak ditu, kontratu lerroa emateko egindako lanaren kostua eta diru sarrera potentzialak kalkulatzen laguntzen dutenak.

Proiektuetan oinarritutako kontratu lerro bat kalkulatzeko, joan **Kontratu-lerroaren xehetasuna** proiektuan oinarritutako fitxa **Kontratu-lerroa**.  Proiektuan oinarritutako kontratu lerro batean aurrekontua sortzeko bi modu daude:

   - Sortu aurrekontua zuzenean kontratuaren lerroan, kontratuaren lerroaren xehetasunak eskuz gehituz.
   - Sortu proiektu bat eta proiektu plana, eta, ondoren, proiektua eta zereginak proiektuaren kontratu lerroarekin lotu. Horrek proiektuaren planaren aurrekontua kontratu lerroan inportatzeko prozesua ahalbidetzen du kontratu lerroan sartutako osagaietan oinarrituta.

## <a name="create-an-estimation-directly-on-a-projectbased-contract-line"></a>Sortu aurreikuspenak zuzenean proiektuetan oinarritutako kontratuaren lerro batean

Proiektuan oinarritutako kontratu lerroan zenbatespena zuzenean sortzeko, jarraitu urrats hauei:

1. Joan kontratuaren lerrora eta hautatu **Kontratu-lerroaren xehetasuna** fitxa. Fitxa honetan sortzen dituzun lerroak laburtu eta bistaratzen dira **Kontratatutako balioa** **Kontratuaren lerroa** eremuan. 
2. **Kontratuaren lerroaren xehetasunak** azpisarean, hautatu **Kontratu linea berrien xehetasuna**. Bizkor sortzeko graduatzailea irekitzen da. Ondorengo eremuak eskuragarri daude **Kontratu-lerroaren xehetasunak** orrialdea.

| Eremua | Kokapena | Deskribapenak | Downstream eragina |
| --- | --- | --- | --- |
| **Azalpena** | **Sorrera bizkorra** | Aurreikuspen jakin baten azalpena. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Transakzio-klasea** | **Sorrera bizkorra** | Hau da fitxategian sartutako transakzio klaseen zerrenda **Orokorra** proiektuan oinarritutako kontratu lerroaren fitxa. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Hautatu produktua** | **Sorrera bizkorra** | Transakzio klasea dagoenean aplikatzen da **Materiala**. Zehatz dezakezu aurreikusitako lerro hau **Lehendik dagoen** (katalogoa) produktu edo **Katalogotik kanpoko** produktu batena den. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Produktu** | **Sorrera bizkorra** | Produktuen katalogoko produktuaren IDa. Eremu hau gaituta egoteko, **Lehendik dagoen produktuan** hautatu behar duzu **Aukeratu produktua** eremuan. IDa salmenta prezioa kontratuan jasotako proiektuaren zerrendatik berreskuratzeko erabiltzen da. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Katalogotik kanpoko produktua** | **Sorrera bizkorra** | Produktuaren izena sartzeko testu eremua. Eremu hau hautatzen duzunean gaituta egongo da **Idatzi** produktuan **Aukeratu produktua** eremua.| Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Funtzioa** | **Sorrera bizkorra** | Lan hori egiten ari den edo gastu hori eragiten duen pertsonaren papera. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak.|
| **Kategoria** | **Sorrera bizkorra** | Lanaren edo gastuaren kategoria. |Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak.|
| **Hasiera-data** | **Sorrera bizkorra** | Lanaren hasiera-data. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Amaiera-data** | **Sorrera bizkorra** | Lanaren amaiera-data. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Baliabide-unitatea** | **Sorrera bizkorra** | Kostu hori suposatzen duen eta bertan lan egiteko baliabidea eskaintzen duen baliabideen unitatea. |Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak eta kostuaren prezioan erabiltzen da. |
| **Unitate-antolaketa** | **Sorrera bizkorra** | Lanaren, produktuaren edo gastuaren unitate taldea. Unitateak unitateen ordutegiari edo unitate talde bati dagozkie. Adibidez, *miliak* eta *kilometroak (km)* distantzia deskribatzen duten unitate multzo bateko kide diren unitateak dira. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Unitatea** | **Sorrera bizkorra** | Lanaren, produktuaren edo gastuaren unitatea. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Kantitatea** | **Sorrera bizkorra** | Lanaren, produktuaren edo gastuaren zenbatekoa. | Balio horrek lehenetsitako lotura duen kontratuaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| **Unitate-prezioa** | **Sorrera bizkorra** | Lana burutzen duen rolaren faktura-tasa, produktuaren unitateko prezioa edo produktuaren edo gastu-kategoriaren salmenta-prezioa. Eremu honek lehenetsitakoa da **Denbora** hasierako datarako eraginkorra den proiektuaren prezioen zerrendako rol prezioen lerroan prezioen dimentsio balioen konbinazioan oinarrituta. **Gastuak** eremuari dagokienez, eremu honen lehenetsia hasierako datarako eraginkorra den proiektuaren prezioen zerrendako transakzioen kategoriako prezioaren konfiguraziokoa da. Transakzio-kategoriaren prezio-metodoa **unitateko prezioa** ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. Produktuetarako, eremu honen lehenetsia **Prezioen zerrendako elementua** hasiera datarako eraginkorra den proiektuaren prezioen zerrendan.| Lana burutzen duen rolaren kostu-tasa, edo gastuen kategoriaren kostua unitateko edo produktuaren kostua unitateko. Eremu honek lehenetsitakoa da **Denbora** hasierako datarako eraginkorra den kontratu-unitateari atxikiko kostuaren prezio-zerrendako rol prezioen lerroan prezioen dimentsio balioen konbinazioan oinarrituta. Gastuei dagokienez, eremu honen lehenetsia hasierako datarako eraginkorra den kontratu-unitateen zerrendako transakzioen kategoriako prezioaren konfiguraziokoa da. Transakzio-kategoriaren prezio-metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. Produktuetarako, eremu honen lehenetsia **Prezioen zerrendako elementua** hasiera datarako eraginkorra den kontratu-unitateari atxikitako kostuaren prezio-zerrendan.|
| **Aurreikusitako zerga** | **Sorrera bizkorra** | Lan edo gastu horren zerga zenbatetsia. | Lan edo gastu horren zerga zenbatetsia. |
| **Kopurua** | **Sorrera bizkorra** | Eremu honetan balioa gehi dezakezu **Kopurua** eta **Prezioa** eremuak hutsik geratzen dira. **Kopurua** eta **Prezioa** betetzen dira **Zenbatekoa** eremua irakurtzeko soilik da eta honela kalkulatzen da **(Kopurua \*Unitateko prezioa) + Zerga**. | &nbsp; |

## <a name="update-prices-on-contract-line-details"></a>Eguneratu prezioak kontratuaren lineako xehetasunetan

Kontratuarekin bat datorren proiektuaren prezioen zerrendan edo kontratazio unitatearen kostuen prezioen zerrendan prezioak aldatzen badituzu, kontratua banakako lerroaren xehetasunetan berritu ditzakezu aldaketa islatzeko. **Kontratua** orrian, hautatu **Kalkulatu berriro**. Abisu bat agertzen da kontratu honetako kontratu linea guztien prezioak berrezarri direla jakinarazteko. Aukeratu **Bai** salmenten zein kostuen kontratuaren lerroaren xehetasunak berritzeko.

## <a name="access-contract-line-details-for-cost"></a>Sarbidea kontratuaren lineako xehetasunak kostuaren truke

**Kontratuaren lerroaren xehetasunak** fitxa, hautatu lerro bat saretan azpi-sarearen tresna-barran ekintzak bistaratzeko. Azpi-sarearen tresna-barran lehenengo ekintza da **Ireki kostuaren xehetasuna**. Kontratu-lerro honen xehetasunekin lotutako kostu-tasa eta zenbatekoa ikusteko, hautatu **Ireki kostuaren xehetasuna**. 

> [!NOTE]
> Baliabideen enpresa, baliabideen unitatea, kantitatea, datak, eginkizuna edo kategoriako balioak aldatzea kontratuaren lerroaren xehetasunetarako **Kostua** kontratuaren lerroaren xehetasunari dagozkion balioak aldatzen ditu **Salmentak**.

## <a name="currency-on-contract-line-details-for-cost-and-sales"></a>Kontratuaren lineako xehetasunen kostua eta salmenten xehetasunak

Kontratuaren lerroaren xehetasuna **Salmentak** kontratuaren lerroaren xehetasunaren hasierako datan eraginkorra den proiektuaren prezioen zerrendako moneta lehenetsia ezartzen du.

Kontratuaren lerroaren xehetasuna **Kostua** kontratuaren lerroaren xehetasunaren hasierako datan eraginkorra den kontratuaren kontratazio-unitatearen prezioen zerrendako moneta lehenetsia ezartzen du **Kostua** parametrorako.

Errentagarritasunaren kalkuluek kontratuaren lerroaren xehetasunen zenbatekoak bihurtzen dituzte **Kostua** eta **Salmentak** inguruneko oinarrizko monetara kontratuan benetako eta aurreikusitako marjina orokorrak jakinarazteko.

> [!NOTE]
> Moneta biribiltzeko akatsak eta aldatutako marjinak gerta litezke data truke-tasa eraginkorrik ez dagoelako. Erabil itzazu kalkulu hauek proiektuen kontratuetan soilik, gutxi gorabeherakoak baitira eta ez baitira legezko biribilketarako edo bestelako biribiltzeetarako zehaztasun handiagoa eskatzen dutenak eta truke-tasen dataren eraginkortasunaz jabetzea.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
