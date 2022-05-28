---
title: Zer den berria edo zer aldatu den Project Service Automation-en 3. bertsioan
description: Gai honek Project Service Automation-en 3. bertsioan berria denari eta aldatu denari buruzko informazioa eskaintzen du.
ms.custom:
- dyn365-projectservice
ms.date: 11/28/2018
ms.topic: article
author: JohnPBurrows
ms.author: rumant
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
ms.openlocfilehash: 15925cb88cc413f9a23a25e89ddd29668e9171de
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581637"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3"></a>Zer den berria edo zer aldatu den Project Service Automation-en 3. bertsioan

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]



Gai honek erabiltzaile-interfazeari (UI), funtzionaltasunari eta terminologiari buruzko informazioa eskaintzen du Project Service Automation-en 2. bertsioaren edo 1. bertsioaren eta 3. bertsioaren artean.

## <a name="project-scheduling"></a>Proiektuen antolaketa
Proiektuaren antolaketak, aurreko bertsioetan Zereginen xehetasunen egitura (WBS) izenarekin ezagutzen zena, Antolaketa izena hartu du eta **Antolaketa** fitxan klik eginez atzitu daiteke. 

![Proiektuaren antolaketa.](media/psa-schedule-01.png)

Antolaketak elkarrekintzarako gainazal berria du, modernoa eta erabilerraza dena. Hala ere, azpian dagoen Project Service Automation antolaketa-motorra ez da aldatu. Antolaketa-saretaren zinta kontrolatzeko botoiek Project Service Automation-en aurreko bertsioaren antzeko antolaketarekin elkarreragiteko aukera ematen dute. Hauek dira antolaketan egindako aldaketa gehigarriak:

- **Gantt diagrama** - Gantten diagrama ez dago jada. Gannt-en beste bistaratze bat egongo da etorkizuneko eguneratze batean.
- **Zutabeen goiburuak** - Zutabeen goiburuak saretan ezkutatu ditzakezu zutabeen izenaren ondoan dagoen adierazlean klik eginez. 
- **Zutabeak** - Ezkutatutako zutabeak erakutsi ditzakezu **Gehitu zutabea** aukeran klik eginez. 
- **Transakzioen kategoria** - A **Transakzioen kategoria** bilaketa egutegiko saretara gehitu da eta lehenespenez erakusten da. 
 
## <a name="project-templates"></a>Proiektuen txantiloiak
Txantiloi funtzionalak proiektatzeko honako aldaketa hauek egin dira.

### <a name="create-a-project-template"></a>Sortu proiektu-txantiloiak 
Proiektuaren txantiloia sor dezakezu 3. bertsioan Project Service Automation-en aurreko bertsioen antzera. Txantiloiak antolaketa bat bakarrik izan dezake eta antolaketak esleipenak izan ditzake, baina ez dira beharrezkoak. Antolaketak esleipenak baditu, baliabide orokorretarako soilik izan daitezke. Baliabide orokorretarako baliabide-eskakizunak sor ditzakezu, baina ezin dira erreserbatu txantiloian baliabide errealekin. Ezin duzu erreserbatu benetako baliabide bat txantiloi bateko talde batean. 

### <a name="create-a-template-from-an-existing-template"></a>Sortu txantiloi bat lehendik dagoen txantiloi batetik
Project Service Automation-en 3. bertsioan lehendik dagoen txantiloi batetik proiektu-txantiloi bat sortzen duzunean, hau gertatzen da: 

- Iturburuko proiektuaren antolaketa txantiloian kopiatzen da. 
- Baliabide orokorrak taldean kopiatzen dira eta baliabide orokorren esleipenak kopiatzen dira. Ez dira kopiatzen baliabide orokorretarako eskakizunak. 

### <a name="create-a-template-from-an-existing-project"></a>Sortu txantiloi bat lehendik dagoen proiektu batetik
Lehendik dagoen proiektu batetik proiektu-txantiloi bat sortzen duzunean, hau gertatzen da: 

- Iturburuko proiektuaren antolaketa txantiloian kopiatzen da. 
- Baliabide orokorrak taldean kopiatzen dira eta baliabide orokorren esleipenak gordetzen dira. Ez dira kopiatzen baliabide orokorretarako eskakizunak.    
- Izendatutako baliabideak, esleitutakoak zein esleitu gabeak, taldetik kendu eta baliabide orokorretan ezartzen dira.
- Horrelakorik gertatzen bada, bezeroari buruzko informazioa kentzen da. 
- Horrelakorik gertatzen bada, eskaintzei eta kontratuei buruzko erreferentziak kentzen dira. 

