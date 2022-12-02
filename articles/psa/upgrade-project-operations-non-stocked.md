---
title: Berritu-berritu Project Service Automation-etik Project Operations-era
description: Artikulu honek Microsoft Dynamics 365 Project Service Automation-etik Dynamics 365 Project Operations-era bertsio berritzeko prozesuaren ikuspegi orokorra eskaintzen du.
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
ms.openlocfilehash: ac2435c99f3aa9b2a6cdb08d7ce5f6628e7f6ac4
ms.sourcegitcommit: bea5f9b4066277344add1da3a1567ed56a0cfd31
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/02/2022
ms.locfileid: "9736651"
---
# <a name="upgrade-from-project-service-automation-to-project-operations"></a>Berritu-berritu Project Service Automation-etik Project Operations-era

Pozik gaude Microsoft Dynamics 365 Project Service Automation-etik Microsoft Dynamics 365 Project Operations-era bertsio-berritzeko hiru faseetatik bigarrena iragartzeko. Artikulu honek ibilbide zirraragarri honetan hasten ari diren bezeroentzako ikuspegi orokorra eskaintzen du. 

Bertsio-berritzearen entrega-programa hiru zatitan banatuko da.

| Berritu entrega | 1. fasea (2022ko urtarrila) | 2. fasea (2022ko azaroa) | 3. fasea (2023ko apirileko kaleratzea)  |
|------------------|------------------------|---------------------------|---------------------------|
| Proiektuen zereginen xehetasunen egituran (WBS) mendekotasunik ez | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBSk gaur egun onartzen diren Project Operations-en mugetan sartzen da | | :heavy_check_mark: | :heavy_check_mark: |
| Project Operations-en gaur egun onartzen diren mugetatik kanpoko WBS, Project desktop client bezeroaren laguntza barne | | | :heavy_check_mark: |

## <a name="upgrade-process-features"></a>Bertsio-berritzeko eginbideak 

Bertsio-berritzeko prozesuaren zati gisa, eguneratze-erregistroak gehitu ditugu gune-mapan, administratzaileek hutsegiteak errazago diagnostikatzeko aukera izan dezaten. Interfaze berriaz gain, baliozkotze-arau berriak gehituko dira eguneratze baten ondoren datuen osotasuna bermatzeko. Berritze-prozesuari ondorengo balioztapenak gehituko zaizkio.

| Balidazioa | 1. fasea (2022ko urtarrila) | 2. fasea (2022ko azaroa) | 3. fasea  |
|-------------|------------------------|---------------------------|---------------------------|
| WBS datuen integritatearen urratze arrunten aurrean baliozkotuko da (adibidez, zeregin nagusi berari lotuta dauden baina proiektu nagusi desberdinak dituzten baliabide-esleipenak). | | :heavy_check_mark: | :heavy_check_mark: |
| WBS [Project for the Web-en muga ezagunen](/project-for-the-web/project-for-the-web-limits-and-boundaries) arabera baliozkotuko da. | | :heavy_check_mark: | :heavy_check_mark: |
| WBS Project desktop client-en muga ezagunen arabera baliozkotuko da. | |  | :heavy_check_mark: |
| Erreserba daitezkeen baliabideak eta proiektuen egutegiak egutegi-arau bateraezin arrunten salbuespenen arabera ebaluatuko dira. | | :heavy_check_mark: | :heavy_check_mark: |

2. fasean, Project Operations-era bertsio-berritzen duten bezeroek lehendik dauden proiektuak irakurtzeko soilik izango dituzte proiektuak planifikatzeko. Irakurtzeko soilik den esperientzia honetan, WBS osoa ikusgai egongo da jarraipen-sarean. WBS editatzeko, proiektu-kudeatzaileek hauta dezakete [**Bihurtu**](/PSA-Upgrade-Project-Conversion.md) proiektuaren orrialde nagusian. Ondoren, atzeko planoko prozesu batek proiektua eguneratzen du, Project for the Web-en proiektuaren programazio esperientzia berria onartzen duen. Fase hau egokia da [Project for the Web-en muga ezagunen](/project-for-the-web/project-for-the-web-limits-and-boundaries) barruan sartzen diren proiektuak dituzten bezeroentzat.

