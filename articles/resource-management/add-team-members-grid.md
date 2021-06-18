---
title: Gehitu Team kideen saretako taldeko kideak
description: Gai honek talde kideko baliabideak kudeatzeko moduari buruzko informazioa eskaintzen du.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 95f9e1d836e49672cfb51ace59aa77ea9da65b35
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998846"
---
# <a name="add-team-members-from-the-team-member-grid"></a>Gehitu Team kideen saretako taldeko kideak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-ek baliabideen kudeaketako panela biltzen du baliabideen eskaeraren eta erakundearen erabileraren ikuspegi orokorra eskaintzen duena. Panel honetako diagramak erabil ditzakezu informazioa ikusteko:

- **Baliabideen eskaria**: **Baliabide aktiboen eskaera** taulan aurkeztu diren baliabideak erakusten dira. Baliabideak funtzioaren edo proiektuaren arabera biltzen dira.
- **Bidali gabeko baliabideen eskaria**: **Esleitu gabeko baliabideen eskaria** taulan aurkeztu ez diren baliabide-eskakizun guztiak erakusten dira. Grafiko honekin, Baliabideen kudeatzailek eskaera ez dela irmoa ikusten dute eta baliabide eskaera bidez bidaltzen laguntzen die.
- **Erabilera erabilgarriak azken astean**: **Erabilera funtzioa** taulan ikus daiteke erakundearen benetako fakturazioaren portzentajea bere eginkizunaren arabera fakturazioaren aldera.

    > [!NOTE]
    > **Erabilera funtzioa** taula eskuragarri egoteko, sortu **UpdateRoleUtilization** lan-fluxua exekutatzen duen lana. Lan errepikari hau zazpi egunez behin egiten da aurreko zazpi egunetako erabilgarritasuna kalkulatzeko. Emaitzak funtzioaren arabera batu dira.

## <a name="manage-project-team-members"></a>Proiektu-taldekideak kudeatu

Proiektuaren kudeatzaileek Baliabideen kudeatzailearen panela erabil dezakete proiektuetan baliabideak kudeatzeko. Adibidez, taldekide bat zuzenean gehitu dezakete proiektu batean eta taldekide bat erreserbatu baliabide generiko batek harrapatutako baliabide eskakizunak betetzeko.

### <a name="add-a-team-member-directly-to-a-project"></a>Gehitu taldekidea zuzenean proiektu bati

Taldekide bat zuzenean proiektu batean gehitzeko, **Proiektuak** inprimakian **Taldea** fitxan, aukeratu **Berria**. **Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroa agertuko da. Elkarrizketa-koadro honetan zeregin hauek egin ditzakezu:

- **Erreserbatu izendatutako baliabidea**: **Baliabide erreserbagarria** eremuan, hautatu baliabidearen izena. Ondoren, hautatu funtzioa, zehaztu epea eta hautatu esleipen metodoa. Aukeratu duzun izena duen baliabidea proiektuari gehitzen zaio hautatutako esleipen metodoa eta baliabideen egutegia erabiliz.
- **Gehitu baliabide generikoa**: utzi **Baliabide erreserbagarria** eremua hutsik eta, ondoren, hautatu funtzioa, ezarri aldia eta hautatu hobetsitako esleipen metodoa. Baliabide generiko bat gehitzen zaio taldeari leku-marka gisa. Leku-hartzaileak taldean izendatutako baliabideak erreserbatzeko erabiltzen den eskaera eredua du. Baldintza proiektuaren egutegiaren arabera egiten da.
- **Gehitu izendatutako baliabidea taldeari baliabideen ahalmena kontsumitu gabe**: **Baliabide erreserbagarria** eremuan, hautatu baliabide bat. Hautatu aldia eta hautatu **Ez** esleipen metodoa. Baliabidea taldeari gehitzen zaio, baina baliabidearen ahalmena ez da erreserba bidez kontsumitzen.

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a>Erreserbatu taldekide bat baliabide generiko baterako eskakizunak betetzeko

