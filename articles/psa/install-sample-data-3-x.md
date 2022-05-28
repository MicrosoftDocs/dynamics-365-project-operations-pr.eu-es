---
title: Adibide-datuen instalazioa
description: Gai honek Project Service Automation-eko lagin-datuak instalatzeari buruzko informazioa eskaintzen du.
ms.custom: dyn365-projectservice
ms.date: 11/08/2018
ms.reviewer: johnmichalak
ms.suite: ''
applies_to: Dynamics 365 Project Service Automation
author: ruhercul
ms.author: ruhercul
search.audienceType: IT Pro, Developer
search.app: ''
ms.openlocfilehash: 952f3c3c037bb8459bdd1400288c4ea8604ce282
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581821"
---
# <a name="sample-data-installation-for-the-project-service-application"></a>Project Service aplikazioaren adibide-datuen instalazioa

[!include [banner](../includes/psa-now-project-operations.md)]

Zure ingurune ereduak eraikitzen laguntzeko, Microsoft-ek aplikazioen gaitasunak erakusten dituzten lagin deskargatu paketeak eskaintzen ditu. Bi adibideko datu-pakete mota daude:
- erreferentzia/konfigurazio-datuak
- adibide-datuak (erreferentzia/instalazioa eta, hala nola, lana eskaera eta projects datuak transactional)

Adibideko **erreferentzia** datu-paketeak hiru pakete desberdinetan daude deskargagarri, Project Service-ren datuak soilik, edo Field Service-ren datuak soilik instalatu ahal izateko, edo bi aplikazioen adibide-datuak aldi berean instala ditzakezu.

Adibideko konfigurazioaren/erreferentziaren datu-paketeak dira:

- [**V902PSMasterData** - Project Service 3.x bertsioa soilik](https://go.microsoft.com/fwlink/?linkid=2026540&clcid=0x409)

- [**V902FSMasterData** - Field Service 8.x bertsioa soilik](https://go.microsoft.com/fwlink/?linkid=2026536&clcid=0x409)

- [**V902FPSMasterData** - Field Service 8.x eta Project Service 3.x](https://go.microsoft.com/fwlink/?linkid=2026041&clcid=0x409)

**Demo** datu-pakete berriena da:

 - [**FPSDemoData** - Field Service 8.x eta Project Service 3.x](https://aka.ms/fpsdemodatapackage)

   Instalazio-jarraibideak desberdinak izan daitezke slightly sortu eta konfiguratu sekzio erabiltzaileek baina gainerako aplikatzen zaie, aurreko bai [**blog mezua**](https://aka.ms/fpsdemodatablog). Pakete horren features reduced erakusgai datu multzoa eta inguru 3 ordu instalatzeko ez ditu irauten.

Adibide-datuak paketeak hauek daude erabilgarri ingelesez soilik.

> [!IMPORTANT]
> **Ezin dira inolaz adibide-datuak desinstalatu.** Pakete hauek instalatu behar dituzu adibide- ebaluazio, trebakuntza- edo proba-sistemetan. Ere kontutan banakako paketea instalatu eta, ondoren, instalatu beste banakako paketea, ez da onartzen. (Hau da, ezin instalatu duzu **FSMasterData** atzetik **PSMasterData**, edo vice versa.) Ikusi aplika diezaiokezu zeure buruari beharra adibide-datuak aldi berean bi aplikazioak etorkizunean, instalatu behar duzu, **v902FPSMasterData** paketea.

Instalatzerakoan adibide-datuak paketeak-, instalazio prozesuan ekintzak burutzen ditu hauek:

- Sortu eta erabili Project Service, Field Service edo bi aplikazioak (zerga aplikagarriak) parametroak lehenetsia ezartzen du.

- Inportazioen adibide-aplikazio batzuk, esaterako bookable baliabideak, funtzioak aplikazio zehatz, salmentak eta kostua prezio-zerrendak, erakundeen unitateak, salmenta-prozesuak erregistroak eta beste entitateen gako ahalmenak demonstrate, datuak.  

**Demo-datuak** paketearekin, duzun lehenengo urratsak eremu egokira eta gehigarria transactional datuak, hala nola, lana eskaera eta projects.

Ahalmenak zer wondering duzu dezakezu demostrazio adibide-datuekin? Ikusi Fabrikam Robotics itxurazkoak agertoki jarraian, [Ohar teknikoak](#technical-notes).

Galderak izanez gero instalatu horiek adibidea datuak paketeak buruzko aldi [mezu elektroniko bat bidal diezagukezu fpsdemodata@microsoft.com](mailto:fpsdemodata@microsoft.com) helbidera.

## <a name="requirements"></a>Eskakizunak

Protokoloa instalazioa burutu aurretik, zure helburuko instantzia (erakunde) buruzko hauek:

- Oinarrizko hizkuntza da Ingelesez eta oinarrizko monetaren AEBKO dolarra (USD, $).

- Project Service edo Field Service dagoeneko edo soilik datuek edozein beste erakunde batekin etortzen diren barebones lehenetsia datuak

- Negozio-aplikazioaren bertsio zuzena dagoeneko instalatuta dago:
       
    - **FPSDemoData edo V902FPSMasterData bertsiorako:** Field Service-ren 8.x bertsioa eta Project Service 3.x bertsio honetan instalatuta dagoen bertsioa.

    - **V902PSMasterData:** erakundeak Project Service 3.x bertsioa instalatuta badu.

    - **V902FSMasterData:** erakundeak Field Service 3.x bertsioa instalatuta badu.

> [!NOTE]
> Goialdean lehendik dauden Project Service eta Field Service-ren probako edo dagoeneko (ez gomendatzen) datuak erakusgai ingurunea bat adibide-datuak instalatu behar beharko duzu instalatzailea egindako segurtasun-ekipoen prechecks eteteko. Informazio gehiago eskuratzeko, ikusi ohar teknikoak.

## <a name="prepare-for-installation"></a>Prestatu instalatzeko

Window-en azken bertsioa (Windows 10 hobetsia) duen ordenagailua, instalatzailea abiarazi behar duzu.

Ordenagailua sarera konektatuta mantentzea planeatu behar duzu, instalazioa exekutatzeko **1 orduz** **konfigurazio-/erreferentzia-datuetarako**. (Duzuenan instalazioak minutu ez ditu irauten around 30- **FPSMasterData**, zein aplikazio bi adibide-datuak ditu.) -- **FPSDemoData**, instalazioa egingo aplikazioa **3 ordu**.

Ordenagailua aktibatuta pantaila saver funtzioa izan behar ditu. Bestela, saioa kredentzialak instalaziorako galduko dira pantaila saver (ez duzu mantendu saioa aktibo erabiliko den) engages denean.

> [!div class="mx-imgBorder"]
> ![Pantaila-babeslearen pantaila-argazkiaren ezarpenak pantaila-babeslea itzalita dagoela.](media/sample-data-1.png)

## <a name="download-and-unpack"></a>Deskargatu eta unpack

Project Service eta Field Service adibide-datuak instalatzailea banatzen executable extracting bateratuak gisa. Fitxategien izen adibide-datuak paketea arabera desberdinak izan daitezke, baina bestela urratsak berdinak dira no matter zer paketea instalatu.

Paketeak deskargatu ondoren exekutatu .exe fitxategia eta, ondoren, onartu konprimitutako zip fitxategiak unpack baldintzak betetzera. Fitxategi horretako edukia erauzi behar dituzu ordenagailuko karpeta horretara.

Eta arabera, sistema eragilearen segurtasun-ezarpenak, baliteke behar zip fitxategiak unpacking ondoren hurrengo urratsak egiteko:

1. Bilatu eta egin klik eskuineko botoiarekin **FPSDemoData.dll** fitxategia **v902FPSMasterData** / **PackageDeployer_FPSDemoData** karpeta.

2. Aukeratu **Desblokeatu**.

3. Hautatu **Aplikatu**.

4. Hautatu **Ados**.


## <a name="create-or-configure-users"></a>Sortu edo konfiguratu erabiltzaileak

**FPSDemoData** pakete behar da erabiltzaileak sei **FPSMasterData** paketeak erabiltzaile batek izan behar dira. Zuzendu bat zure adibide-datuak pakete-egiten diote erreferentzia.

## <a name="create-or-configure-users---setupreference-data-packages"></a>Sortu edo konfiguratu erabiltzaile - instalazioak/erreferentzia datuak paketeak

**FPSMasterData** pakete izeneko Spencer txikia Balioa hemen azaldutako ezarpenekin erabiltzaile instalatzeko diseinatuta dago. Instalatzeko behar bezala paketea, behar duzun sortu (edo aldi baterako aldatu) erabiltzaileak zure ingurunean sarrerako adibide-datuak konfigurazio bat etor daitezen.

Sortu edo konfiguratu erabiltzaileak, joan **Ezarpenak** > **Segurtasuna** > **Erabiltzaileak**, eta egin honako hau:

1. Ezarri UserFullname = "Spencer txikia Balioa" eskatuko "spencerl" batekin (**lowercase**) funtzio Proiektua Kudeatzailea eta Practice Kudeatzailea.

2. Hautatu **Spencer Low** erabiltzailea eta, ondoren, hautatu **Kudeatu Funtzioak**. Bilatu eta hautatu, **Sistemaren administratzailea** funtzioak eta, ondoren, hautatu **ados** Spencer txikia Balioa osoa administrazio-eskubideak emateko. Urrats honen da duzun adibidea erregistroak dagokien erabiltzaile jabetza batekin sortzen dira eta beraz betetzeko ikuspegiak behar bezala.

3. Deskargatutako paketea batetik eguneratu behar dizkiezun datu-esleipen fitxategia lehenetsiak erabiltzaile-testuinguru helbide elektroniko batekin. Hori egiteko, ireki **PkgFolder**, eta, ondoren, bilatu eta ireki, **ImportUserMapFile.xml** ohar-Blokarekin (edo Visual Studio edo beste XML editorea) fitxategia. Ezarri, **DefaultUserToMapTo =** eremua Spencer txikia Balioa erabiltzaile baten helbide elektronikoa.

4. Spencer txikia Balioa erabiltzen ez duen eskatuko **spencerl**, fitxategi gehiago eguneratu behar duzu. Ireki, **DemoDataPreImportConfig.xml** fitxategia eta, ondoren, bilaketa- **userstocreateandconfigure** tag. Eguneratu **\<login\>** etiketa Gotzon Galarraga erabiltzailearen erabiltzaile-izenarekin. Informazio osagarria eskuratzeko, ikusi [Ohar teknikoak](#technical-notes).

## <a name="create-or-configure-users---demo-data-package"></a>Sortu edo konfiguratu erabiltzaile - erakusgai datuak paketea

Datuak erakusgai paketea sei erabiltzaileak behar du. Behar bezala instalatu paketea, ondokoa egin:

 1. Sortu edo lehendik dauden erabiltzaileen adibide-datuak konfigurazio sarrerako amaituko arabera ahalbidetzen aldatu aldi baterako **Ezarpenak** > **Segurtasuna** > **Erabiltzaileak**.
 
    Funtzio hauek soilik behar diren demos persona oinarrituta.  
    - Erabiltzailearen Fullname = "David Beraz" Field Service Teknikari gisa   
    - Erabiltzailearen Fullname = "Jamie Reding" Field Service Dispatcher & bezeroarentzako Arreta-Zerbitzua   
    - Erabiltzailearen Fullname = "Molly Clark" gisa Kontu-Kudeatzailea   
    - Erabiltzailearen Fullname = "Spencer txikia" Balioari Practice gisa eta Proiektua Kudeatzailea  
    - Erabiltzailearen Fullname = "Veronica Quek" Taldeko Kide gisa   
    - Erabiltzailearen Fullname = "William Contoso"
  
2. Datuak inportatzeko erakusgai helburuetarako, buruari esleitzen, Administratzailearen funtzioa gaineko sei erabiltzaileak adibidea erregistroak behar bezala inportatu. 

3. Ireki **PkgFolder** eta, ondoren, bilatu eta ireki **ImportUserMapFile.xml**. Eguneratze- **Berriak =** eremuak zure sisteman dagokion Erabiltzaileen helbide elektronikoak.

   > [!div class="mx-imgBorder"]
   > ![UserMapFile pantaila-argazkia.](media/sample-data-7.png)

4. Izen-abizenak "Spencer txikia Balioa" erabiltzaileak baino beste erabiltzaile ID batekin badu **"spencerl"**, gero gehigarria fitxategia eguneratu behar duzu. Ireki **DemoDataPreImportConfig.xml** fitxategia eta, ondoren, bilaketa- **userstocreateandconfigure** tag. Eguneratu **\<login\>** etiketa saioa hasteko IDarekin (maiuskulak eta minuskulak bereizten ditu). 

5. Lehen erabiltzailearen egutegia (aplikazioan- **userstocreateandconfigure** tag) erakusgai datuak atalean bookable baliabide guztiak lanorduak betetzeko erabiltzen da. Joan **Ezarpenak** > **Segurtasun** > **Erabiltzaileak**"Spencer txikia Balioa" erabiltzaileak aurkitzeko, eta ireki "Lanorduak" aukera. Dauden lanorduak, hautatu editatu, **asteko antolaketa errepikaria hasieratik amaiera Osoa** aukera. Ziurtatu **lanorduak konfiguratuta badaude, 8 AM - 5 PM (9 Ordu iraungo ditu), Bostetara Ostiralera eta ezarri Pazifikoko Ordua (aeb eta Kanada) Timezone batekin**. Ziurtatu Proiektua eta Antolaketa board bezala erakutsi egin behar da hau.

**Recommendation:** Hartu orain, zure erakundea babeskopia sortzen kasuen leheneratu edukitzeko hasiera zure zerbait behar da adibide-datuen instalazioa egiterakoan baduzu beharko duzu. Informazio gehiago eskuratzeko, ikusi [Egin instantzien babeskopia eta leheneratu](/dynamics365/customer-engagement/admin/backup-restore-instances).

## <a name="run-the-package-deployer"></a>Exekutatu Package Deployer.

1. Bilatu eta exekutatu **PackageDeployer.exe** **v902FPSMasterData** EDO **PackageDeployer_FPSDemoData** karpetan.

2. Onartu zehaztapenak eta baldintzak.

3. Hurrengo leihoan:

   a. Inplementazio mota hautatu: **Office 365**.

   b. Erabiltzaile eta pasahitza aplikazioan konfiguratu sistemaren administratzaileak erabiltzailearen erabili "Sortu edo konfiguratu erabiltzaileek" ("Spencer txikia" Balioari "spencerl" eskatuko dituzten).

   c. Ziurtatu **Bistaratu erabilgarri dauden erakundeen zerrenda** inaktibo gisa hautatuta.

      > [!div class="mx-imgBorder"]
      > ![Package Deployer leihoaren pantaila-argazkia "Bistaratze-zerrenda duen erabilgarri dauden erakundeak" hautatuta](media/sample-data-2.png)

4. Hautatu erakundearen adibide-datuak instalatu nahi duzun tokian.

5. Hautatu **Hurrengo** ikusi arte, **Erakusgai Datuak Instalazio** elkarrizketa.

   > [!div class="mx-imgBorder"]
   > ![Eginbideei leihoaren erakusgai datuak instalatzailea egoera.](media/sample-data-3.png)

6. Jarraitu, aurretik kontuan duzun adibide-datuak instalatzen iraun gehienez ordu bakarrean (duzuenan ~ 10 minutuak). Ziurtatu ordenagailua atalean egoerarik eta sareko instalazio prozesuan erabiliko den konektatuta eta saioa aktibo egoerarik behar duzu.   

7. Prest zaudenean, sakatu **Hurrengo** adibidea datuak instalazio-prozesua hasteko. Adibide-datuak kargatu ondoren sakatu **Amaitu**.

## <a name="verify-the-sample-data-installation"></a>Adibide-datuen instalazioa egiaztatu

Sanity kontrol, egiaztatu erregistro-kopurua eta entitate-mota honetako agertoki bezala agertuko Fabrikam Robotics zerrendatuta dela.

Ondoren guztiz kargatu adibide-datuak, hasi saioa Spencer txikia Balioa erabiltzaile eta berretsi hauek:

- Project Service aplikazioa instalatuta badago, joan **Project Service** > **Ezarpenak** > **Prezio-zerrendak** aukerara. Berretsi fakturaziorako tasak eta kostu tasak badago, dagokion moneta, bakoitzak herrialdea/eskualdea datu multzo batekin.

- Project Service aplikazioa instalatuta badago, joan **Universal Resource Scheduling** > **Ezarpenak** > **Erakunde unitateak** atalera. Berretsi duzun kostua prezio-zerrenda egokia monetari delako lotutako (sartuz hiria sarrerak) erakunde bakoitzeko unitatearekin. Falta dira edozein, bilatu eta lotu zuzena kostua prezio-zerrenda.

- Field Service aplikazioa instalatuta badago, joan **Project Service** > **Ezarpenak** > **Prezio-zerrendak** aukerara. Berretsi den fakturazio-tasak eta kostu tasak dago. Joan **Field Service** > **Ezarpenak** > **Prezio-Zerrendak** eta markatu duzun fakturaziorako tasak eta kostu tasak badago, dagokion moneta, bakoitzak herrialdea/eskualdea datu multzo batekin.

  > [!div class="mx-imgBorder"]
  > ![Aktibo prezio-zerrendak Eginbideei.](media/sample-data-4.png)

  > [!div class="mx-imgBorder"]
  > ![Eginbideei erakundeen unitate aktiboak.](media/sample-data-5.png)

## <a name="technical-notes"></a>Ohar teknikoak

Ikusi azpiko datu instalazioan xehetasunak teknikoa lortzeko.

### <a name="installing-sample-data-on-top-of-existing-data-not-recommended"></a>Instalatu adibide-datuak arrastatzean dauden datuak (ez gomendatua)

Oharra: goialdean lehendik dauden Field Service edo Project Service-ren probako edo dagoeneko (ez gomendatzen) datuak erakusgai ingurunea bat adibide-datuak instalatu behar beharko duzu instalatzailea egindako segurtasun-ekipoen prechecks eteteko.

Horretarako, joan- **PkgFolder** karpeta aurkitu eta ireki, **DemoDataPreImportConfig.xml** Notepad (edota XML editore beste) duen fitxategia.

Balio hauek aurkitzeko, eta, ondoren, aldatu faltsua gisa true to batetik ezarpena:

```alias
<TerminateOnPreCheckFailure>true</TerminateOnPreCheckFailure>
```

Aldaketa badira instalatzailea bypass zenbait segurtasun-ekipoen garrantzitsua egiaztapenak, besteak beste:

- Dela bat baino gehiago ez confirming aktibo **Antolakuntza Unitatea** erregistro, eta ondoren elkarren dadin **Fabrikam U.S.**.

- Dela bat baino gehiago ez confirming aktibo **Lan Txantiloia** erregistroa.

- Dela bat baino gehiago ez confirming aktibo **Proiektu-parametroa** erregistro, eta ondoren elkarren dadin **Parametroak**.

### <a name="configuration-components"></a>Konfigurazio-osagaiak

Ez dago inportazio aurreko konfigurazio-fitxategia hau konfigurazio beste osagai-kopurua. Erabiltzaile teknikoa zenbait hauek dira:

- **\<RequiredSolutions\>** aldez aurretik zehaztutako soluzioa eta bere bertsio zenbakiak zehazten ditu.

- **\<InstallSampleData\>** atalak kontrolatzen du berezko datuak instalatu diren.

    - Faltsua - integratutako datuen instalazioa saltatzen du (kengarria baita)

    - egia - datuak sortu aldi instalazio-FS eta PSA adibide-datuak instalatu

- **\<PreImportDataCollection\>** Lagin-datuen instalazio nagusiaren aurretik inportatzeko Datu-esleipen lauak eta erlazionatutako erregistroak zehazten ditu.

- **\<EntitiesToEnableScheduling\>** atalak zehazten du zein entitate gaituta egon behar diren Microsoft Dynamics Scheduling-en (edo Universal Resource Scheduling).

- **\<UsersToCreateAndConfigure\>** atalak lagin-datuak inportatzea exekutatu baino lehen sortuko diren (oraindik ez badago) erreserba daitezkeen baliabideak zehazten ditu. Kontuan hartu, iturburuko sistemaren adibide-datuak Bookable Baliabide dute helburuko sistemaren Bookable Baliabide erregistroak FullName eta baliabide bakoitzaren sarrera batekin. Beraz, EZIN da aldatu preconfiguration fitxategi honetan izenak ez duzu lehenik inportatzeko adibide-datuak izenak erabiliz helburuko sisteman eta, ondoren, aldatu izena bakoitzarekin nahi duzun zure izena, Baliabideak Bookable ezarri bai Gaituta Erabiltzaile-erregistroak eta, ondoren, esportatu datuak berriro inportatzeko hasi azken instalaziorako zure sisteman (eguneratzen du **ImportUserMapFile.xml** Zaharra eta Berria sarrerak accordingly).

- **\<PluginsToDisable\>** lagin-datuak inportatzean desgaitu behar diren eta, ondoren berriro gaitu behar diren lerro-elementuko plugin oso diskretuak zehazten ditu.

### <a name="fabrikam-robotics-fictitious-scenario"></a>Fabrikam Robotics itxurazkoak agertoki

Instalatzeko, Field Service eta Project Service adibideko erreferentzia-datuak paketeak, **Fabrikam Fabrikazioa Nagusia Datuak (v3.0.0.0) soluzio**, bai eta erregistro 4.000 inguru eta entitate 40 inguru. Aplikazioko funtzioen azpimultzo bat izan Field Service edo Project Service paketeak datuak beste adibide- **v902FPSMasterData** adibidea aplikazio hori datuak. **Erakusgai Datuak** instalazioetan paketatzeko, **Fabrikam Produkzio-Erakusgai Datuak (v3.0.0.7) soluzio** 22.000 inguru erregistroekin 148 entitate zutabetan zehar.

Fictional enpresaren, Fabrikam Robotics muntaia lineako robots gutunaren gailu manufacturer bat da eta beren produktu kalitatea, innovation eta lerro bezeroarentzako arreta-zerbitzua, instalazioa antolatu, inplementazio eta mantentze jarraitua barne ezagutzen zerbitzuak. Fabrikam ameriketako Estatu Batuez (Fabrikam U.S.) headquartered da, eta Frantzia, India, Erresuma Batua eta Suitza proiektua oinarritutako zerbitzu-eragiketak da.

Field Service eragiketak Estatu Batuetan jartzen dute arreta, batez ere Seattle eremuan. Enpresaren bezero aktiboa errendimendua eta mantenduta increasingly proactive onsite zerbitzuak Interneteko-Gauzak (IoT) konektibitatea leveraging ugaldu da.

Bat high-level informazio orokorra, adibide-datuak honela da:

- Ohiko adibidea datuak elementuak (sartzen aplikazioak bi)

    - 1. erabiltzailea

    - 71 kontu

    - 137 kontaktu

    - Hainbat transakzio mota eta kategoria

    - 50 produktu 1 produkturen prezio-zerrendarekin

    - 14 prezio/kostu-zerrendak

    - 31 ezaugarri (baliabide trebakuntza) 3 maila (sailkapena balio) batekin sailkapena 2 ereduak aplikazioan

- Project Service

    - 8 erakundearen unitateak

    - 6 funtzioa espezifikoak utilization maila

    - 2.8 k + funtzioa prezio azalpenak

- Field Service

    - 4 lurralde

    - 5 lan-eskaeren mota

    - 22 bezero-aktiboak

    - 9 gatazka mota tarte baten batekin erlazionatutako baliabide ezaugarri (9) zerbitzuak (13 zerbitzuko erabiltzailearen) eta zerbitzu-zereginak (13 zerbitzuko erabiltzailearen)
   
**Erakusgai Datuak** paketea instalatu inguru 179 lan eskaerak, 12 projects eta transactional lotutako datuak. 

### <a name="change-the-work-hours-for-sample-resources"></a>Aldatu adibidea baliabideen lanorduekin lan egin

Modu lehenetsian, baliabide guztiak bookable bat 24 lan-orduen egutegia dituzte.

Aldatu adibidea bookable baliabideen lanorduekin lan egin nahi badituzu, joan **Universal Resource Scheduling** > **Scheduling** > **Baliabideak** atalera.

Hautatu erabiltzaile bat (adibidez, Spencer txikia Balioa) eta erabiltzaile bati baino gehiagori aplikatu nahi duzun ordu Spencer baten lanorduak aldatu. Joan **Universal Resource Scheduling** > **Ezarpenak** > **Lan ordu txantiloiak** eta editatzeko, **Lan yxantiloi lehenetsia** erregistroa. **Txantiloia Baliabide** eremuan, hautatu beste baliabide aplikatu nahi duzun lanorduak duen erabiltzaile bat. Joan **Universal Resource Scheduling** > **Programazioa** > **Baliabideak** > **Baliabide-erreserbatu aktiboak**. Aldatu eta, ondoren, hautatu nahi dituzun baliabideak hautatu **Ezarri Egutegi**. **Lan Txantiloia** goitibeherako zerrendan, hautatu, **Lehenetsia Lana Ordu** txantiloia edo zuzena templating baliabidearekin beste txantiloi. Antolaketa board zarenean, izan duzun baliabideak orain izan eguneratu lanorduak ikusteko gai.

> [!div class="mx-imgBorder"]
> ![Baliabide erreserbagarri aktiboen bilaketa bizkorraren pantaila-argazkia.](media/sample-data-6.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]