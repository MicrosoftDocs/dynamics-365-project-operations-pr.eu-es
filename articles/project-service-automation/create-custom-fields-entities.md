---
title: Sortu eremu eta entitate pertsonalizatuak
description: Gai honetan Power Apps plataformako soluzioan aukera multzoak eta entitateak nola sortu azaltzen da.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748930"
---
# <a name="create-custom-fields-and-entities"></a>Sortu eremu eta entitate pertsonalizatuak 

Jarraitu urrats hauei aukera multzo edo entitate pertsonalizatu bat sortu nahi duzunean Power Apps plataforman.  
Gai honetako prozedurak Project Service Automation-en (PSA) web interfazea erabiliz osatu behar dira.

> [!IMPORTANT]
> Gomendatzen dugu prezio-dimentsio pertsonalizatuen aldaketa guztiak soluzio bereizi batean egitea. Praktika on garrantzitsu honek etorkizunean malgutasuna eskaintzen du aldaketak eguneratzeko edo kentzeko, zure lana berrerabiltzen lagunduko du eta aldaketak beste instantzia batera eramatea erraztuko du. Beharrezko aldaketa guztiak egin ondoren, esportatu soluzioa **kudeatutako soluzio** gisa, eta inportatu beste instantzia batzuetan zure prezioen konfigurazioa berrerabiltzeko.


## <a name="create-a-custom-solution-for-pricing-dimensions"></a>Sortu prezio-dimentsioetarako soluzio pertsonalizatua
1. PSAn, egin klik **Ezarpenak** > **Soluzioak** aukeran eta, ondoren, egin klik **Berria** aukeran soluzio berri bat sortzeko. 
2. Soluzioari eman **\<zure erakundearen izena> prezio-dimentsioak** izena, sartu gainerako beharrezko informazioa eta ondoren egin klik **Gorde** aukeran.

> ![Sortu prezio-dimentsioetarako soluzio pertsonalizatua](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>Sortu eremu pertsonalizatuak eta aukera multzoak prezio-dimentsioaren soluzioan

Prezio-dimentsioa aukera multzo edo entitate bat izan daiteke. Biak prezio-soluzioan sortu behar dira. Prozedura honen urratsek azaltzen dute nola sortu entitatean oinarritutako dimentsioak eta aukera multzoan oinarritutako dimentsioak.

### <a name="entity-based-dimensions"></a>Entitatean oinarritutako dimentsioak

1. PSAn egin klik **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **\<zure erakundearen izena> prezioen dimentsioak** atalean.
2. Soluzio arakatzailean, ezkerreko nabigazio panelean, hautatu **Entitateak**.
3. Egin klik **Berria** atalean **Titulu estandarra** izeneko entitate berria sortzeko. Sartu geratzen den informazioa eta, ondoren, egin klik **Gorde** aukeran.

> ![Titulu estandarraren entitatearen definizioa](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a>Aukera multzoetan oinarritutako dimentsioak 
Aukera multzoan oinarritutako bi dimentsio sor ditzakezu. **Baliabideen lanaren kokapena** entitatea **Hasiera** kokapen lanaren eta **Gunean** lanaren prezioaren jarraipena egiteko, eta erabili **Baliabideen lanorduak** entitatea **Ohiko** eta **Aparteko orduak** entitateetan lana amaitutakoan gainprezio bat aplikatzeko.


1. PSAn egin klik **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **\<zure erakundearen izena> prezioen dimentsioak** atalean. 
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

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a>Gehitu beharrezko PSA entitate guztiak eta horiekin lotutako osagaiak prezio-dimentsioaren soluzioan
Project Service-eko entitate hauek gehitu beharko dituzu prezio-soluzioan. Erabili prozedura honen urratsak prezio-soluzioaren eskema garrantzitsu batzuk egiteko, entitateak prezio-dimentsio berriez jabetzeko.

1. PSAn egin klik **Ezarpenak** > **Soluzioak** atalean eta ondoren egin klik bikoitza **\<zure erakundearen izena> prezioen dimentsioak** atalean. 
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

> ![Gehitu lehendik dauden entitateak prezio-dimentsioen soluzioari](media/Existing-entities-to-PD-solution.png)

> ![Hautatu soluzioaren osagaiak](media/Dimension-Components.png)

> [!NOTE]
> Ziurtatu aukeratutako erakunde bakoitzerako inprimaki eta ikuspegi guztiak sartzea.

4. Goiko hautatutako entitateen menpeko erakunderen bat eskatuko zaizunean, egin klik **Ez** aukeran.

> ![Ez sartu erlazionatutako osagaiak](media/Do-not-include-required.png)


