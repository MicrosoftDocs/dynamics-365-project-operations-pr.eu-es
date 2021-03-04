---
title: Sortu eremu eta entitate pertsonalizatuak
description: Gai honetan Power Apps plataformako soluzioan aukera multzoak eta entitateak nola sortu azaltzen da.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
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
ms.openlocfilehash: b9e32c8871a8986ba827f742baf4e4d5cd9dd235
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144848"
---
# <a name="create-custom-fields-and-entities"></a>Sortu eremu eta entitate pertsonalizatuak 

[!include [banner](../includes/psa-now-project-operations.md)]

Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean Power Apps plataforman.  
Gai honetako prozedurak Project Service Automation-en (PSA) web interfazea erabiliz osatu behar dira.

> [!IMPORTANT]
> Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea. Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du. Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan

Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke. Biak prezio-soluzioan sortu behar dira. Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.

### <a name="entity-based-dimensions"></a>Entitatean oinarritutako dimentsioak

1. PSAn, sakatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**.
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.
3. Egin klik **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko. Sartu geratzen den informazioa eta, ondoren, egin klik **Gorde** aukeran.

> ![Titulu estandarraren entitatearen definizioa](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a>Aukera multzoetan oinarritutako dimentsioak 
Aukera multzoan oinarritutako bi dimentsio sor ditzakezu. **Baliabideen lanaren kokapena** entitatea **Hasiera** kokapen lanaren eta **Gunean** lanaren prezioaren jarraipena egiteko, eta erabili **Baliabideen lanorduak** entitatea **Ohiko** eta **Aparteko orduak** entitateetan lana amaitutakoan gainprezio bat aplikatzeko.


1. PSAn, sakatu **Ezarpenak** > **Soluzioak** eta, ondoren, sakatu bi aldiz **\<your organization name> prezio-dimentsioa**. 
2. Soluzio arakatzailean, ezkerreko nabigazio-panelean, hautatu **Aukera multzoak**. 
3. Egin klik **Berria** aukeran aukera multzo berri bat sortzeko, sartu falta den informazioa eta egin klik **Gorde** aukeran.

> ![Baliabideen lanaren kokalekua izeneko aukera multzoan oinarritutako prezio-dimentsioa ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![Baliabideen lanorduen izeneko aukera multzoan oinarritutako prezio-dimentsioa ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a>Sortu datuak erakundeetan oinarritutako dimentsioetarako

Erakundeetan oinarritutako dimentsioetarako datuak sor ditzakezu eskuz edo Microsoft Excel inportazio edo zerbitzu deiak erabiliz. Erabili prozedura honen urratsak bi titulu estandar sortzeko, adibidez, **Sistemen ingeniaria** eta **Sistemen ingeniari nagusia**, **Titulu estandarra** entitatean oinarritutako dimentsiotik. Sortu nahi dituzun datuak txikiak badira, hurrengo adibidean bezala, inprimaki estandarra erabil dezakezu.

1. PSAn, sakatu **Bilaketa aurreratua**. Hautatu entitatea eta, ondoren, **Titulu estandarra** atalean, sakatu **Emaitzak**. **Titulu estandarra** entitateko errenkada guztiak erakutsiko dira.
2. Sakatu **Berria**. **Izena** atalean, idatzi "Sistemen ingeniaria" eta, ondoren, sakatu **Gorde**.
3. Itxi inprimakia. 
4. Errepikatu 1-3 urratsak "Sistemen ingeniari nagusia" titulu estandarra sortzeko.

> ![Titulu estandarraren entitatearen laginak ](media/ST-data.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]