---
title: Proiektuetan oinarritutako eskaintzaren lerroa aurreikustea
description: Artikulu honek proiektuetan oinarritutako aurrekontu-lerro batean zenbatespena sortzeko moduari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 2a8aa2971431cd1f2082c8fc80db1438be185f5b
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914341"
---
# <a name="estimating-a-project-based-quote-line"></a>Proiektuetan oinarritutako eskaintzaren lerroa aurreikustea

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuan oinarritutako aurrekontu lerroak aurrekontua lerroa emateko lanaren kostua eta diru sarrera potentzialak kalkulatzen laguntzen duten xehetasunak ditu.

Proiektuan oinarritutako aurrekontu lerroa kalkulatzeko, hautatu proiektuan oinarritutako aurrekontu lerroan **Aipatu lerroaren xehetasuna** fitxa. Proiektuan oinarritutako aurrekontu lerro batean aurrekontua sortzeko bi modu daude:

- Eskuz sortu aurrekontua aurrekontuaren lerroan zuzenean aurrekontuaren lerroaren xehetasunak erabiliz. 
- Sortu proiektu bat eta proiektuaren plana, eta, ondoren, lotu proiektua eta proiektuko zereginak aurrekontu lerroarekin. Eman duzun informazioan oinarrituta proiektuaren planeko aurrekontuak aurrekontuaren lerroan inportatzeko prozesua gaituta egongo da.

## <a name="create-estimates-directly-on-a-project-based-quote-line"></a>Sortu aurreikuspenak zunenean proiektuan oinarritutako eskaintzaren lerro batean

Proiektuan oinarritutako aurrekontu lerro batean aurrekontua sortzeko, hautatu **Aipatu lerroaren xehetasuna** fitxa. Fitxa honetan sortzen duzun lerroaldean aurrekontu lerro honetarako aipatutako balioa laburbilduko da. 

Aurrekontuaren lerroaren xehetasunak sortzeko, hautatu **Aurrekontuaren lerroaren xehetasun berria** gainean **Aipatu lerroaren xehetasunak** azpisarea. Sortzeko graduatzaile bizkorra irekiko da. Ondorengo taulan fitxategien eremuei buruzko xehetasunak ematen dira **Aipatu lerroaren xehetasuna** orrialdeak eta balioek funtzionaltasunean duten eragina.

| **Eremua** | **Kokapena** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Deskribapenak | Sorrera bizkorra | Aurreikuspen jakin baten azalpena. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Transakzio-klasea | Sorrera bizkorra | Goitibeherako zerrenda honek aukeran dauden transakzio klaseak eskaintzen ditu **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa.  | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Hautatu produktua | Sorrera bizkorra | Transakzio klasea dagoenean aplikatzen da **Materiala**. Hauta dezakezu aurreikusitako lerro hau **Lehendik dagoen** (katalogoa) produktu edo **Katalogotik kanpoko** produktu batena den. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Produktu | Sorrera bizkorra | Produktuen katalogoko produktuaren IDa. Eremu hau gaituta egoteko, **Lehendik dagoena** hautatu behar duzu **Aukeratu produktua** eremuan. IDa salmenta prezioa eskaintzan jasotako proiektuaren zerrendatik berreskuratzeko erabiltzen da. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Katalogotik kanpoko produktua | Sorrera bizkorra | Produktuaren izena idazteko testu-koadroa. Eremu hau hautatzen duzunean gaituta egongo da **Idatzi** produktuan **Aukeratu produktua** eremua.| Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Funtzioa | Sorrera bizkorra | Lan hori egingo duen edo gastu hori suposatuko duen pertsonaren papera. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Kategoria | Sorrera bizkorra | Lanaren edo gastuaren kategoria. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Hasiera-data | Sorrera bizkorra | Lanaren hasiera-data. | Eremu horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Amaiera-data | Sorrera bizkorra | Lanaren amaiera-data. | Eremu horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Baliabide-unitatea | Sorrera bizkorra | Kostu hori suposatzen duen eta bertan lan egiteko baliabidea eskainiko duen baliabideen unitatea. | Balio honek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak eta kostuaren prezioan erabiltzen da. |
| Unitate-antolaketa | Sorrera bizkorra | Lanaren, produktuaren edo gastuaren unitate taldea. Unitateak unitateen ordutegiari edo unitate talde bati dagozkie. Adibidez, miliak eta kilometroak distantzia deskribatzen duten unitate multzo bateko kide diren unitateak dira. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Unitatea | Sorrera bizkorra | Lanaren, produktuaren edo gastuaren unitatea. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Kantitatea | Sorrera bizkorra | Lanaren, produktuaren edo gastuaren zenbatekoa. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Unitateko prezioa | Sorrera bizkorra |Lana burutzen duen rolaren faktura-tasa, produktuaren unitateko prezioa edo produktuaren edo gastu-kategoriaren salmenta-prezioa. Eremu honek lehenetsitakoa da **Denbora** hasierako datarako eraginkorra den proiektuaren prezioen zerrendako rol prezioen lerroan prezioen dimentsio balioen konbinazioan oinarrituta. **Gastuak** eremuari dagokienez, lehenetsia hasierako datarako eraginkorra den proiektuaren prezioen zerrendako transakzioen kategoriako prezioaren konfiguraziokoa da. Transakzio kategoriako prezioen metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. Produktuetarako, lehenetsitakoa **Prezioen zerrendako elementua** hasiera datarako eraginkorra den proiektuaren prezioen zerrendan.| Lana burutzen duen rolaren kostu-tasa, gastuen kategoriaren kostua unitateko edo produktuaren kostua unitateko. Eremu honek lehenetsitakoa da **Denbora** hasierako datarako eraginkorra den proiektuaren prezioen zerrendako rol prezioen lerroan prezioen dimentsio balioen konbinazioan oinarrituta. **Gastuak** eremuari dagokienez, lehenetsia hasierako datarako eraginkorra den proiektuaren prezioen zerrendako transakzioen kategoriako prezioaren konfiguraziokoa da. Transakzio kategoriako prezioen metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. Produktuetarako, lehenetsitakoa **Prezioen zerrendako elementua** hasiera datarako eraginkorra den proiektuaren prezioen zerrendan.|
| Aurreikusitako zerga | Sorrera bizkorra | Eskuz sar dezakezu lan edo gastu honen zerga. | Ez dago alor honen beherako eraginik. |
| Kopurua | Sorrera bizkorra | Informazioa eskuz sar dezakezu eremu honetan **Kopurua** eta **Prezioa** eremuak hutsik geratzen dira. Eremu horiek hutsik ez badaude, eremu hau irakurtzeko soilik bihurtzen da eta honela kalkulatzen da (Kopurua \* Unitateko prezioa) + Zerga. | Ez dago alor honen beherako eraginik. |


