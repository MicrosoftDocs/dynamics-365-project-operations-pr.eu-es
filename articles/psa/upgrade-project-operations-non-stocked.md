---
title: Berritu-berritu Project Service Automation-etik Project Operations-era
description: Artikulu honek bertsio berritzeko prozesuaren ikuspegi orokorra eskaintzen du Microsoft Dynamics 365 Project Service Automation to Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/11/2022
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
ms.openlocfilehash: 06a4de89be8176049d3a14a8c0d6427e228744ba
ms.sourcegitcommit: 73aff2b3c5e5b8a2254735b0b25931cbb6754c87
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/20/2022
ms.locfileid: "9709429"
---
# <a name="upgrade-from-project-service-automation-to-project-operations"></a>Berritu-berritu Project Service Automation-etik Project Operations-era

Pozik gaude berritzeko hiru faseetatik bigarrena iragartzeko Microsoft Dynamics 365 Project Service Automation Microsoft-era Dynamics 365 Project Operations. Artikulu honek ibilbide zirraragarri honetan hasten ari diren bezeroentzako ikuspegi orokorra eskaintzen du. 

Berrikuntza emateko programa hiru fasetan banatuko da.

| Berritu entrega | 1. fasea (2022ko urtarrila) | 2. fasea (2022ko azaroa) | 3. fasea (2023ko apirileko olatua)  |
|------------------|------------------------|---------------------------|---------------------------|
| Proiektuen lanaren banaketa egituraren (WBS) menpekotasunik ez | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS bat Proiektu Eragiketen gaur egun onartzen diren mugen barruan | | :heavy_check_mark: | :heavy_check_mark: |
| WBS bat Project Operations-ek gaur egun onartzen dituen mugetatik kanpo, Project mahaigaineko bezeroaren laguntza barne | | | :heavy_check_mark: |

## <a name="upgrade-process-features"></a>Berritu prozesuaren ezaugarriak 

Bertsio-prozesuaren zati gisa, eguneratze-erregistroak gehitu ditugu gune-mapan, administratzaileek hutsegiteak errazago diagnostikatzeko aukera izan dezaten. Interfaze berriaz gain, baliozkotze-arau berriak gehituko dira eguneratze baten ondoren datuen osotasuna bermatzeko. Berritze-prozesuari ondorengo balioztapenak gehituko zaizkio.

| Balioztatzeak | 1. fasea (2022ko urtarrila) | 2. fasea (2022ko azaroa) | 3. fasea  |
|-------------|------------------------|---------------------------|---------------------------|
| WBS datuen osotasun-hauste arrunten aurrean baliozkotuko da (adibidez, guraso-ataza berari lotuta dauden baina proiektu nagusi desberdinak dituzten baliabide-esleipenak). | | :heavy_check_mark: | :heavy_check_mark: |
| WBS-ren aurka baliozkotuko da [Weberako Project-en muga ezagunak](/project-for-the-web/project-for-the-web-limits-and-boundaries). | | :heavy_check_mark: | :heavy_check_mark: |
| WBS proiektuaren mahaigaineko bezeroaren mug ezagunekin balioztatuko da. | |  | :heavy_check_mark: |
| Erreserba daitezkeen baliabideak eta proiektuen egutegiak egutegi-arau bateraezin arrunten salbuespenen arabera ebaluatuko dira. | | :heavy_check_mark: | :heavy_check_mark: |

2. fasean, Project Operations-era berritzen duten bezeroek lehendik dauden proiektuak irakurtzeko soilik izango dituzte proiektuak planifikatzeko. Irakurtzeko soilik den esperientzia honetan, WBS osoa ikusgai egongo da jarraipen-sarean. WBS editatzeko, proiektu-kudeatzaileek hauta dezakete [**Bihurtu**](/PSA-Upgrade-Project-Conversion.md) proiektuaren orrialde nagusian. Ondoren, atzeko planoko prozesu batek proiektua eguneratzen du, Project for Web-en proiektuaren programazio esperientzia berria onartzen duen. Fase hau egokia da barruan sartzen diren proiektuak dituzten bezeroentzat [Weberako Project-en muga ezagunak](/project-for-the-web/project-for-the-web-limits-and-boundaries).

3. fasean, Project mahaigaineko bezeroaren euskarria gehituko da, aplikazio horretatik proiektuak editatzen jarraitu nahi duten bezeroen mesedetan. Hala ere, lehendik dauden proiektuak Weberako Proiektu berrira bihurtzen badira, gehigarrirako sarbidea desgaitu egingo da bihurtutako proiektu bakoitzeko.

## <a name="prerequisites"></a>Aurrebaldintzak

1. fasea berritzeko eskubidea izateko, irizpide hauek bete behar dituzu:

