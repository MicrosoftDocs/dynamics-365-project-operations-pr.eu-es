---
title: Kudeatu baliabideak
description: Gai honek baliabideak kudeatzeko moduari buruzko informazioa eskaintzen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
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
ms.openlocfilehash: 548595e3951f824e1c79a641d3f336e381fcaaf9
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4132318"
---
# <a name="manage-resources"></a>Kudeatu baliabideak

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation-ek baliabideen kudeaketako panela biltzen du baliabideen eskaeraren eta erakundearen erabileraren ikuspegi orokorra eskaintzen duena. Panel honetako diagramak erabil ditzakezu informazioa ikusteko:

- **Baliabideen eskaria**: **Baliabide aktiboen eskaera** taulan aurkeztu diren baliabideak erakusten dira. Baliabideak funtzioaren edo proiektuaren arabera biltzen dira.
- **Bidali gabeko baliabideen eskaria**: **Esleitu gabeko baliabideen eskaria** taulan aurkeztu ez diren baliabide-eskakizun guztiak erakusten dira. Baliabideen kudeatzaileei eskaera ez dela irmoa ikusten dute eta baliabide eskaera bidez bidaltzen laguntzen die.
- **Erabilera erabilgarriak azken astean**: **Erabilera funtzioa** taulan ikus daiteke erakundearen benetako fakturazioaren portzentajea bere eginkizunaren arabera fakturazioaren aldera.

    > [!NOTE]
    > **Erabilera funtzioa** taula eskuragarri egoteko, sortu UpdateRoleUtilization lan-fluxua exekutatzen duen lana. Lan errepikari hau zazpi egunez behin egiten da aurreko zazpi egunetako erabilgarritasuna kalkulatzeko. Emaitzak funtzioaren arabera batu dira.

## <a name="manage-project-team-members"></a>Proiektu-taldekideak kudeatu

Proiektuaren kudeatzaileek baliabideen kudeatzailearen panela erabil dezakete proiektuetan baliabideak kudeatzeko. Adibidez, taldekide bat zuzenean gehitu dezakete proiektu batean eta taldekide bat erreserbatu baliabide generiko batek harrapatutako baliabide eskakizunak betetzeko.

### <a name="add-a-team-member-directly-to-a-project"></a>Gehitu taldekidea zuzenean proiektu bati

Taldekide bat zuzenean proiektu batean gehitzeko, **Proiektuak** orrialdean **Taldea** fitxan, aukeratu **Berria**. **Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroa agertuko da. Elkarrizketa-koadro honetan zeregin hauek egin ditzakezu:

- **Erreserbatu izendatutako baliabidea**: **Baliabide erreserbagarria** eremuan, hautatu baliabidearen izena. Ondoren, hautatu funtzioa, zehaztu epea eta hautatu esleipen metodoa. Aukeratu duzun izena duen baliabidea proiektuari gehitzen zaio hautatutako esleipen metodoa eta baliabideen egutegia erabiliz.
- **Gehitu baliabide generikoa**: utzi **Baliabide erreserbagarria** eremua hutsik eta, ondoren, hautatu funtzioa, ezarri aldia eta hautatu hobetsitako esleipen metodoa. Baliabide generiko bat gehitzen zaio taldeari leku-marka gisa, taldean izena duten baliabide erabiltzen diren eskaera-eredua mantentzeko. Baldintza proiektuaren egutegiaren arabera egiten da.
- **Gehitu izendatutako baliabidea taldeari baliabideen ahalmena kontsumitu gabe**: **Baliabide erreserbagarria** eremuan, hautatu baliabide bat. Ondoren, hautatu aldia eta hautatu **Ez** esleipen metodoa. Baliabidea taldeari gehitzen zaio, baina baliabidearen ahalmena ez da erreserba bidez kontsumitzen.

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a>Erreserbatu taldekide bat baliabide generiko baterako eskakizunak betetzeko

PSAn, baliabide generikoak proiektu talde batean erreserbatu ditzakezu eta zeregina, behar den gaitasuna eta nola banatzen den zehaztu dezakezu. Baliabidearen eskakizunean, baliabide generikoarekin lotutako atributuak zehaztu ditzakezu. Ezaugarri horien artean beharrezkoak diren trebetasunak, nahiago den antolakuntza-unitatea eta hobetsitako baliabideak daude.

