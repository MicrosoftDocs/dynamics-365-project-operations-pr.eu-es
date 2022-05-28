---
title: Sortu zereginen xehetasunen egitura
description: Gai honetan azaltzen da nola sortu lanaren matxuraren egitura (WBS) oinarrizko kontrolak barne antolaketa-interfaze berrian.
author: ruhercul
ms.date: 12/16/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: cdc1ffdd1f53f65627b511582e52ca27fa53c127
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8597783"
---
# <a name="create-a-work-breakdown-structure-wbs"></a>Sortu zereginen xehetasunen egitura (WBS)

Proiektuaren antolaketak zein lan egin behar, zein baliabidek osatuko duen lana eta zein denbora-tartetan egingo den lana adierazten du. Antolaketak proiektua garaiz entregatzearekin lotutako lan guztia islatzen du. Dynamics 365 Project Operations-en, proiektuaren egutegia sortzen duzu honela:

  - Lana zeregin kudeagarritan zatitzea.
  - Zeregin bakoitza egiteko behar den denbora kalkulatzea.
  - Zereginen mendekotasunak ezartzea.
  - Zereginen iraupenak ezartzea.
  - Zereginak egingo dituzten baliabide generikoak kalkulatzea. 

Proiektuaren antolaketa **Proiektua** orriko **Antolaketa** fitxan sortu da.

## <a name="tasks"></a>Zereginak

Proiektuaren antolaketa sortzeko lehen urratsa lana zati kudeagarrietan zatitzea da. Project Operations-en antolaketak eginbide hauek onartzen ditu:

- Laburpena edo edukiontzi-zereginak
- Hosto-nodoaren zereginak

### <a name="summary-tasks"></a>Laburpen-zereginak

Laburpen-zereginek laburpen-zereginak edo hosto-nodoak gorde ditzakete. Ez dute lan ahaleginik edo kosturik. Horren ordez, beren lan esfortzua eta kostua zeregin edukitzaileen lan ahaleginaren eta kostuaren bateratzea da. Laburpen zereginaren hasiera-data zeregin edukitzailearen hasiera-data da, eta amaiera-data zeregin edukitzailearen amaiera-data da. Laburpen zeregin baten izena editatu daiteke, baina antolaketaren propietateak (ahalegina, datak eta iraupena barne) ezin dira editatu. Laburpen zeregin bat ezabatzen baduzu, bere zeregin edukiontzi guztiak ere ezabatuko dituzu.

### <a name="leaf-node-tasks"></a>Hosto-nodoaren zereginak

Hosto-nodoaren zereginek proiektuaren lan xehatuena adierazten du. Aurreikusitako ahalegina, baliabideak, antolatutako hasiera- eta amaiera-datak eta iraupena dituzte.

## <a name="create-a-task-hierarchy"></a>Sortu zereginen hierarkia

### <a name="add-a-task"></a>Gehitu zeregina

Osatu urrats hauek zeregin bat edo gehiago gehitzeko.

1. Joan **Proiektuak** aukerara eta hautatu eta ireki egutegia sortu nahi duzun proiektuaren erregistroa. 
2. Hautatu **Zereginak** fitxa. 
3. Aukeratu **Gehitu zeregin berria**, idatzi zereginaren izena eta sakatu Sartu.
2. Idatzi beste zeregin baten izena eta sakatu Sartu berriro zereginen zerrenda osoa izan arte.

### <a name="manage-hierarchy-of-a-task"></a>Kudeatu zeregin baten hierarkia

Zeregin bati koska jartzen zaionean, zuzenean gainetik dagoen zereginaren bigarren mailako zeregin bihurtzen da. Zereginaren antolaketaren IDa berriro kalkulatuko da, nagusi berriaren antolaketaren IDan oinarrituta egon dadin eta eskemako zenbakizko eskema jarraitu dezan. Guraso zeregina laburpen zeregina da orain. Hori dela eta, bigarren mailako zereginen bateraketa bihurtzen da. Zeregin bat mailaz igotzean, ez da gehiago zeregin nagusiaren bigarren mailako zeregina izango. Antolaketaren IDa berriz kalkulatuko da zereginak hierarkian duen eguneratutako sakontasuna eta posizioa islatzeko. Aurreko zeregin nagusiaren esfortzua, kostua eta datak berriro kalkulatuko dira zeregin hori ez barneratzeko.

