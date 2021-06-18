---
title: Aurreikusi proiektuko eskaintzaren lerroa
description: Gai honek proiektuaren aurrekontu lerro batean aurrekontua nola sortu jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: adb5a7f113b15abd2fe7364fa9b592d2c02db389
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000691"
---
# <a name="estimate-a-project-quote-line"></a>Aurreikusi proiektuko eskaintzaren lerroa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuan oinarritutako aurrekontu lerroak aurrekontua lerroa emateko lanaren kostua eta diru sarrera potentzialak kalkulatzen laguntzen duten xehetasunak ditu.

Proiektuan oinarritutako aurrekontu lerro bat kalkulatzeko, aurrekontu lerroan, hautatu **Aipatu lerroaren xehetasuna** fitxa. Proiektuan oinarritutako aurrekontu lerro batean aurrekontua sortzeko bi modu daude:

   - Eskuz sortu aurrekontua aurrekontuaren lerroan zuzenean aurrekontuaren lerroaren xehetasunak erabiliz. 
   - Sortu proiektu bat eta proiektuaren plana, eta, ondoren, lotu proiektua eta proiektuko zereginak aurrekontu lerroarekin. Eman duzun informazioan oinarrituta proiektuaren planeko aurrekontuak aurrekontuaren lerroan inportatzeko prozesua gaituta egongo da.

## <a name="create-estimates-directly-on-a-project-based-quote-line"></a>Sortu aurreikuspenak zunenean proiektuan oinarritutako eskaintzaren lerro batean

Proiektuan oinarritutako eskaintza lerroan zenbatespena zuzenean sortzeko, jarraitu urrats hauei:

1. Proiektuan oinarritutako aurrekontu lerro batean aurrekontua sortzeko, hautatu **Aipatu lerroaren xehetasuna** fitxa. Fitxa honetan sortzen duzun lerroaldean aurrekontu lerro honetarako aipatutako balioa laburbilduko da. 
2. Aurrekontuaren lerroaren xehetasunak sortzeko, hautatu **Aurrekontuaren lerroaren xehetasun berria** gainean **Aipatu lerroaren xehetasunak** azpisarea. Sortzeko graduatzaile bizkorra irekiko da. Hurrengo eremuak **Aipatu lerroa** orrialdea.

| **Eremua** | **Kokapena** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Deskribapenak | Sorrera bizkorra | Aurreikuspen jakin baten azalpena. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Transakzio-klasea | Sorrera bizkorra | Goitibeherako zerrenda honek aukeran dauden transakzio klaseak eskaintzen ditu **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxa.  | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Hautatu produktua | Sorrera bizkorra | Transakzio klasea dagoenean aplikatzen da **Materiala**. Hauta dezakezu aurreikusitako lerro hau **Lehendik dagoen** (katalogoa) produktu edo **Katalogotik kanpoko** produktu batena den. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Produktu | Sorrera bizkorra | Produktuen katalogoko produktuaren IDa. Eremu hau gaituta egoteko, **Lehendik dagoena** hautatu behar duzu **Aukeratu produktua** eremuan. IDa salmenta prezioa eskaintzan jasotako proiektuaren zerrendatik berreskuratzeko erabiltzen da. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Katalogotik kanpoko produktua | Sorrera bizkorra | Produktuaren izenean idazteko testu-koadroa. Eremu hau hautatzen duzunean gaituta egongo da **Idatzi** produktuan **Aukeratu produktua** eremua.| Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Funtzioa | Sorrera bizkorra | Lan hori egingo duen edo gastu hori suposatuko duen pertsonaren papera. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Kategoria | Sorrera bizkorra | Lanaren edo gastuaren kategoria. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Hasiera-data | Sorrera bizkorra | Lanaren hasiera-data. | Eremu horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Amaiera-data | Sorrera bizkorra | Lanaren amaiera-data. | Eremu horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Baliabideen enpresa | Sorrera bizkorra | Kostu hori suposatzen duen eta bertan lan egiteko baliabidea eskaintzen duen baliabideen enpresa edo legezko unitatea. | Balioak lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak eta kostuaren prezioan erabiltzen da. |
| Baliabide-unitatea | Sorrera bizkorra | Kostu hori suposatzen duen eta bertan lan egiteko baliabidea eskaintzen duen baliabideen unitatea. | Balio honek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak eta kostuaren prezioan erabiltzen da. |
| Unitate-antolaketa | Sorrera bizkorra | Lanaren, produktuaren edo gastuaren unitate taldea. Unitateak unitateen ordutegiari edo unitate talde bati dagozkie. Adibidez, miliak eta kilometroak distantzia deskribatzen duten unitate multzo bateko kide diren unitateak dira. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Unitatea | Sorrera bizkorra | Lanaren, produktuaren edo gastuaren unitatea. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Kantitatea | Sorrera bizkorra | Lanaren, produktuaren edo gastuaren zenbatekoa. | Balio horrek lehenetsitako lotura duen eskaintzaren lerroaren xehetasunak lehenetsitakoak dira automatikoki sortzen diren kostuak. |
| Unitateko prezioa | Sorrera bizkorra |Lana burutzen duen rolaren faktura-tasa, produktuaren unitateko prezioa edo produktuaren edo gastu-kategoriaren salmenta-prezioa. Lehenetsitakoa da **Denbora** hasierako datarako eraginkorra den proiektuaren prezioen zerrendako rol prezioen lerroan prezioen dimentsio balioen konbinazioan oinarrituta. **Gastuak** eremuari dagokienez, lehenetsia hasierako datarako eraginkorra den proiektuaren prezioen zerrendako transakzioen kategoriako prezioaren konfiguraziokoa da. Transakzio-kategoriaren prezio-metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. Produktuetarako, eremu honen lehenetsia **Prezioen zerrendako elementua** hasiera datarako eraginkorra den proiektuaren prezioen zerrendan.| Lana burutzen duen rolaren kostu-tasa, gastuen kategoriaren kostua unitateko edo produktuaren kostua unitateko. Lehenetsitakoa da **Denbora** hasierako datarako eraginkorra den kontratu-unitateari atxikiko kostuaren prezio-zerrendako rol prezioen lerroan prezioen dimentsio balioen konbinazioan oinarrituta. Gastuetarako, eremu honen lehenetsia kategoria-prezioaren zerrendako elementua hasiera datarako eraginkorra den kontratu-unitateari atxikitako kostuaren prezio-zerrendan. Transakzio kategoriako prezioen metodoa unitateko prezioa ez bada, ez dago lehenespenik eta eremu hau hutsik geratuko da. Produktuetarako, eremu honen lehenetsia **Prezioen zerrendako elementua** hasiera datarako eraginkorra den kontratu-unitateari atxikitako kostuaren prezio-zerrendan.|
| Aurreikusitako zerga | Sorrera bizkorra | Eskuz sar dezakezu lan edo gastu honen zerga. | Ez dago alor honen beherako eraginik. |
| Kopurua | Sorrera bizkorra | Informazioa eskuz sar dezakezu eremu honetan **Kopurua** eta **Prezioa** eremuak hutsik geratzen dira. Eremu horiek hutsik ez badaude, eremu hau irakurtzeko soilik bihurtzen da eta honela kalkulatzen da (Kopurua \* Unitateko prezioa) + Zerga. | Ez dago alor honen beherako eraginik. |