Jarraitu urrats hauek garatzaileentzako baliabide generiko batean eskatutako trebetasunak zehazteko.

1. **Proiektuak** orrialdean **Taldea** fitxan, hautatu **Berria** baliabide generikoa erreserbatzeko.

    ![Balio generikoa taldean erreserbatuta](media/Resource-Management-image9.png)

2. **Taldekide guztiak** ikuspegian, **Baliabideen eskakizuna** zutabean, hautatu esteka baliabide generikorako beharrezkoak diren trebetasunak gehitzeko.

    ![Eskakizun esteka](media/Resource-Management-image10.png)

3. **Baliabideen eskakizuna** orrian, **Trebetasunak** saretan agertzen denean, hautatu elipsia (**...**) eta hautatu **Gehitu eskakizun berriaren ezaugarria** sustatzailearentzako beharrezkoak diren gaitasunak gehitzeko.

    ![Eskakizunen ezaugarri-komando berria hautatu](media/Resource-Management-image11.png)

4. **Sorrera bizkorra: eskakizunaren ezaugarria** elkarrizketa-koadroan **Ezaugarria** eremuan agertzen denean, hautatu eskatutako trebetasuna. Ondoren, **Balorazioaren balioa** eremuan, hautatu trebetasun horren maila. Azkenean, **Baliabideen eskakizuna** eremuan, ezarri eskakizuna baliabide iturriak antolakuntza unitateetatik edo baita izendatutako baliabideak ere. Bukatu duzunean, hautatu **Gorde**.

    ![Sorrera bizkorra: eskakizunaren elkarrizketa-koadroa](media/Resource-Management-image12.png)

5. **Baliabideen eskakizuna** orrian, hautatu **Liburua** baliabide eskakizuna betetzeko.

    ![Liburuaren botoia Baliabide Eskakizuna orrian](media/Resource-Management-image13.png)

    Baliabide generikoak ere hauta ditzakezu **Taldekide guztiak** saretan eta gero hautatu **Liburua**.

    ![Erreserbatu botoia Taldekide guztien sarearen gainetik](media/Resource-Management-image14.png)

    > [!NOTE]
    > Adibide honetan, 40 ordu behar dira baina ez erreserbatu gabeko orduak, baliabide generikoek erreserbaziorik ez dutelako. Gainera, ez dira ordu esleituak, baliabide generikoa zuzenean taldeari gehitu zitzaiolako. Ez da zereginen esleipena erabiliz gehitu.

    **Programazio laguntzailea** orrialdean, erabilgarri dauden baliabideak iragazi ditzakezu baliabideen eskakizunean zehazten diren baldintzen arabera. Baliabideak Antolaketa taulan zehaztutako sailkapen parametroen arabera ordenatzen dira.

    ![Antolaketa-laguntzailearen orria](media/Resource-Management-image15.png)

    Hona hemen maiz erabiltzen diren iragazki batzuk:

    - **Ezaugarriak puntuazioarekin batera**: gaitasunak, ziurtagiriak eta baliabideen beste ezaugarri batzuen arabera iragazi, gaitasunen balorazioez gain.
    - **Funtzioak**: iragazi baliabide erreserbagarrietan esleitzen zaizkion funtzio lehenetsiak.
    - **Antolamendu unitateak**: erreserbatu baliabideak esleitzen zaizkion antolaketa unitateen arabera.

6. Hasierako eskakizunaren emaitzarekin konforme ez bazaude, iragazkiaren irizpideak alda ditzakezu. Zabaldu **Iragazkiaren ikuspegia** orria ezkerrean eta ondoren hautatu **Bilatu** baliabide osagarriak aurkitzeko.

    ![Iragazi ikuspegiaren panela](media/Resource-Management-image16.png)

7. Emaitzak nola ordenatzen diren aldatzeko, hautatu **Ordenatu**.

    ![Ordena komandoa](media/Resource-Management-image17.png)

8. Hautatu baliabideak eskakizunean zehaztutako eskaeraren arabera, saretaren goiko aldean adierazten den moduan. Saretako gelaxken aukera garbitu eta baliabide-ahalmena irekita utzi dezakezu. Baliabide bakarra aldi berean erreserbatu daiteke.