- Xede-inguruneak ez du erregistrorik eduki behar **msdyn_projecttask** entitate.
- Baliozko Project Operations lizentziak erabiltzaile aktibo guztiei esleitu behar zaizkie. 
- Bertsio-prozesua balioztatu behar duzu produkzio-ingurunearekin bat datorren datu-multzo adierazgarri bat duen produkzioa ez den ingurune batean gutxienez.
- Xede-ingurunea Project Service Automation Update Release 37 (V3.10.58.120) edo geroago eguneratu behar da.

2. fasea berritzeko eskubidea izateko, irizpide hauek bete behar dituzu:

- Baliozko Project Operations lizentziak erabiltzaile aktibo guztiei esleitu behar zaizkie. 
- Bertsio-prozesua balioztatu behar duzu produkzio-ingurunearekin bat datorren datu-multzo adierazgarri bat duen produkzioa ez den ingurune batean gutxienez.
- Xede-ingurunea Project Service Automation Update Release 37 (V3.10.58.120) edo geroago eguneratu behar da.
- Zereginak dituzten inguruneak (msdyn_projecttask) proiektu bakoitzeko zereginen kopuru osoa 500 edo txikiagoa bada soilik onartzen dira.

3. faserako aurrebaldintzak eguneratuko dira erabilgarritasun data orokorra hurbildu ahala.

## <a name="licensing"></a>Lizentzia-ematea

Project Service Automation-en lizentzia aktiboak badituzu, Project Service Automation-en gaitasun guztiak eta gehiago biltzen dituen Project Operations instalatu eta erabil dezakezu. Modu honetan, Project Operations-en gaitasunak probatu ditzakezu ekoizpenean Project Service Automation erabiltzen jarraitzen duzun bitartean. Zure Project Service Automation lizentziak iraungi ondoren, Project Operations-era igaro beharko duzu. Trantsizio hau planifikatzen duzunean, kontuan hartu behar duzu Project Operations lizentziak ez duela Project Service Automation lizentziarik. Project Service Automation inplementatu duten eta Project Operations-era pasatzeko asmoa duten bitartean PSA lizentziak erabiltzen jarraitu edo handitzen jarraitu behar duten bezeroek aldi baterako PSA lizentziak eska ditzakete Project Operations-ek erositako lizentzietan oinarrituta. Project Service Automation lizentzia bat emango da Project Operations lizentzia baterako. Aldi baterako PSA lizentziak esteka hau erabiliz eska daitezke: aka.ms/ineedpsa

## <a name="testing-and-refactoring-customizations"></a>Pertsonalizazioak probatu eta birfactorizatzea

Abiapuntu gisa, inportatu pertsonalizazio guztiak Project Operations (Lite) ingurune garbi batera inportatzea arrakastatsua dela eta negozio-eragiketak espero bezala jokatzen dutela baieztatzeko.

Hona hemen konturatu beharreko gauza batzuk:

- Baliteke inportazioak huts egitea, mendekotasunak falta direlako. Beste era batera esanda, pertsonalizazioen erreferentzia-eremuak edo beste osagai batzuk Proiektu Eragiketetan ezabatu diren. Kasu honetan, kendu mendekotasun horiek garapen ingurunetik.
- Kudeatu gabeko eta kudeatutako soluzioek pertsonalizatu gabeko osagaiak badituzte, kendu osagai horiek soluziotik. Adibidez, pertsonalizatzen duzunean **Proiektua** entitatea, gehitu entitatearen goiburua soilik zure soluzioari. Ez gehitu eremu guztiak. Aurretik azpiosagai guztiak gehitu badituzu, baliteke eskuz irtenbide berri bat sortu eta osagai garrantzitsuak gehitu behar izatea.
- Baliteke inprimakiak eta ikuspegiak espero bezala ez agertzea. Zenbait kasutan, kutxaz kanpoko inprimaki edo ikuspegiren bat pertsonalizatu baduzu, baliteke pertsonalizazioek Project Operations-en eguneratze berriak indarrean jartzea eragotzi. Arazo hauek identifikatzeko, Project Operations-en instalazio garbi baten eta zure pertsonalizazioak barne hartzen dituen Project Operations instalazio baten alboan-albo berrikustea gomendatzen dizugu. Konparatu zure negozioan gehien erabiltzen diren inprimakiak, inprimakiaren bertsioak oraindik zentzua duela eta inprimakiaren bertsio garbian ezer falta ez dela ziurtatzeko. Egin elkarren ondoan berrikuspen mota bera pertsonalizatu dituzun ikuspegietarako.
- Negozio-logikak huts egin dezake exekuzioan. Zure plug-inetako eremuen erreferentziak ez direlako balioztatu inportatzeko unean, baliteke negozio-logikak huts egitea jada existitzen ez diren eremuen erreferentziak direla eta, eta baliteke adibide honen antzeko errore-mezu bat jasotzea: "'Proiektua' entitateak ez du Name = 'msdyn_plannedhours' eta NameMapping = 'Logikoa' duten atributurik." Kasu honetan, aldatu zure pertsonalizazioak eremu berriak erabil ditzaten. Automatikoki sortutako proxy-klaseak eta mota sendoko erreferentziak erabiltzen badituzu zure plug-in-logikan, kontuan hartu proxy horiek instalazio garbi batetik birsortzea. Modu honetan, zure pluginak zaharkitutako eremuen mende dauden leku guztiak erraz identifikatu ditzakezu.

