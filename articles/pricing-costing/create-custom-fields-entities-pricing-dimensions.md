---
title: Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa
description: Gai honek aukera multzo pertsonalizatuak edo entitateak nola sortu jakiteko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 616bcd5758b434b45bd06aa1a026f32efc8b7f99
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130878"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a>Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean.

> [!IMPORTANT]
> Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea. Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du. Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.


## <a name="create-a-custom-solution-for-pricing-dimensions"></a>Sortu prezio-dimentsioetarako soluzio pertsonalizatua
1. Joan **Ezarpenak** > **Soluzioak** aukerara eta, ondoren, hautatu **Berria** aukeran soluzio berri bat sortzeko. 
2. Soluzioari eman **\<your organization name> prezio-dimentsioak** izena, sartu gainerako beharrezko informazioa eta, ondoren, hautatu **Gorde** aukeran.
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan

Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke. Biak prezio-soluzioan sortu behar dira. Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.

### <a name="entity-based-dimensions"></a>Entitatean oinarritutako dimentsioak

1. Joan **Ezarpenak** > **Soluzioak** aukerara eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.
3. Hautatu **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko. 
4. Sartu geratzen den informazioa eta, ondoren, hautatu **Gorde** aukeran.


### <a name="option-set-based-dimensions"></a>Aukera multzoetan oinarritutako dimentsioak 
Aukera multzoan oinarritutako bi dimentsio sor ditzakezu. **Baliabideen lanaren kokapena** entitatea **Hasiera** kokapen lanaren eta **Gunean** lanaren prezioaren jarraipena egiteko, eta erabili **Baliabideen lanorduak** entitatea **Ohiko** eta **Aparteko orduak** entitateetan lana amaitutakoan gainprezio bat aplikatzeko.


1. Joan **Ezarpenak** > **Soluzioak** aukerara eta sakatu bi aldiz **\<your organization name> prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio-panelean, hautatu **Aukera multzoak**. 
3. Hautatu **Berria** aukeran aukera multzo berri bat sortzeko, sartu falta den informazioa eta hautatu **Gorde** aukeran.

## <a name="create-data-for-entity-based-dimensions"></a>Sortu datuak erakundeetan oinarritutako dimentsioetarako

Erakundeetan oinarritutako dimentsioetarako datuak sor ditzakezu eskuz edo Microsoft Excel inportazio edo zerbitzu deiak erabiliz. Erabili prozedura honen urratsak bi titulu estandar sortzeko, adibidez, **Sistemen ingeniaria** eta **Sistemen ingeniari nagusia**, **Titulu estandarra** entitatean oinarritutako dimentsiotik. Sortu nahi dituzun datuak txikiak badira, hurrengo adibidean bezala, inprimaki estandarra erabil dezakezu.

1. Hautatu **Bilaketa aurreratua**, hautatu entitatea **Izenburu estandarra** eta, ondoren, hautatu **Emaitzak**. **Titulu estandarra** entitateko errenkada guztiak erakutsiko dira.
2. Hautatu **Berria**, eta **Izena** atalean, idatzi "Sistemen ingeniaria" eta, ondoren, hautatu **Gorde**.
3. Itxi inprimakia. 
4. Errepikatu 1-3 urratsak "Sistemen ingeniari nagusia" titulu estandarra sortzeko.

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a>Gehitu beharrezko entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan
Entitate hauek gehitu beharko dituzu prezio-soluzioan. Erabili prozedura honen urratsak prezio-soluzioaren eskema garrantzitsu batzuk egiteko, entitateak prezio-dimentsio berriez jabetzeko.

1. Hautatu **Ezarpenak** > **Soluzioak** eta sakatu bi aldiz **\<your organization name> prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Gehitu badaudenak** > **Entitateak**.
3. **Soluzio-osagaiak** elkarrizketa-koadroan, hautatu aukera hauetariko bat:

  - Benetakoa
  - Baliabide erreserbagarria
  - Aurreikuspenaren lerroa
  - Fakturaren lerroaren xehetasunak
  - Kutxako liburuaren lerroa
  - Proiektu-kontratuaren lerroko xehetasunak
  - Proiektu-taldeko kidea
  - Eskaintzaren lerroaren xehetasunak
  - Funtzio-prezioaren gainprezioa
  - Funtzioaren prezioa 
  - Denbora-sarrera 


> [!NOTE]
> Ziurtatu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak sartzea.

4. Goiko hautatutako entitateen menpeko erakunderen bat eskatuko zaizunean, hautatu **Ez** aukeran.