### <a name="create-a-project-from-a-template"></a>Sortu proiektua txantiloitik
Project Service Automation-en 3. bertsioan, txantiloi batetik proiektu berri bat sortzen duzunean, hau gertatzen da:

- Antolaketa, taldea eta esleipenak proiektu berrira kopiatzen dira.   
- Hasiera-data erabiltzaileak hautatutako data edo kopiaren data da.   
- Txantiloian baliabide-eskakizunak dituzten taldekide orokorrei dagokienez, eskakizunak ez dira automatikoki kopiatzen edo sortzen. Sortu egin beharko dituzu. 

## <a name="copy-a-project"></a>Kopiatu proiektua
Project Service Automation-en 3. bertsioan, proiektu bat kopiatzen duzunean, hau gertatzen da: 

- Aurreikusitako hasiera-data kopiatuta dago, baina alda daiteke.  
- Proiektuaren antolaketa eta zereginak kopiatzen dira. 
- Baliabide orokorrak eta haien esleipenak kopiatzen dira. Ez dira kopiatzen baliabide orokorretarako baliabide-eskakizunak. Berriro sortu beharko dituzu. 
- Baliabide errealak eta haien esleipenak ez dira kopiatzen. Horren ordez, baliabide orokorrek ordezkatzen dituzte. 
- Benetako datuak ez dira kopiatzen proiektu berrian. 

## <a name="move-a-scheduled-project"></a>Mugitu antolatutako proiektua
Lehendik dagoen proiektuaren antolaketa aurrera eramaten duzunean, hau gertatzen da: 

- Zereginen datak automatikoki mugitzen dira mugimenduaren aldiarekin bat etortzeko. 
- Esleitutako baliabide orokorrek esleituta jarraitzen dute.   
- Proiektua mugitu baino lehen sortzen badira, baliabide orokorretarako eskakizunak berdinak dira eta ez dira automatikoki sortzen. Zereginen mugimenduaren ondorioz, berriro sortu beharko dituzu esleipen berriak islatzeko. 
- Baliabide errealen esleipenak aldatu egiten dira zereginaren dataren mugimenduarekin bat etortzeko. Baliabide errealen erreserbak ez dira aldatzen. Erreserbak aldatu beharko dituzu kontziliazioaren ikuspegia erabiliz. 
- Erreserbak dituzten taldeko baliabideak, baina ez da esleipenik aldatzen. 
- Benetako datuak ez dira mugitzen. 

## <a name="estimates"></a>Aurreikuspenak
Aurreikuspenak bi fitxetan banatu dira, **Baliabide-esleipena** eta **Aurreikuspenak**. **Baliabide-esleipena** fitxak ahaleginaren aurreikuspenak biltzen ditu eta zereginetarako baliabide-zereginak erakusten ditu denbora-fasearen ikuspegian. Benetako datuak editatu ditzakezu antolaketa-motorrak sortutakoan oinarrituta.

![Baliabide-esleipenaren fitxak ahaleginen aurreikuspenak eta baliabide-esleipenak erakusten ditu.](media/resource-assignments-tab-02.png)

**Aurreikuspenak** fitxak baliabide-esleipenen kostuen eta salmenten kopuruak erakusten ditu. Zenbatekoak irakurtzeko soilik dira. Kostuen eta salmenten prezioak taldekideen esleipenean oinarritzen dira egutegian. Horrek esan nahi du esleipenik babeko zeregin bat baduzu, zeregina esleitu gabeko multzoaren azpian agertuko dela. Horrek ere esan nahi du **Funtzioa** aukerarik gabe, hau da, prezioen dimentsio lehenetsirik gabe, ez dela aurreikusitako kostu edo salmentarik izango proiektuarekin lotutako bezero edo kontraturen/eskaintzaren bat izanez gero. 

![Aurreikuspenen fitxak kostuen eta salmenten zenbatekoak erakusten ditu.](media/estimates-tab-03.png)
  
Kategoria ere onartzen da antolaketa-ikuspegiko zereginetan. Denbora-sarreraren ikuspegiko aurreikuspenetako kategorien arabera sailkatzeak esperientzia hobea emango du, batez ere zure proiektuan gastuen aurreikuspenak ere izaten dituzunean. Gastuen aurreikuspenak bereizitako fitxa bateko sareta erabiliz sartzen dira. 

Gastuen aurreikuspenak **Gastuen aurreikuspenak** fitxako saretan sar daitezke. 