Project Operations-en, baliabide generiko bat erreserbatu dezakezu proiektuko talde batean. Rola, behar den gaitasuna eta gaitasun hori nola banatzen den ere zehaztu dezakezu. Baliabidearen eskakizunean, baliabide generikoarekin lotutako atributuak zehaztu ditzakezu. Ezaugarri horien artean beharrezkoak diren trebetasunak, nahiago den antolakuntza-unitatea eta hobetsitako baliabideak daude.

Jarraitu urrats hauei garatzaileentzako baliabide generiko batean eskatutako trebetasunak zehazteko.

1. **Proiektuak** inprimakian **Taldea** fitxan, hautatu **Berria** baliabide generikoa erreserbatzeko.
2. **Taldekide guztiak** ikuspegian, **Baliabideen eskakizuna** zutabean, hautatu esteka baliabide generikorako beharrezkoak diren trebetasunak gehitzeko.
3. **Baliabideen eskakizuna** inprimakian, **Trebetasunak** saretan, hautatu elipsia (**...**) eta hautatu **Gehitu eskakizun berriaren ezaugarria** sustatzailearentzako beharrezkoak diren gaitasunak gehitzeko.
4. **Sorrera bizkorra: eskakizunaren ezaugarria** elkarrizketa-inprimakian **Ezaugarria** eremuan agertzen denean, hautatu eskatutako trebetasuna.
5. **Balorazioaren balioa** eremuan, hautatu trebetasun horren maila. 
6. **Baliabideen eskakizuna** eremuan, ezarri eskakizuna baliabide iturriak antolakuntza unitateetatik edo baita izendatutako baliabideak ere. Bukatu duzunean, hautatu **Gorde**.
7. **Baliabideen eskakizuna** inprimakian, hautatu **Liburua** baliabide eskakizuna betetzeko. Baliabide generikoak ere hauta ditzakezu **Taldekide guztiak** saretan eta gero hautatu **Liburua**.

    > [!NOTE]
    > Adibide honetan, 40 ordu behar dira baina ez erreserbatu gabeko orduak, baliabide generikoek erreserbaziorik ez dutelako. Gainera, ez dira ordu esleituak, baliabide generikoa zuzenean taldeari gehitu zitzaiolako, zeregin-esleipena erabiliz gehitu beharrean.

    **Programazio laguntzailea** inprimakian, erabilgarri dauden baliabideak iragazi ditzakezu baliabideen eskakizunean zehazten diren baldintzen arabera. Baliabideak Antolaketa taulan zehaztutako sailkapen parametroen arabera ordenatzen dira.

   Hauek dira gehien erabiltzen diren iragazkiak:

    - **Ezaugarriak puntuazioarekin batera**: gaitasunak, ziurtagiriak eta baliabideen beste ezaugarri batzuen arabera iragazi, gaitasunen balorazioez gain.
    - **Funtzioak**: iragazi baliabide erreserbagarrietan esleitzen zaizkion funtzio lehenetsiak.
    - **Antolamendu unitateak**: erreserbatu baliabideak esleitzen zaizkion antolaketa unitateen arabera.

8. Hasierako eskakizunaren emaitzarekin konforme ez bazaude, iragazkiaren irizpideak alda ditzakezu. Zabaldu **Iragazkiaren ikuspegia** orria ezkerrean eta ondoren hautatu **Bilatu** baliabide osagarriak aurkitzeko. Emaitzak nola ordenatzen diren aldatzeko, hautatu **Ordenatu**.
9. Hautatu baliabideak eskakizunean zehaztutako eskaeraren arabera, saretaren goiko aldean adierazten den moduan. Saretako gelaxken aukera garbitu eta baliabide-ahalmena irekita utzi dezakezu. Baliabide bakarra aldi berean erreserbatu daiteke.
10. Aukeratu **Liburua** hautatutako baliabidea erreserbatzea eta Antolaketa taula irekita uztea, baliabide osagarriak aukeratu ahal izateko. Bestela, hautatu **Liburua eta irteera** hautatutako baliabidea erreserbatzeko eta Antolaketa taula ixteko.
11. Itzuli **Taldekide guztiak** ikuspegira. Saretan, ohartu baliabide generikoa izena duen baliabide ordez aldatu dela, eta 40 ordu zerrendatzen direla baliabide horretarako erreserbatuta.

    > [!NOTE]
    > Ez dira esleitutako orduak erakusten, zuzenean taldean erreserbatu direlako. Ez zuten zereginen zereginaz baliatu.

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a>Esleitu baliabide generikoak zereginei eta sortu baliabide eskakizunak

