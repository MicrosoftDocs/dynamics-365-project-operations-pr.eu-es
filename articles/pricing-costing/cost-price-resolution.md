---
title: Aurreikuspenen eta benetako datuen kostuaren prezioa ebaztean
description: Gai honek kostuaren prezioa ebazteko moduari eta estimazioei buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d3422ef2eacc1e0617e60d41b7ddbcefe44d5b90
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070898"
---
# <a name="resolving-cost-prices-for-estimates-and-actuals"></a>Aurreikuspenen eta benetako datuen kostuaren prezioa ebaztean

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Kostuen prezioak eta kostuen prezioen zerrenda kalkulatzeko eta benetako datuak ebazteko, sistemak informazioa erabiltzen du **Data** , **Moneta** eta **Kontratazio unitatea** lotutako proiektuaren eremuak. Kostuen prezioen zerrenda ebatzi ondoren, aplikazioak kostuen tasa ebazten du.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-time"></a>Benetako kostuen tasak ebaztea eta denborarako kalkulatutako lerroak

Denboraren zenbatespen lerroek proiektu bateko denbora eta baliabideak esleitzeko aurrekontuaren eta kontratuaren lerroaren xehetasunak aipatzen dituzte.

Kostuaren prezio-zerrenda bat ebatzi eta gero, sistemak **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** kalkulatzeko lerroaren eremuak, ebatzitako prezio zerrendako rol prezioen lerroekin bat etortzeko. Partida honek suposatzen du kutxaz kanpoko prezioen neurriak erabiltzen dituzula eskulanaren kosturako. Bat etortzeko sistemaren eremuak konfiguratu badituzu edo ez horren ordez **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** , orduan hori da bat datorren rolaren prezio lerroa berreskuratzeko erabiliko den konbinazioa. Aplikazioak kostuaren tasa duen rola prezio lerro bat aurkitzen badu **Rola** , **Baliabideen enpresa** eta **Baliabideen uitatea** konbinazioa, kostuaren tasa lehenetsia da. Aplikazioa ezin bada **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** balioak, ondoren, rolen prezioen lerroak berreskuratzen ditu bat datozen rolekin baina balio baliogabeak **Baliabideen unitatea**. Egokitutako rolen prezioen erregistroa izan ondoren, kostu-tasa erregistro horretatik lehenetsita dago. 

> [!NOTE]
> Lehenespen desberdina konfiguratu baduzu **Rola** , **Baliabideen enpresa** eta **Baliabideen unitatea** , edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, portaera horren arabera aldatuko da. Sistemak rolen prezioen erregistroak berreskuratzen ditu prezioen dimentsioen balio bakoitzarekin bat datozen balioekin lehentasunen arabera ordenatuta azken dimentsioetarako balio baliorik gabeko errenkadekin.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-expense"></a>Benetako kostuen tasak ebaztea eta Gastuaren kalkulatutako lerroak

Gastuaren zenbatespen lerroek proiektu bateko proiektu bateko gastuak eta aurreikusitako gastuen lerroaren eskaintzaren eta kontratuaren lerroko xehetasunak.

Kostuaren prezio-zerrenda bat ebatzi eta gero, sistemak **Kategoria** , **Unitatea** eta **Kategoriaren unitatea** kalkulatzeko lerroaren eremuak, ebatzitako prezio zerrendako rol prezioen lerroekin bat etortzeko. Sistemak kostu tasa duen kategoriako prezio lerro bat aurkitzen badu **Kategoria** eta **Unitatea** eremuen konbinazioa, kostu tasa lehenetsita dago. Sistema ezin bada **Kategoria** eta **Unitatea** balioak, edo bat datorren kategoria prezio lerro bat aurkitzeko gai bada, baina prezioen metodoa ez da **Unitateko prezioa** , kostuaren tasa zero (0) lehenetsita dago.