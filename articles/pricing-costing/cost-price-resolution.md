---
title: Aurreikuspenen eta benetako datuen kostuaren prezioa ebaztean
description: Gai honek kostuaren prezioa ebazteko moduari eta estimazioei buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/09/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d81b521acbfd97127cf056bd41a3249c01108374
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001366"
---
# <a name="resolving-cost-prices-for-estimates-and-actuals"></a>Aurreikuspenen eta benetako datuen kostuaren prezioa ebaztean

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Kostuen prezioak eta kostuen prezioen zerrenda kalkulatzeko eta benetako datuak ebazteko, sistemak informazioa erabiltzen du **Data**, **Moneta** eta **Kontratazio unitatea** lotutako proiektuaren eremuak. Kostuen prezioen zerrenda ebatzi ondoren, aplikazioak kostuen tasa ebazten du.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-time"></a>Benetako kostuen tasak ebaztea eta denborarako kalkulatutako lerroak

Denboraren zenbatespen lerroek proiektu bateko denbora eta baliabideak esleitzeko aurrekontuaren eta kontratuaren lerroaren xehetasunak aipatzen dituzte.

Kostuaren prezio-zerrenda bat ebatzi eta gero, sistemak **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea** kalkulatzeko lerroaren eremuak, ebatzitako prezio zerrendako rol prezioen lerroekin bat etortzeko. Partida honek suposatzen du kutxaz kanpoko prezioen neurriak erabiltzen dituzula eskulanaren kosturako. Bat etortzeko sistemaren eremuak konfiguratu badituzu edo ez horren ordez **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea**, orduan hori da bat datorren rolaren prezio lerroa berreskuratzeko erabiliko den konbinazioa. Aplikazioak kostuaren tasa duen rola prezio lerro bat aurkitzen badu **Rola**, **Baliabideen enpresa** eta **Baliabideen uitatea** konbinazioa, kostuaren tasa lehenetsia da. Aplikazioa ezin bada bat etorri **Rola**, **Baliabideen Enpresa** eta **Baliabideen Unitatea** balioak, rolen prezioen lerroak berreskuratuko ditu bat datorren rolaren balioarekin, baina balio baliogabeak izango ditu **Baliabideen Unitatea** eta **Baliabideen Enpresa**. Bat datorren rolaren prezioen erregistroa bat datorren rolaren prezioaren balioarekin aurkitu ondoren, erregistro horretako kostuen tasa lehenetsita dago. 

> [!NOTE]
> Lehenespen desberdina konfiguratu baduzu **Rola**, **Baliabideen enpresa** eta **Baliabideen unitatea**, edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, portaera horren arabera aldatuko da. Sistemak rolen prezioen erregistroak berreskuratzen ditu prezioen dimentsioen balio bakoitzarekin lehentasunen arabera bat datozen balioekin lehentasun ordenan azkeneko dimentsioetarako balio baliodun errenkadekin.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-expense"></a>Benetako kostuen tasak ebaztea eta Gastuaren kalkulatutako lerroak

Gastuaren zenbatespen lerroek proiektu bateko proiektu bateko gastuak eta aurreikusitako gastuen lerroaren eskaintzaren eta kontratuaren lerroko xehetasunak.

Kostuaren prezio-zerrenda bat ebatzi eta gero, sistemak **Kategoria**, **Unitatea** eta **Kategoriaren unitatea** kalkulatzeko lerroaren eremuak, ebatzitako prezio zerrendako rol prezioen lerroekin bat etortzeko. Sistemak kostu tasa duen kategoriako prezio lerro bat aurkitzen badu **Kategoria** eta **Unitatea** eremuen konbinazioa, kostu tasa lehenetsita dago. Sistema ezin bada **Kategoria** eta **Unitatea** balioak, edo bat datorren kategoria prezio lerro bat aurkitzeko gai bada, baina prezioen metodoa ez da **Unitateko prezioa**, kostuaren tasa zero (0) lehenetsita dago.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-material"></a>Materialen kostu tasak ebaztea eta materialaren estimazio lerroak

Materialaren zenbatespen lerroek materialen aurrekontuaren eta kontratuaren lerroaren xehetasunak eta proiektu bateko materialen estimazio lerroak aipatzen dituzte.

Kostuen prezioen zerrenda ebatzi ondoren, sistemak konbinazio bat erabiltzen du **Produktua** eta **Unitatea** kalkulu-lerroaren eremuak kalkulu materialarekin bat etortzeko **Prezioen zerrendako elementuak** prezioen zerrendako lerroak. Sistemak kostu tasa duen produktuaren prezio lerroa aurkitzen badu **Produktua** eta **Unitatea** eremuen konbinazioa, kostu tasa lehenetsita dago. Sistema ezin bada **Produktua** eta **Unitatea** balioak, unitateko kostua zero da lehenetsita. Lehenespen hori ere gertatuko da bat datorren prezioen zerrendako elementu lerroa baldin badago, baina prezioen metodoa produktuan zehazten ez den kostu estandarrean edo uneko kostuan oinarritzen da.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