Project Operations-en, zereginak sor ditzakezu eta gero baliabide generikoak esleitu. Baliabideen eskaera tokiko ordezkariek ordezkatu dezakete zure egutegia eta finantza-zenbakiak zenbatzen dituzun bitartean. Baliabide generikoetarako baliabide eskakizunak sor ditzakezu eta bete.

1. **Proiektuak** inprimakian, **Antolaketa** fitxan, aukeratu **Gehitu** zeregin bat sortzeko.
2. **Baliabideak** eremuan aukeratu **Baliabideen hautatzailea** sinboloa. Baliabide hautatzailea proiektuan dauden taldekideak agertzen dira.
3. Idatzi baliabide generiko berriaren izena eta, ondoren, hautatu **Sortu**.
4. **Sorrera bizkorra: proiektuko taldekidea** elkarrizketa-koadroan **Funtzioa** eremuan agertzen denean, hautatu baliabide generikorako funtzioa. 
5. **Baliabide-unitatea** eremuan, hautatu baliabide generikoa lortzeko antolakuntza-unitatea. Ondoren, hautatu **Gorde**. Taldekide generikoa orain zereginera esleituta dago.

   **Taldea** fitxan, taldekide generikoko berria ikusiko duzu. Kontuan izan orduak bakarrik esleituta dituela. Ordu horiek taldekide generikoari esleitzen zaizkion zeregin guztien batura dira. Taldekide generikoak ez du ordurik edo baliabide eskakizunik behar.

6. Orain taldekide generikoa beste zeregin batzuei esleitu diezaiekezu Baliabide hautatzailea erabiliz.

   Baliabide generikoa zereginetan esleitzen amaitu duzunean, baliabide generikorako baliabide eskakizuna sor dezakezu.

7. **Taldea** fitxa, hautatu baliabide generikoa eta ondoren hautatu **Sortu eskakizuna**. Baldintza sortzen denean, taldekide generikoak orduak eta esteka beharko ditu baliabideen eskakizuna lortzeko.

  Erreserba izena duen baliabide batek osatu eta bete ostean, baliabide generikoa taldetik kenduko da eta izena duen baliabidearen bidez ordezkatuko da. **Antolaketa** fitxan, baliabide generikoen esleipenak izena duen baliabidearen bidez kendu eta ordezkatu egingo dira.

  > [!NOTE]
  > Jokabide hau izena duen baliabide bat baliabide generikoen eskakizuna guztiz erreserbatzen denean gertatzen da. Izena duen baliabide batek partzialkui baliabide generikoen eskakizuna ordezkatzen duenean edo izena duten baliabide anitzek baliabide generikoen eskakizuna ordezkatzen dutenean, baliabide generikoa zereginari esleitzen zaio.

Project Operations-ek ez ditu bi baliabideak zereginera esleitzen, jokaera horrek aurreikusteko antolaketa txikiagoa sortuko lukeelako. Adibide erraz honetan, erraza da orduak bi baliabideen artean banatzea. Hala ere, zeregin anitz eta baliabide anitz biltzen dituzten eszenatoki konplexuagoetan, PSAk zeregin ugaritan baliabide ugarietarako jasotzen diren erreserbak nola esleitu behar litzaizkion hipotesi batzuk egin beharko lituzke.

Hori dela eta, gertakari horietan, Proiektuaren arduraduna arduratzen da erreserba anitzak analizatzeaz eta behar izanez gero esleitzea. Erreserbak esleitzeko, Proiektuaren arduradunak zereginak baliabide generikoetatik esleitzen dizkio izendatutako baliabideei, eta ondoren erabiltzen du **Kontziliazioa** ikuspegia, esleipena erreserbak funtzionatzen duela ziurtatzeko.

### <a name="edit-a-resource-requirement"></a>Baliabidearen eskakizuna editatu

Baliabideen eskakizuna sortu ondoren, Proiektu-kudeatzaileak edo Baliabideen kudeatzaileak xehetasunak editatu nahi ditu bilaketa-irizpideak afinatzeko. Baliabideen eskakizuna editatzeko, jarraitu urrats hauek.