![Gastuen aurreikuspenen fitxak gastuen aurreikuspenen sareta erakusten du.](media/expense-estimates-tab-04.png)

## <a name="resource-management"></a>Baliabideen kudeaketa
Project Service Automation-en 3. bertsioan, bezeroaren UI bateratu berriarekin eta erreserben eta esleipenen arteko erlazioak aldaketekin, baliabide orokorrak edo errealak dituen proiektu batean langileak sartzea izugarri aldatu da 2. bertsiotik eta 1. bertsiotik. Hala ere, baliabide erreserbagarrien kontzeptuak, biek **benetakoa** eta **orokorra** berdinak izaten jarraitzen dute, taldekideak, eskakizunak, esleipenak eta erreserbak bezala.   

![Erabili baliabide-hautatzailea.](media/resource-management-05.png)

### <a name="assign-a-real-bookable-resource"></a>Esleitu benetako baliabide erreserbagarri bat 
Project Service Automation-en 3. bertsioan, erreserbak eta zereginen esleipenak ez dira elkarren artean katramilatzen Project Service Automation-en aurreko bertsioetan bezala. Taldearen sareta erabil dezakezu taldekide **erreala** erreserbatzeko, merkatuan egiten den atzera.

Antolaketan baliabide-hautatzailea erabiliz, taldearen ikuspegian sortutako taldekidea aukera dezakezu eta, ondoren, esleitu zereginak. Zereginak esleitzen jarraitu dezakezu, baita erreserbak gainditu ere. Erabili **Kontziliazioa** fitxa erreserba eta esleipenetan desberdintasunak dituzten taldekideak bateratzeko.

Baliabide-hautatzaileak proiekturako dauden taldekideei berri emango du. Baliabide-hautatzailea ere erabil dezakezu proiektu-taldeko parte ez diren baliabide erreserbagarriak bilatu eta ikusteko. Zeregin bat eslei diezaiokezu eta proiektu-taldeko zati bihurtuko dira. Erreserba **Antolaketa-panela** edo **Kontziliazioa** fitxa erabiliz egin beharko duzu.

### <a name="assign-a-generic-bookable-resource-on-a-task-and-project-team-and-then-fulfill-with-a-real-resource-via-schedule-board"></a>Esleitu zeregin eta proiektu-talde bati baliabide erreserbagarri orokorra eta, ondoren, bete baliabide erreal batekin antolaketa-panelaren bidez 
Project Service Automation-en 3. bertsioan, sortutako taldearen funtzionaltasuna ez da erabiltzen baliabide orokorretarako. Horren ordez, antolaketatik baliabide orokor bat sortu eta zuzenean esleitu dezakezu baliabide orokorren posizioaren izena idatziz antolaketako baliabidearen gelaxkan. Edo gelaxkako baliabidearen ikonoa hautatu dezakezu eta, ondoren, baliabide-hautatzailea erabiliz, idatzi sortu nahi duzun baliabide orokorraren izena. Horrek sorrera bizkorreko panela irekiko du, baliabide orokorreko taldekidearen funtzioa eta antolaketa unitatea zehazteko aukera ematen duena. Baliabidea sortu ondoren, zereginari esleitzen zaio eta baliabide orokor hori antolaketako beste zeregin batzuei esleitzen jarraitu dezakezu.    
 
Baliabidea zeregin egoki guztiei esleitu zaionean, baliabide-eskakizuna sor dezakezu eta, ondoren, osa ezazu zuzenean erreserbatuz **Antolaketa-panela** erabiliz edo baliabide-eskaera aurkeztuz. Baliabide orokorrak ere zuzenean gehitu ditzakezu taldekideen saretan. 

Baliabide orokorrak proiektu-taldera gehitzen dira baliabide-eskakizunik gabe eta proiektuaren hasiera- eta amaiera-datekin baliabide-eskakizuna sortu arte. Eskakizun bat sortzeko, hautatu baliabide orokorra eta egin klik **Sortu** aukeran. Eskaeraren esteka bistaratuko da eta behar diren orduak esleitutako orduekin beteko dira. Estekan klik egin dezakezu eskakizuna irekitzeko eta eguneratzeko.
  
Erreserba izendatutako baliabide batekin osatuta eta guztiz beteta dagoenean, baliabide orokorra baliabide izendatuarekin ordezkatuko da eta antolaketako esleipena baliabide izendatuarekin eguneratzen da. 

Eskakizunetarako proposatutako baliabideak fitxa batean gordetzen dira atal bereizi batean gorde beharrean.

