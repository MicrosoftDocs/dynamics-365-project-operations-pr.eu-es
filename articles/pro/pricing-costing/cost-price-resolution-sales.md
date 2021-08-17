---
title: Ebatzi proiektu-aurreikuspenen eta benetako datuen kostuaren prezioak
description: Gai honek proiektuaren kalkuluen eta benetako datuen kostu-prezioak ebazteari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 04/07/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a2a2df7672118a4a4d7748795174e8e8238dd7618a48437185879e06a253a381
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6997546"
---
# <a name="resolve-cost-prices-on-project-estimates-and-actuals"></a>Ebatzi proiektu-aurreikuspenen eta benetako datuen kostuaren prezioak 

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Kostuen prezioak eta kostuen prezioen zerrenda kalkulatzeko eta benetako datuak ebazteko, sistemak informazioa erabiltzen du **Data**, **Moneta** eta **Kontratazio unitatea** lotutako proiektuaren eremuak. Kostuen prezioen zerrenda ebatzi ondoren, aplikazioak kostuen tasa ebazten du.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-time"></a>Benetako kostuen tasak ebaztea eta denborarako kalkulatutako lerroak

Denboraren zenbatespen lerroek proiektu bateko denbora eta baliabideak esleitzeko aurrekontuaren eta kontratuaren lerroaren xehetasunak aipatzen dituzte.

Kostuen prezioen zerrenda ebatzi ondoren, **Funtzioa** eta **Baliabideen unitatea** denbora kalkulatzeko lerroaren eremuak prezioen zerrendako rol prezioen lerroekin parekatzen dira. Bat-etortze honen arabera, lan kostuaren prezio estandarreko neurriak erabiltzen ari zarela suposatzen da. Bat etortzeko sistemaren eremuak konfiguratu badituzu edo ez horren ordez **Rola** eta **Baliabideen unitatea**, orduan hori da bat datorren rolaren prezio lerroa berreskuratzeko erabiliko den konbinazioa. Aplikazioak kostuaren tasa duen rola prezio lerro bat aurkitzen badu **Rola** eta **Baliabideen unitatea** konbinazioa, kostuaren tasa lehenetsia da. Aplikazioa ezin bada **Rola** eta **Baliabideen unitatea** balioak, ondoren, rolen prezioen lerroak berreskuratzen ditu bat datozen rolekin baina balio baliogabeak **Baliabideen unitatea**. Egokitutako rolen prezioen erregistroa izan ondoren, kostu-tasa erregistro horretatik lehenetsita dago. 

> [!NOTE]
> Lehenespen desberdina konfiguratu baduzu **Rola** eta **Baliabideen unitatea**, edo lehentasun handiagoa duten beste dimentsio batzuk badituzu, portaera horren arabera aldatuko da. Sistemak rolen prezioen erregistroak berreskuratzen ditu prezioen dimentsioen balio bakoitzarekin bat datozen balioekin lehentasunen arabera ordenatuta azken dimentsioetarako balio baliorik gabeko errenkadekin.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-expense"></a>Benetako kostuen tasak ebaztea eta Gastuaren kalkulatutako lerroak

Gastuaren zenbatespen lerroek proiektu bateko proiektu bateko gastuak eta aurreikusitako gastuen lerroaren eskaintzaren eta kontratuaren lerroko xehetasunak.

Kostuen prezioen zerrenda ebatzi ondoren, sistemak konbinazio bat erabiltzen du **Kategoria** eta **Unitatea** gastua kalkulatzeko lerroaren eremuak **Kategoriaren prezioa** prezioen zerrendako lerroak. Sistemak kostu tasa duen kategoriako prezio lerro bat aurkitzen badu **Kategoria** eta **Unitatea** eremuen konbinazioa, kostu tasa lehenetsita dago. Sistema ez badator bat **Kategoria** eta **Unitatea** balioekin, edo bat datorren kategoria prezio lerro bat aurkitzeko gai bada, baina prezioen metodoa ez da **Unitateko prezioa**, kostuaren tasa zero (0) lehenetsita dago.

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-material"></a>Materialen kostu tasak ebaztea eta materialaren estimazio lerroak

Materialaren zenbatespen lerroek materialen aurrekontuaren eta kontratuaren lerroaren xehetasunak eta proiektu bateko materialen estimazio lerroak aipatzen dituzte.

Kostuen prezioen zerrenda ebatzi ondoren, sistemak konbinazio bat erabiltzen du **Produktua** eta **Unitatea** kalkulu-lerroaren eremuak kalkulu materialarekin bat etortzeko **Prezioen zerrendako elementuak** prezioen zerrendako lerroak. Sistemak kostu tasa duen produktuaren prezio lerroa aurkitzen badu **Produktua** eta **Unitatea** eremuen konbinazioa, kostu tasa lehenetsita dago. Sistema ezin bada **Produktua** eta **Unitatea** balioak edo bat datorren prezioen zerrendako elementu lerro bat aurkitzeko gai bada, baina prezioen metodoa kostu estandarrean edo kostu arruntean oinarritzen da eta produktuan ez dago zehaztuta, kostu unitarioa zero da lehenetsita.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