1. **Proiektuak** inprimakian, **Taldea** fitxan, hautatu baliabide generikoko edozein eskakizunerako esteka.
2. **Baliabideen eskakizuna** inprimakia agertzen denean, sartu beharrezko eremuko informazioa

   **Baliabideen eskakizuna** inprimakian, proiektuaren kudeatzaileak edo baliabideen kudeatzaileak gaitasunak, rolak, baliabideen lehentasunak eta lehentasunezko antolakuntza-unitatea ere defini ditzake.

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a>Eguneratu baliabideen erreserbak proiektu batean erreserbatu ondoren

Baliabide generikoak edo izena dutenak proiektu talde batean gehitu ondoren, baliabidearen erreserbak alda ditzakezu.

1. **Proiektuak** inprimakian **Taldea** fitxan, aukeratu taldekidea eta gero hautatu **Mantendu erreserbak**.
 
   Antolaketa-panela agertzen da eta proiektuko taldekideen erreserbak agertzen dira. Zabaldu taldekidearen erregistroa proiektu honen aurka erreserbatu diren orduak eta taldekidearen ahalmena kontsumitzen duten gainerako proiektuak ikusteko.

2. Hautatu eta arrastatu erreserba luzatzeko edo laburtzeko. **Sortu Baliabideen Erreserba** elkarrizketa-koadroa agertuko da erreserba egokitzeko.
3. Egin klik eskuineko botoiarekin erreserban. Jarraian, ekintza hauek burutzeko lasterbide menua erabil dezakezu:

    - Aldatu erreserbaren egoera
    - Editatu erreserba
    - Proiektuko taldeko baliabide bat ordeztu

### <a name="change-the-booking-status"></a>Aldatu erreserbaren egoera

Lehenetsitako edo pertsonalizatutako erreserba egoera alda dezakezu.

Egoera hauek daude Project Operations aplikazioan:

- **Utzita**: baliabideen erreserba bertan behera uzten du eta baliabidearen ahalmena askatzen du.
- **Erreserba tinkoa**: baliabideen ahalmena kontsumitzen du. Erreserbak normalean egoera hau du **Mantendu Erreserbak** **Taldekide guztiak** saretatik **Proiektuak** inprimakian irekitzen duzunean.
- **Behin-behineko erreserba**: baliabide bat gehitzen dio taldeari baina ez du baliabidearen ahalmena kontsumitzen. Egoera honek baliabidea lan potentzialerako erreserbatu dela adierazten du, baina hala ere, gaitasuna badu beste lan batzuetan behar bada. Baliabideen erabilgarritasun orokorraren iritziz, erreserba leunek erreserba gogorrak baino beste egoera bat dute.
- **Proposatua**: Baliabideen kudeatzailearen edo Proiektuaren kudeatzailearen proposamena adierazten du. Proposamenek ez dute baliabide baten ahalmena kontsumitzen eta baliabidea ez da proiektuko taldeari gehitzen. Baliabidea taldean erreserbatzeko, Proiektuaren zuzendariak proposamena onartu behar du.

### <a name="submit-resource-requests"></a>Bidali baliabide-eskaerak

Baliabide-kudeatzaile batek bete behar duen eskaera, edo baliabide-eskakizuna, egiteko erabiltzen dira Baliabide-eskakizunak. Dagoeneko taldean dagoen baliabide generikoa lortzeko, baliabide eskaera zuzenean bidal dezakezu. Baliabide eskaera bi eratara bete daiteke:

- Baliabideen kudeatzaileak eskaera zuzenean betetzen du. +Kasu honetan, baliabide generikoa izena duen baliabide erreserba gogorraren ordez ordezkatuko da.
- Baliabideen kudeatzaileak baliabide bat proposatzen dio Proiektuaren kudeatzaileari, eta Proiektuaren kudeatzaileak proposatutako baliabidea onartu edo arbuiatu egiten du.

#### <a name="direct-fulfillment-of-resource-requests"></a>Baliabideen eskaerak zuzenean betetzea