### <a name="multiple-named-resources-fulfilling-a-generic-resource"></a>Hainbat baliabide izendatuk baliabide orokor bat betetzea
Eskakizun bat baliabide ugarirekin betetzen denean, baliabide orokorra taldean geratzen da eta zereginari esleitzen zaio. Erreserbatutako taldekide izendatuak ez dira esleitzen karguaren zati gisa. Proiektu-kudeatzaileak lana baliabide errealei eslei diezaieke beharraren arabera.  **Kontziliazioa** ikuspegiak baliabide ugariren eta zereginen esleipen ugarien arteko erreserben xehetasunak eskaintzen ditu. Hori ez da automatikoki egiten; izan ere, egoera zailagoetan, esaterako, eskakizuna osatzen duen zeregin-sorta bat daukazunean, proiektu-kudeatzaileak esleipena egin nahi duen moduaren helburua ezaguna izan behar da. Sistemak ezin duenez ulertu helburua, posible da suposizioak aurreikusitakoengandik desberdinak izatea eta aurreikusitako emaitza okerra edo aurreikusi ezin dena gertatuko dela. Aurreikusi daitekeen emaitza baliabide orokorra esleituta mantentzen dela da proiektu-kudeatzaileak nahitaez zereginak esleitu arte **Kontziliazioa** ikuspegia erabiliz.

### <a name="reconciliation"></a>Kontziliazioa
**Kontziliazioa** fitxak proiektu-taldeko kide bakoitzaren erreserbak eta zereginak erakusten ditu. Ikuspegiak orduak erakusten ditu gelaxkatan, zeinak hilabetetik egunera arteko denbora-puntuak adieraz ditzakeen. Ikuspegi horrek proiektu-kudeatzaileei taldekideen erreserbak eta esleipenak bateratzen laguntzen die haien proeiktu-talderako. Hori lagungarria da erreserbak eta zereginen esleipenak ez direlako ongi lotzen, eta horrek malgutasun handiagoa ematen du proiektu bat antolatzerakoan. 

![Kontziliazioaren fitxak proiektu-taldeko kideen erreserbak eta esleipenak erakusten ditu.](media/resource-reconciliation-tab-06.png)

Baliabide bakoitzerako, ikuspegiak taldekideen erreserbak eta beren zereginen esleipenak biltzen ditu eta proiektu batean erreserbak eta zereginak izan ditzaketen bi desberdintasunak erakusten ditu: 

- **Erreserba eskasia** - Erreserba eskasia gertatzen da baliabideek erreserbak baino esleipen gehiago dituztenean. Ez denez erreserbatu gaitasun hori, proiektu-kudeatzaileak hori zuzendu dezake baliabideen erreserbak hedatuz defizita estaltzeko. 
- **Gehiegizko erreserbak** - Gehiegizko erreserbak baliabide bat proiektuan erreserbatuta dagoenean baina zereginetara esleitu ez denean gertatzen da.  Baldintza hori onargarria izan daiteke, adibidez, baliabidea zereginen esleipena egin aurretik erreserbatu bada. Dena den, baliteke beste kasu batzuetan baliabidea ez egotea esleitzeko aurreikusita, eta PMak baliabideen erreserbak bertan behera uztea pentsatu beharko luke, gaitasuna beste proiektu batetarako erabiltzeko. 

Zeregin baterako esleipenak erreserbarik gabe dituzunean (erreserba eskasia), gehitu erreserba eskasia aukeratu dezakezu eta egin klik **Hedatu erreserba** aukeran. Hemendik, baliabidearen eskasia eta horien eskuragarritasuna lortzeko behar den erreserba ikus daiteke. 
 
## <a name="time-and-expense"></a>Denbora eta gastua
Atal honetan Project Service Automation-en 3. bertsioko denborari, gastuei eta onarpenari buruzko informazioa ematen da. Dynamics 365 Project Service Automation soluzioko zati gisa, **Denbora-sarrera** eginbidea freskatu egin da Interfaze bateratu esparrua aprobetxatzeko. Horren bidez, edozein pantaila-tamaina edo gailutan ikusteko modu egokia lortzeko erabiltzaile-interfaze koherente eta uniformea eskaintzen da. 

### <a name="landing-page"></a>Helburu-orria
Hedagarria ez den denbora-sarrera pertsonalizatuaren esperientzia zaharkitu egin da 3. bertsioan. Horren ordez, eskuragarri dago jatorrizko sareta esperientzia hedagarri eta atzigarria. Denbora-sarreraren funtzionalitatean sar zaitezke ezkerreko gunearen mapa erabiliz. Aldaketa horrekin, ezin izango duzu denbora sartu astean behin. Horren ordez, saretan egun bakoitzeko denbora-sarrera bat sortu beharko duzu. Zenbait denbora-sarrera sortu ondoren, erabiltzaileek denbora-sarrerak modu masiboan sor ditzakete gai honetan geroago azalduko den **Kopiatu** funtzioa erabiliz. 