3. fasean, Project desktop client-en laguntza-zerbitzua gehituko da, aplikazio horretatik proiektuak editatzen jarraitu nahi duten bezeroen mesedetan. Hala ere, lehendik dauden proiektuak Project for the Web esperientzia berrira bihurtzen badira, gehigarrirako sarbidea desgaitu egingo da bihurtutako proiektu bakoitzeko.

## <a name="prerequisites"></a>Aurrebaldintzak

1. fasea berritzeko eskubidea izateko, irizpide hauek bete behar dituzu:

- Xede-inguruneak ez du erregistrorik eduki behar **msdyn_projecttask** entitatean.
- Baliozko Project Operations lizentziak erabiltzaile aktibo guztiei esleitu behar zaizkie. 
- Bertsio-berritzeko prozesua balioztatu behar duzu produkzio-ingurunearekin bat datorren datu-multzo adierazgarri bat duen produkzioa ez den ingurune batean gutxienez.
- Xede-ingurunea Project Service Automation-en 37. eguneratzearen bertsiora (V3.10.58.120) edo geroagokora eguneratu behar da.

2. fasea berritzeko eskubidea izateko, irizpide hauek bete behar dituzu:

- Baliozko Project Operations lizentziak erabiltzaile aktibo guztiei esleitu behar zaizkie. 
- Bertsio-berritzeko prozesua balioztatu behar duzu produkzio-ingurunearekin bat datorren datu-multzo adierazgarri bat duen produkzioa ez den ingurune batean gutxienez.
- Xede-ingurunea Project Service Automation-en 37. eguneratzearen bertsiora (V3.10.58.120) edo geroagokora eguneratu behar da.
- Zereginak dituzten inguruneak (msdyn_projecttask) proiektu bakoitzeko zereginen kopuru osoa 500 edo txikiagoa bada soilik onartzen dira.

3. faserako aurrebaldintzak eguneratuko dira erabilgarritasun data orokorra hurbildu ahala.

## <a name="licensing"></a>Lizentzia-ematea

Project Service Automation-en lizentzia aktiboak badituzu, Project Service Automation-en gaitasun guztiak eta gehiago biltzen dituen Project Operations instalatu eta erabil dezakezu. Modu honetan, Project Operations-en gaitasunak probatu ditzakezu ekoizpenean Project Service Automation erabiltzen jarraitzen duzun bitartean. Zure Project Service Automation lizentziak iraungi ondoren, Project Operations-era igaro beharko duzu. Trantsizio hau planifikatzen duzunean, kontuan hartu behar duzu Project Operations lizentziak ez duela Project Service Automation lizentziarik. Project Service Automation inplementatu duten eta Project Operations-era pasatzeko asmoa duten bitartean PSA lizentziak erabiltzen jarraitu edo handitzen jarraitu behar duten bezeroek aldi baterako PSA lizentziak eska ditzakete Project Operations-ek erositako lizentzietan oinarrituta. Project Service Automation lizentzia bat emango da Project Operations lizentzia baterako. Aldi baterako PSA lizentziak esteka hau erabiliz eska daitezke: aka.ms/ineedpsa

## <a name="testing-and-refactoring-customizations"></a>Pertsonalizazioak probatu eta berriro faktorizatzea

Abiapuntu gisa, inportatu pertsonalizazio guztiak Project Operations (Lite) ingurune garbi batera inportatzea arrakastatsua dela eta negozio-eragiketak espero bezala jokatzen dutela baieztatzeko.

Hona hemen kontuan hartu beharreko gauza batzuk:

