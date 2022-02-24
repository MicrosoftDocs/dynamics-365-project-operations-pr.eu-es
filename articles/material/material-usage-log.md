---
title: Erregistratu proiektuetako eta proiektu-zereginetako material-erabilera
description: Gai honek materialaren erabilera proiektuekin eta proiektuen zereginekin nola erregistratu buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 03/31/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ab431ce4c18a4283cd887de9afcba0dd556d2567
ms.sourcegitcommit: b4a05c7d5512d60abdb0d05bedd390e288e8adc9
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/02/2021
ms.locfileid: "5852826"
---
# <a name="record-material-usage-on-projects-and-project-tasks"></a>Erregistratu proiektuetako eta proiektu-zereginetako material-erabilera

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako Project Operations, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektu taldeak proiektu bateko zereginen bidez lan egiten duenez, materialak kontsumitzen edo erabiltzen dituzte. Materialaren erabilera erregistroak erabilera hori erregistratzeko modua eskaintzen du, proiektuaren kudeatzaileak onartu eta azkenean bezeroari faktura diezaion. 

Katalogoko edo idazteko materialen erabilera erregistratzeko eta homologatzaileari bidaltzeko, jarraitu urrats hauek: 

1. Nabigazio panelean, hautatu **Materialaren erabilera** eta, ondoren, hautatu **Berria**.
2. **Materialen erabilera berria** orrialdean, sartu beharrezko materialaren erabilera informazioa eta hautatu **Gorde**.

Ondorengo taulan fitxategien eremuei buruzko informazioa ematen da **Materialaren erabilera erregistroa** orrialdea. 

| **Eremua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- |
| Deskribapenak | Materialaren erabilera zehatzaren deskribapena. | Ez dago alor honen beherako eraginik. |
| Data | Materiala noiz erabiliko den aurreikusten da. | Ez dago alor honen beherako eraginik. |
| Project | Aktibo dauden proiektuen zerrenda. | Materialaren erabilera erregistroaren proiektu bat hautatzeak eragina du **Egitekoa** eremuan proiektuan dauden zereginak bakarrik erakusteko. |
| Ataza | Proiektuaren zereginen zerrenda laburpen eta hosto nodo zereginak barne. | Materialaren erabilera egunkari baterako ataza hautatzeak materialaren benetako kostuan eta zeregin baten benetako material salmentetan eragina du. Eremu hau hutsik badago, dagokion materialaren erabileraren kostua eta salmentak proiektuaren mailan jarraipena eta laburpena egiten dira. |
| Hautatu produktua | Zehaztu material erabilera hau **Lehendik dagoena** (katalogoa) produktua edo **Idatzi** produktua. | Eremu honek produktu mota zehazten du. |
| Produktu | Produktuen katalogoko produktuaren IDa. Produktuaren IDa hautatzen duzunean, **Aukeratu produktua** eremua automatikoki eguneratzen da **Lehendik dagoen produktua**. IDa prezioen zerrendatik kostuak eta salmenta prezioak berreskuratzeko erabiltzen da. | Ez dago alor honen beherako eraginik. |
| Katalogotik kanpoko produktuaren deskribapena | Produktuaren izena idazteko testu eremua. Eremu hau hautatzen duzunean erabilgarri dago **Idatzi** produktuan **Aukeratu produktua** eremua.| Ez dago alor honen beherako eraginik. |
| Baliabide erreserbagarria| Material hau proiektuan erabili duen baliabidea. Eremu honen lehenetsia saioa hasita duen erabiltzailearen baliabide erreserbagarria da, baina proiektuaren taldeko beste kideen izenean erabilera erregistratzeko alda daiteke. | Ez dago alor honen beherako eraginik. |
| Salmenta-unitatea | Eremu honetako balio lehenetsia katalogoko produktuan lehenetsitako konfiguratutako unitate taldetik dator. Eremu hau egunera dezakezu beste unitate talde bat hautatzeko. | Ez dago alor honen beherako eraginik. |
| Unitatea | Eremu honetako balio lehenetsia hautatutako produktuaren unitate lehenetsia da. Eremu hau egunera dezakezu beste unitate bat hautatzeko. | Unitatea aldatzeak unitateko prezio eta kostu lehenetsi desberdinak lortzen ditu. |
| Kantitatea | Proiektuan edo zereginean erabili den produktuaren kantitatea. | Ez dago alor honen beherako eraginik. |
| Unitatearen kostua | Aukeratutako produktuaren eta unitate konbinazioaren kostu unitarioa aplikagarri den kostuen prezioen zerrendan ezarritako moduan. | Unitatearen kostua proiektuaren kostuaren monetan agertzen da beti. Prezio zerrendan produktu konbinatuaren eta unitatearen kostu unitarioik ez badago, kostu unitarioa 0,00 izango da lehenetsita. |
| Kostua guztira | Kopuru gisa kalkulatzen den kostuaren zenbatekoa \* unitateko kostua.| Kostuaren zenbatekoa proiektuaren kostuaren monetan agertzen da beti. |


## <a name="submit-material-usage-for-review-and-approval"></a>Bidali materialaren erabilera berrikusteko eta onartzeko 
Zure materialaren erabilera guztia harrapatu ondoren eta onartua izateko prest zaudenean, erabileraren informazioa bidali behar duzu berrikusteko.

1. Joan **Materialaren erabilera erregistroa** eta hautatu sarrera bat edo gehiago. Edo hautatu materialaren erabilera erregistro guztiak goiburuko kontrol-laukia erabiliz.
2. Hautatu **Bidali**. Sistemak hautatutako sarrerak prozesatzen ditu eta gero materialaren erabilera onartzeko eskaerak sortzen ditu.

## <a name="recall-a-material-usage-log"></a>Berreskuratu material-erabileraren erregistroa

Beharrezkoa denean, bidalitako materialaren erabilera gogora dezakezu. Materialaren erabilera sarrera gogoratzeko behar den denbora onarpen fasearen araberakoa da.  Onartzaileak oraindik sarrera onartu ez badu, gogora ekartzea berehala gerta daiteke. Hala ere, sarrera dagoeneko onartuta badago, onartzaileari berreskurapena onartzea eta transakzioak atzeratzea eskatzen zaio.

1. Joan **Materialaren erabilera**, eta materialaren erabilera erregistroen zerrendan, hautatu gogora ekarri nahi duzun materialaren erabilera.
2. Hautatu **Berreskuratu**. Materialaren erabilera sarrera oraindik onartu ez bada, sistemak berehala gogorarazten du. Material sarrera dagoeneko onartuta badago, berreskuratzeko eskaera bat sortuko da onartzaileari materialaren erabilera gogora ekarri nahi duzula jakinarazteko. Onartzaileak gero atzerapena egin daitekeela baieztatuko du eta sarrera itzuliko da.

## <a name="delete-a-material-usage-log"></a>Ezabatu material-erabileraren erregistroa

Bidali ez diren materialen erabilera erregistroak ezaba ditzakezu. Jadanik bidalitako materialaren erabilera erregistroa ezabatzeko, lehenik eta behin gogoratu behar duzu.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