![Denbora-sarrera helburu-orrian.](media/time-entry-landing-page-07.png)
 
### <a name="create-new-time-entries"></a>Sortu beste denbora-sarrera batzuk 
Egin klik zintako **Berria** aukeran denbora minututan, ordutan edo egunetan sartuko duzun denbora-sarrerarako sorrera bizkorreko orria irekitzeko. Horretarako, hasi kantitatearekin batera h, m edo d idazten.  

![Denbora-sarreraren sorrera bizkorra.](media/quick-create-time-entry-08.png)

Sistemaren ikuspegiek bilatze-eremuak babesten dituzte. Adibidez, proiektuaren informazioa sartu ondoren, **Proiektuaren zeregina** eremua lehenespenez ezarrita dago **Nire irekitako proiektuen zereginak** ikuspegian. Erabiltzaile bati esleitu ez zaizkion zereginetarako denbora-sarrerak sortzeko, egin klik **Aldatu ikuspegia** aukeran bilaketan eta hautatu **Proiektuko zeregin aktibko guztiak**. Denbora-sarrera sortzen denean eta saretan erakutsi ondoren, lerroko balioak zuzenean editatu ahal izango dituzu saretan.  

### <a name="bulk-createcopy"></a>Sortu edo kopiatu modu masiboan 
Denbora-sarrera sortu eta minutu batzuk geroago, kopiatu funtzionaltasuna erabil dezakezu denbora-sarrera gehigarriak sortzeko modu masiboan. Egin klik **Kopiatu** aukeran **Kopiatu** elkarrizketa irekitzeko. **Epe honetatik: hasiera-data** atalean, ezarri denbora-epeak hortik kopiatu behar diren data-tarteak. **Epe honetara: hasiera-data** atalean, zehaztu denbora-sarrerak sortzeko data. Egin klik **Kopiatu** aukeran denbora-sarrerak **Epea honetara** atalean adierazitako dagokion asteko egunera kopiatzeko. Adibidez, pasa den asteko asteleheneko denbora-sarrera **Epe honetara** atalean zehaztutako asteko astelehenean kopiatuko da. 

![Kopiatu denbora-sarrerak modu masiboan.](media/bulk-copy-time-entry-09.png)
 
### <a name="import-data"></a>Inportatu datuak 
Esleipenek eta trukeek UI eredu bera jarraitzen dute, erabiltzaileari erreserbak inportatu behar diren data-tartea zehazteko aukera ematen diotenak. Ondoren, modu esplizituan hautatu behar dituzu **Zirriborroa** denbora-sarreretan kopiatu beharko liratekeen erreserbak. 3. bertsioan ezin duzu jada ikusi **Iradokitakoak** denbora-sarreren ereduak saretan eta egutegian.  

### <a name="change-in-calendar-control"></a>Egutegiaren kontroleko aldaketa
3. bertsioan, egutegiko kontrol pertsonalizatutik aldendu gara eta orain UC Egutegia erabiltzen ari gara asteko denbora-sarrerak erakusteko. Egutegi horrekin, eguna, astea eta hilabetea ikusi ahal izango dituzu. 

> [!NOTE]
> Egutegiaren muga da kontrol horrek ez dituela onartzen ekintzak egutegiko elementu indibidualetan. Adibidez, ezin izango duzu aukeratu egutegiko elementu bat edo gehiago eta elementu horiek bidali edo ezabatu. Egutegiaren elementu batean klik egitean, **Denbora-sarreraren entitatea** ekintza gehigarrientzako orria irekiko da. 

### <a name="extensibility"></a>Hedagarritasuna
**Bildu datuak eremu pertsonalizatuetan denbora- eta gastu-sarrerako entitateetan soilik** - Denbora-sarrerak plataformako sareta editagarria, irakurtzeko soilik den sareta eta egutegiaren kontrolak erabiltzen ditu. Kontrol horiek guztiak jatorrizkoak dira eta, beraz, pertsonalizazioak onartzen dituzte. Project Service Automation-en 3. bertsioan, eremu pertsonalizatu osagarriak gehitu ditzakezu, bilaketa-eremuak konfiguratu eta ikuspegi pertsonalizatuekin babestu ditzakezu. Aukeratutako balioetan oinarritutako negozio-logika pertsonalizatua ere ezarri dezakezu eremu pertsonalizatuetan.  