9. Aukeratu **Liburua** hautatutako baliabidea erreserbatzea eta Antolaketa taula irekita uztea, baliabide osagarriak aukeratu ahal izateko. Bestela, hautatu **Liburua eta irteera** hautatutako baliabidea erreserbatzeko eta Antolaketa taula ixteko.

    ![Erreserbatzeko baliabidea](media/Resource-Management-image19.png)

    Erreserbatutako orduen jakinarazpena jasotzen duzu. Eskariaren adierazleek erreserba-eskakizuna betetzen den eta zenbat geratzen den erakusten dute. Aukeratutako baliabidearen ahalmena zenbat kontsumitzen den ere ikus dezakezu. Aukeratu **Zabaldu** baliabide erreserbagarriei buruzko xehetasun gehiago ikusteko.

9. Itzuli **Taldekide guztiak** ikuspegira. Saretan, ohartu baliabide generikoa izena duen baliabide ordez aldatu dela, eta 40 ordu zerrendatzen direla baliabide horretarako erreserbatuta.

    ![Taldekide guztien sareta eguneratua](media/Resource-Management-image20.png)

    > [!NOTE]
    > Ez dira esleitutako orduak erakusten, zuzenean taldean erreserbatu direlako. Ez zuten zereginen zereginaz baliatu.

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a>Esleitu baliabide generikoak zereginei eta sortu baliabide eskakizunak

PSAn, zereginak sor ditzakezu eta gero baliabide generikoak esleitu. Horrela, baliabideen eskaera tokiko ordezkariek ordezkatu dezakete zure egutegia eta finantza-zenbakiak zenbatzen dituzun bitartean. Baliabide generikoetarako baliabide eskakizunak sor ditzakezu eta bete.

1. **Proiektuak** orrialdean **Antolaketa** fitxan, aukeratu **Gehitu** zeregin bat sortzeko.

    ![Zeregin berria sortuta](media/Resource-Management-image21.png)

2. **Baliabideak** eremuan aukeratu **Baliabideen hautatzailea** sinboloa. Baliabide hautatzailea proiektuan dauden taldekideak agertzen dira.

    ![Baliabideen hautatzailea](media/Resource-Management-image22.png)

3. Idatzi baliabide generiko berriaren izena eta, ondoren, hautatu **Sortu**.

    ![Sartu den baliabide generiko berri baten izena](media/Resource-Management-image23.png)

4. **Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroan **Funtzioa** eremuan agertzen denean, hautatu baliabide generikorako funtzioa. **Baliabide-unitatea** eremuan, hautatu baliabide generikoa lortzeko antolakuntza-unitatea. Ondoren, hautatu **Gorde**.

    ![Sorrera bizkorra: proiektuko taldekidea elkarrizketa-koadroa](media/Resource-Management-image24.png)

    Taldekide generikoa orain zereginera esleituta dago.

    ![Taldekide generikoa zereginera esleituta dago.](media/Resource-Management-image25.png)

    **Taldea** fitxan, taldekide generikoko berria ikusiko duzu. Kontuan izan orduak bakarrik esleituta dituela. Ordu horiek taldekide generikoari esleitzen zaizkion zeregin guztien batura dira. Taldekide generikoak oraindik ez du ordurik edo baliabide eskakizunik behar.

    ![Taldekide generikoa Taldea fitxan](media/Resource-Management-image26.png)

5. Orain taldekide generikoa beste zeregin batzuei esleitu diezaiekezu Baliabide hautatzailea erabiliz.

    ![Baliabide hautatzailean taldekide generikoa](media/Resource-Management-image27.png)

    Baliabide generikoa zereginetan esleitzen amaitu duzunean, baliabide generikorako baliabide eskakizuna sor dezakezu.