Osatu urrats hauek zeregina mailaz jaitsi edo igotzeko.

1. **Proiektua** orriko **Zereginak** fitxan, **Laburpen-zereginak** aukeran, hautatu hiru puntu bertikalak atazaren izenaren arabera, eta hautatu **Egin azpiataza**. 
2. Aukeratu koska edo sustatu beharreko zeregina. Zeregin bat baino gehiago hautatzeko, hautatu zeregin bat, luze sakatu Ktrl, eta hautatu zeregin osagarriak.
2. Hautatu **Jaitsi mailaz** edo **Sustatu azpiataza** zereginak laburpen-zereginetara eramateko edo haietatik ateratzeko.

### <a name="move-tasks-up-and-down"></a>Eraman zereginak gora eta behera

Zereginak lanaren banakako egituraren edozein mailara eraman nitzake bi modu hauetako batean:

- Aukeratu zeregin bat gehiago eta arrastatu nahi duzun lekura.
- Aukeratu zeregin bat edo gehiago, egin klik eskuineko botoiarekin eta hautatu **Ebaki**, hautatu helburuko gelaxka programazioan, eta egin klik eskuineko botoiarekin eta hautatu **Itsatsi**.

## <a name="task-attributes"></a>Zeregin-atributuak

Zereginaren izenak egin beha den lana deskribatzen du. Project Operations-en, zeregin bati lotuta dauden atributuek zereginaren antolaketa eta langileen eskakizunak deskribatzen dituzte.

## <a name="schedule-attributes"></a>Antolaketa-atributuak

**Ahalegina**, **Hasiera-data**, **Amaiera-data**, eta **Iraupena** atributuek zereginaren antolaketa zehazten dute.

Hurrengo taulan ordutegiaren atributu osagarriak agertzen dira.

| **Azken bistaratzeko izena** | **Azken azalpena** |
| --- | --- |
| Egindako ahalegina (orduak) | Zereginaren amaitutako lana ordutan. |
| Iraupena | Zereginaren iraupena bistaratzen du egunetan. |
| Ahalegina, guztira | Zereginaren lan kopurua, guztira, orduetan. |
| Amaitu | Amaiera-data eta -ordua. |
| Osatutako ehunekoa (%) | Osatutako atazaren ehunekoa. |
| Proiektuaren ontzia | Ontzien arabera sailka daiteke zereginaren panela; horrela, ontzi bakoitzak zutabe bat dauka. |
| Geratzen den ahalegina (orduak) | Zereginaren geratzen den lana ordutan. |
| Hasi | Hasiera-data eta -ordua. |
| Izena | Zereginaren izena. |
| ID | Zereginen xehetasunen egiturako zereginaren IDa. |

Administratzaile gisa, eremu pertsonalizatuak defini ditzakezu atazako entitatean. Hala ere, eremuak ezin dira programazio-saretan bistaratu. Zure eremu pertsonalizatuak ikusteko, gehitu **Proiektuaren zeregina** xehetasunen orria.

## <a name="staffing-attributes"></a>Betetze-atributuak

Langileen atributuak **Baliabideak** eremuaren bidez atzitzen dira antolaketan. Lehendik dagoen baliabide bat bilatu dezakezu edo hautatu **Sortu** eta **Sorrera bizkorra** panelean, gehitu proiektu-taldeko kide bat baliabide berri gisa.  Ataza-sareko, arbel-ikuspeko edo gantt-eko baliabide-hautatzailea erabiliz baliabide bat bilatzen duzunean, bilaketak lehendik dauden proiektuko taldeko kideak edo erreserba daitezkeen baliabide aktiboak itzultzen ditu.