- Baliteke inportazioak huts egitea, mendekotasunak falta direlako. Beste era batera esanda, pertsonalizazioen erreferentzia-eremuak edo beste osagai batzuk Project Operations-en ezabatu diren. Kasu honetan, kendu mendekotasun horiek garapen ingurunetik.
- Kudeatu gabeko eta kudeatutako soluzioek pertsonalizatu gabeko osagaiak badituzte, kendu osagai horiek soluziotik. Adibidez, pertsonalizatzen duzunean **Proiektua** entitatea, gehitu entitatearen goiburua soilik zure soluzioari. Ez gehitu eremu guztiak. Aurretik azpiosagai guztiak gehitu badituzu, baliteke eskuz irtenbide berri bat sortu eta osagai garrantzitsuak gehitu behar izatea.
- Baliteke inprimakiak eta ikuspegiak espero bezala ez agertzea. Zenbait kasutan, kutxaz kanpoko inprimaki edo ikuspegiren bat pertsonalizatu baduzu, baliteke pertsonalizazioek Project Operations-en eguneratze berriak indarrean jartzea eragotzi. Arazo hauek identifikatzeko, Project Operations-en instalazio garbi baten eta zure pertsonalizazioak barne hartzen dituen Project Operations instalazio baten alboan-albo berrikustea gomendatzen dizugu. Konparatu zure negozioan gehien erabiltzen diren inprimakiak, inprimakiaren bertsioak oraindik zentzua duela eta inprimakiaren bertsio garbian ezer falta ez dela ziurtatzeko. Egin elkarren ondoan berrikuspen mota bera pertsonalizatu dituzun ikuspegietarako.
- Negozio-logikak huts egin dezake exekuzioan. Zure plug-in-etako eremuen erreferentziak ez direlako balioztatu inportatzeko unean, baliteke negozio-logikak huts egitea jada existitzen ez diren eremuen erreferentziak direla eta, eta baliteke adibide honen antzeko errore-mezu bat jasotzea: "'Proiektua' entitateak ez du Name = 'msdyn_plannedhours' eta NameMapping = 'Logikoa' duten atributurik." Kasu honetan, aldatu zure pertsonalizazioak eremu berriak erabil ditzaten. Automatikoki sortutako proxy-klaseak eta mota sendoko erreferentziak erabiltzen badituzu zure plug-in logikan, kontuan hartu proxy horiek instalazio garbi batetik birsortzea. Modu honetan, zure pluginak zaharkitutako eremuen mende dauden leku guztiak erraz identifikatu ditzakezu.

Project Operations garbi inportatzeko pertsonalizazioak eguneratu ondoren, joan hurrengo urratsetara.

## <a name="end-to-end-testing-in-development-environments"></a>Amaieratik amaierako probak garapen-inguruneetan

### <a name="initiate-upgrade"></a>Hasi bertsio-berritzea 

1. Joan Power Platform administrazio-zentrora, eta bilatu eta hautatu zure ingurunea. Aplikazioetan, bilatu eta aurkitu **Dynamics 365 Project Operations**.
2. Aukeratu **Instalatu** bertsio-berritzea hasteko. Power Platform administrazio zentroak instalazio hau instalazio berri gisa aurkeztuko du. Hala ere, Project Service Automation-en aurreko bertsio baten presentzia detektatuko da, eta lehendik dagoen instalazioa berrituko da.

    Berritzea amaitu ondoren, inguruneak Project Operations instalatuta dagoela eta Project Service Automation ez dagoela erakutsi beharko luke.

    Prozesuak hainbat ordu iraun dezake inguruneko datu kopuruaren arabera. Bertsio-berritzea kudeatzen ari den oinarrizko taldeak horren arabera planifikatu eta berritzea exekutatu beharko luke negozio-orduetan. Zenbait kasutan, datu-bolumena handia bada, eguneratzea asteburuan zehar exekutatu beharko litzateke. Programazioari buruzko erabakia ingurune baxuetan egindako proben emaitzetan oinarritu behar da.

