---
title: Proiektuen antolaketa
description: Gai honek antolaketa sortzeari buruzko informazioa ematen du.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 3/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: f0d052efda1b78161feed1c1e4cd70a31f3c4dea
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8915859"
---
# <a name="project-schedules"></a>Proiektuen antolaketa 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuaren antolaketak zein lan egin behar, zein baliabidek gauzatuko duen lana eta zein denbora-tartetan egingo den lana adierazten du. Proiektua garaiz entregatzearekin lotutako lan guztia islatzen du. Dynamics 365 Project Service Automation aplikazioan, proiektuaren antolaketa sortzen duzu lana zeregin kudeagarrietan zatituz, zeregin bakoitza egiteko behar den denbora kalkulatuz, zereginen mendekotasunak ezarriz, zereginen iraupenak ezarriz eta zereginak egingo dituzten baliabide generikoak aurreikusiz. Proiektuaren antolaketa proiektuaren orriko **Antolaketa** fitxan sortu da.
 
## <a name="tasks"></a>Zereginak

Proiektuaren antolaketa sortzeko lehen urratsa lana zati kudeagarrietan zatitzea da. PSA-ren antolaketak eginbide hauek onartzen ditu:

- Proiektuaren erroko nodoa
- Laburpena edo edukiontzi-zereginak
- Hosto-nodoaren zereginak

### <a name="project-root-node"></a>Proiektuaren erroko nodoa

Proiektuaren erro nodoa proiektuaren goi-mailako laburpen zeregina da. Gainerako proiektu-zereginak bere barnean sortzen dira. Erroko nodoaren izena ezartzen zaio proiektuaren izenari. Erroko nodoaren ahalegina, datak eta iraupena bere azpiko hierarkiako balioetan oinarrituta laburbiltzen dira. Ezin dituzu editutatu erroko nodoaren propietateak. Horretaz gain, ezin duzu erroko nodoa ezabatu.

### <a name="summary-or-container-tasks"></a>Laburpena edo edukiontzi-zereginak 

Laburpen-zereginek azpiatalak edo zeregin edukitzaileak dituzte. Ez dute lan ahaleginik edo kosturik. Horren ordez, beren lan esfortzua eta kostua zeregin edukitzaileen lan ahaleginaren eta kostuaren bateratzea da. Laburpen zereginaren hasiera-data zeregin edukitzailearen hasiera-data da, eta amaiera-data zeregin edukitzailearen amaiera-data da. Laburpen zeregin baten izena editatu daiteke, baina antolaketaren propietateak (ahalegina, datak eta iraupena) ezin dira editatu. Laburpen zeregin bat ezabatzen baduzu, bere zeregin edukiontzi guztiak ere ezabatuko dituzu.

### <a name="leaf-node-tasks"></a>Hosto-nodoaren zereginak

Hosto-nodoaren zereginek proiektuaren lan xehatuena adierazten du. Aurreikusitako ahalegina, baliabideak, antolatutako hasiera- eta amaiera-datak eta iraupena dituzte.
 
## <a name="creating-a-task-hierarchy"></a>Zereginen hierarkia bat sortzea

Aukera hauek erabiliz, zereginen hierarkia sor dezakezu:

- **Gehitu zeregina** botoia
- **Jarri koska zereginari** botoia
- **Kendu koska zereginari** botoia
- **Eraman gora** eta **Eraman behera** botoiak
- Erabilerraztasuna eta teklatuko lasterbideak

### <a name="add-task"></a>Gehitu zeregina

**Gehitu zeregina** botoiak hierarkian beste zeregin bat sortzeko aukera ematen dizu. Ez baduzu hautatzen posiziorik, zeregina amaieran gehituko da. 

Eginkizun bakoitzari antolaketaren ID bat esleitzen zaio. Antolaketaren IDak zereginak hierarkian duen sakontasuna eta kokapena adierazten du. Eskemako numerazioa erabiltzen du. Proiektuaren erroko nodoaren azpian dagoen lehen mailan dauden zereginetarako, 1, 2, 3 eta abar zenbakizko eskema erabiltzen da. Lehen mailaren azpian dauden zereginetarako, 1.1, 1.2, 1.3 eta abar zenbakizko eskema erabiltzen da.

### <a name="indent-task"></a>Jarri koska zereginari