## <a name="update-prices-on-quote-line-details"></a>Eguneratu prezioak aurrekontuaren lerroaren xehetasunetan

Aurrekontuan erantsitako proiektuaren prezioen zerrendan edo kontratazio unitatearen kostuen prezioen zerrendan prezioak aldatu badituzu, hauta dezakezu **Birkalkulatu** gainean **Aurrekontua** orrialdea banakako aurrekontuaren lerroaren xehetasunetan prezioak freskatzeko, aldaketa hori islatzeko. Hautatzen duzunean **Birkalkulatu**, Aurrekontu honetako aurrekontu lerro guztietako prezioak berrezarri egingo direla jakinarazten duen abisua agertzen da. Aukeratu **Bai**, salmenten zein kostuen aurrekontuaren lerroaren xehetasunak freskatzeko.

## <a name="access-quote-line-details-for-cost"></a>Sar ezazu aurrekontuaren lerroaren kostua

**Eskaintzaren lerroaren xehetasunak** fitxa, hautatu lerro bat saretan azpi-sarearen tresna-barran ekintzak gaitzeko. Azpi-sarearen tresna-barran aurreneko aurrekontua lerroaren xehetasuna hautatzen denean lehenengo ekintza da **Ireki kostuaren xehetasuna**. Aukeratu **Ireki kostuaren xehetasuna** aurrekontu lerro honi lotutako kostu tasa eta zenbatekoa ikusteko.

> [!NOTE]
> Aurrekontuaren lerroaren xehetasunean baliabideen hornikuntza-unitatea, kantitatea, datak, rola edo kategoriako balioak aldatzeak salmentetarako aurrekontuaren lerroaren xehetasunetan dagozkien balioak aldatuko ditu.
## <a name="currency-on-quote-line-details-for-cost-and-sales"></a>Aurrekontuaren lineako xehetasunen moneta kostu eta salmentetarako

Aurrekontuaren lerroaren xehetasuneko moneta proiektuaren prezioen zerrendako salmenten lehenespenetarako, aurrekontuaren lerroaren xehetasunaren hasierako datan eraginkorra.

Aurrekontuaren lerroaren kostuen xehetasuneko moneta eskaintzaren kontratatze-unitatearen prezioen zerrendako kostuen lehenespenetarako, aurrekontuaren lerroaren xehetasunaren hasierako datan eraginkorra.

Errentagarritasunaren kalkuluek kostuaren eta salmenten aurrekontuaren lerroaren xehetasunen zenbatekoa inguruneko oinarrizko moneta bihurtzen dute aurrekontuan estimatutako marjina orokorra jakinarazteko.

> [!OHARRA
> > Moneta biribiltzeko akatsak eta aldatutako marjinak gerta litezke data truke-tasa eraginkorrik ez dagoelako. Erabil itzazu kalkulu hauek proiektuen kontratuetan soilik, gutxi gorabeherakoak baitira eta ez baitira legezko biribilketarako edo bestelako biribiltzeetarako zehaztasun handiagoa eskatzen dutenak eta truke-tasen dataren eraginkortasunaz jabetzea.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