3. Berritu irtenbide pertsonalizatuak egoki den moduan. Une honetan, zabaldu zure pertsonalizazioetan egin dituzun aldaketak [Pertsonalizazioak probatu eta berriro faktorizatzea](#testing-and-refactoring-customizations) artikulu honen atalean.
4. Joan **make.powerapps.com**, hautatu zure ingurunea atariaren goiko eskuineko goitibeheran, hautatu **Soluzioak** ezkerreko menuan, hautatu **Project Operations-en osagai zaharkituak** soluzioa eta **Desinstalatu**.

    Soluzio hau eguneratzean dauden datu-eredua eta osagaiak gordetzen dituen aldi baterako soluzioa da. Soluzio hau kenduz gero, erabiltzen ez diren eremu eta osagai guztiak kenduko dituzu. Horrela, interfazea errazten eta integrazioa eta hedapena errazten lagunduko duzu.
    
### <a name="upgrade-to-project-operations-lite"></a>Bertsio-berritu Project Operations Lite-ra

Pauso hauek bertsio berritzeko prozesua eta lotutako erroreen erregistroa deskribatzen dute:

1. **PSA bertsioaren egiaztapena:** Project Operations instalatzeko, V3.10.58.120 edo berriagoa izan behar duzu.
1. **Aurre-balioztapena:** Administratzaile batek bertsio berritzea hasten duenean, sistemak aurrebaliozkotze-eragiketa bat egiten du Project Operations soluzioan oinarrizkoa den entitate bakoitzean. Urrats honek egiaztatzen du entitateen erreferentzia guztiak baliozkoak direla, eta WBSrekin erlazionatutako datuak Project for the Web-en argitaratutako mugen barruan daudela ziurtatzen du.
1. **Metadatuak eguneratzea:** Aurrez baliozkotu ondoren, sistemak eskeman aldaketak hasten ditu eta zaharkitutako osagaien soluzioa sortzen du. Zaharkitutako soluzio hau ken dezakezu pertsonalizazioen birfaktorizazio guztiak amaitu ondoren. Urrats hau berritze-prozesuaren zatirik luzeena da eta gehienez lau ordu behar izan ditzake burutzeko.
1. **Datuen eguneratzea:** Metadatuak eguneratzeko urratsean beharrezkoak diren eskema-aldaketa guztiak osatu ondoren, zure datuak eskema berrira migratzen dira eta beharrezko lehenetsiak eta birkalkuluak egiten dira.
1. **Proiektuaren antolaketaren motorra eguneratzea:** Datuak arrakastaz eguneratu ondoren, **Antolaketa** orrialde nagusiko fitxa berriro etiketatzen da **Zereginak** gisa. Erabiltzaile batek bertsio berritu ondoren fitxa hau hautatzen duenean, jarraipen-sarera nabigatzera bideratzen da WBS-ren irakurtzeko soilik den bertsio bat ikusteko. WBS editatzeko, programazioa hasi behar dute [bihurtze prozesua](/PSA-Upgrade-Project-Conversion.md). Aurrez existitzen den WBSrik gabeko proiektu guztiek zuzenean erabil dezakete programazio-esperientzia berria, bihurtu gabe.
 
### <a name="validate-common-scenarios"></a>Baliozkotu ohiko agertokiak

Zure pertsonalizazio zehatzak baliozkotzen dituzunean, aplikazioetan onartzen diren negozio-prozesuak ere berrikustea gomendatzen dizugu. Negozio-prozesu hauek, besteak beste, salmenta-entitateak sortzea, hala nola aurrekontuak eta kontratuak, eta WBSak eta errealak onartzea barne hartzen duten proiektuak sortzea dira.

## <a name="major-changes-between-project-service-automation-and-project-operations"></a>Project Service Automation-etik Project Operations-erako aldaketa nagusiak

Atal honek Project Service Automation eta Project Operations artean espero ditzakezun aldaketa nagusien laburpena eskaintzen du.

### <a name="project-planning"></a>Proiektuaren antolaketa

Project Operations-en proiektuak planifikatzeko gaitasunak jada ez dira bezeroaren aldeko logika eta zerbitzariaren konbinazio batean oinarritzen. Horren ordez, Project Operations-ek erabiltzen du Project for the Web bere programazio-motor nagusi gisa. Programazio-gaitasunen aldaketa honek hainbat funtzio berri ahalbidetzen ditu, hala nola, Board eta Gantt ikuspegiak, baliabideen araberako plangintza, [zereginen zerrendako elementuak](https://support.microsoft.com/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c), eta proiektuak antolatzeko moduak. Programazio gaitasun berriak [aplikazioak programatzeko interfazeen (APIak)](../project-management/schedule-api-preview.md) multzo berri eta aberats batek ere onartzen ditu. API hauek WBSn entitate bat sortzeko, eguneratzeko edo ezabatzeko eragiketa programatikorik programazioko kalkulatutako eremuak hondatzen ez dituela ziurtatzen dute.

### <a name="billing-and-pricing"></a>Fakturazioa eta prezioak

Project Operations-en etengabeko inbertsioen barruan, hainbat gaitasun berri daude eskuragarri Fakturazioan eta prezioetan. Hona hemen zenbait adibideak:

- [Erregistratzea proiektuetako eta proiektu-zereginetako material-erabilera](../material/material-usage-log.md)
- [Azpikontratatuen kudeaketa](../pro/subcontracting/managing-subcontracts-overview.md)
- [Aurrerakinak eta atxikipenetan oinarritutako kontratuak](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Kontratuan gainditu ezin den egoera eta balidazioak](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- Zereginetan oinarritutako fakturazioa

### <a name="resource-management"></a>Baliabideen kudeaketa

Project Operations-ek aukerako laguntza eskaintzen du Universal Resource Scheduling (URS) taula eta programazio laguntzailerako. Esperientzia berri hau derrigorrezkoa izango da 2023ko apirilean.

## <a name="frequently-asked-questions"></a>Ohiko galderak

### <a name="which-deployment-types-are-currently-supported-for-upgrade"></a>Gaur egun, zein inplementazio mota onartzen dira bertsio berritzeko?

| Iturburua                                                 | Helburua                                                    | Fasea                  |
|--------------------------------------------------------|-----------------------------------------------------------|-------------------------|
| Project Service Automation                             | Project Operations Lite-ren inplementazioa                        | Onartzen da               |
| Dynamics 365 Finance Project Management and Accounting | Project Operations Lite-ren inplementazioa                        | Une honetan ez da onartzen |
| Finance Project Management and Accounting              | Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations     | Une honetan ez da onartzen |
| Project Service Automation 3.x                         | Baliabideak edo izakinik gabeko produktuak izatearen egoeretarako Project Operations     | Une honetan ez da onartzen |
| Project for the web (berariazko ingurunea)            | Project Operations Lite-ren inplementazioa                        | Une honetan ez da onartzen |

### <a name="how-can-i-install-project-operations-before-the-upgrade-tooling-is-available"></a>Nola instalatu dezaket Project Operations bertsio berritzeko tresna erabilgarri egon aurretik?

Bi aukera daude Project Operations instalatzeko, bertsio berritzeko tresna erabilgarri egon aurretik:

- Eman ingurune berri bat.
- Inplementatu Project Operations bereizita Project Service Automation ez dagoen edozein salmenta-erakundetan.

Project Service Automation erakunde batean instalatuta badago, baina erabili ez bada, desinstalatu egin daiteke. Project Service Automation erabat kendu ondoren, Project Operations erakunde berean instalatu daiteke.