Zeregin bati koska jartzen zaionean, zuzenean gainetik dagoen zereginaren bigarren mailako zeregin bihurtzen da. Zereginaren antolaketaren IDa berriro kalkulatuko da, nagusi berriaren antolaketaren IDan oinarrituta egon dadin eta eskemako zenbakizko eskema jarraitu dezan. Zeregin nagusia laburpen edo zeregin edukitzaile bat da orain. Hori dela eta, bigarren mailako zereginen bateraketa bihurtzen da.

### <a name="outdent-task"></a>Kendu koska zereginari 

Zeregin bati koska kentzean, ez da gehiago zeregin nagusiaren bigarren mailako zeregina izango. Antolaketaren IDa berriz kalkulatuko da zereginak hierarkian duen eguneratutako sakontasuna eta posizioa islatzeko. Aurreko zeregin nagusiaren esfortzua, kostua eta datak berriro kalkulatuko dira zeregin hori ez barneratzeko.

### <a name="move-up-and-move-down"></a>Eraman gora eta Eraman behera 

**Eraman gora** eta **Eraman behera** botoiek zeregin baten kokapena aldatzen dute nagusien hierarkian. Mota honetako aldaketek ez dute eraginik zereginen ahaleginean, kostuan, datuetan edo iraupenean. Zereginen antolaketaren IDean bakarrik du eragina. Antolaketaren IDa berriz kalkulatuko da zereginaren posizio berria islatzeko zeregin nagusien bigarren mailako zereginen zerrendan.

### <a name="accessibility-and-keyboard-shortcuts"></a>Erabilerraztasuna eta teklatuko lasterbideak

**Antolaketa** sareta guztiz eskuragarria da eta pantaila-irakurleekin erabil daiteke, esaterako, JAWS edo NVDA. Saretako eremuan mugi zaitezke gezi-teklak erabiliz (Microsoft Excel-en bezala), Tab tekla erabil dezakezu interfazearen UI elementutan aurrera egiteko, eta Behera gezi-tekla, Sartu tekla edo Zuriune-barra erabil ditzakezu goitibeherako menuak hautatzeko eta deitzeko. Zutabeen goiburuak ere interaktiboak dira. Zutabeak ezkutatu eta erakusteko, erabili Tab tekla eta gezi-teklak zutabeetako goiburuetatik mugitzeko eta erabili tresna-barrako ekintza-botoiak. Gainera, honako laster-tekla hauek erabil ditzakezu:

- **Freskatu**: ALT+MAIUS+F5
- **Gehitu**: ALT+MAIUS+Txertatu
- **Ezabatu**: ALT+MAIUS+Ezabatu
- **Mugitu gora/behera**: ALT+MAIUS+Gora/Behera geziak
- **Jarri koska / Kendu koska**: ALT_MAIUS+Ezker/Eskuineko geziak
- **Hedatu/Tolestu hierarkiak**: ALT+MAIUS+Gehi/Ken teklak

## <a name="task-attributes"></a>Zeregin-atributuak

Zereginaren izenak egin beha den lana deskribatzen du. PSA-n, zeregin bati lotuta dauden atributuek zereginaren antolaketa eta langileen eskakizunak deskribatzen dituzte.

> ![Zeregin-atributuak.](media/project-2.png)
 
### <a name="schedule-attributes"></a>Antolaketa-atributuak

**Ahalegina**, **Hasiera-data**, **Amaiera-data**, eta **Iraupena** atributuek zereginaren antolaketa zehazten dute.

Antolaketa atributu gehigarrien artean hauek daude:

- **Ahalegin orduak**: idatzi zeregina burutzeko behar diren orduen aurreikuspena. 
- **Iraupena**: zehaztu zeregina burutzeko behar den lanegun kopurua.
- **Antolaketaren IDa**: automatikoki sortutako ID hau hierarkian zereginak ordenatzeko erabiltzen da. Zereginen arteko mendekotasunak atazak lantzen diren benetako ordena kudeatzen du.
 
### <a name="staffing-attributes"></a>Betetze-atributuak

Langileen atributuak **Baliabideak** eremuaren bidez atzitzen dira antolaketan. Lehendik dagoen baliabide bat bilatu dezakezu edo egin klik **Sortu** aukeran eta **Sorrera bizkorra** panelean, gehitu proiektu-taldeko kide bat baliabide berri gisa.

