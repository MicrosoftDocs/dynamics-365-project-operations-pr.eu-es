---
title: Eremu pertsonalizatuak prezio-dimentsio gisa konfiguratzea
description: Gai honek prezio-dimentsio pertsonalizatuak ezartzeko informazioa eskaintzen du.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/20/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 81f926e0aa209dd83f9b850c2342bd35a4f236c3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282453"
---
# <a name="setting-up-custom-fields-as-pricing-dimensions"></a>Eremu pertsonalizatuak prezio-dimentsio gisa konfiguratzea 

[!include [banner](../includes/psa-now-project-operations.md)]

Hasi aurretik, gai honek honako gai hauetan azaldutako prozedurak bete dituzula suposatzen du: [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities.md) eta [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan](field-references.md). Prozedura horiek bete ez badituzu, itzuli, bete itzazu eta, ondoren, itzuli gai honetara. 

Gai honek prezio-dimentsio pertsonalizatuak ezartzeko informazioa eskaintzen du. Project Service-ren web interfazean, **Parametroak** orrian, **Zenbatekoan oinarritutako prezio-dimentsioak** fitxak prezio-dimentsioen entitateetako erregistroak erakusten ditu. Lehenespenez, Project Service-ren instalazioak 2 errenkada sortzen ditu fitxa honen saretan:

- **msdyn_resourcecategory** (Funtzioa)
- **msdyn_OrganizationalUnit** (Erakundearen unitatea)

> [!IMPORTANT]
> Ez ezabatu errenkada horiek. Hala ere, ez badituzu behar, testuinguru zehatz batean ez aplikagarri gisa ezar daitezke **Kostuari aplikagarria**, **Salmentei aplikagarria** eta **Erosketei aplikagarria** eremuak **Ez** gisa ezarriz. Atributu-balio horiek **Ez** gisa ezartzeak eremua prezio-dimentsio gisa ez izatearen eragin bera du.

Eremu bat prezio-dimentsio bihurtzeko, honelakoa izan behar da:

- Eremu gisa sortua **Funtzio-prezioa** eta **Funtzio-prezioen gainprezioa** entitateetan. Hori egiteko moduari buruzko informazio gehiago lortzeko, ikusi [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan](field-references.md).
- Errenkada gisa sortua **Prezio-dimentsioa** taulan. Adibidez, gehitu prezio-dimentsioen errenkadak hurrengo grafikoan erakusten den bezala. 

![Zenbatekoan oinarritutako prezio-dimentsioen errenkadak](media/Amt-based-PD.png)

Kontuan izan Baliabideen lanorduak (**msdyn_resourceworkhours**) gainprezioan oinarritutako dimentsio gisa gehitu dela eta saretan gehitu dela **Gainprezioan oinarritutako prezio-dimentsioa** fitxan.

![Gainprezioan oinarritutako prezio-dimentsioen errenkadak](media/Markup-based-PD.png)

> [!IMPORTANT]
> Taula honetako prezio-dimentsioko datuen aldaketa guztiak, lehendik daudenak edo berriak, Project Service-ren prezioen negozio logikara hedatzen dira cachea freskatu ondoren soilik. Cachea freskatzeko denbora 10 minutu ingurukoa da. Onartu denbora hori prezio-dimentsioko datuen aldaketek eragin behar duten prezioen lehenetsitako logikaren aldaketak ikusteko.


## <a name="attributes-of-the-pricing-dimensions-table"></a>Prezio-dimentsioen taularen atributuak
Hurrengo ataletan, atributuen ezaugarriei buruzko informazioa ematen da **Prezio-dimentsioak** taulan.

### <a name="pricing-dimension-name"></a>Prezio-dimentsioaren izena
Balio horrek prezio-dimentsio pertsonalizatuetarako **Funtzio-prezioa** taulan gehitzen den eremuaren eskemaren izenaren berdina izan behar du. Eremuak **Funtzio-prezioa** tauln gehitzeari buruzko informazio gehiago lortzeko, ikusi [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan](field-references.md).

