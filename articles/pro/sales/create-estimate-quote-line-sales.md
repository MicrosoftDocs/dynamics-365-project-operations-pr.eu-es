---
title: Proiektuetan oinarritutako eskaintzaren lerroa aurreikustea
description: Gai honek proiektuan oinarritutako eskaintzaren lerro baterako aurrekontu bat nola sortu jakiteko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 56892a134c0c739958f7f939214930631dea7420
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180357"
---
# <a name="estimating-a-project-based-quote-line"></a>Proiektuetan oinarritutako eskaintzaren lerroa aurreikustea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuan oinarritutako aurrekontu lerroak aurrekontua lerroa emateko lanaren kostua eta diru sarrera potentzialak kalkulatzen laguntzen duten xehetasunak ditu.

Proiektuan oinarritutako aurrekontu lerroa kalkulatzeko, hautatu proiektuan oinarritutako aurrekontu lerroan **Aipatu lerroaren xehetasuna** fitxa. Proiektuan oinarritutako aurrekontu lerro batean aurrekontua sortzeko bi modu daude:

- Eskuz sortu aurrekontua aurrekontuaren lerroan zuzenean aurrekontuaren lerroaren xehetasunak erabiliz 
- Sortu proiektu bat eta proiektuaren plana, eta, ondoren, lotu proiektua eta proiektuko zereginak aurrekontu lerroarekin. Eman duzun informazioan oinarrituta proiektuaren planeko aurrekontuak aurrekontuaren lerroan inportatzeko prozesua gaituta egongo da.

## <a name="create-estimates-directly-on-a-project-based-quote-line"></a>Sortu aurreikuspenak zunenean proiektuan oinarritutako eskaintzaren lerro batean

Proiektuan oinarritutako aurrekontu lerro batean aurrekontua sortzeko, hautatu **Aipatu lerroaren xehetasuna** fitxa. Fitxa honetan sortzen duzun lerroaldean aurrekontu lerro honetarako aipatutako balioa laburbilduko da. 

Aurrekontuaren lerroaren xehetasunak sortzeko, hautatu **+ Aurrekontuaren lerroaren xehetasun berria** gainean **Aipatu lerroaren xehetasunak** azpisarea. Sortzeko graduatzaile bizkorra irekiko da. **Eskaintzaren lerroa** inprimakiko eremu hauek:

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Deskribapena | Sorrera bizkorra | Aurreikuspen jakin baten azalpena. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Transakzio-klasea | Sorrera bizkorra | Goitibeherako zerrenda honek aukeran dauden transakzio klaseak eskaintzen ditu **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa.  | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Funtzioa | Sorrera bizkorra | Lan hori egingo duen edo gastu hori suposatuko duen pertsona. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Kategoria | Sorrera bizkorra | Lanaren edo gastuaren kategoria. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Hasiera-data | Sorrera bizkorra | Lanaren hasiera-data. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Amaiera-data | Sorrera bizkorra | Lanaren amaiera-data. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Baliabide-unitatea | Sorrera bizkorra | Kostu hori eragingo duen eta bertan lan egiteko baliabidea emango duen baliabideen unitatea. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. Eremu hau kostuen prezioak berreskuratzeko ere erabiltzen da. |
| Unitate-antolaketa | Sorrera bizkorra | Lanaren edo gastuaren unitate taldea. Unitateak unitateen ordutegiari edo unitate talde bati dagozkie. Adibidez, Kilometroak eta KMak distantzia deskribatzen duen unitate multzo bateko kide dira. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Unitatea | Sorrera bizkorra | Lanaren edo gastuaren unitatea. | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Kopurua | Sorrera bizkorra | Lanaren edo gastuaren kopurua | Eremu honek lehenetsitako lerroaren xehetasunen arabera lehenetsitakoa da automatikoki sortzen den kostua. |
| Unitate-prezioa | Sorrera bizkorra | Lana burutzen duen rolaren faktura-tasa edo gastu-kategoriako Salmenta-prezioa. Eremu honek Denbora lehenetsia du hasierako datarako eraginkorra den proiektuaren prezioen zerrendako funtzio eta baliabideen konbinazioan oinarrituta. Gastuei dagokienez, eremu honek hasierako datarako eraginkorra den proiektuaren prezioen zerrendako transakzioen kategoriako prezioa konfiguratzen du lehenespenez. Transakzio-kategoriaren prezio-metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. | Lana burutzen duen rolaren kostu-tasa edo gastu-kategoriaren kostua unitateko. Eremu honek Denbora lehenetsia du hasierako datarako eraginkorra den Eskaintzaren prezioaren Kontratatze-unitatearen prezioen zerrendako funtzio eta baliabideen konbinazioan oinarrituta. Gastuei dagokienez, eremu honek hasierako datarako eraginkorra den Kontratatze-unitatearen kostuaren prezio-zerrendako transakzioen kategoriako prezioa konfiguratzen du lehenespenez. Transakzio-kategoriaren prezio-metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. |
| Aurreikusitako zerga | Sorrera bizkorra | Eskuz sar dezakezu lan edo gastu honen zerga. | Ez dago alor honen beherako eraginik. |
| Kopurua | Sorrera bizkorra | Informazioa eskuz sar dezakezu eremu honetan **Kopurua** eta **Prezioa** eremuak hutsik geratzen dira. Eremu horiek hutsik ez badaude, eremu hau irakurtzeko soilik bihurtzen da eta honela kalkulatzen da (Kopurua \* Unitateko prezioa) + Zerga. | Ez dago alor honen beherako eraginik. |