**Biladu datuak denbora- eta gastu-sarreren eremu pertsonalizatuetan eta hedatu bidalketa eta onarpen fluxuak onartzen dituzten entitateetan** - Denbora-sarreren prozesaketa tipikoa agertzen da hurrengo diagraman.

![Prozesatu denbora-sarreraren fluxua.](media/process-time-entries-10.png)

Negozioaren eskakizunek denbora- eta gastu-entitateek pertsonalizatutako prezio-dimentsioak bildu behar dituztela eta aurreko grafikoan zehaztetuako entitateetan pertsonalizatutako prezio-dimentsioetako denborak eta sarrera-baliabideak ezarritako balioak hedatu behar dituztela zehazten badute, ikusi [Ezarri eremu pertsonalizatuak prezioen dimentsio gisa](set-up-pricing-dimensions.md)

Denbora- eta gastu-entitateek pertsonalizatutako prezioak ez diren dimentsioak bildu eta balioak hedatu behar diren tokian negozio eskakizunak onartzeko, prezioen dimentsioen konfigurazioa erabil dezakezu eta neurri pertsonalizatuak prezioen dimentsio gisa adierazteko kostu edo faktura tasarik gabe. Beste egoera bat entitate bakoitzari eremu pertsonalizatua gehitzea izango litzateke, eremu-izen bera erabiliz entitate guztietan. Plugin pertsonalizatuak sor daitezke bidalketa/onarpen fluxuan parte hartzen duten entitateetako erregistroak erlazionatzeko transakzioaren jatorria eta transakzio konexio entitateak erabiliz.  

### <a name="delegate-time-and-expense-entry"></a>Ordezkariaren orduen eta gastuen sarrera
Common Data Service plataformak ez du onartzen erabiltzaile batek beste batzuk ordezkatzen. Horrek esan nahi du Project Service Automation-en 3. bertsioan ez dagoela laguntza ordezkariaren orduen eta gastuen sarrerarako. Hala ere, bazkideek eta bezeroek irtenbide bat aprobetxatu dute 3. bertsioan eskuordetutako denbora-sarreraren esperientziei laguntza emateko. Konponbide bat baino ez da, eta ez da soluzio oso bat; beraz, garrantzitsua da mugak ulertzea eta ikuspegi hori mugak onargarriak badira soilik erabiltzea. 

> [!IMPORTANT]
> Informazio hori bazkideak edo bezeroak ezarritako inplementazio pertsonalizatuetarako gomendio gisa bakarrik hartu beharko litzateke kontuan. Produktu-taldeak ez du laguntza formalik eskainiko funtzionaltasun horretarako gure laguntza-kanaletakoren batean.

### <a name="customization-details"></a>Pertsonalizazioaren xehetasunak 
Pertsonalizazioak **Baliabide erreserbagarria** sortu eta editu esperientzian gehitzeko aukera ematen du, erabiltzaileari delegatu gisa jarduteko aukera emango diona **Baliabide erreserbagarria** eremua este erabiltzaile batera aldatuz, zeinaren denbora- eta gastu-sarrerak erregistratu behar diren. Ondorengo urratsek denbora-sarreraren delegazioa hartzen dute. Informazio bera aplikatzen zaio gastu-sarrerako ordezkaritzari. 
 
1.  Ziurtatu erabiltzaile delegatuak segurtasunerako sarbide globala duela proiektuetan eta proiektuen zereginetan. 
1.  **Baliabide erreserbagarriak**, hau da **Denbora-sarrera** entitatearen eremua, ez dagoenez agerian **Sorrera bizkorra** orrialdean, gehitu behar duzu.

    edo

    Sortu ikuspegi pertsonalizatua, **Erreserba daitekeen baliabidea** zutabea dituen, baliabiderako sortu diren denbora-sarrerak ikusteko. Argitaratu aplikazio moduluen diseinatzailean pertsonalizazioak ikuspegi hau **Ikusi hautatzailea** aukeraren behean erakusteko **Denbora-sarrerak** orrian. Proiektuaz kanpoko denbora-sarrerak dituen kudeatzailearen ezarpena kudeatzen dituzten bi plugin daude:

    - PreValidateTimeEntryCreate
    - PreValidateTimeEntryUpdate
 