Proiektuaren Eragiketak garbi inportatzeko pertsonalizazioak eguneratu ondoren, joan hurrengo urratsetara.

## <a name="end-to-end-testing-in-development-environments"></a>Muturreko probak garapen-inguruneetan

### <a name="initiate-upgrade"></a>Hasi berritzea 

1. urtean Power Platform administrazio-zentroa, bilatu eta hautatu zure ingurunea. Ondoren, aplikazioetan, bilatu eta hautatu **Dynamics 365 Project Operations**.
2. Hautatu **Instalatu** berritzea hasteko. The Power Platform administrazio zentroak instalazio hau instalazio berri gisa aurkeztuko du. Hala ere, Project Service Automation-en aurreko bertsio baten presentzia detektatuko da, eta lehendik dagoen instalazioa berrituko da.

    Berritzea amaitu ondoren, inguruneak Project Operations instalatuta dagoela eta Project Service Automation ez dagoela erakutsi beharko luke.

    Inguruko datu-kopuruaren arabera, eguneratzeak hainbat ordu behar izan ditzake. Bertsio-berritzea kudeatzen ari den oinarrizko taldeak horren arabera planifikatu eta berritzea exekutatu beharko luke negozio-orduetan. Zenbait kasutan, datu-bolumena handia bada, eguneratzea asteburuan zehar exekutatu beharko litzateke. Programazioari buruzko erabakia ingurune baxuetan egindako proben emaitzetan oinarritu behar da.

