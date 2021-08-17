---
title: Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa
description: Gai honek aukera multzo pertsonalizatuak edo entitateak nola sortu jakiteko informazioa eskaintzen du.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 40a6a4173cb0e4d7ea5bcf24c8954fe9d7e079d1e9ecf4aac252b5133f12d3ff
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7003621"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a>Sortu eremu eta entitate pertsonalizatuak prezio-dimentsio gisa

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean prezio-dimentsio gisa erabiltzeko. Informazio gehiago lortzeko, ikusi [Prezio-dimentsioen informazio orokorra](pricing-dimensions-overview.md).  

> [!IMPORTANT]
> Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea. Praktika on garrantzitsu honek malgutasuna eskaintzen du etorkizunean aldaketak beharren arabera eguneratu edo kentzeko. Horrek zure lana berrerabiltzen lagunduko du eta aldaketa hauek beste instantzia batera eramatea erraztuko du Eskatutako aldaketa guztiak egin ondoren, esportatu irtenbide hau **Kudeatutako soluzioa** eta inportatu beste instantzia batzuetara zure prezioen konfigurazioa berrerabiltzeko.

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan

Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke. Biak prezio-soluzioan sortu behar dira. Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.

### <a name="entity-based-dimensions"></a>Entitatean oinarritutako dimentsioak
Entitateetan oinarritutako dimentsioak sortzeko, jarraitu urrats hauei:

1. Joan **Ezarpenak** > **Soluzioak** aukerara eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.
3. Hautatu **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko. 
4. Sartu geratzen den informazioa eta, ondoren, hautatu **Gorde** aukeran.

> ![Titulu estandarraren entitatearen definizioa.](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a>Aukera multzoetan oinarritutako dimentsioak 
Aukera multzoan oinarritutako bi dimentsio sor ditzakezu. 

- Erabili **Baliabideen lanaren kokapena** prezioaren jarraipena egiteko **Etxea** kokapen lana eta **Gunean** lana. 
- Erabili **Baliabideen lan orduak** balioekin **Erregularra** eta **Aparteko orduak** lana amaitutakoan marka bat aplikatzeko.

Ondorengo grafikoan **Baliabideen lanaren kokapena** dimentsioa. 

> ![Baliabideen lanaren kokalekua izeneko aukera multzoan oinarritutako prezio-dimentsioa.](media/Option-set-PD-called-Resource-Work-Location.png)

Ondorengo grafikoan **Baliabideen lan-orduak** dimentsioa. 

> ![Baliabideen lanorduen izeneko aukera multzoan oinarritutako prezio-dimentsioa.](media/Option-set-PD-called-Resource-Work-Hours.png)

1. Joan **Ezarpenak** > **Soluzioak** aukerara eta sakatu bi aldiz **\<your organization name> prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio-panelean, hautatu **Aukera multzoak**. 
3. Hautatu **Berria** aukeran aukera multzo berri bat sortzeko, sartu falta den informazioa eta hautatu **Gorde** aukeran.

## <a name="create-data-for-entity-based-dimensions"></a>Sortu datuak erakundeetan oinarritutako dimentsioetarako

Erakundeetan oinarritutako dimentsioetarako datuak sor ditzakezu eskuz edo Microsoft Excel inportazio edo zerbitzu deiak erabiliz. Erabili prozedura honen urratsak bi titulu estandar sortzeko, adibidez, **Sistemen ingeniaria** eta **Sistemen ingeniari nagusia**, **Titulu estandarra** entitatean oinarritutako dimentsiotik. Sortu nahi dituzun datuak txikiak badira, hurrengo adibidean bezala, inprimaki estandarra erabil dezakezu.

1. Hautatu **Bilaketa aurreratua** atalera.
2. Hautatu entitatea eta, ondoren, **Titulu estandarra** atalean, hautatu **Emaitzak**. **Titulu estandarra** entitateko errenkada guztiak erakutsiko dira.
3. Hautatu **Berria**, eta **Izena** atalean, idatzi "Sistemen ingeniaria" eta, ondoren, hautatu **Gorde**.
4. Itxi orria. 
5. Errepikatu 1-3 urratsak "Sistemen ingeniari nagusia" titulu estandarra sortzeko.

> ![Titulu estandarraren entitatearen datuen laginak.](media/ST-data.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]