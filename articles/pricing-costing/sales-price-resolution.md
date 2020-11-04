---
title: Ebatzi aurreikuspenen eta benetako datuen salmentak
description: Gai honek salmenten tasak ebazteko moduari eta estimazioei buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b4ae5b3c4a4378330caed97011f55ca11175e644
ms.sourcegitcommit: f8edff6422b82fdf2cea897faa6abb51e2c0c3c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/21/2020
ms.locfileid: "4087798"
---
# <a name="resolve-sales-prices-for-estimates-and-actuals"></a>Ebatzi aurreikuspenen eta benetako datuen salmentak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Estimazioen eta benetako salmenten prezioak Dynamics 365 Project Operations-en ebazten direnean, sistemak lehenik eta behin lotutako proiektuaren aurrekontuaren edo kontratuaren data eta moneta erabiltzen ditu salmenta prezioen zerrenda konpontzeko. Salmenta prezioen zerrenda ebatzi ondoren, sistemak salmenten edo fakturen tasa ebazten du.

## <a name="resolve-sales-rates-on-actual-and-estimate-lines-for-time"></a>Ebatzi benetako salmenten tasak eta denborarako kalkulatutako lerroak

Project Operations-en, denbora kalkulatzeko lerroak erabiltzen dira aurrekontuaren lerroa eta kontratuaren lerroaren xehetasunak eta proiektuaren baliabideen esleipenak adierazteko.

Salmenten prezio zerrenda ebatzi ondoren, sistemak urrats hauek betetzen ditu faktura tasa lehenesteko.

1. Sistemak **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** denbora kalkulatzeko lerroaren eremuak, ebatzitako prezio zerrendako rol prezioen lerroekin bat etortzeko. Partida honek suposatzen du kutxaz kanpoko prezioen neurriak erabiltzen dituzula fakturazio-tasetarako. Prezioak beste edozein eremutan oinarrituta konfiguratu badituzu edo ez horren ordez **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** , orduan hori da bat datorren rolaren prezio lerroa berreskuratzeko erabiliko den konbinazioa.
2. Sistemak fakturazio tasa duen rola prezio lerro bat aurkitzen badu **Rola** , **Baliabideen enpresa** eta **Baliabideen uitatea** eremuen konbinazioa, faktura tasa lehenetsita dago.
3. Sistema ezin bada **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** eremuko balioak, ondoren, rolen prezioen lerroak berreskuratzen ditu bat datozen rolekin baina balio baliogabeak **Baliabideen unitatea**. Sistemak bat datorren rolaren prezioen erregistroa aurkitu ondoren, faktura-tasa lehenetsiko du erregistro horretatik. Bat etortze honek kutxaz kanpoko konfigurazioa suposatzen du **Rola** vs **Baliabideen Unitatea** salmenten prezioen dimentsio gisa.

> [!NOTE]
> -Ren lehenespen desberdina konfiguratu baduzu **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** , edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, portaera horren arabera aldatuko da. Sistemak rolen prezioen erregistroak berreskuratzen ditu prezioen dimentsioen balio bakoitzarekin bat datozen balioekin lehentasunen arabera ordenatuta azken dimentsioetarako balio baliorik gabeko errenkadekin.

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