### <a name="type-of-dimension"></a>Dimentsio mota
Bi prezio-dimentsio mota daude:
  
  - **Zenbatekoaren araberako dimentsioak**: sarrerako testuinguruko dimentsio-balioak bat datoz **Funtzio-prezioa** lerroko dimentsio-balioekin eta prezioa/kostua zuzenean lehenesten dira **Funtzio-prezioa** taulatik.
  - **Gainprezioan oinarritutako dimentsioak**: dimentsio horietan Project Service-k jarraian azaltzen den hiru pausoko prozesua hasiko du prezioa/kostua lortzeko
 
    1. Project Service-k sarrerako testuinguruko gainprezioan oinarritzen ez diren dimentsio-balioak Funtzio-prezioaren lerroarekin lotzen ditu oinarrizko tasa lortzeko.
    2. Project Service-k sarrerako testuinguruko dimentsio-balio guztiak **Funtzio-prezioaren gainprezioa** lerroarekin lotzen ditu gainprezioaren ehunekoa lortzeko.
    3. Project Service-k bigarren urratsean lortutako gainprezioaren ehunekoa aplikatzen du lehen urratsean lortutako **Funtzio-prezioa** taulatik lortutako oinarrizko tasan azken preziora/kostura iristeko.
   
   Hurrengo taulan prezioaren gainprezioen kalkulua azaltzen da.
  
| Funtzioa        | Erakunde-unitatea    |Lantokiaren kokalekua      |Titulu estandarra      |Baliabideen lanorduak      |  Gainprezioa|
| ------------|-------------|-------------------|--------------------|-------------------------|--------:|
|             | Contoso India|In situ            |                    |Aparteko orduak                 |15     |
|             | Contoso India|Lokala             |                    |Aparteko orduak                 |10     |
|             | Contoso US   |Lokala             |                    |Aparteko orduak                 |20     |


Oinarrizko tasa 100 USD duen Contoso India-ko baliabide bat lanean ari bada, eta ohiko orduetan 8 ordu eta aparteko orduetan 2 ordu erregistratzen badituzte, Project Service-ren prezioaren motorrak 100eko oinarri-tasa erabiliko du 8 orduetarako 800 USD grabatzeko. Aparteko 2 orduetarako, % 15eko gainprezioa aplikatuko zaio 100eko oinarrizko tasari 115 USD-eko unitate-prezioa lortzeko eta 230 USD-eko kostu osoa erregistratuko du.

### <a name="applicable-to-cost"></a>Kostuari aplikagarria 
Aukera hori **Bai** gisa ezarrita badago, sarrerako testuinguruko dimentsioaren balioa **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** eremuekin lotzeko erabili behar dela adierazten du kostu- eta balorazio-tasak berreskuratzean.

### <a name="applicable-to-sales"></a>Salmentei aplikagarria
Aukera hori **Bai** gisa ezarrita badago, sarrerako testuinguruko dimentsioaren balioa **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** eremuekin lotzeko erabili behar dela adierazten du faktura- eta gainprezio-tasak berreskuratzean.

### <a name="applicable-to-purchase"></a>Erosketari aplikagarria
Aukera hori **Bai** gisa ezarrita badago, sarrerako testuinguruko dimentsioaren balioa **Funtzio-prezioa** eta **Funtzio-prezioaren gainprezioa** eremuekin lotzeko erabili behar dela adierazten du erosketa-prezioa berreskuratzean. Gaur egun, Project Service-k ez du azpikontratazio egoerarik onartzen, beraz, eremu hau ez da erabiltzen. 

### <a name="priority"></a>Lehentasuna
Dimentsioaren lehentasuna zehazteak Project Service-ren prezioari prezio bat sortzen laguntzen dio sarrerako dimentsio-balioen eta **Funtzio-prezioa** edo **Funtzio-prezioaren gainprezioa** tauletako balioen arteko bat etortzea aurkitu ezin duenean. Egoera honetan, Project Service-k balio nuluak erabiliko ditu bat etortzerik gabeko dimentsio-balioetarako, dimentsioak beren lehentasunen arabera neurtuz.

- **Kostuen lehentasuna**: dimentsio baten kostuaren lehentasunaren balioak dimentsio horren pisua adieraziko du kostuen prezioen konfigurazioarekin bat datorrenean. **Kostuen lehentasuna** eremuaren balioak bakarra izan behar du **Kostuari aplikagarria** dimentsioetan.
- **Salmenten lehentasuna**: dimentsio baten salmenten lehentasunaren balioak dimentsio horren pisua adieraziko du salmenten prezioen edo faktura-tasen konfigurazioarekin bat datorrenean. **Salmenten lehentasuna** eremuaren balioak bakarra izan behar du **Salmentei aplikagarria** dimentsioetan.


[!INCLUDE[footer-include](../includes/footer-banner.md)]