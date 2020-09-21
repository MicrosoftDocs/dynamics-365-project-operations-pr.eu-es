---
title: Bertsio-berritzeko gogoetak. Microsoft Dynamics 365 Project Service Automation aplikazioaren 2.x edo 1.x bertsiotik 3. bertsiora
description: Gai honek Project Service Automation aplikazioaren 2.x edo 1.x bertsiotik 3. bertsiora bertsio-berritzean egin behar dituzun gogoetei buruzko informazioa ematen du.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 11/13/2018
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x
author: JohnPBurrows
ms.assetid: e4fae2ea-9013-488e-a666-f7192dd42c0b
ms.author: john.burrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: ba710eb8c07df7dac97e8b911184c00b87b14548
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748899"
---
# <a name="upgrade-considerations---psa-version-2x-or-1x-to-version-3"></a>Bertsio-berritzeko gogoetak. PSA aplikazioaren 2.x edo 1.x bertsiotik 3. bertsiora
[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="project-service-automation-and-field-service"></a>Project Service Automation eta Field Service
Dynamics 365 Project Service Automation eta Dynamics 365 Field Service aplikazioek Universal Resourcing Scheduling (URS) soluzioa erabiltzen dute baliabideak antolatzeko. Zure instantzian Project Service Automation eta Field Service badituzu, bi soluzioak bertsio-berritu beharko zenituzke azken bertsiora (Project Service Automation-en 3.x bertsioa eta Field Service-ren 8.x bertsioa). Project Service Automation edo Field Service eguneratzeak URS-ren azken bertsioa instalatuko du. Horrek esan nahi du portaera inkoherenteak egon daitezkeela Project Service Automation eta Field Service soluzioak azken bertsiora bertsio-berritzen ez badira.

## <a name="resource-assignments"></a>Baliabide-esleipenak
Project Service Automation aplikazioaren 2. bertsioan eta 1. bertsioan, zereginen esleipenak bigarren mailako zeregin gisa (lineako zereginak ere deitzen dira) gorde ziren **Zereginen entitatea** atalean, eta zeharka erlazionatuta daude **Baliabideen esleipena** erakundearekin. Lineako zeregina ikusgai zegoen Work Breakdown Structure (WBS) zerbitzuko leiho gainerakorrean.

![Project Service Automation 2. bertsioko eta 1. bertsioko WBSko lerro-zereginak](media/upgrade-line-task-01.png)

Project Service Automation aplikazioaren 3. bertsioan, baliabide erreserbagarriak zereginei esleitzeko azpiko eskema aldatu da. Lerroko zeregina zaharkitu egin da eta 1:1 erlazio zuzena dago **Zereginen entitatea** eremuko zereginaren eta **Baliabideen esleipena** entitateko taldekidearen artean. Proiektu-taldeko kide bati esleitzen zaizkion zereginak zuzenean gordetzen dira "Baliabideen esleipena" entitatean.  

Aldaketa horiek eragina dute projektu talde batean erreserbagarriak diren baliabide izendatuetarako eta baliabide orokorretarako baliabide-esleipena duten lehendik dagoen edozein proiekturen bertsio-berritzean. Gai honek 3. bertsiora eguneratzen duzunean proiektuan kontuan hartu beharko dituzun puntuak zeintzuk diren erakusten du. 

### <a name="tasks-assigned-to-named-resources"></a>Izendatutako baliabideei esleitutako zereginak
Azpiko zereginen entitatea erabiliz, 2. bertsioan eta 1. bertsioan egin ziren zereginei esker, taldekideek lehenetsitako zereginaz gain beste funtzio bat har zezaketen. Adibidez, Rakel Eguzkiagirreri, modu lehentsian programa-kudeatzailearen funtzioa esleitu zitzaionari, garatzailearen eginkizuna duen zeregin bat esleitu ziezaioken. 3. bertsioan, izendatutako taldekide baten eginkizuna lehenetsia da beti. Beraz, Rakel Eguzkiagirreri esleitzen zaion edozein zereginek programa-kudeatzailearen eginkizun lehenetsia erabiltzen du.

2. bertsioan eta 1. bertsioan baliabide bati funtzio lehenetsitik kanpoko zeregin bat esleitu baduzu, bertsio-berritzean, izendatutako baliabideari zereginen esleipen guztientzako eginkizun lehenetsia emango zaio, 2. bertsioko funtzioen esleipena kontuan izan gabe. Horrek kalkulatutako estimazioen aldeak ekarriko ditu 2. bertsiotik edo 1. bertsiotik 3. bertsiora pasatzean, estimazioak baliabidearen funtzioaren arabera kalkulatzen baitira eta ez lerroaren zereginaren esleipenaren arabera. Adibidez, 2. bertsioan bi zeregin esleitu zaizkio Nerea Ibarrondori. 1. zereginaren lerroko zereginaren funtzioa garatzailea da eta 2. zereginarena, programa-kudeatzailea. Nerea Ibarrondok programa-kudeatzailearen funtzio lehenetsia du.

![Baliabide bati esleitutako funtzio anitzak](media/upgrade-multiple-roles-02.png)

Garatzaile eta programa-kudeatzaile funtzioak desberdinak direnez, hauek dira kostuen eta salmenten kalkuluak:

![Baliabideen funtzioen kostuen kalkuluak](media/upggrade-cost-estimates-03.png)

![Baliabideen funtzioen salmenten kalkuluak](media/upgrade-sales-estimates-04.png)

3. bertsiora bertsio-berritzean, lerroko zereginak baliabideen esleipenekin ordezkatuko dira baliabide erreserbagarriko taldekidearen zereginean. Esleipenak baliabide erreserbagarriaren eginkizun lehenetsia erabiliko du. Hurrengo grafikoan, programa-kudeatzailea funtzioa duen Nerea Ibarrondo, baliabidea agertzen da.

![Baliabide-esleipenak](media/resource-assignment-v2-05.png)

Estimazioak baliabidearen funtzio lehenetsian oinarrituta daudenez, salmenten eta kostuen kalkuluak aldatu egin daitezke. Kontuan izan hurrengo grafikoan ez duzula ikusten **Garatzailea** funtzioa, orain, baliabide erreserbagarriaren lehenetsitako funtziotik hartzen baita.

![Funtzio lehenetsien kostuen kalkuluak](media/resource-assignment-cost-estimate-06.png)
![Funtzio lehenetsien salmenten kalkulua](media/resource-assignment-sales-estimate-07.png)

Bertsio-berritzea amaitu ondoren, taldekideen rola editatu dezakezu esleitutako lehenespenezkoa ez den beste zerbait izateko. Hala ere, taldekide baten eginkizuna aldatzen baduzu, esleitutako zeregin guztietan aldatuko da; izan ere, 3. bertsioan ezin zaie esleitu taldekideei funtzio bat baino gehiago.

![Baliabide funtzioa eguneratzea](media/resource-role-assignment-08.png)

Berdina gertatzen da izendatutako baliabideei esleitutako lineako zereginekin baliabidearen antolaketa unitatea lehenetsitakotik beste erakunde unitate batera aldatzean. 3. bertsiorako bertsio-berritzea amaitu ondoren, esleipenak baliabidearen antolaketa unitate lehenetsia erabiliko du lineako zereginetan ezarritakoaren ordez.

### <a name="tasks-assigned-to-generic-resources"></a>Baliabide orokorrei esleitutako zereginak
2. bertsioan eta 1. bertsioan, funtzio eta erakunde-unitateak zeregin batean ezar ditzakezu eta, ondoren, erabili **Sortu taldea** eginbidea zereginetan ezarritako atributuetan oinarritutako baliabide generikoak sortzeko. 3. bertsioan, sortu taldekide generikoak funtzio eta erakunde-unitateekin eta, ondoren, esleitu taldekideak zereginetara.

2. bertsioan eta 1. bertsioan, baliabide generikoak dituzten proiektuak bi egoeratan egon daitezke, edo biak nahasita egon daitezke zeregin-mailan. Adibidez, honako egoera hauek izan ditzakezu:

- Funtzio eta erakunde-unitateak dituzten zereginak, baina ez da afiliatutako baliabide esleipenik sortu.
- **Sortu taldea** eginbidea erabiliz baliabide orokorrak sortuta esleitutako taldekide orokorren baliabideen esleipenak dituzten zereginak.

Bertsio-berritzea hasi aurretik, taldea berriro sortzea gomendatzen dizugu baliabide generikoei esleitutako zereginak dituen proiektu bakoitzerako edo oraindik taldea sortzeko prozesua exekutatzen duten proiektuetarako.

**Sortu taldea** eginbidearekin sortutako taldekide orokorrei esleitutako zereginetarako, bertsio-berritzeak baliabide generikoa taldean utziko du eta esleipena taldekide orokor horri utziko dio. Bertsio-berritzearen ondoren talde generikoko kideari baliabide eskakizuna sortzea gomendatzen dugu, baina baliabideen eskaera erreserbatu edo bidali aurretik. Horrek proiektuko kontratazioaren erakunde-unitatearengandik desberdinak diren entitate unitateen esleipenak gordeko ditu taldekide orokorretan.

Adibidez, Project Z proiektuan, kontratazioareb erakunde-unitatea Contoso US da. Proiektuaren planean, Inplementazio fasean saiakuntzak egiteko zereginei aholkulari teknikoa funtzioa esleitu zaie eta esleitutako erakunde-unitatea Contoso India da.

![Ezarpen fasearen entitate esleipena](media/org-unit-assignment-09.png)

Ezarpen fasea igaro ondoren, integrazio probaren zeregina aholkulari teknikoari esleitzen zaio, baina entitatea Contoso US-en ezarrita dago.  

![Integrazio probaren zereginen entitate esleipena](media/org-unit-generate-team-10.png)

Proiekturako talde bat sortzen duzunean, bi taldekide generiko sortzen dira zereginetako erakunde-unitate desberdinengatik. 1. aholkulari teknikoari Contoso Indiako zereginak esleituko zaizkio eta 2. aholkulari teknikoak Contoso US zereginak izango ditu.  

![Sortutako taldekide orokorrak](media/org-unit-assignments-multiple-resources-11.png)

> [!NOTE]
> Project Service Automation aplikazioaren 2. bertsioan eta 1. bertsioan, taldekideak ez du antolaketa unitatea, lerroko zereginean mantentzen dena.

![Project Service Automation-eko 2. bertsioko eta 1. bertsioko lerro-zereginak](media/line-tasks-12.png)

Erakundearen unitatea kalkuluen ikuspegian ikus dezakezu. 

![Erakunde-unitatearen kalkuluak](media/org-unit-estimates-view-13.png)
 
Bertsio-berritzea amaitutakoan, taldekide orokorrari dagokion lerroko zereginari buruzko erakunde-unitatea taldekide orokorrari gehitzen zaio eta lerroko zeregina kentzen da. Hori dela eta, bertsioa eguneratu aurretik, taldea sortzea edo berriro sortzea gomendatzen dugu baliabide generikoak dituen proiektu bakoitzean.

Kontratazio proiektuaren erakunde unitatearengandik desberdina den erakunde-unitate bat duen funtzio bati esleitutako zereginetarako, eta talde bat sortu ez bada, eguneratzeak taldekide orokorra sortuko du funtziorako, baina taldekidearen erakunde-unitaterako proiektuaren kontratazio unitatea erabiliko du. Proiektua Z-ren adibidera itzuliz, horrek esan nahi du Contoso US kontratazio erakunde-unitatea eta inplementazio faseko proiektuaren planak probatzeko zereginei aholkulari teknikoa funtzioa esleitu zaiela Contoso India-ri esleitutako erakunde unitatearekin. Inplementazioaren fasea aholkulari teknikoaren funtzioari esleitu ondoren osatutako integrazio probaren zeregina. Erakunde-unitatea Contoso US da eta ez da talderik sortu. Eguneratzeak taldekide orokor bat, hiru zereginetarako esleitutako orduak dituen aholkulari tekniko bat eta Contoso US-en erakunde-unitate bat, hau da, roiektuaren kontratazioaren erakunde-unitatea sortuko ditu.   
 
Sortu gabeko taldekideen baliabide desberdinen erakunde-unitatearen lehenespenak aldatzea da eguneratu aurretik baliabide orokorrak dituzten proiektu bakoitzeko taldekideak sortzea edo berriro sortzea gomendatzearen arrazoia, erakunde-unitateen esleipenak galdu ez daitezen.

