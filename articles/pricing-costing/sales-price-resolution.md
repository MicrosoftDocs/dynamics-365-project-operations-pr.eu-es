---
title: Erabaki proiektuetan oinarritutako aurreikuspenen eta benetako datuen salmenta-prezioak
description: Artikulu honek proiektuaren kalkulu eta salmenten prezioetan oinarritutako kostu-tasak zehazteari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 09/12/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: f0b95c651983230cbf340f2c06089a287b2c8a10
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475354"
---
#  <a name="determine-sales-prices-for-project-based-estimates-and-actuals"></a>Erabaki proiektuetan oinarritutako aurreikuspenen eta benetako datuen salmenta-prezioak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Salmenten prezioak kalkuluetan eta benetako datuetan zehazteko Microsoft Dynamics 365 Project Operations-en, sistemak sarrerako kalkuluaren edo benetako datuen testuinguruaren data eta moneta erabiltzen ditu salmenta prezioen zerrenda konpontzeko. Benetako testuinguruan zehazki, sistemak erabiltzen du **Transakzio data** eremua zein prezio-zerrenda aplikagarria den zehazteko. Sarrerako estimazioaren edo benetakoaren **Transakzio data** balioa prezio-zerrendako **Hasiera eraginkorra (Ordu-eremuaren independentea)** eta **Amaiera eraginkorra (Ordu-eremuaren independentea)** balioarekin alderatzen da. Salmenta prezioen zerrenda zehaztu ondoren, sistemak salmenten edo fakturen tasa zehazten du.

## <a name="determining-sales-rates-on-actual-and-estimate-lines-for-time"></a>Zehaztu benetako salmenten tasak eta denborarako kalkulatutako lerroak

**Denbora** elementuaren testuinguru estimatuak aipatzen du:

- **Denboraren** eskaintzaren lerroen xehetasunak.
- **Denboraren** kontratu-lerroen xehetasunak.
- Proiektuan baliabideak esleitzea.

**Denbora** elementuaren benetako datuen testuingurua aipatzen du:

- Sarrera eta Zuzenketa egunkari-lerroak **Denbora** elementurako.
- Denbora-sarrera bat bidaltzean sortzen diren egunkari-lerroak.
- **Denboraren** faktura-lerroen xehetasunak. 

Salmenten prezio zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu faktura tasa lehenetsia sartzeko.

1. Sistemak **funtzioa**, **baliabideen enpresa** eta **baliabideen unitatea** eremuak erabiltzen ditu **denbora** elementuaren testuinguru estimatuan edo benetako datuetan prezio-zerrendako funtzioen prezio-lerroetan. Partida honek suposatzen du kutxaz kanpoko prezioen neurriak erabiltzen dituzula fakturazio-tasetarako. Prezioak beste edozein eremutan oinarrituta konfiguratu badituzu edo ez horren ordez **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea**, orduan hori da bat datorren rolaren prezio lerroa berreskuratzeko erabiliko den konbinazioa.
1. Sistemak fakturazio tasa duen rola prezio lerro bat aurkitzen badu **Rola**, **Baliabideen enpresa** eta **Baliabideen uitatea** eremuen konbinazioa, faktura tasa lehenetsita dago.

> [!NOTE]
> Lehenespen desberdina konfiguratu baduzu **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea**, edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, portaera horren arabera aldatuko da. Sistemak lehentasun-ordenaren arabera prezio-dimentsio-balio bakoitzarekin bat datozen balioak dituzten rol-prezioaren erregistroak berreskuratzen ditu. Dimentsio horietarako balio nuluak dituzten errenkadak azkenak dira.

## <a name="determining-sales-rates-on-actual-and-estimate-lines-for-expense"></a>Zehaztu benetako salmenten tasak eta gastuetarako kalkulatutako lerroak

**Gastua** elementuaren testuinguru estimatuak aipatzen du:

- **Gastua** eskaintzaren lerroen xehetasunak.
- **Gastua** kontratu-lerroen xehetasunak.
- Proiektuaren gastu-lerroen aurreikuspenak.

**Gastua** elementuaren benetako testuingurua aipatzen du:

- Sarrera eta Zuzenketa egunkari-lerroak **Gastua** elementurako.
- Gastu-sarrera bat bidaltzean sortzen diren egunkari-lerroak.
- **Gastua** faktura-lerroen xehetasunak. 

Salmenten prezio zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu unitateen salmenta-prezioa lehenetsia sartzeko.

1. Sistemak **Kategoria** eta **Unitateak** eremuen konbinazioa erabiltzen du kategoriaren prezio-lerroekin bat datorren **gastua** kalkulatzeko ebatzitako prezio-zerrendan.
1. Sistemak salmenta-tasa duen kategoriako prezio lerro bat aurkitzen badu **Kategoria** eta **Unitatea** eremuen konbinazioa, salmenta-tasa lehenetsita dago.
1. Sistemak bat datorren kategoriako prezio lerroa aurkitzen badu, prezioen metodoa erabil daiteke salmenta prezioa lehenesteko. Beheko taulan, Project Operations-en gastuen prezioen betebeharrak agertzen dira.

    | Testuingurua | Prezio-metodoa | Prezio lehenetsia |
    | --- | --- | --- |
    | Aurreikuspena | Prezioa unitate bakoitzeko | Kategoriaren prezio lerroan oinarrituta. |
    |        | Kostuan | 0.00 |
    |        | Markaketa kostuaren gainetik | 0.00 |
    | Unekoa" | Prezioa unitate bakoitzeko | Kategoriaren prezio lerroan oinarrituta. |
    |        | Kostuan | Lotutako kostu errealean oinarrituta. |
    |        | Markaketa kostuaren gainetik | Aplikatutakoan kategoria prezioen lerroak lotutako kostu errealaren unitateko kostuaren tasan markatutako marka. |

1. Sistema ezin bada **Kategoria** eta **Unitatea** balioak, salmenta-tasa **0** (zero) gisa ezartzen da lehenespenez.

## <a name="determining-sales-rates-on-actual-and-estimate-lines-for-material"></a>Materialen salmenta-tasak zehaztea eta materialaren estimazio lerroak

**Materiala** elementuaren testuinguru estimatuak aipatzen du:

- **Materiala** eskaintzaren lerroen xehetasunak.
- **Materiala** kontratu-lerroen xehetasunak.
- Materialaren aurreikuspen-lerroak proiektuan.

**Materiala** elementuaren benetako testuingurua aipatzen du:

- Sarrera eta Zuzenketa egunkari-lerroak **Materiala** elementurako.
- Material-erabileraren erregistro bat bidaltzean sortzen diren egunkari-lerroak.
- **Materiala** faktura-lerroen xehetasunak. 

Salmenten prezio zerrenda zehaztu ondoren, sistemak urrats hauek betetzen ditu unitateen salmenta-prezioa lehenetsia sartzeko.

1. Sistemak **Produktua** eta **Unitatea** **Material** konbinazioa kalkulatutako lerroan ebatzi zen prezio zerrendako elementuen lerroekin bat etortzeko.
1. Sistemak salmenta tasa duen prezioen zerrendako elementu lerro bat aurkitzen badu **Produktua** eta **Unitatea** eremuen konbinazioa eta prezioen metodoa da **Moneta zenbatekoa**, prezioen zerrendan zehaztutako salmenta-prezioa erabiltzen da. 
1. Bada **Produktua** eta **Unitatea** eremuen balioak ez datoz bat, edo prezioen metodoa beste zerbait bada **Dibisaren zenbatekoa**, salmenta-tasa ezarrita dago **0** (zero) lehenespenez. Portaera hau Project Operations-ek soilik onartzen duelako gertatzen da **Monetaren zenbatekoa** proiektu batean erabiltzen diren materialen prezioen metodoa.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
