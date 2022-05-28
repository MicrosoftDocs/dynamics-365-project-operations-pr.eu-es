---
title: Berritu Project Service Automation-etik Project Operations-era
description: Gai honek bertsio berritzeko prozesuaren ikuspegi orokorra eskaintzen du Microsoft Dynamics 365 Project Service Automation to Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/13/2022
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
ms.openlocfilehash: 3f31173197a3055cdc51567261dd91925fc9f430
ms.sourcegitcommit: bec7382d1319d59645e8e79fdb20df58617c97c6
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/21/2022
ms.locfileid: "8626730"
---
# <a name="upgrade-from-project-service-automation-to-project-operations"></a>Berritu Project Service Automation-etik Project Operations-era

Pozik gaude berritzeko hiru faseetako lehena iragartzeko Microsoft Dynamics 365 Project Service Automation to Dynamics 365 Project Operations. Gai honek ibilbide zirraragarri honetan hasten ari diren bezeroei ikuspegi orokorra eskaintzen die. Etorkizuneko gaietan garatzaileen gogoetak eta eginbideen hobekuntzei buruzko xehetasunak izango dira. Project Operations-en bertsio-berritzea prestatzen lagunduko dizuten jarraibideak emateaz gain, bertsio berritu ondoren zer espero dezakezun azalduko dizute.

Berrikuntza emateko programa hiru fasetan banatuko da.

| Berritu entrega | 1. fasea (2022ko urtarrila) | 2. fasea (2022ko apirileko olatua) | 3. fasea  |
|------------------|------------------------|---------------------------|---------------------------|
| Proiektuen lanaren banaketa egituraren (WBS) menpekotasunik ez | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS Proiektuaren Eragiketen gaur egun onartzen diren mugen barruan | | :heavy_check_mark: | :heavy_check_mark: |
| WBS Project Operations-ek gaur egun onartzen dituen mugetatik kanpo, Project mahaigaineko bezeroaren laguntza barne | | | :heavy_check_mark: |

## <a name="upgrade-process-features"></a>Berritu prozesuaren ezaugarriak 

Bertsio-prozesuaren zati gisa, eguneratze-erregistroak gehitu ditugu guneko mapan, administratzaileek hutsegiteak errazago diagnosti ditzaten. Interfaze berriaz gain, baliozkotze-arau berriak gehituko dira eguneratu ondoren datuen osotasuna bermatzeko. Berritze-prozesuari ondorengo balioztapenak gehituko zaizkio.

| Balioztatzeak | 1. fasea (2022ko urtarrila) | 2. fasea (2022ko apirileko olatua) | 3. fasea  |
|-------------|------------------------|---------------------------|---------------------------|
| WBS datuen osotasun-hauste arrunten aurrean baliozkotuko da (adibidez, zeregin nagusi berdinarekin lotutako baina proiektu nagusi desberdinak dituzten baliabide-esleipenak). | | :heavy_check_mark: | :heavy_check_mark: |
| WBS-ren aurka baliozkotuko da [Weberako Project-en muga ezagunak](/project-for-the-web/project-for-the-web-limits-and-boundaries). | | :heavy_check_mark: | :heavy_check_mark: |
| WBS Proiektuko mahaigaineko bezeroaren mug ezagunekin balioztatuko da. | |  | :heavy_check_mark: |
| Erreserba daitezkeen baliabideak eta proiektuen egutegiak egutegi-arau bateraezin arrunten salbuespenen arabera ebaluatuko dira. | | :heavy_check_mark: | :heavy_check_mark: |

2. fasean, Project Operations-era berritzen duten bezeroek lehendik dauden proiektuak berrituko dituzte irakurtzeko soilik den esperientzia batera proiektuaren plangintzarako. Irakurtzeko soilik den esperientzia honetan, WBS osoa ikusgai egongo da jarraipen-sarean. WBS editatzeko, proiektu-kudeatzaileek hauta dezakete **Bihurtu** nagusian **Proiektuak** orrialdea. Ondoren, atzeko planoko prozesu batek proiektua eguneratuko du, Project for Web-eko proiektuen programazio esperientzia berria onartzen duen. Fase hau egokia da barruan sartzen diren proiektuak dituzten bezeroentzat [Weberako Project-en muga ezagunak](/project-for-the-web/project-for-the-web-limits-and-boundaries).