1. Sortu beste plugin bat **Kudeatzailea** eremua gainidazteko **Baliabide erreserbagarriak** eremuan esleitutako erabiltzailearen kudeatzaileari. Erabili **Exekuzio-fasea** bera bandaz kanpoko (OOB) plugin gisa (aurre-balioztapena) eta erabili OOB plugin-a baino handiagoa den (1 baino handiagoa)**Exekuzio-agindua**. Horrek plugin pertsonalizatua OOB plugin-a exekutatu ondoren exekutatuko dela ziurtatuko du.  
 
### <a name="end-user-experience"></a>Amaitu erabiltzailearen esperientzia
1.  Sorrera bizkorreko orrialdean denbora-sarrera bat sortzen duzunean, sartu Proiektua eta Proiektuaren zereginen xehetasunak eta, ondoren, aukeratu erabiltzailea **Baliabide erreserbagarria** eremuan noiz sartu behar den erregistratzeko. 
2.  Lehenespenez, eremu hau saioa hasita duen erabiltzaileari lehenesten zaio; hala ere, erabiltzaileak eremu hau gainditu duelakoan, denbora-sarrera aukeratutako **Baliabide erreserbagarria** aukerarako sortzen da.
3.  Erregistro horietarako sortu dituzun denbora-sarrerak bidaltzen dituzunean, sarrerak proiektuaren oneslearentzako ilaran jarriko dira espero bezala. 
4.  Beste erabiltzailearentzat sortutako denbora-sarrerak berreskuratzen dituzunean, denbora-sarrerak **Zirriborroa** egoerara itzuliko dira **Baliabide erreserbagarria** eremua beste erabiltzaile bati ezarrita. 
5.  Aukeran, ikuspegi pertsonalizatu batera alda dezakezu beste erabiltzaile batentzat sortutako denbora-sarrerak iragazteko. 
 
### <a name="limitations"></a>Mugak
**Kopiatu** eta **Inportatu** funtzionaltasun lanak saioa hasi duen erabiltzailearen testuinguruan soilik. Horrek esan nahi du ezin dela sortu edo inportatu baliabide erreserbagarri gisa saioa hasi duen erabiltzailearentzako sortutako denbora-sarrerak.

Proiektu batekoak ez diren denbora-sarrerak baliabide erreserbagarriaren kudeatzaileari bideratu zaizkio onar dezan soilik **Pertsonalizazioaren xehetasunak** sekzioko 4. urratsa osatu bada. Bestela, beste erabiltzaileentzako proiektuaz kanpoko denbora-sarrerak gaizki bideratuko dira saioa hasi duen erabiltzailearen kudeatzailearengana. 

### <a name="other-changes"></a>Beste aldaketak 
**Erreserbak eta zereginak** funtzionalitatea kendu da. 

## <a name="multidimensional-pricing"></a>Dimentsio anitzeko prezioak
Malgutasuna lortzeko eta negozio eskakizun desberdinak betetzeko, Project Service Automation-en 3. bertsioak onartzen du prezioen dimentsio multzoen aplikazio diskretua kostuen eta fakturen tasetan. Dimentsioaren balioak lehenetsi gisa ezar daitezke eta, ondoren, kostu- eta prezio-prozesuan hedatu daitezke, baliabideen profiletik denbora-proiektura bitarteko proiektuetara. Bezeroaren berariazko konfigurazioa eta aldaketa edo hedapenak pertsonalizagarritasun azpiegitura estandarra erabiltzen ditu.

Project Service Automation-ek prezioen dimentsio eta funtzio eta baliabide unitateen multzo lehenetsiak ditu, eta funtzioen eta antolaketa unitateen konbinazio bakoitzeko prezioak eta kostuak konfiguratzeko aukera ematen du.

3. bertsioan tasaz kanpoko eremu hauek erabiltzen jarraitu nahi duten Project Service Automation-eko bezeroentzat, ez da aldaketarik egongo. Project Service Automation erabiltzen jarraitu dezakezu ohi bezala. Hala ere, zure baliabideen prezioa edo kostua behar baduzu beste atributu osagarriak erabiliz, 3. bertsioak zure pertsonalizatutako prezioen dimentsioak Project Service Automation-era gehitzeko aukera ematen du. Pertsonalizatutako prezioen dimentsioen hedapena konfigurazio esperientzia konplexua da. 

## <a name="quotes-and-contracts"></a>Eskaintzak eta kontratuak
Project Service Automation-en 3. bertsioan eskaintzen eta kontratuen konfigurazioaren eta kudeaketaren ezarpenak aldatu egin dira. Hurrengo ataletan informazio zehatzagoa eskaintzen da.