Baliabide-eskakizuna sortzen denean, Proiektu-kudeatzaileak baliabide generiko baterako baliabide-eskaera aurkez dezake baliabidea hautatuz eta ondoren hautatuta **Bidali eskaera** aukera. Baliabideari buruzko iruzkinak eskaera betetzen ari den Baliabide-kudeatzaileari eman diezaiokezu. Eskaera bidali ondoren, **Egoera** eremua taldekidearentzako aldatu egingo da **Bidalita** egoerara. Baliabideen kudeatzaileak eskaera betetzen duenean, taldekide generikoa izena duen baliabidearen ordez ordezkatuko da **Taldekide guztiak** saretan.

#### <a name="use-a-resource-proposal-for-resource-requests"></a>Erabili baliabide proposamen bat baliabide eskaeretarako

Baliabideen eskaera zuzenean erreserbatu beharrean, Baliabideen kudeatzaileak Proiektuaren kudeatzaileari baliabidea proposatu diezaioke. Baliabideen kudeatzaile batek aukera hau erabil dezake eskakizunekin bat datorrenean eskuragarri ez dagoenean. Baliabideen kudeatzaileak baliabide bat proposatzen duenean, Proiektuaren kudeatzaileak ikusten du **Egoera** eremua taldekide generikorako aldatu egingo dela **Beharrak berrikustea** egoerara.

Proposatutako baliabidea proposamenaren erreserbaren efektuaren bistaratzearekin batera ikus dezakezu. 

1. Egin klik bikoitza egoera duen taldekidean **Berrikuspen-beharrak**. 
2. Hautatu **Proposatutako baliabideak** fitxa.
3. Aukeratu **Onartu proposamen guztiak** proposatutako baliabide guztiak onartzeko edo **Proposamen guztiak arbuiatu** arbuiatzeko. Proposatutako baliabideak onartzen badituzu, proiektuan erreserbatu egiten dira taldekide gisa eta baliabide generikoak ordezkatzen dituzte.

> [!NOTE]
> Proposatutako baliabide guztiak onartu edo baztertu beharko dituzu. Ezin dituzu partzialki onartu edo arbuiatu.

### <a name="substitute-a-resource-on-the-project-team"></a>Proiektuko taldeko baliabide bat ordeztu

Batzuetan, Proiektuko kudeatzaileak proiektuan erreserbatutako taldekide bat ordezkatu behar du.

1. **Proiektuak** inprimakian **Taldea** fitxan, aukeratu ordezkoa behar duen baliabidea eta gero hautatu **Mantendu erreserbak**.
2. Zabaldu baliabidea esleitutako proiektuak ikusteko.
3. Egin klik proiektuan eskuineko botoiarekin, eta, ondoren, hautatu **Baliabidea ordezkatu**.
4. Uneko baliabidea ordezkatu nahi duzun baliabidea ezagutzen baduzu, hautatu edo idatzi izena eta, ondoren, hautatu **Esleitu berriro**.

Edo. baliabide bat bilatu behar baduzu, jarraitu urrats hauek.

1. Hautatu **Bilatu ordezkoa**.

   Antolaketa laguntzaileak eskuragarri dauden ordezkoen zerrenda itzultzen du. Antolaketa laguntzailean, erabilgarri dauden baliabideak iragazi ditzakezu ordezko egoki bat bilatzeko.

2. Baliabidea ordezkatzeko, hautatu nahi duzun baliabidea eta, gero, hautatu **Ordezkatu**.   

   Erreserbak eta zereginak baliabide berriarekin ordezkatuko dira.

## <a name="reconcile-team-member-bookings-and-assignments"></a>Kontziliatu taldekideen erreserbak eta esleipenak

Taldekideentzat, erreserbak eta zereginak bateratu egiten dira. Alegia, baliabideek zereginak izan ditzakete baina erreserbarik ez, edo erreserbak izan ditzakete baina zereginik ez. Egokiena, erreserbak eta zereginak lerrokatuta egotea izango litzateke, baliabideek zereginak betetzeko gaitasuna konprometituta izan dezaten. Hala ere, erreserbak erabilgarritasunean oinarrituta egon litezke, eta zereginen aldaketak proiektuak aurrera egin ahala alda litezke. Hori dela eta, erreserbak eta zereginen akoplamendu solteak malgutasuna ematen du.