3. fasean, Project mahaigaineko bezeroaren euskarria gehituko da, aplikazio horretatik proiektuak editatzen jarraitu nahi duten bezeroen mesedetan. Hala ere, lehendik dauden proiektuak Weberako Proiektu berrira bihurtzen badira, gehigarrirako sarbidea desgaitu egingo da bihurtutako proiektu bakoitzeko.

## <a name="prerequisites"></a>Aurrebaldintzak

1. faseko bertsio berritzeko eskubidea izateko, bezeroak irizpide hauek bete behar ditu:

- Xede-inguruneak ez du erregistrorik eduki behar **msdyn_projecttask** entitate.
- Baliozko Project Operations lizentziak bezeroaren erabiltzaile aktibo guztiei esleitu behar zaizkie. 
- Bezeroak eguneratze-prozesua balioztatu behar du produkzio-datuekin bat datorren datu-multzo adierazgarri bat duen produkzioa ez den ingurune batean gutxienez.
- Xede-ingurunea Project Service Automation Update Release 41 (3.10.62.162) edo geroago eguneratu behar da.

2. eta 3. faserako aurrebaldintzak eguneratuko dira erabilgarritasun-data orokorrak hurbildu ahala.

## <a name="licensing"></a>Lizentzia-ematea

Project Service Automation-en lizentzia aktiboak badituzu, Project Service Automation-en gaitasun guztiak eta gehiago biltzen dituen Project Operations instalatu eta erabil dezakezu. Modu honetan, Project Operations-en gaitasunak probatu ditzakezu ekoizpenean Project Service Automation erabiltzen jarraitzen duzun bitartean. Zure Project Service Automation lizentziak iraungi ondoren, Project Operations-era igaro beharko duzu. Trantsizio hau planifikatzen duzunean, kontuan hartu behar duzu Project Operations lizentziak ez duela Project Service Automation lizentziarik.

## <a name="testing-and-refactoring-customizations"></a>Pertsonalizazioak probatu eta birfactorizatzea

Abiapuntu gisa, inportatu pertsonalizazio guztiak Project Operations (lite) ingurune garbi batera inportatzea arrakastatsua dela eta negozio-eragiketak espero bezala jokatzen dutela baieztatzeko.

Hona hemen konturatu beharreko gauza batzuk:

- Inportazioak huts egin dezake mendekotasunak falta direlako. Beste era batera esanda, pertsonalizazioak erreferentzia-eremuak edo beste osagai batzuk Proiektu Eragiketetan ezabatu diren. Kasu honetan, kendu mendekotasun horiek garapen-ingurunetik.
- Kudeatu gabeko eta kudeatutako soluzioek pertsonalizatu gabeko osagaiak badituzte, kendu osagai horiek soluziotik. Adibidez, pertsonalizatzen duzunean **Proiektua** entitatea, gehitu entitatearen goiburua soilik zure soluzioari. Ez gehitu eremu guztiak. Aurretik azpiosagai guztiak gehitu badituzu, baliteke eskuz irtenbide berri bat sortu eta osagai garrantzitsuak gehitu behar izatea.
- Baliteke inprimakiak eta ikuspegiak espero bezala ez agertzea. Zenbait kasutan, kutxaz kanpoko inprimaki edo ikuspegiren bat pertsonalizatu baduzu, baliteke pertsonalizazioek Project Operations-en eguneratze berriak indarrean jartzea eragotzi. Arazo hauek identifikatzeko, gomendatzen dugu Project Operations instalazio garbi baten eta zure pertsonalizazioak barne hartzen dituen Project Operations instalazio baten berrikuspena egitea. Konparatu zure negozioan gehien erabiltzen diren inprimakiak, inprimakiaren bertsioak oraindik zentzua duela eta inprimakiaren bertsio garbian ezer falta ez dela ziurtatzeko. Egin elkarren ondoan berrikuspen mota bera pertsonalizatu dituzun ikuspegietarako.
- Negozio-logikak huts egin dezake exekuzioan. Zure plug-inetako eremuen erreferentziak ez direlako balioztatu inportatzeko unean, baliteke negozio-logikak huts egitea jada existitzen ez diren eremuen erreferentziak direla eta, eta baliteke adibide honen antzeko errore-mezu bat jasotzea: "'Proiektua' entitateak ez du Name = 'msdyn_plannedhours' eta NameMapping = 'Logikoa' duten atributurik." Kasu honetan, aldatu zure pertsonalizazioak eremu berriak erabil ditzaten. Automatikoki sortutako proxy-klaseak eta motako erreferentzia sendoak erabiltzen badituzu zure plug-in-logikan, kontuan hartu proxy horiek instalazio garbi batetik birsortzea. Modu honetan, zure pluginak zaharkitutako eremuen mende dauden leku guztiak erraz identifikatu ditzakezu.

