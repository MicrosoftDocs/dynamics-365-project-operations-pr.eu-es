---
title: Data-eraginkorra den prezioak gainidaztea
description: Artikulu honek prezioen zerrendako prezio espezifikoetarako prezioen gainidatziak nola konfiguratu azaltzen du.
author: rumant
ms.date: 09/01/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 41af5176c0809c9621fc0fa946a04492da7d152b
ms.sourcegitcommit: 37293b0b28f072deafc00112ddbbea91c48a7802
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/08/2022
ms.locfileid: "9445995"
---
# <a name="date-effective-price-overrides"></a>Data-eraginkorra den prezioak gainidaztea 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

*Data-eraginkorra den prezioak gainidaztea* prezioen zerrendan prezio zehatzak gainidazteko edo aldatzeko modu bat eskaini. Adibidez, prezio-zerrenda estandar bat duzu, 2022ko urtarrilaren 1etik 2022ko abenduaren 31ra arte indarrean dagoena. Prezio zerrenda honek rol askotarako prezioak ditu. Ezarritako prezioa **Sareko teknikaria** rola 100 dolar (USD) orduko da. Sareko teknikari batek 2022ko urtarrilaren 1etik 2022ko abenduaren 31ra bitartean denbora erregistratzen duenean, denboraren prezioa 100 USD da. 2022ko urriaren 1ean, prezioa egokitu behar duzu *bakarrik* rentzat **Sareko teknikaria** rola, 100 USD orduko 110 USD orduko. The **Indarrean dagoen prezioa gainidaztea** funtzioak aldaketa hau rolaren prezio zehatz horretarako errenkadaren gainidatzi gisa konfiguratzeko aukera ematen dizu. Beraz, ez duzu prezioen zerrenda osoa kopiatu beharrik eta errenkada horren prezioa aldatu beharrik.

## <a name="date-effective-price-overrides-for-labor-pricing"></a>Data-eraginkorra den prezioen ordezkapenak eskulanaren prezioetarako

Proiektu batean lan-denboraren data-eraginkorra den prezioen baliogabetzeak ezartzeko prozesuak oinarrizko bi urrats ditu.

1. Gaitu **Indarrean dagoen prezioa gainidaztea** ezaugarria.
1. Konfiguratu data-eraginkorra den prezioa gainidazteko.

### <a name="enable-the-date-effective-price-overrides-feature"></a>Gaitu Data indarrean dagoen prezioa gainidazteko funtzioa

> [!NOTE]
> Ondoren **Indarrean dagoen prezioa gainidaztea** eginbidea gaituta dago, ezin da desgaitu.

Gaitzeko **Data-eraginkorra den prezioak gainidaztea** eginbidea, jarraitu urrats hauek.

1. Joan **Ezarpenak** \> **Parametroak**.
1. Ireki **Parametroak** erregistroa.
1. Ekintza-panelean, gunean **Ezaugarrien Kontrola** fitxa, hautatu **Gaitu data baliozko prezioen baliogabetzeak**.
1. Berrespenaren elkarrizketa-koadroan, hautatu **Ados**.
1. Une batzuk igaro ondoren, freskatu arakatzailea. Data eraginkorra den prezioa gainidazteko gaitasunek eskuragarri egon beharko lukete orain. Jakingo duzu gaitasun hauek gaituta daudela baldin **Gaitu data baliozko prezioen baliogabetzeak** jada ez da Ekintza Panelean agertzen.

### <a name="set-up-a-date-effective-price-override"></a>Konfiguratu data-eraginkorra den prezioa gainidazteko

Data-eraginkorra den prezioen baliogabetzeak konfigura daitezke **Kostua**, **·**, edo **Erosketa** prezioen zerrendak.

> [!NOTE]
>Duen portaera **Indarrean dagoen prezioa gainidaztea** gaur egun muga hauek ditu:
>
> - Rolen prezioek eta rolen prezioen markek soilik onartzen dute **Indarrean dagoen prezioa gainidaztea** Proiektuaren Eragiketetan eginbidea.
> - Prezio zerrenda bat kopiatzen duzunean erabiliz **Kopiatu** buruzko ekintza **Prezio zerrendaren xehetasunak** orrialdean, eta kontratua sortzean prezioen zerrenda estandar edo pertsonalizatu batetik proiektuaren prezio-zerrenda bat sortzen duzunean, data-eraginkorra den prezioen baliogabetzeak dira.**ez** iturriko prezioen zerrendatik kopiatua.

Rolaren prezioa edo rolaren prezioaren markaketa datan eragingarria den prezioa ezartzeko, jarraitu urrats hauek.