3. Berritu irtenbide pertsonalizatuak egoki den moduan. Une honetan, zabaldu zure pertsonalizazioetan egin dituzun aldaketak [Pertsonalizazioak probatu eta birfactorizatzea](#testing-and-refactoring-customizations) artikulu honen atala.
4. Joan **Ezarpenak** \> **Irtenbideak**, eta hautatu desinstalatzeko **Proiektuaren Eragiketak Osagai zaharkituak** irtenbidea.

    Irtenbide hau eguneratzean dauden datu-eredua eta osagaiak gordetzen dituen aldi baterako irtenbidea da. Irtenbide hau kenduz gero, erabiltzen ez diren eremu eta osagai guztiak kenduko dituzu. Horrela, interfazea errazten eta integrazioa eta hedapena errazten lagunduko duzu.
    
### <a name="upgrade-to-project-operations-lite"></a>Berritu Project Operations Lite-ra

Pauso hauek bertsio berritzeko prozesua eta lotutako erroreen erregistroa deskribatzen dute:

1. **PSA bertsioaren egiaztapena:** Project Operations instalatzeko, V3.10.58.120 edo handiagoa izan behar duzu.
1. **Aurre-balioztapena:** Administratzaile batek bertsio berritzea hasten duenean, sistemak aurrebaliozkotze-eragiketa bat exekutatzen du Project Operations irtenbidean oinarrizkoa den entitate bakoitzean. Urrats honek egiaztatzen du entitateen erreferentzia guztiak baliozkoak direla, eta WBSrekin erlazionatutako datuak Project for the Web-en argitaratutako mugen barruan daudela ziurtatzen du.
1. **Metadatuak eguneratzea:** Aurrez baliozkotu ondoren, sistemak eskeman aldaketak hasten ditu eta zaharkitutako osagaien irtenbidea sortzen du. Zaharkitutako irtenbide hau ken dezakezu pertsonalizazioen birfactorizazio guztiak amaitu ondoren. Urrats hau berritze-prozesuaren zatirik luzeena da eta gehienez lau ordu behar izan ditzake burutzeko.
1. **Datuen eguneratzea:** Metadatuak eguneratzeko urratsean beharrezkoak diren eskema-aldaketa guztiak burutu ondoren, zure datuak eskema berrira migratzen dira eta beharrezko lehenetsiak eta birkalkuluak egiten dira.
1. **Proiektuaren egutegia motorra eguneratzea:** Datuak arrakastaz eguneratu ondoren, **Ordutegia** orrialde nagusiko fitxa berriro etiketatuta dago **Zereginak**. Erabiltzaile batek bertsio berritu ondoren fitxa hau hautatzen duenean, jarraipen-sarera nabigatzera bideratzen da WBS-ren irakurtzeko soilik den bertsio bat ikusteko. WBS editatzeko, programazioa hasi behar dute [bihurtze prozesua](/PSA-Upgrade-Project-Conversion.md). Aurrez existitzen den WBSrik gabeko proiektu guztiek zuzenean erabil dezakete programazio-esperientzia berria, bihurtu gabe.
 
### <a name="validate-common-scenarios"></a>Baliozkotu ohiko eszenatokiak

Zure pertsonalizazio zehatzak baliozkotzen dituzunean, aplikazioetan onartzen diren negozio-prozesuak ere berrikustea gomendatzen dizugu. Negozio-prozesu hauek, besteak beste, salmenta-entitateak sortzea, hala nola aurrekontuak eta kontratuak, eta WBSak eta errealak onartzea barne hartzen duten proiektuak sortzea dira.

## <a name="major-changes-between-project-service-automation-and-project-operations"></a>Aldaketa handiak Project Service Automation eta Project Operations artean

Atal honek Project Service Automation eta Project Operations artean espero ditzakezun aldaketa nagusien laburpena eskaintzen du.

### <a name="project-planning"></a>Proiektuaren antolaketa

Project Operations-en proiektuak planifikatzeko gaitasunak jada ez dira bezeroaren aldeko logika eta zerbitzariaren konbinazio batean oinarritzen. Horren ordez, Project Operations-ek Weberako Project erabiltzen du programazio-motor gisa. Programazio-gaitasunen aldaketa honek hainbat funtzio berri ahalbidetzen ditu, hala nola, Board eta Gantt ikuspegiak, baliabideen araberako plangintza, [zereginen zerrendako elementuak](https://support.microsoft.com/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c), eta proiektuak antolatzeko moduak. Programazio gaitasun berriak berri multzo aberats batek ere onartzen ditu [aplikazioak programatzeko interfazeak (APIak)](../project-management/schedule-api-preview.md). API hauek WBSn entitate bat sortzeko, eguneratzeko edo ezabatzeko eragiketa programatikorik programazioko kalkulatutako eremuak hondatzen ez dituela ziurtatzen dute.

### <a name="billing-and-pricing"></a>Fakturazioa eta prezioak

Proiektuen Eragiketetan etengabeko inbertsioen barruan, hainbat gaitasun berri daude eskuragarri Fakturazioan eta prezioetan. Hona hemen zenbait adibideak:

- [Proiektuetan eta proiektuetako zereginetan materialaren erabilera erregistratzea](../material/material-usage-log.md)
- [Azpikontratuen kudeaketa](../pro/subcontracting/managing-subcontracts-overview.md)
- [Aurrerakinak eta atxikipenetan oinarritutako kontratuak](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Kontratuaren egoera ez gainditzeko eta baliozkotzeak](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- Zereginen araberako fakturazioa

### <a name="resource-management"></a>Baliabideen kudeaketa

Project Operations-ek aukerako laguntza eskaintzen du Universal Resource Scheduling (URS) taula eta programazio laguntzailea. Esperientzia berri hau derrigorrezkoa izango da 2023ko apirilean.

## <a name="frequently-asked-questions"></a>Ohiko galderak

### <a name="which-deployment-types-are-currently-supported-for-upgrade"></a>Gaur egun, zein inplementazio mota onartzen dira bertsio berritzeko?

| Iturburua                                                 | Helburua                                                    | Fasea                  |
|--------------------------------------------------------|-----------------------------------------------------------|-------------------------|
| Project Service Automation                             | Project Operations Lite inplementazioa                        | Onartzen da               |
| Dynamics 365 Finance Proiektuen kudeaketa eta kontabilitatea | Project Operations Lite inplementazioa                        | Une honetan ez da onartzen |
| Finantza Proiektuen Kudeaketa eta Kontabilitatea              | Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations     | Une honetan ez da onartzen |
| Project Service Automation 3.x                         | Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations     | Une honetan ez da onartzen |
| Weberako proiektua (ingurune dedikatua)            | Project Operations Lite inplementazioa                        | Une honetan ez da onartzen |

### <a name="how-can-i-install-project-operations-before-the-upgrade-tooling-is-available"></a>Nola instalatu dezaket Project Operations bertsio berritzeko tresna erabilgarri egon aurretik?

Bi aukera daude Project Operations instalatzeko, bertsio berritzeko tresna erabilgarri egon aurretik:

- Ingurune berri bat eskaintzea.
- Inplementatu Project Operations bereizita Project Service Automation ez dagoen edozein salmenta-erakundetan.

Project Service Automation erakunde batean instalatuta badago, baina erabili ez bada, desinstalatu egin daiteke. Project Service Automation erabat kendu ondoren, Project Operations erakunde berean instalatu daiteke.