Zure pertsonalizazioak eguneratu ondoren Proiektu Eragiketak garbi inportatzeko, joan hurrengo urratsetara.

## <a name="end-to-end-testing-in-development-environments"></a>Muturreko probak garapen-inguruneetan

### <a name="initiate-upgrade"></a>Hasi berritzea 

1. urtean Power Platform administrazio-zentroa, bilatu eta hautatu zure ingurunea. Ondoren, aplikazioetan, bilatu eta hautatu **Dynamics 365 Project Operations**.
2. Hautatu **Instalatu** berritzea hasteko. The Power Platform administrazio zentroak instalazio hau instalazio berri gisa aurkeztuko du. Hala ere, Project Service Automation-en aurreko bertsio baten presentzia detektatuko da, eta lehendik dagoen instalazioa berrituko da.

    Berritzea amaitu ondoren, inguruneak erakutsi beharko luke Project Operations instalatuta dagoela eta Project Service Automation ez dagoela instalatuta.

    > [!NOTE]
    > Inguruneko datu kopuruaren arabera, eguneratzeak ordu batzuk behar izan ditzake. Bertsio-berritzea kudeatzen ari den oinarrizko taldeak horren arabera planifikatu eta berritzea exekutatu beharko luke negozio-orduetan. Zenbait kasutan, datu-bolumena handia bada, eguneratzea asteburuan zehar exekutatu beharko litzateke. Programazioari buruzko erabakia ingurune baxuetan egindako proben emaitzetan oinarritu behar da.