**Funtzioa**, **Baliabide-unitatea**, eta **Lanpostuaren izena** eremuak zereginerako langileen eskakizunak deskribatzeko erabiltzen dira. Langileen atributu horiek, zereginen antolaketarekin batera, zeregina egiteko erabilgarri dauden baliabideak aurkitzeko erabiltzen dira.

   - **Rola** : Zehaztu zeregina egiteko behar den baliabide mota.,
   - **Baliabide-unitatea**: Zehaztu zeregineko baliabideak zein unitatetik esleitu behar diren. Atributu horrek zereginerako kostuen eta salmenten aurreikuspenean eragiten du baliabidearen kostua eta faktura-tasa baliabide unitateetan oinarrituta ezartzen badira.
   - **Lanpostuaren izena**: idatzi lana egingo duen baliabiderako leku-marka gisa balio duen baliabide orokorrerako izena.

**Baliabideak** eremuan aurkitzen da baliabide generikoaren edo izendatutako baliabidearen posizioaren izena bat aurkitzen denean.

**Kategoria** zereginak taldekatu dezakeen lan mota zabalagoa adierazten duten balioak gordetzen ditu. Eremu horrek ez du eraginik antolaketan edo langileengan. Horren ordez, eremua txostenak egiteko soilik erabiltzen da.

## <a name="task-dependencies"></a>Zeregin-mendekotasunak

Project Operations-eko antolaketa erabil dezakezu zereginen arteko aurreneko harremanak sortzeko. **Aurrekoak** eremuak balio bat edo gehiago erabiltzen ditu zeregin baten menpe dauden zereginak adierazteko. Zeregin bati aurrenekoen balioak esleitzean, zeregina aurreko zeregin guztiak osatu direnean soilik abiarazi daiteke. Mendekotasuna dela eta, zereginaren aurreikusitako hasiera-data aurreko zereginak bukatzen diren datara berrezarriko da.

Zereginaren moduak ez du eraginik aurreko/mendeko zereginen hasiera- eta amaiera-datetan egiten diren eguneratzeetan.

## <a name="accessibility-and-keyboard-shortcuts"></a>Erabilerraztasuna eta teklatuko lasterbideak

**Antolaketa** sareta guztiz eskuragarria da eta pantaila-irakurleekin erabil daiteke, esaterako, JAWS edo NVDA. Saretako eremuan mugi zaitezke gezi-teklak erabiliz (Microsoft Excel-en bezala), Tab tekla erabil dezakezu interfazearen erabiltzaile-interfazearen elementutan aurrera egiteko, eta Behera gezi-tekla, Sartu tekla edo Zuriune-barra erabil ditzakezu goitibeherako menuak hautatzeko eta irekitzeko.

## <a name="project-limitations"></a>Proiektuaren mugak 
Ondoko mugak ezagutu behar dituzu Project Operations-en zereginen xehetasunen egitura erabiltzen ari bazara. Muga hauek proiektu eta zereginei aplikatzen zaizkie. Informazio gehiagorako, ikusi [Project for the Web-en mugak](/project-for-the-web/project-for-the-web-limits-and-boundaries).

| **Eremua**                                          |  **Muga**           |
|----------------------------------------------------|----------------------|
| Proiektu baterako gehieneko zereginak                  | 500                  |
| Proiektu baten gehieneko iraupena               | 3650 egun (10 urte) |
| Proiektu baterako gehieneko baliabideak              | 300                  |
| Proiektu bateko gehieneko estekak (ondorengoak soilik) | 600                  |
| Proiektu baterako gehieneko eremu pertsonalizatuak          | 1,0                   |
| Gehienezko zerrendako elementuak zeregin bakoitzeko                   | 20                   |

**Zereginen mugak**

| **Eremua**                               |   **Muga**           |
|-----------------------------------------|-----------------------|
| Gehieneko hierarkia-maila                 | 10 maila             |
| Gehieneko estekak (ondorengoa + aurrekoa) | 20                    |
| Hosto-zereginaren gehienezko iraupena           | 1250 egun             |
| Laburpen-zeregin baten gehieneko iraupena      | 3650 egun (10 urte)  |
| Zeregin bati esleitutako gehieneko baliabideak    | 20 baliabide          |
| Zeregin baterako onartutako data-tartea         | 2000/1/1 - 2149/12/31 |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