5. **Taldea** fitxa, hautatu baliabide generikoa eta ondoren hautatu **Sortu eskakizuna**.

    ![Sortu eskakizuna komandoa](media/Resource-Management-image28.png)

    Baldintza sortzen denean, taldekide generikoak orduak eta esteka beharko ditu baliabideen eskakizuna lortzeko.

    ![Baliabidearen eskakizunaren esteka](media/Resource-Management-image29.png)

    Erreserba izena duen baliabide batek osatu eta bete ostean, baliabide generikoa taldetik kenduko da eta izena duen baliabidearen bidez ordezkatuko da.

    ![Baliabide generikoa izena duen baliabidearen ordez](media/Resource-Management-image30.png)

    **Antolaketa** fitxan, baliabide generikoen esleipenak izena duen baliabidearen bidez kendu eta ordezkatu egingo dira.

    ![Antolaketa fitxan, baliabide generikoen esleipenak izena duen baliabidearen bidez ordezkatuta](media/Resource-Management-image31.png)

    > [!NOTE]
    > Jokabide hau izena duen baliabide bat baliabide generikoen eskakizuna guztiz erreserbatzen denean gertatzen da. Izena duen baliabide batek partzialkui baliabide generikoen eskakizuna ordezkatzen duenean edo izena duten baliabide anitzek baliabide generikoen eskakizuna ordezkatzen dutenean, baliabide generikoa zereginari esleitzen zaio.

    Hurrengo irudian, 80 orduko zereginak bost eguneko iraupena izan dezan aurreikusi da (egunean 16 ordu bost egunetan zehar) eta **Funtzionala** izena duen baliabide generikoari esleitu zaio.

    ![Laurogei ordu eta bost eguneko zeregina Funtzionala baliabide generikoari esleituta](media/Resource-Management-image32.png)

    Eskakizuna sortzen duzunean, 80 orduz bost egunetan zehar izaten da.

    ![80 egunetan sortutako eskakizuna bost egunetan zehar](media/Resource-Management-image33.png)

    Eskuragarri dauden baliabideak egunean zortzi orduz bakarrik funtzionatzen dutenez, bi baliabide behar dira baldintza betetzeko.

    ![Bigarren baliabidea](media/Resource-Management-image35.png)

    **Taldea** fitxan, ikus dezakezu baliabide generikoak ez duela ordurik behar, baina esleitutako orduak betetzea osatzen duten bi baliabideekin batera agertzen dira.

    ![Bi baliabide izendatu dira Taldea fitxan](media/Resource-Management-image36.png)

    **Antolaketa** fitxan, baliabide generikoa zereginari esleitzen zaio.

    ![Baliabide generikoak Antolaketa fitxan](media/Resource-Management-image37.png)

PSAk ez ditu bi baliabideak zereginera esleitzen, jokaera horrek aurreikusteko antolaketa txikiagoa sortuko lukeelako. Adibide erraz honetan, erraza da orduak bi baliabideen artean banatzea. Hala ere, zeregin anitz eta baliabide anitz biltzen dituzten eszenatoki konplexuagoetan, PSAk zeregin ugaritan baliabide ugarietarako jasotzen diren erreserbak nola esleitu behar litzaizkion hipotesi batzuk egin beharko lituzke.

Hori dela eta, gertakari horietan, proiektuaren arduraduna arduratzen da erreserba anitzak analizatzeaz eta behar izanez gero esleitzea. Erreserbak esleitzeko, proiektuaren arduradunak zereginak baliabide generikoetatik esleitzen dizkio izendatutako baliabideei, eta ondoren erabiltzen du **Kontziliazioa** ikuspegia, esleipena erreserbak funtzionatzen duela ziurtatzeko.

### <a name="edit-a-resource-requirement"></a>Baliabidearen eskakizuna editatu

Baliabideen eskakizuna sortu ondoren, proiektu-kudeatzaileak edo baliabideen kudeatzaileak xehetasunak editatu nahi ditu bilaketa-irizpideak afinatzeko. Baliabideen eskakizuna editatzeko, jarraitu urrats hauek.

1. **Proiektuak** orrialdean **Taldea** fitxan, hautatu baliabide generikoko edozein eskakizunerako esteka.
2. **Baliabideen eskakizuna** agertzen den orrian, hainbat atributu eguneratu ditzakezu. Hona hemen zenbait adibideak:

    - Izena
    - Hasiera-data
    - Amaiera-data
    - Iraupena
    - Baliabide mota

**Baliabideen eskakizuna** orrialdean, proiektuaren kudeatzaileak edo baliabideen kudeatzaileak informazio hau ere defini dezake:

- Trebetasunak
- Funtzioak
- Baliabideen hobespenak
- Hobetsitako erakunde-unitateak

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a>Eguneratu baliabideen erreserbak proiektu batean erreserbatu ondoren

Baliabide generikoak edo izena dutenak proiektu talde batean gehitu ondoren, baliabidearen erreserbak alda ditzakezu.