**Funtzioa**, **Baliabide-unitatea**, eta **Lanpostuaren izena** eremuak zereginerako langileen eskakizunak deskribatzeko erabiltzen dira. Langileen atributu horiek, zereginen antolaketarekin batera, zeregina egiteko erabilgarri dauden baliabideak aurkitzeko erabiltzen dira.

**Funtzioa** - Zehaztu zeregina egiteko behar den baliabide mota.

**Baliabide-unitatea** - Zehaztu zeregineko baliabideak zein unitatetik esletiu behar diren. Atributu horrek zereginerako kostuen eta salmenten aurreikuspenean eragiten du baliabidearen kostua eta faktura-tasa baliabide unitateetan oinarrituta ezartzen badira.

**Lanpostuaren izena** - Idatzi lana egingo duen baliabiderako leku-marka gisa balio duen baliabe orokorrerako lagunarteko izena.

**Baliabideak** eremuan aurkitzen da baliabide generikoaren edo izendatutako baliabidearen posizioaren izena bat aurkitzen denean.

**Kategoria** zereginak taldekatu dezakeen lan mota zabalagoa adierazten duten balioak gordetzen ditu. Eremu horrek ez du eraginik antolaketan edo langileengan. Txostenak egiteko soilik erabiltzen da.

### <a name="task-dependencies"></a>Zeregin-mendekotasunak 

PSA-ko antolaketa erabil dezakezu zereginen arteko aurreneko harremanak sortzeko. **Aurrekoak** eremua, **Zereginak** atalaren barrukoak, balio bat edo gehiago hartzen ditu zeregin baten menpe dauden zereginak adierazteko. Zeregin bati aurrenekoen balioak esleitzean, zeregina aurreko zeregin guztiak osatu direnean soilik abiarazi daiteke. Mendekotasuna dela eta, zereginaren aurreikusitako hasiera-data aurreko zereginak bukatzen diren datara berrezarriko da.

Zereginaren moduak ez du eraginik aurreko/mendeko zereginen hasiera- eta amaiera-datetan egiten diren eguneratzeetan.

## <a name="task-mode"></a>Zeregin modua 

Zereginaren moduak hosto-nodoen zereginen programazioa zehazten du. PSA-k zeregin bakoitzerako bi zeregin modu onartzen ditu: antolaketa automatikoa eta eskuzko antolaketa.

### <a name="auto-scheduling"></a>Antolaketa automatikoa 
 
Zereginaren modua **Automatikoki antolatuta** gisa ezartzen duzunean zeregin baterako, zeregina antolatzeko motorrak antolaketa-arauak erabiltzen ditu zeregin-atributu horietan zereginaren antolaketa zehazteko.

#### <a name="scheduling-rules"></a>Antolaketa-arauak

Modu lehenetsian, hosto-nodoaren zereginak aurrekaririk ez badu, haren hasiera-data proiektuaren antolaketarako planifikatutako hasiera-data izango da. Hosto-nodoaren zereginaren iraupena hasiera- eta amaiera-datuen arteko lan-egun kopuru gisa kalkulatzen da beti. Zeregina automatikoki antolatzen denean, antolaketa-motorrak arau hauei jarraitzen die:

- Zereginen hasiera- eta amaiera-datek lanegunak izan behar dute, proiektuaren antolaketa-egutegiaren arabera. 
- Aurreko zereginak dituen edozein zereginerako, hasiera-data bere aurrekarien azken amaiera-dataren berdina izango da.
- Ahalegina formula hau erabiliz kalkulatzen da: Pertsona kopurua × Iraupena × Orduak proiektuko egutegiko lanaldi estandarrean.

### <a name="manual-scheduling"></a>Eskuzko antolaketa

Planifikazio automatikoaren arauak zure baldintzak betetzen ez badituzu, zereginerako modua alda dezakezu **Eskuz programatuta** modura. Ezarpen horrek beste antolaketa-atributu batzuen balioak kalkulatzea eragozten dio antolaketa-motorrari. Zereginaren modua edozein dela ere, zereginetan aurrekoak ezartzen badituzu, beti eragomgp dio menpeko zereginaren hasiera-datari.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