1. Ireki data-eraginkorra den prezioaren baliogabetzea konfiguratu nahi duzun prezio-zerrendaren orria.
1. Hautatu **Rolen prezioak** fitxa. Fitxa honek guztiak zerrendatzen ditu **Rolaren prezioa** prezioen zerrendako erregistroak.
1. Hautatu **Rolaren prezioa** erregistratu data-eraginkorra den baliogabetze-prezio berri bat konfiguratu nahi duzula, eta, ondoren, sakatu bi aldiz (edo egin klik bikoitza) **Rolaren prezioa** irekitzeko **Rolaren prezioaren xehetasunak** orrialdea.
1. Hautatu **Indarrean dauden datak gainidaztea** fitxa. Fitxa honetako sareak hautatutako prezioen baliogabetze data guztiak zerrendatzen ditu **Rolaren prezioa** erregistroa.
1. Saretaren gaineko tresna-barran, hautatu **Rolaren prezioa gainidaztea**. The **Rolaren prezioa gainidaztea** graduatzailea irekitzen da.
1. Zehaztu hasierako data, unitatea eta prezio berria baliogabetzeko. Ondoren, hautatu **Gorde**, eta itxi formularioa.

> [!NOTE]
> - Rolaren prezioaren edo rolaren prezioaren markatze datan eragingarria den prezioa baliogabetzea gurasoan dagoen prezio-dimentsio-balioen konbinazio berean aplikatzen da.**Rolaren prezioa** edo **Rolen prezioen markaketa** ilara.
> - Atalean aukeratzen den data **-tik eraginkorra** eremuak prezioen zerrenda nagusiaren eragin-egunetan egon behar du. Prezioa gainidaztean eragina izango da aukeratzen den datan **-tik eraginkorra** eremuan eta prezio-zerrenda nagusiaren amaiera-data amaitu arte aplikatuko da. Rolaren prezio berdinerako beste data-eraginkorra den prezioaren baliogabetzea konfiguratzen baduzu, lehen prezioa baliogabetzea aukeratutako datan izango da indarrean.**-tik eraginkorra** eremua eta bigarren baliogabetzea hasi arte aplikatuko da.

## <a name="examples"></a>Adibideak

### <a name="example-1-determining-date-effectivity-for-a-role-price-that-has-role-price-overrides"></a>1. adibidea: data-eraginkortasuna zehaztea rol-prezioa gainidatzitako rol-prezio baterako

Ondorengo adibideak erakusten du data-eraginkortasuna nola zehazten den rol-prezio-prezio zehatz baterako rol-prezioen baliogabetzeak ezartzen dituen.

**A prezio zerrenda: urtarrilaren 1etik ekainaren 30era**

*Rolaren prezioa*

| Rolaren prezioa | Unitatea | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|---|
| Sareko teknikaria | Ordu | 100 | Prezio hori transakzio-data urtarrilaren 1etik martxoaren 14ra arteko transakzioetan erabiliko da. |

*Rolaren prezioa gainidaztea*

| -tik eraginkorra | Unitatea | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|---|
| Martxoak 15 | Ordu | 110 | Prezio hori transakzio-data martxoaren 15etik martxoaren 30era arteko transakzioetan erabiliko da. |
| Apirilak 1 | Ordu | 120 | Prezio hori transakzio-data apirilaren 1etik ekainaren 30era arteko transakzioetan erabiliko da. |

### <a name="example-2-determining-date-effectivity-for-a-role-price-markup-that-has-role-price-markup-overrides"></a>2. adibidea: rolaren prezioaren marka gainidatziak dituen rol-prezio-marka baten data-eraginkortasuna zehaztea

Ondorengo adibideak erakusten du nola zehazten den data-eraginkortasuna rol-prezio-marka-marka zehatz baterako, rol-prezio-markak gainidazteko konfiguratzen diren.

**A prezio zerrenda: urtarrilaren 1etik ekainaren 30era**

*Rolaren prezioa*

| Rolaren prezioa | Lanorduak | Unitatea | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|---|---|
| Sareko teknikaria | Erregularra | Ordu | 100 | Prezio hori transakzio-data urtarrilaren 1etik martxoaren 14ra arteko transakzioetan erabiliko da. |

*Rolen prezioen markaketa*

| Antolaketa unitatea | Lanorduak | Markatu % |
|---|---|---|
| Contoso US | Aparteko orduak | %10 |

*Rolaren prezioaren marka gainidaztea*

| -tik eraginkorra | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|
| Martxoak 15 | %20 | Markaketaren ehuneko hori transakzio-data martxoaren 15etik martxoaren 30era arteko transakzioetan erabiliko da. |
| Apirilak 1 | % 25 | Markatze hori transakzio-data apirilaren 1etik ekainaren 30era arteko transakzioetan erabiliko da. |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
