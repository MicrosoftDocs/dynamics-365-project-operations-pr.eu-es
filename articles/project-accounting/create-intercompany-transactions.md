---
title: Sortu enpresen arteko transakzioak
description: Artikulu honetan enpresen arteko transakzioak nola sortu behar den ematen da.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: da6fd8e0e6bfe2e2543f5c4a453ed769e412f1e9
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8919355"
---
# <a name="create-intercompany-transactions"></a>Sortu enpresen arteko transakzioak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Enpresen arteko transakzioak proiektu bateko kontratu bateko denbora eta gastu transakzioak dira, enpresa edo antolakuntza unitate batekoak diren bitartean, proiektuaren kontratuko baliabideak enpresa edo antolakuntza unitate desberdinetakoak diren bitartean.

Enpresen arteko transakzioa onartzen denean, benetako transakzio hauek sortzen dira

| **Transakzio mota** | **Aplikatutako prezio-zerrenda** | **Transakzio-moneta** |
| --- | --- | --- |
| Kostua | Kontratazio unitateko kostuen prezioen zerrenda | Moneta prezioen lerroan |
| Fakturatu gabeko salmentak. Hauek fakturazio mota, denbora eta materialarekin kontratu lerro batekin lotzen diren errealitateetarako bakarrik sortzen dira. | Kontratu-proiektuko salmenten prezio-zerrenda | Kontratuaren dibisa |
| Baliabidearen unitate-kostua | Baliabide-unitateko kostuen prezioen zerrenda | Moneta prezioen lerroan |
| Erakunde arteko unitate-salmentak | Kontratazio unitateko kostuen prezioen zerrenda | Moneta prezioen lerroan |

Kostua, baliabideen unitateko kostua eta erakundeen arteko unitateen salmenten transakzioen prezioa eta moneta dira **antolakuntza unitatea**. Garrantzitsua da hori gogoratzea zure ezarpenean enpresak eta antolakuntza unitateak nola egituratu erabakitzeko orduan.

Aukera, aurrekontua, proiektuaren kontratua eta proiektuaren erregistroak sortzen dituzunean, sistemak egiaztatzen du kontratazio unitatearen moneta kontratatutako enpresaren kontabilitate monetarekin bat datorren. Berdinak ez direnean, ezin dira erregistro hauek sortu. Urtean antolakuntza unitatearen moneta definitzen da Dynamics 365 Project Operations joanez **Dataverse** > **Ezarpenak** > **Antolakuntza-unitateak**. Enpresa bateko kontabilitate-moneta Dynamics 365 Finance-n definitzen da, Ledger setup **Ledger liburu nagusira** > **·** > **joanez**. Moneta zurekin sinkronizatuta dago Dataverse ingurunea Ledgers Dual Write mapa erabiliz.

Sistemak baliabideen unitateko kostua eta erakundeen arteko unitateen salmenten errealitatea sortzen du egoera hauetan:

  - Baliabideen unitatea kontratazio unitatearekin desberdina denean
  - Baliabideen enpresa kontratazio-enpresarekin desberdina denean

Hala ere, enpresa kontratatzailea ez den beste baliabide-enpresa batek dituen transakzioak bakarrik transferituko dira Dynamics 365 Finance ingurunera kontabilitate gehigarri baterako.

Proiektuaren datuen kontabilitatea Project Operations integrazio aldizkarian jasotzen da Finantzan. Sistemak aldizkari lerro hauek sortzen ditu.

| **Transakzio mota** | **Legezko entitatea** | **Proiektuaren transakzioa sortzen du argitaratzean** | **Finantza-dimentsio lehenetsien inprimakia** | **Fakturazio-salmenta lehenetsien gaineko zerga taldea eta fakturazio elementuen salmenten gaineko zerga taldea** |
| --- | --- | --- | --- | --- |
| Kostua | Ez da integrazio aldizkarian gehitzen | E/E | E/E | E/E |
| Fakturatu gabeko salmentak | Pertsona juridikoen integrazio aldizkaria maileguan | Yes | Project | **Fakturazio salmenten gaineko zerga taldea**: **Kontratuko bezeroan** oinarrituta <br/> **Fakturazio elementuen salmenten gaineko zerga taldea**: Aldizkariaren lerroan dagoen pertsona juridikoaren proiektuaren kategoriatik |
| Baliabidearen unitate-kostua | Pertsona juridikoen integrazio aldizkaria maileguan ematea | No | Enpresen arteko bezeroa | **Fakturazio salmenten gaineko zerga taldea**: **Enpresen arteko bezeroan** oinarrituta <br/> **Fakturazio elementuen salmenten gaineko zerga taldea**: Aldizkariaren lerroan dagoen pertsona juridikoaren proiektuaren kategoriatik |
| Erakunde arteko salmentak | Pertsona juridikoen integrazio aldizkaria maileguan ematea | No | Enpresen arteko bezeroa | **Fakturazio salmenten gaineko zerga taldea**: **Enpresen arteko bezeroan** oinarrituta <br/> **Fakturazio elementuen salmenten gaineko zerga taldea**: Aldizkariaren lerroan dagoen pertsona juridikoaren proiektuaren kategoriatik |

### <a name="example-intercompany-transactions"></a>Adibidez: enpresen arteko transakzioak