## <a name="update-prices-on-quote-line-details"></a>Eguneratu prezioak aurrekontuaren lerroaren xehetasunetan

Aurrekontuan erantsitako proiektuaren prezioen zerrendan edo kontratazio unitatearen kostuen prezioen zerrendan prezioak aldatu badituzu, hauta dezakezu **Birkalkulatu** **Aurrekontua** orrialdean, banakako aurrekontuaren lerroaren xehetasunetan prezioak freskatzeko, aldaketa hori islatzeko. Hautatzen duzunean **Birkalkulatu** Aurrekontu lerro guztietako xehetasunen prezioak berrezarriko direla jakinarazten dizun abisua gertatzen da. Aukeratu **Bai**, salmenten zein kostuen aurrekontuaren lerroaren xehetasunak freskatzeko.

## <a name="access-quote-line-details-for-cost"></a>Sar ezazu aurrekontuaren lerroaren kostua

**Eskaintzaren lerroaren xehetasunak** fitxa, hautatu lerro bat saretan azpi-sarearen tresna-barran ekintzak gaitzeko. Azpi-sarearen tresna-barran aurreneko aurrekontua lerroaren xehetasuna hautatzen denean lehenengo ekintza da **Ireki kostuaren xehetasuna**. Aukeratu **Ireki kostuaren xehetasuna** aurrekontu lerro honi lotutako kostu tasa eta zenbatekoa ikusteko.

> [!NOTE]
> Aurrekontuaren lerroaren xehetasunean baliabideen hornikuntza-unitatea, kantitatea, datak, rola edo kategoriako balioak aldatzeak salmentetarako aurrekontuaren lerroaren xehetasunetan dagozkien balioak aldatuko ditu.
## <a name="currency-on-quote-line-details-for-cost-and-sales"></a>Aurrekontuaren lineako xehetasunen moneta kostu eta salmentetarako

Aurrekontuaren lerroaren xehetasuneko moneta proiektuaren prezioen zerrendako salmenten lehenespenetarako, aurrekontuaren lerroaren xehetasunaren hasierako datan eraginkorra.

Aurrekontuaren lerroaren kostuen xehetasuneko moneta eskaintzaren kontratatze-unitatearen prezioen zerrendako kostuen lehenespenetarako, aurrekontuaren lerroaren xehetasunaren hasierako datan eraginkorra.

Errentagarritasunaren kalkuluek kostuaren eta salmenten aurrekontuaren lerroaren xehetasunen zenbatekoa inguruneko oinarrizko moneta bihurtzen dute aurrekontuan estimatutako marjina orokorra jakinarazteko.

Horrek moneta biribiltzeko akatsak eta marjinak aldatzea eragin lezake, data truke-tasa eraginkorrak ez daudelako. Erabili kalkulu hauek Proiektuaren aurrekontuetan, gutxi gorabehera, gutxi gorabehera eta ez legezko txostenak edo bestelako txostenak behar dituztenak, biribiltzeko zehaztasun handiagoa eta truke-tasen dataren eraginkortasuna ezagutzea.