3. Berritu irtenbide pertsonalizatuak egoki den moduan. Une honetan, zabaldu zure pertsonalizazioetan egin dituzun aldaketak [Pertsonalizazioak probatu eta birfactorizatzea](#testing-and-refactoring-customizations) gai honen atala.
4. Joan **Ezarpenak** \> **Irtenbideak**, eta hautatu desinstalatzeko **Proiektuaren Eragiketak Osagai zaharkituak** irtenbidea.

    Irtenbide hau aldi baterako irtenbide bat da, eguneratzean dauden datu-eredua eta osagaiak gordetzen dituena. Soluzio hau kenduz gero, erabiltzen ez diren eremu eta osagai guztiak kenduko dituzu. Horrela, interfazea errazten eta integrazioa eta hedapena errazten lagunduko duzu.
    
### <a name="validate-common-scenarios"></a>Baliozkotu ohiko eszenatokiak

Zure pertsonalizazio zehatzak baliozkotzen dituzunean, aplikazioetan onartzen diren negozio-prozesuak ere berrikustea gomendatzen dizugu. Negozio-prozesu hauek, besteak beste, salmenta-entitateak sortzea, hala nola aurrekontuak eta kontratuak, eta WBSak eta errealak onartzea barne hartzen duten proiektuak sortzea dira.

## <a name="major-changes-between-project-service-automation-and-project-operations"></a>Aldaketa handiak Project Service Automation eta Project Operations artean

Atal honek Project Service Automation eta Project Operations artean espero ditzakezun aldaketa nagusien laburpena eskaintzen du.

### <a name="project-planning"></a>Proiektuaren antolaketa

Project Operations-en proiektuak planifikatzeko gaitasunak jada ez dira bezeroaren aldeko logika eta zerbitzariaren konbinazio batean oinarritzen. Horren ordez, Project Operations-ek Weberako Project erabiltzen du programazio-motor gisa. Programazio-gaitasunen aldaketa honek hainbat funtzio berri ahalbidetzen ditu, hala nola, Board eta Gantt ikuspegiak, baliabideen araberako plangintza, [zereginen zerrendako elementuak](https://support.microsoft.com/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c), eta proiektuak antolatzeko moduak. Programazio gaitasun berriak berri multzo aberats batek ere onartzen ditu [aplikazioak programatzeko interfazeak (APIak)](../project-management/schedule-api-preview.md). API hauek WBSn entitate bat sortzeko, eguneratzeko edo ezabatzeko eragiketa programatikorik programazioko kalkulatutako eremuak hondatzen ez dituela ziurtatzen dute.

## <a name="billing-and-pricing"></a>Fakturazioa eta prezioak

Proiektuen Eragiketetan etengabeko inbertsioen barruan, hainbat gaitasun berri daude eskuragarri Fakturazioan eta prezioetan. Hona hemen zenbait adibideak:

- [Proiektuetan eta proiektuetako zereginetan materialaren erabilera erregistratzea](../material/material-usage-log.md)
- [Azpikontratuen kudeaketa](../pro/subcontracting/managing-subcontracts-overview.md)
- [Aurrerakinak eta atxikipenetan oinarritutako kontratuak](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Kontratuaren egoera ez gainditzeko eta baliozkotzeak](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- Zereginen araberako fakturazioa

## <a name="frequently-asked-questions"></a>Ohiko galderak

### <a name="which-deployment-types-are-currently-supported-for-upgrade"></a>Zein inplementazio mota onartzen dira eguneratzeko?

| Iturburua                                                 | Helburua                                                    | Fasea                  |
|--------------------------------------------------------|-----------------------------------------------------------|-------------------------|
| Project Service Automation                             | Project Operations Lite inplementazioa                        | Onartzen da               |
| Dynamics 365 Finance Proiektuen kudeaketa eta kontabilitatea | Project Operations Lite inplementazioa                        | Une honetan ez da onartzen |
| Finantza Proiektuen Kudeaketa eta Kontabilitatea              | Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations     | Une honetan ez da onartzen |
| Finantza Proiektuen Kudeaketa eta Kontabilitatea              | Izakinak edo ekoizpen-eskaerak izatearen egoeretarako Project Operations | Une honetan ez da onartzen |
| Project Service Automation 3.x                         | Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations     | Une honetan ez da onartzen |
| Weberako proiektua (ingurune dedikatua)            | Project Operations Lite inplementazioa                        | Une honetan ez da onartzen |

### <a name="how-can-i-install-project-operations-before-the-upgrade-tooling-is-available"></a>Nola instalatu ditzaket Project Operations berritze-tresnak erabilgarri egon aurretik?

Bi aukera daude Project Operations instalatzeko, bertsio berritzeko tresna erabilgarri egon aurretik:

- Ingurune berri bat eskaintzea.
- Inplementatu Project Operations bereizita Project Service Automation ez dagoen edozein salmenta-erakundetan.

> [!NOTE]
> Project Service Automation erakunde batean instalatuta badago, baina ez bada erabili, desinstalatu egin daiteke. Project Service Automation erabat kendu ondoren, Project Operations erakunde berean instalatu daiteke.