1. **Proiektuak** orrialdean **Taldea** fitxan, aukeratu taldekidea eta gero hautatu **Mantendu erreserbak**.

    ![Antolaketa-panela ireki da hautatutako taldekideentzat](media/Resource-Management-image40.png)

    Antolaketa-panela agertzen da eta proiektuko taldekideen erreserbak agertzen dira. Zabaldu taldekidearen erregistroa proiektu honen aurka erreserbatu diren orduak eta taldekidearen ahalmena kontsumitzen duten gainerako proiektuak ikusteko.

2. Hautatu eta arrastatu erreserba luzatzeko edo laburtzeko. **Sortu Baliabideen Erreserba** elkarrizketa-koadroa agertuko da erreserba egokitzeko.

    ![Sortu baliabide-erreserba elkarrizketa-koadroa](media/Resource-Management-image41.png)

3. Egin klik eskuineko botoiarekin erreserban. Jarraian, ekintza hauek burutzeko lasterbide menua erabil dezakezu:

    - Aldatu erreserbaren egoera.
    - Editatu erreserba.
    - Proiektuko taldeko baliabide bat ordeztu.

### <a name="change-the-booking-status"></a>Aldatu erreserbaren egoera

Lehenetsitako edo pertsonalizatutako erreserba egoera alda dezakezu.

![Komandoaren egoera aldatu](media/Resource-Management-image42.png)

Egoera hauek daude PSA aplikazioan:

- **Utzita**: egoera honek baliabideen erreserba bertan behera uzten du eta baliabidearen ahalmena askatzen du.
- **Erreserba gogorra**: egoera honek baliabideen ahalmena kontsumitzen du. Erreserbak normalean egoera hau du **Mantendu Erreserbak** **Taldekide guztiak** saretatik **Proiektuak** orrian irekitzen duzunean.
- **Erreserba biguna**: egoera honek baliabide bat gehitzen dio taldeari baina ez du baliabidearen ahalmena kontsumitzen. Baliabidea lan potentzialerako erreserbatu dela adierazten du, baina hala ere, gaitasuna badu beste lan batzuetan behar bada. Baliabideen erabilgarritasun orokorraren iritziz, erreserba leunek erreserba gogorrak baino beste egoera bat dute.
- **Proposatua**: egoera honek baliabideen kudeatzailearen edo proiektuaren kudeatzailearen proposamena adierazten du. Proposamenek ez dute baliabide baten ahalmena kontsumitzen eta baliabidea ez da proiektuko taldeari gehitzen. Baliabidea taldean erreserbatzeko, proiektuaren zuzendariak proposamena onartu behar du.

### <a name="submit-resource-requests"></a>Bidali baliabide-eskaerak

Baliabide-kudeatzaile batek bete behar duen eskaera (baliabide-eskakizuna) egiteko erabiltzen dira baliabide eskakizunak. Dagoeneko taldean dagoen baliabide generikoa lortzeko, baliabide eskaera zuzenean bidal dezakezu. Baliabide eskaera bi eratara bete daiteke:

- Baliabideen kudeatzaileak eskaera zuzenean betetzen du. +Kasu honetan, baliabide generikoa izena duen baliabide erreserba gogorraren ordez ordezkatuko da.
- Baliabideen kudeatzaileak baliabide bat proposatzen dio proiektuaren kudeatzaileari, eta proiektuaren kudeatzaileak proposatutako baliabidea onartu edo arbuiatu egiten du.

#### <a name="direct-fulfillment-of-resource-requests"></a>Baliabideen eskaerak zuzenean betetzea

Baliabide-eskakizuna sortzen denean, proiektu-kudeatzaileak baliabide generiko baterako baliabide-eskaera aurkez dezake baliabidea hautatuz eta ondoren hautatuta **Bidali eskaera** aukera.

![Bidali eskaera botoia](media/Resource-Management-image45.png)

Baliabideari buruzko iruzkinak eskaera betetzen ari den baliabide kudeatzaileari eman diezaiokezu. Eskaera bidali ondoren, **Egoera** eremua taldekidearentzako aldatu egingo da **Bidalita** egoerara.

![Aukerako iruzkinak sartu](media/Resource-Management-image46.png)

Baliabideen kudeatzaileak eskaera betetzen duenean, taldekide generikoa izena duen baliabidearen ordez ordezkatuko da **Taldekide guztiak** saretan.

