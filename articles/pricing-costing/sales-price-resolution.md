---
title: Ebatzi aurreikuspenen eta benetako datuen salmentak
description: Gai honek salmenten tasak ebazteko moduari eta estimazioei buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/07/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b78d0f970f942513ecb6911d64fcffa629567f93f1a763eef20ca168080e4d02
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986251"
---
# <a name="resolve-sales-prices-for-estimates-and-actuals"></a>Ebatzi aurreikuspenen eta benetako datuen salmentak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Aurrekontuen eta benetako salmenten prezioak urtean ebazten direnean Dynamics 365 Project Operations-en, sistemak lehenengo proiektuaren edo kontratuaren data eta moneta erabiltzen ditu salmenta prezioen zerrenda konpontzeko. Salmenta prezioen zerrenda ebatzi ondoren, sistemak salmenten edo fakturen tasa ebazten du.

## <a name="resolve-sales-rates-on-actual-and-estimate-lines-for-time"></a>Ebatzi benetako salmenten tasak eta denborarako kalkulatutako lerroak

Project Operations-en, denbora kalkulatzeko lerroak erabiltzen dira aurrekontuaren lerroa eta kontratuaren lerroaren xehetasunak eta proiektuaren baliabideen esleipenak adierazteko.

Salmenten prezio zerrenda ebatzi ondoren, sistemak urrats hauek betetzen ditu faktura tasa lehenesteko.

1. Sistemak **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea** denbora kalkulatzeko lerroaren eremuak, ebatzitako prezio zerrendako rol prezioen lerroekin bat etortzeko. Partida honek suposatzen du kutxaz kanpoko prezioen neurriak erabiltzen dituzula fakturazio-tasetarako. Prezioak beste edozein eremutan oinarrituta konfiguratu badituzu edo ez horren ordez **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea**, orduan hori da bat datorren rolaren prezio lerroa berreskuratzeko erabiliko den konbinazioa.
2. Sistemak fakturazio tasa duen rola prezio lerro bat aurkitzen badu **Rola**, **Baliabideen enpresa** eta **Baliabideen uitatea** eremuen konbinazioa, faktura tasa lehenetsita dago.
3. Sistema ezin bada **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea** eremuko balioak, ondoren, rolen prezioen lerroak berreskuratzen ditu bat datozen rolekin baina balio baliogabeak **Baliabideen unitatea**. Sistemak bat datorren rolaren prezioen erregistroa aurkitu ondoren, faktura-tasa lehenetsiko du erregistro horretatik. Bat etortze honek kutxaz kanpoko konfigurazioa suposatzen du **Rola** vs **Baliabideen Unitatea** salmenten prezioen dimentsio gisa.

> [!NOTE]
> -Ren lehenespen desberdina konfiguratu baduzu **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea**, edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, portaera horren arabera aldatuko da. Sistemak rolen prezioen erregistroak berreskuratzen ditu prezioen dimentsioen balio bakoitzarekin bat datozen balioekin lehentasunen arabera ordenatuta azken dimentsioetarako balio baliorik gabeko errenkadekin.

## <a name="resolve-sales-rates-on-actual-and-estimate-lines-for-expense"></a>Ebatzi benetako salmenten tasak eta gastuetarako kalkulatutako lerroak

Project Operations-en, gastua kalkulatzeko lerroak erabiltzen dira kontratuaren lerroa eta kontratuaren gastuak baliabideen esleipenak adierazteko.

Salmenten prezio zerrenda ebatzi ondoren, sistemak urrats hauek betetzen ditu unitateen salmenta-prezioa lehenesteko.

1. Sistemak **Kategoria** eta **Unitatea** eremuen konbinazioa erabiltzen du kategoriaren prezio-lerroekin bat datorren gastua kalkulatzeko ebatzitako prezio-zerrendan.
2. Sistemak salmenta-tasa duen kategoriako prezio lerro bat aurkitzen badu **Kategoria** eta **Unitatea** eremuen konbinazioa, salmenta-tasa lehenetsita dago.
3. Sistemak bat datorren kategoriako prezio lerroa aurkitzen badu, prezioen metodoa erabil daiteke salmenta prezioa lehenesteko. Beheko taulan, proiektuaren eragiketetan gastuen prezioen betebeharrak agertzen dira.

    | Testuingurua | Prezio-metodoa | Prezio lehenetsia |
    | --- | --- | --- |
    | Aurreikuspena | Prezioa unitate bakoitzeko | Kategoriaren prezio lerroan oinarrituta |
    | &nbsp; | Kostuan | 0.00 |
    | &nbsp; | Markaketa kostuaren gainetik | 0.00 |
    | Unekoa" | Prezioa unitate bakoitzeko | Kategoriaren prezio lerroan oinarrituta |
    | &nbsp; | Kostuan | Lotutako kostu errealean oinarrituta |
    | &nbsp; | Markaketa kostuaren gainetik | Kategoria prezioen lerroak lotutako kostu errealaren unitateko kostuaren tasan markatutako marka aplikatuz |

4. Sistema ezin bada **Kategoria** eta **Unitatea** eremuko balioak, salmenten tasa zero (0) lehenetsita dago.

## <a name="resolve-sales-rates-on-actual-and-estimate-lines-for-material"></a>Ebatzi materialen salmenta-tasak eta materialaren estimazio lerroak

Project Operations-en, materialaren zenbatespen lerroak erabiltzen dira materialen eskaintzaren lerroaren eta kontratuaren lerroaren xehetasunak eta proiektu bateko materialen estimazio lerroak aipatzen dituzte.

Salmenten prezio zerrenda ebatzi ondoren, sistemak urrats hauek betetzen ditu unitateen salmenta-prezioa lehenesteko.

1. Sistemak **Produktua** eta **Unitatea** material konbinazioa kalkulatutako lerroan ebatzi zen prezio zerrendako elementuen lerroekin bat etortzeko.
2. Sistemak salmenta tasa duen prezioen zerrendako elementu lerro bat aurkitzen badu **Produktua** eta **Unitatea** eremuen konbinazioa eta prezioen metodoa da **Moneta zenbatekoa**, prezioen zerrendan zehaztutako salmenta-prezioa erabiltzen da.
3. **Produktua** eta **Unitatea** eremuen balioak bat ez badatoz, salmenta-tasa zero da lehenetsita.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