### <a name="set-up-chargeability-options"></a>Konfiguratu kobragarritasun-aukerak
1. eta 2. bertsioetan, eskaintza eta kontratu espezifikoetarako funtzio eta kategorien kobragarritasun konfigurazioa **Kobragarritasuna** ikuspegia erabiliz egiten zen, eskaintza-lerro edo kontratu-lerro baten goiko nabigazioan zegoen ikuspegia. Hor funtzio eta gastu kategorietarako prezioak ere finka zitezkeen.

3. bertsiotik aurrera, funtzio eta gastuen kategorien bidezko kobragarritasun aukeren konfigurazioa eskaintzaren edo kontratuaren lerro mailan egingo da. Prezioen konfigurazioa kobragarritasun konfiguraziotik aparte dago. **Kobratzeko funtzioak** eta **Kobra daitezkeen kategoriak** fitxan gisa aurkituko dituzu **Eskaintzaren lerroa** eta **Kontratuaren lerroa** orrialdeetan goiko nabigazioa erabili beharrik izan gabe.

![Kobra daitezkeen funtzioak.](media/chargeable-12.png)
 
Kobra daitezkeen funtzioen eta kobra daitezkeen kategorien konfigurazioak erabiltzeko prest dagoen saretaren kontrol editagarria aprobexaten du. Funtzio eta kategoria bakoitzerako, Eskaintza eta kontratazio-fasean zehar fakturaziorako onartutako aukerak aldatu gabe jarraitzen dute aurreko bertsioetatik **Kobratu daitekeena** eta **Kobratu ezin daitekeena** gisa. **Osagarria** ez da Eskaintza edo Kontratazio fasean onartutako mota. **Osagarria** Denbora edo Gastuak onartzerakoan bakarrik onartzen da.  
 
### <a name="create-and-edit-custom-pricing-for-a-project-service-automation-quote-and-project-contract"></a>Sortu eta editatu prezio pertsonalizatuak Project Service Automation eskaintzarako eta proiektu kontraturako
1. eta 2. bertsioetan, eskaintza eta kontratu zehatzen prezio-zerrenda pertsonalizatua erabiliz egin zen **Editatu prezioak** erabiliz **Kobratu daitekeena** ikuspegian. **Kobratu daitekeena** ikuspegia eskaintza-lerro baten edo kontratuaren lerroaren goiko nabigazioan zegoen. Hor funtzio eta gastu kategorietarako kobragarritasun aukerak ere ezarri zitezkeen.

3. bertsioaz geroztik, Project Service Automation eskaintzan eta Project Service Automation proiektuaren kontratuan pertsonalizatutako proiektuen prezio-zerrenda sortu eta erabiltzea kargagarritasun konfiguraziotik bereiztu da. Project Service Automation-en eskaintza eta Project Service Automation proiektuaren aurrekontuek **Proiektuen prezio-zerrendak** izeneko fitxa berria dute. Fitxa horrek Project Service Automation-en eskaintzari edo proiektuaren kontratuei atxikitako proiektuen prezio-zerrenda guztiei lotutako ikuspegia erakusten du. Proiektuaren eskaintza edo kontratuei dagozkien lehendik dagoen prezio-zerrenda batetik prezio-zerrenda pertsonalizatua sortzeko, egin klik **Sortu prezio pertsonalizatuak** aukeran. Horrek loturiko prezio-zerrenda guztien kopia egingo du eta eskaintzari edo kontratuari erantsiko dio. Orain prezio-zerrenda ireki dezakezu eta funtzioaren edo gastu-kategoriaren prezioa editatu ahal izango duzu, prezio aldaketa horiek eskaintza edo kontratu honi bakarrik aplikatzeko. 
  
Hurrengo irudia prezio-zerrenda pertsonalizatuak sortu baino lehenagokoa da.

![Prezio-zerrenda pertsonalizatuak baino lehen.](media/before-custom-price-lists-13.png)

Hurrengo irudia prezio-zerrenda pertsonalizatuak sortu ondorengoa da.

![Prezio-zerrenda pertsonalizatuak eta gero.](media/after-custom-price-lists-14.png)

> [!NOTE]
> Atzerapena egon daiteke **Sortu pertsonalizatutako prezioak** aukeran klik egitean prezio-zerrenda pertsonalizatua sortzen denean. Hainbat aldiz klik egin beharrean, sareta freskatzea gomendatzen dugu. Prezio-zerrenda pertsonalizatua sortu da lotutako prezio-zerrendaren izenak eskaintzaren izena edo proiektuaren kontratuaren izena eransten badu.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