![Taldekide generikoa izena duen baliabidearengatik ordezkatu dute Taldekide guztiak sartean](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a>Erabili baliabide proposamen bat baliabide eskaeretarako

Baliabideen eskaera zuzenean erreserbatu beharrean, baliabideen kudeatzaileak proiektuaren kudeatzaileari baliabidea proposatu diezaioke. Baliabideen kudeatzaile batek aukera hau erabil dezake eskakizunekin bat datorrenean eskuragarri ez dagoenean. Baliabideen kudeatzaileak baliabide bat proposatzen duenean, proiektuaren kudeatzaileak ikusten du **Egoera** eremua taldekide generikorako aldatu egingo dela **Beharrak berrikustea** egoerara.

![Taldekide generikoaren egoera Beharrak berrikustea egoerara aldatu da](media/Resource-Management-image48.png)

Proposatutako baliabidea proposamenaren erreserbaren eragina bistaratzearekin batera ikusteko, egin klik bikoitza **Beharrak berrikustea** egoera duen taldekidean. Ondoren hautatu **Proposatutako baliabideak** fitxa.

![Baliabide proposatuak fitxa](media/Resource-Management-image49.png)

Aukeratu **Onartu proposamen guztiak** proposatutako baliabide guztiak onartzeko edo **Proposamen guztiak arbuiatu** arbuiatzeko. Proposatutako baliabideak onartzen badituzu, proiektuan erreserbatu egiten dira taldekide gisa eta baliabide generikoak ordezkatzen dituzte.

> [!NOTE]
> Proposatutako baliabide guztiak onartu edo baztertu beharko dituzu. Ezin dituzu partzialki onartu edo arbuiatu.

### <a name="substitute-a-resource-on-the-project-team"></a>Proiektuko taldeko baliabide bat ordeztu

Batzuetan, proiektuko kudeatzaileak proiektuan erreserbatutako taldekide bat ordezkatu behar du.

1. **Proiektuak** orrialdean **Taldea** fitxan, aukeratu ordezkoa behar duen baliabidea eta gero hautatu **Mantendu erreserbak**.
2. Zabaldu baliabidea esleitutako proiektuak ikusteko.

    ![Esleitutako proiektuak erakusteko zabaldutako baliabidea](media/Resource-Management-image50.png)

3. Egin klik proiektuan eskuineko botoiarekin, eta, ondoren, hautatu **Baliabidea ordezkatu**.
4. Uneko baliabidea ordezkatu nahi duzun baliabidea ezagutzen baduzu, hautatu edo idatzi izena eta, ondoren, hautatu **Esleitu berriro**.

    ![Ordezko baliabidea zehaztea](media/Resource-Management-image51.png)

    Bestela, jarraitu urrats hauei baliabidea bilatzeko:

    1. Hautatu **Bilatu ordezkoa**.

        ![Ordezko baliabidea bilatzea](media/Resource-Management-image52.png)

        Antolaketa laguntzaileak eskuragarri dauden ordezkoen zerrenda itzultzen du. Antolaketa laguntzailean, erabilgarri dauden baliabideak iragazi ditzakezu ordezko egoki bat bilatzeko.

        ![Erabilgarri dauden ordezkoen zerrenda.](media/Resource-Management-image53.png)

    2. Baliabidea ordezkatzeko, hautatu nahi duzun baliabidea eta, gero, hautatu **Ordezkatu**.

        ![Ordeztu hautatutako baliabidea](media/Resource-Management-image54.png)

    Erreserbak eta zereginak baliabide berriarekin ordezkatuko dira.

    ![Erreserbak eta zereginak baliabide berriarekin ordezkatuko dira](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a>Kontziliatu taldekideen erreserbak eta esleipenak

Taldekideentzat, erreserbak eta zereginak bateratu egiten dira. Alegia, baliabideek zereginak izan ditzakete baina erreserbarik ez, edo erreserbak izan ditzakete baina zereginik ez. Egokiena, erreserbak eta zereginak lerrokatuta egotea izango litzateke, baliabideek zereginak betetzeko gaitasuna konprometituta izan dezaten. Hala ere, erreserbak erabilgarritasunean oinarrituta egon litezke, eta zereginen aldaketak proiektuak aurrera egin ahala alda litezke. Hori dela eta, erreserbak eta zereginen akoplamendu solteak malgutasuna ematen du.

PSAk proiektu-kudeatzaileei taldekideen erreserbak eta proiektuko taldeen zereginak bateratzeko aukera ematen dien **Kontziliazioa** fitxa du.

![Kontziliazioa fitxa](media/Resource-Management-image56.png)

**Kontziliazioa** fitxak erreserbak eta zereginak erakusten ditu zereginen esleipen bakoitzaren mailan taldekide bakoitzarentzat. Denbora erakusten ditu gelaxkatan, hilabetetik egunera arteko epeak.

Fitxak proiektuaren guztizko garbi osoa ere erakusten du, zutabe guztiekin batera.

Baliabide bakoitzerako, fitxak taldekidearen erreserben desberdintasunak kalkulatzen ditu eta taldekideen zereginen esleipenekin bateratzen ditu. Egokiena, aldea 0 (zero) izatea da. Beste modu batera esanda, ez litzateke alderik egon behar erreserbaren eta esleipenen artean. Desberdintasunak koloreztatuta eta itzalpean daude bi baldintzetan arreta jartzeko:

- **Erreserba eskasia**: erreserba eskasia gertatzen da baliabideek erreserbak baino esleipen gehiago dituztenean. Ez denez erreserbatu gaitasun hori, baliteke proiektu-kudeatzaileak baldintza hori zuzentzea baliabideen erreserbak hedatuz defizita estaltzeko.
- **Gehiegizko erreserbak** - Gehiegizko erreserbak baliabide bat proiektuan erreserbatuta dagoenean baina zereginetara esleitu ez denean gertatzen da. Baldintza hau onargarria izan daiteke zereginen esleipena gertatu baino lehen proiektuan erreserbatu den kasuetan. Hala ere, baliteke beste kasu batzuetan baliabidea ez izatea aurreikusita zereginei esleitzeko. Kasu horietan, proiektu-kudeatzaileak baliabidearen erreserbak bertan behera uztea pentsatu beharko luke, gaitasuna beste proiektu baterako erabili ahal izateko.

Zenbait kasutan, eguneko maila baino maila altuagoan ikusten baduzu (adibidez, hilabetearen maila), baliteke zero diferentzia garbia izatea baliabide batentzat (beste modu batera esanda, erreserbak = zereginak). Hala ere, Astea mailari erreparatuz gero, baliteke 0 (zero) orduko esleipenak eta 40 orduko erreserbak daudela ikustea lehenengo astean, baina 40 orduko esleipenak eta 0 (zero) orduko erreserbak bigarren astean. Oro har, erreserbak eta zereginak bateratu egiten dira, baina aste batetik bestera desberdinak dira.

Denbora-maila altuagoak ikusten dituzunean, **Kontziliazioa** fitxak gelaxkak adierazle bat du denbora maila baxuagoetan desberdintasunak daudela jakinarazteko. Gelaxka batean klik bikoitza eginez, handiagotu dezakezu aldea ikusteko. Ondoren, egin klik eskuineko botoiarekin hurbiltzeko. Baliabide bat hautatuta eta, ondoren, erabilita **Hurrengo aldea** kontrola saretako tresna-barran, baliabide horren erreserbak eta zereginen arteko hurrengo diferentziara joan zaitezke. Ondoren, erabil dezakezu **Aurreko aldea** kontrola atzera egiteko. Alderantzizko adierazlea eta nabigazio portaera ere desaktiba ditzakezu **Ezarpenak** aukeran.

![Diferentziaren adierazlea](media/Resource-Management-image57.png)

Zereginen esleipenak dituzun baina erreserbarik ez baduzu, **Proiektuak** aorrian, **Kontziliazioa** fitxan, erreserba eskasia aukeratu dezakezu eta, ondoren, hautatu **Hedatu erreserba**. **Luzatu Erreserba** elkarrizketa-koadroa agertuko da eta baliabidearen eskasiari aurre egiteko beharrezkoa den erreserba erakusten du. Gainera, baliabideek dituzten erreserbak agertzen dira proiektu guztietan edo beste erakunde antolatzaile batzuetan. Aukeratzen baduzu **Ados** baliabidearen erreserba sortzeko, baliabidearen erabilgarritasuna edozein dela ere, gerta daiteke erreserba gehiegi egotea.

![Luzatu Erreserba elkarrizketa-koadroa](media/Resource-Management-image58.png)

Orduan, proiektu-kudeatzaileak edo baliabide-kudeatzaileak antolaketa-panela erabil dezake baliabide batek bere ahalmenetatik harago gaitasunak gainditutako edozein egoera kudeatzeko.