## <a name="update-prices-on-quote-line-details"></a>Eguneratu prezioak aurrekontuaren lerroaren xehetasunetan

Aurrekontuan erantsitako proiektuaren prezioen zerrendan edo kontratazio unitatearen kostuen prezioen zerrendan prezioak aldatu badituzu, hauta dezakezu **Birkalkulatu** **Aurrekontua** orrialdean, banakako aurrekontuaren lerroaren xehetasunetan prezioak freskatzeko, aldaketa hori islatzeko. Hautatzen duzunean **Birkalkulatu**, Aurrekontu honetako aurrekontu lerro guztietako prezioak berrezarri egingo direla jakinarazten duen abisua agertzen da. Aukeratu **Bai**, salmenten zein kostuen aurrekontuaren lerroaren xehetasunak freskatzeko.

## <a name="access-quote-line-details-for-cost"></a>Sar ezazu aurrekontuaren lerroaren kostua

Aurrekontuaren lerroaren xehetasunak kostuetarako sartzeko, jarraitu urrats hauei:

1. **Aipatu lerroaren xehetasunak** fitxa, hautatu sarean errenkada bat azpisareko tresna-barran ekintzak gaitzeko. 
2. Aukeratu **Ireki kostuaren xehetasuna** aurrekontu lerro honi lotutako kostu tasa eta zenbatekoa ikusteko.

> [!NOTE]
> Aurrekontuaren lerroaren xehetasunean baliabideen hornikuntza-unitatea, kantitatea, datak, rola edo kategoriako balioak aldatzeak salmentetarako aurrekontuaren lerroaren xehetasunetan dagozkien balioak aldatuko ditu.

## <a name="currency-on-quote-line-details-for-cost-and-sales"></a>Aurrekontuaren lineako xehetasunen moneta kostu eta salmentetarako

Aurrekontuaren lerroaren xehetasuneko moneta proiektuaren prezioen zerrendako salmenten lehenespenetarako, aurrekontuaren lerroaren xehetasunaren hasierako datan eraginkorra dena.

Aurrekontuaren lerroaren xehetasuneko moneta proiektuaren prezioen zerrendako kostuen lehenespenetarako, aurrekontuaren kontratu-unitatearen lerroaren xehetasunaren hasierako datan eraginkorra dena.

> [!NOTE]
> Errentagarritasunaren kalkuluek kostuaren eta salmenten aurrekontuaren lerroaren xehetasunen zenbatekoa inguruneko oinarrizko moneta bihurtzen dute aurrekontuan estimatutako marjina orokorra jakinarazteko. Moneta biribiltzeko akatsak eta aldatutako marjinak gerta litezke data truke-tasa eraginkorrik ez dagoelako. Erabil itzazu kalkulu hauek proiektuen eskaintzetan soilik, gutxi gorabeherakoak baitira eta ez baitira legezko biribilketarako edo bestelako biribiltzeetarako zehaztasun handiagoa eskatzen dutenak eta truke-tasen dataren eraginkortasunaz jabetzea.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