Project Operations-ek Proiektu-kudeatzaileei taldekideen erreserbak eta proiektuko taldeen zereginak bateratzeko aukera ematen dien **Kontziliazioa** fitxa du.

**Kontziliazioa** fitxak erreserbak eta zereginak erakusten ditu zereginen esleipen bakoitzaren mailan taldekide bakoitzarentzat. Denbora erakusten ditu gelaxkatan, hilabetetik egunera arteko epeak.

Fitxak proiektuaren guztizko garbi osoa ere erakusten du, zutabe guztiekin batera.

Baliabide bakoitzerako, fitxak taldekidearen erreserben desberdintasunak kalkulatzen ditu eta taldekideen zereginen esleipenekin bateratzen ditu. Egokiena, aldea 0 (zero) izatea da. Beste modu batera esanda, ez litzateke alderik egon behar erreserbaren eta esleipenen artean. Desberdintasunak koloreztatuta eta itzalpean daude bi baldintzetan arreta jartzeko:

- **Erreserba eskasia**: baliabideek erreserbak baino esleipen gehiago dituztenean gertatzen da. Ez denez erreserbatu gaitasun hori, baliteke Proiektu-kudeatzaileak baldintza hori zuzentzea baliabideen erreserbak hedatuz defizita estaltzeko.
- **Gehiegizko erreserbak**: baliabide bat proiektuan erreserbatuta dagoenean baina zereginetara esleitu ez denean gertatzen da. Baldintza hau onargarria izan daiteke zereginen esleipena gertatu baino lehen proiektuan erreserbatu den kasuetan. Hala ere, baliteke beste kasu batzuetan baliabidea ez izatea aurreikusita zereginei esleitzeko. Kasu horietan, Proiektu-kudeatzaileak baliabidearen erreserbak bertan behera uztea pentsatu beharko luke, gaitasuna beste proiektu baterako erabili ahal izateko.

Zenbait kasutan, eguneko maila baino maila altuagoan ikusten baduzu (adibidez, hilabetearen maila), baliteke zero diferentzia garbia izatea baliabide batentzat. beste modu batera esanda, erreserbak = zereginak. Hala ere, Astea mailari erreparatuz gero, baliteke 0 (zero) orduko esleipenak eta 40 orduko erreserbak daudela ikustea lehenengo astean, baina 40 orduko esleipenak eta 0 (zero) orduko erreserbak bigarren astean. Oro har, erreserbak eta zereginak bateratu egiten dira, baina aste batetik bestera desberdinak dira.

Denbora-maila altuagoak ikusten dituzunean, **Kontziliazioa** fitxak gelaxkak adierazle bat du denbora maila baxuagoetan desberdintasunak daudela jakinarazteko. Sakatu bi aldiz gelaxka bat handiagotu dezakezu aldea ikusteko. Ondoren, egin klik eskuineko botoiarekin hurbiltzeko. Baliabide bat hautatuta eta, ondoren, erabilita **Hurrengo aldea** saretako tresna-barran, baliabide horren erreserbak eta zereginen arteko hurrengo diferentziara joan zaitezke. Hautatu **Aurreko aldea**, itzultzeko. Alderantzizko adierazlea eta nabigazio portaera ere desaktiba ditzakezu **Ezarpenak** aukeran.

Zereginen esleipenak dituzun baina erreserbarik ez baduzu, **Proiektuak** inprimakian, **Kontziliazioa** fitxan, erreserba eskasia aukeratu dezakezu eta, ondoren, hautatu **Hedatu erreserba**. **Luzatu Erreserba** elkarrizketa-koadroa agertuko da eta baliabidearen eskasiari aurre egiteko beharrezkoa den erreserba erakusten du. Elkarrizketa-koadroan baliabideek dituzten erreserbak agertzen dira proiektu guztietan edo beste erakunde antolatzaile batzuetan. Aukeratzen baduzu **Ados** baliabidearen erreserba sortzeko, baliabidearen erabilgarritasuna edozein dela ere, gerta daiteke erreserba gehiegi egotea.

Orduan, Proiektu-kudeatzaileak edo Baliabide-kudeatzaileak antolaketa-panela erabil dezake baliabide batek bere ahalmenetatik harago gaitasunak gainditutako edozein egoera kudeatzeko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]