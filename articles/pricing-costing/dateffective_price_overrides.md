---
title: Dataren araberako prezioen gainidazketak
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
# <a name="date-effective-price-overrides"></a>Dataren araberako prezioen gainidazketak 

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

*Data-eraginkorra den prezioak gainidaztea* prezioen zerrendan prezio zehatzak gainidazteko edo aldatzeko modu bat eskaini. Adibidez, prezio-zerrenda estandar bat duzu, 2022ko urtarrilaren 1etik 2022ko abenduaren 31ra arte indarrean dagoena. Prezio zerrenda honek funtzio askotarako prezioak ditu. Ezarritako prezioa **Sareko teknikaria** funtziorako 100 dolar (USD) orduko da. Sareko teknikari batek 2022ko urtarrilaren 1etik 2022ko abenduaren 31ra bitartean denbora erregistratzen duenean, denboraren prezioa 100 USD da. 2022ko urriaren 1ean, prezioa egokitu behar duzu *bakarrik* **Sareko teknikaria** funtzioarentzat, 100 USD orduko preziotik 110 USD orduko preziora. **Dataren arabera indarrean dagoen prezioa gainidaztea** funtzioak aldaketa hau funtzioaren prezio zehatz horretarako errenkadaren gainidatzi gisa konfiguratzeko aukera ematen dizu. Beraz, ez duzu prezioen zerrenda osoa kopiatu beharrik eta errenkada horren prezioa aldatu beharrik.

## <a name="date-effective-price-overrides-for-labor-pricing"></a>Data-eraginkorra den prezioen ordezkapenak eskulanaren prezioetarako

Proiektu batean dataren arabera eraginkorra den prezioen baliogabetzeak ezartzeko prozesuak oinarrizko bi urrats ditu.

1. Gaitu **dataren araberako prezioen gainidazketak** eginbidea.
1. Konfiguratu dataren araberako prezioen gainidazketa.

### <a name="enable-the-date-effective-price-overrides-feature"></a>Gaitu dataren araberako prezioen gainidazketak eginbidea

> [!NOTE]
> **Dataren araberako prezioaren gainidazketa** eginbidea gaitu ondoren, ezin da desgaitu.

Gaitzeko **Dataren araberako prezioak gainidaztea** eginbidea, jarraitu urrats hauek.

1. Joan **Ezarpenak** \> **Parametroak**.
1. Ireki **Parametroak** erregistroa.
1. Ekintza-panelean, **Ezaugarrien Kontrola** fitxan, hautatu **Gaitu dataren araberako prezioen gainidazketak**.
1. Berrespenaren elkarrizketa-koadroan, hautatu **Ados**.
1. Une batzuk igaro ondoren, freskatu arakatzailea. Dataren araberako prezioen gainidazketa-gaitasunek eskuragarri egon beharko lukete orain. Jakingo duzu gaitasun hauek gaituta daudela baldin **Gaitu Dataren araberako prezioen gainidazketak** jada ez bada Ekintza Panelean agertzen.

### <a name="set-up-a-date-effective-price-override"></a>Konfiguratu dataren araberako prezioen gainidazketa

**Kostua**, **Salmenta**, edo **Erosketa** moduluak dituzten prezio-zerrendetan soilik konfiguratu daitezke dataren araberako prezioen gainidazketak.

> [!NOTE]
>**Dataren araberako prezio-gainidazketen** portaerak gaur egun muga hauek ditu:
>
> - Funtzioen prezioek eta funtzioen prezioen markek soilik onartzen dute **Dataren araberako prezio-gainidazketen** eginbidea Project Operations-en.
> - Prezio zerrenda bat kopiatzen duzunean erabiliz **Kopiatu** ekintza **Prezio zerrendaren xehetasunak** orrialdean, eta kontratua sortzean prezioen zerrenda estandar edo pertsonalizatu batetik proiektuaren prezio-zerrenda bat sortzen duzunean, dataren araberako prezio-gainidazketak **ez** dira kopiatzen iturburuko prezioen zerrendatik.

Funtzioaren prezioa edo funtzioaren prezioaren gainprezioaren dataren araberako prezio-gainidazketa ezartzeko, jarraitu urrats hauek.