Molly Clark, GBPMn lan egiten duen garatzaileak 10 orduko lana erregistratzen du USPM Adventure Works proiektu baten aurka, proiektuaren kudeatzaileak onartzen duena. Garatzaileen GBPM kostua orduko 88 GBP da. GBPM-k USPM 120 USD fakturatuko du garatzaileen orduko. USPM-k bezeroari Adventure Works, 200 USD fakturatuko dio GBPM baliabideak egindako lana. Informazio gehiago eskuratzeko, ikusi [Konfiguratu enpresa arteko fakturak](configure-intercompany-invoicing.md).

1. Project Operations atalean, joan hona: **Baliabideak**, eta hautatu **Molly Clark** zerrendatik. **Antolaketa** fitxako **Enpresa** eremuan, hautatu **GBPM**.
2. Joan **Salmentak** > **Bezeroak** aukerara, eta hautatu **Berria** Adventure Works-eko bezeroen erregistro berria sortzeko.
    1. Ezarri enpresa **USPM** gisa.
    2. Ezarri **Harreman mota** **Bezeroa** gisa.
    3. Aukeratu **10. bezero taldea - Etxekoa**.
    4. Ezarri moneta **USD** gisa.
    5. Erregistroa gorde
3. Joan **Salmentak** > **Proiektuen kontratuak** aukerara, eta sortu Adventure Works-en proiektuaren kontratu berria.
    1. Ezarri jabea den enpresa **USPM** eta kontratazio unitatea **Contoso Robotics US**.
    2. Aukeratu Adventure Works bezero gisa.
    3. Aukeratu produktuen prezioen zerrenda eta gorde erregistroa.
    4. **Kontratu-lerroak** fitxan, sortu kontratu lerro berria. Ezarri edozein izen eta hautatu **Denbora eta materialak** fakturazio metodo gisa.
    5. Sortu proiektu berria eta lotu kontratu lerro honekin.
4. Saioa hasi baliabide gisa, **Molly Clark**. Joan **Proiektuak** > **Denbora-sarrerak** aukerak, eta sortu Adventure Works proiektuaren denbora sarrera.
5. Saioa hasi proiektuaren kudeatzaile gisa. Joan **Proiektuak** > **Onarpenak** aukerara, eta onartu Molly Clark-ek erregistratutako denbora sartzeko transakzioa.
6. Joan Adventure Works proiektura eta hautatu **Erlazionatuta** > **Benetakoak**. Egiazko transakzio hauek sortzen dira.

| **Transakzio mota** | **Prezioa** | **Transakzio-moneta** | **Zenbatekoa** |
| --- | --- | --- | --- |
| Kostua | 120 | USD | 1200 |
| Fakturatu gabeko salmentak | 200 | USD | 2000 |
| Baliabidearen unitate-kostua | 88 | GBP | 880 |
| Erakunde arteko unitate-salmentak | 120 | USD | 1200 |

7. Hasi saioa USPM kontulari gisa. Ireki Project Operations-en Finantza instantzia, eta hautatu enpresa **USPM**. 
8. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Project Operations Customer Engagement-en** > **Inportatu eszenaratzetik** eta hautatu aldian aldiko prozesua abiarazteko. Aldian-aldiko prozesu honek Project Operations Integration aldizkaria beteko du.
9. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkariak** > **Project Operations integrazio aldizkaria** eta aldizkari lerroak berrikusi. Sistemak lerro hauek sortzen ditu.

    | **Transakzio mota** | **Prezioa** | **Transakzio-moneta** | **Zenbatekoa** |
    | --- | --- | --- | --- |
    | Fakturatu gabeko salmentak | 200 | USD | 2000 |

    Sistema proiektu honetarako diru-sarrerak lortzeko konfiguratuta badago, honako hau argitaratuko da:

    - Zordunketa: proiektua - WIP salmenten balioa 200 USD
    - Kreditua: proiektua - Metatutako diru-sarrerak 200 USD

    Fakturarik gabeko salmenta hau fakturatzeko prest dago. Adventure Works bezeroaren faktura ekonomikoki bidal daiteke behar denean.

10. Hasi saioa **GBPM** kontulari gisa. Ireki Project Operations-en Finantza instantzia, eta ireki enpresa, **GBPM**. 
11. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Project Operations integrazioa** > **Inportatu taulako taulatik** eta abian jarri aldian aldiko prozesua Project Operations Integration aldizkaria betetzeko.
12. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkariak** > **Project Operations integrazio aldizkaria** eta lerroak berrikusi. Sistemak lerro hau sortzen du.

    | **Transakzio mota** | **Prezioa** | **Transakzio-moneta** | **Zenbatekoa** |
    | --- | --- | --- | --- |
    | Baliabidearen unitate-kostua | 88 | GBP | 880 |
    | Erakunde arteko unitate-salmentak | 120 | USD | 1200 |

    Erregistro horiek argitaratzeak honako bono transakzio hauek eragiten ditu:

    - Zordunketa: proiektuak 88 GBP balio ditu
    - Kreditua: Nominen esleipena 88 GBP

    Sistema proiektu honetarako enpresa arteko diru-sarrerak lortzeko konfiguratuta badago, honako hau argitaratuko da:

    - Zordunketa: proiektua - WIP salmenten balioa 120 USD
    - Kreditua: proiektua - Metatutako diru-sarrerak 120 USD

    Sistema enpresaren bezeroen arteko faktura sortzeko prest dago.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