1. Ireki Dataren araberako prezio-gainidazketa konfiguratu nahi duzun prezio-zerrendaren orria.
1. Hautatu **Funtzioaren prezioak** fitxa. Fitxa honek zerrendatzen ditu **Funtzioaren prezio** erregistro guztiak prezioen zerrendan.
1. Hautatu **Funtzioaren prezioa** erregistratu data-eraginkorra den baliogabetze-prezio berri bat konfiguratu nahi duzula, eta, ondoren, sakatu bi aldiz (edo egin klik bikoitza) **Funtzioaren prezioa** irekitzeko **Funtzioaren prezioaren xehetasunak** orrialdea.
1. Hautatu **Dataren araberako prezio-gainidazketen** fitxa. Fitxa honetako sareak hautatutako Dataren araberako prezio-gainidazketa guztiak zerrendatzen ditu **Funtzioaren prezioa** erregistrorako.
1. Saretaren gaineko tresna-barran, hautatu **Funtzioaren prezioa gainidaztea**. **Funtzioaren prezioa gainidaztea** graduatzailea irekitzen da.
1. Zehaztu hasierako data, unitatea eta prezio berria gainidazteko. Ondoren, hautatu **Gorde** eta ondoren itxi inprimakia.

> [!NOTE]
> - Funtzioaren prezioaren edo funtzioaren prezioaren gainprezioaren Dataren araberako prezio-gainidazketa aplikatu daiteke prezioaren dimentsio-balioen konbinazio berdinean **funtzioaren prezioa** edo **funtzioaren prezioen gainprezioa** errenkada nagusietan.
> - Aukeratzen den datak **Indarrean sartzeko data** eremuan prezioen zerrenda nagusiaren indarrean sartzeko dataren barruan egon behar du. Prezioa gainidaztean eragina izango da aukeratzen den datan **-tik eraginkorra** eremuan eta prezio-zerrenda nagusiaren amaiera-data amaitu arte aplikatuko da. Funtzioaren prezio berdinerako beste data-eraginkorra den prezioaren gainidazketa konfiguratzen baduzu, lehen prezioaren gainidazketan aukeratutako **-tik eraginkorra** eremuko datan izango da indarrean eta bigarren baliogabetzea hasi arte aplikatuko da.

## <a name="examples"></a>Adibideak

### <a name="example-1-determining-date-effectivity-for-a-role-price-that-has-role-price-overrides"></a>1. adibidea: data-eraginkortasuna zehaztea funtzioaren prezioaren gainidazketa duen funtzioaren prezio baterako

Ondorengo adibideak erakusten du data-eraginkortasuna nola zehazten den funtzioaren prezioaren gainidazketa konfiguratuta duen funtzioaren prezio jakin batean.

**Prezio zerrenda A: urtarrilaren 1etik ekainaren 30era**

*Funtzioaren prezioa*

| Funtzioaren prezioa | Unitatea | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|---|
| Sareko teknikaria | Ordu | 100 | Prezio hori transakzio-data urtarrilaren 1etik martxoaren 14ra arteko transakzioetan erabiliko da. |

*Funtzio-prezioaren gainidazketa*

| Noiztik eraginkorra | Unitatea | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|---|
| Martxoak 15 | Ordu | 110 | Prezio hori transakzio-data martxoaren 15etik martxoaren 30era arteko transakzioetan erabiliko da. |
| Apirilak 1 | Ordu | 120 | Prezio hori transakzio-data apirilak 1etik ekainak 30era arteko transakzioetan erabiliko da. |

### <a name="example-2-determining-date-effectivity-for-a-role-price-markup-that-has-role-price-markup-overrides"></a>2. adibidea: data-eraginkortasuna zehaztea funtzioaren prezioaren gainprezioaren gainidazketa duen funtzioaren prezioaren gainprezio baterako

Ondorengo adibideak erakusten du data-eraginkortasuna nola zehazten den funtzioaren prezioaren gainprezioaren gainidazketa konfiguratuta duen funtzioaren prezioaren gainprezio jakin batean.

**Prezio zerrenda A: urtarrilaren 1etik ekainaren 30era**

*Funtzioaren prezioa*

| Funtzioaren prezioa | Lanorduak | Unitatea | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|---|---|
| Sareko teknikaria | Ohikoak | Ordu | 100 | Prezio hori transakzio-data urtarrilaren 1etik martxoaren 14ra arteko transakzioetan erabiliko da. |

*Funtzio-prezioaren gainprezioa*

| Erakundearen unitatea | Lanorduak | Gainprezioa % |
|---|---|---|
| Contoso US | Aparteko orduak | %10 |

*Funtzio-prezioaren gainprezioaren gainidazketa*

| Noiztik eraginkorra | Prezioa | Sarrerako transakzioen prezioetan eragina |
|---|---|---|
| Martxoak 15 | %20 | Gainprezioaren ehuneko hori transakzio-data martxoaren 15etik martxoaren 30era arteko transakzioetan erabiliko da. |
| Apirilak 1 | % 25 | Gainprezio hori transakzio-data apirilak 1etik ekainak 30era arteko transakzioetan erabiliko da. |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
