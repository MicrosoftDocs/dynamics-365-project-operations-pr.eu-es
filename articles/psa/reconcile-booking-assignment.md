---
title: Bateratu erreserbak eta esleipenak
description: Gai honek benetako datuei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/27/2019
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
ms.openlocfilehash: 9528bd983e6e18197138f0720abccdc6d6fa1ed5
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147908"
---
# <a name="reconcile-bookings-and-assignments"></a>Bateratu erreserbak eta esleipenak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuko taldekidearen proiektuaren erreserbak eta proiektuaren zereginen esleipenak zehaztasun gutxirekin elkartzen dira. Beraz, baliabide batek erreserbarekin bat ez datozen zereginen esleipenak eta zereginen esleipenekin bat ez datorren erreserbak izan ditzake. Egokiena, proiektuen erreserbak eta zereginak lerrokatuta egotea izango litzateke, baliabideek beren zereginak betetzeko gaitasuna konprometituta izan dezaten. Hala ere, errealitatea da erreserbak erabilgarritasunen arabera gerta daitezkeela eta zereginen denborak aldatu egin daitezkeela proiektuak bere bizi-zikloan aurrera egiten duen bitartean. Hortaz, zehaztasun gutxiko bateratzeak malgutasuna ahalbidetzen du.

Proiektuen erreserben eta zereginen esleipenen bateratze ez zehatzaren ondorioz, **Kontziliazioa** fitxa gehitzen da proiektuaren entitatean. Fitxa honek proiektu-kudeatzaileei taldekideen erreserbak eta proiektuko taldeen zereginak bateratzen laguntzen die.

Izendatutako taldekide bakoitzeko, **Kontziliazioa** fitxak erreserbak eta zereginak erakusten ditu zereginen esleipen bakoitzean. Orduak erakusten ditu gelaxkatan, hilabetetik egunera arteko epeak.

**Denbora-eskala** eremuan, **Hilabetea**, **Astea**, edo **Eguna** hauta dezakezu. **Astea** hautatzen da modu lehenetsian. Hala ere, balio lehenetsia alda dezakezu **Ezarpenak** botoia hautatuz. **Kontziliazio** fitxa irekitzean, uneko data erakusten du, baina egutegiaren kontrola erabil dezakezu denboran aurrera edo atzera egiteko. Proiektu batek etorkizuneko hasitako data duenean, fitxak data hori erakusten du irekitzen denean. Egutegiaren kontrolak proiektuaren hasiera eta amaiera datetara mugitzeko aukera ematen duten aukerak ere baditu.

Baliabide bakoitzeko hedatzaileen kontrolak erabil ditzakezu baliabideen erreserbaren xehetasunak erakusteko. Baliabide bakoitzaren esleipenak banakako zereginen mailara ere zabaldu ditzakezu.

**Kontziliazioa** fitxaren behealdean proiektuaren guztizko garbitasun orokorra agertzen da eta fitxak, gainera, zutabe osoa biltzen du. Baliabide bakoitzerako, fitxak taldekidearen proiektuetako erreserben desberdintasunak hartzen ditu eta taldekideen zereginen esleipenekin bateratzen ditu. Egokiena, aldea 0 (zero) izatea da. Beste modu batera esanda, ez litzateke alderik egon behar baliabideen erreserbaren eta bere zereginen esleipenen artean. Desberdintasunak kolore eta itzalen arabera adierazten dira bi baldintza adierazteko:

- **Erreserba eskasia** - Erreserba eskasia gertatzen da baliabideek erreserbak baino esleipen gehiago dituztenean. Ez denez erreserbatu gaitasun hori, proiektu-kudeatzaileak baldintza hori zuzendu dezake baliabideen erreserbak hedatuz eskasia estaltzeko.
- **Gehiegizko erreserbak** - Gehiegizko erreserbak baliabide bat proiektuan erreserbatuta dagoenean baina zereginetara esleitu ez denean gertatzen da. Baldintza hori onargarria izan daiteke, adibidez, baliabidea zereginen esleipena egin aurretik erreserbatu bada. Hala ere, baliteke beste kasu batzuetan baliabidea ez izatea aurreikusita esleitzeko. Kasu horietan, proiektu-kudeatzaileak baliabidearen erreserbak bertan behera uztea pentsatu beharko luke, gaitasuna beste proiektu baterako erabili ahal izateko.

> [!NOTE]
> Baldintza hauen legenda ezkutatuta egon liteke saretari leku gehiago uzteko. Kasu horretan, legenda ikusgai jarri dezakezu **Ezarpenak** botoia hautatuz.

Zenbait kasutan, **Denbora-eskala** eremua **Eguna** baino handiagoa den maila batean finkatuta dagoenean, aldeak 0 (zero) gisa kalkula litezke. Adibidez, **Hilabetea** mailan, baliabide baten diferentzia garbia 0 (zero) izan daiteke erreserbak esleipenen berdinak direla adierazteko. Hala ere, **Astea** mailari erreparatuz gero, baliteke 0 (zero) orduko esleipenak eta 40 orduko erreserbak daudela ikustea hileko lehenengo astean, eta 40 orduko esleipenak eta 0 (zero) orduko erreserbak hileko bigarren astean. Hileko erreserben eta esleipenen guztizko kopuruak berdinak badira ere, astearen arabera desberdinak dira.

Denbora-maila altuagoak ikusten dituzunean, **Kontziliazioa** fitxak gelaxka adierazle bat erakusten du denbora maila baxuagoetan desberdintasunak daudela jakinarazteko. Adibidez, hurrengo irudian, gelaxkaren adierazle bat agertzen da 2018ko urriko gelaxkan Janire Garate izena duen baliabiderako. Beraz, baliabidearen erreserbak eta esleipenak berdinak badira ere **Hilabetea** mailan gehitzean, ez datoz bat beheko mailetan.

![Bat ez datozen erreserbak eta esleipenak hileroko mailan](media/reconcile-assignments-01.JPG)

Egin klik bikoitza gelaxkan hurrengo maila txikiagora gerturatzeko eta aldea ikusteko. Adibidez, Janire Garateko 2018ko urriko aldean klik bikoitza egiten baduzu, **Astea** mailara jaisten zara. Ikusi ahal izango duzu baliabideak 16 orduko erreserbak dituela, baina ez duela esleipenik urriko lehen bi asteetan, eta 16 orduko esleipenak dituela baina ez duela erreserbarik urriaren hirugarren astean.

![Bat ez datozen erreserbak eta esleipenak asteroko mailan](media/reconcile-assignments-02.JPG)

Egin klik eskuineko botoiarekin gelaxkan, hurrengo maila altuagoa txikitzeko. Gelaxkaren adierazlea ere itzali dezakezu **Ezarpenak** botoia hautatua. 

Era berean, sareta gaineko **Aurrekoa** eta **Hurrengoa** botoiak erabil ditzakezu proiektuan dauden desberdintasunen artean mugitzeko. Botoi horiek erabiltzeko, lehenik eta behin baliabide bat aukeratu behar duzu. Hautatu **Hurrengoa** baliabide horren erreserben eta esleipenen arteko hurrengo desberdintasunera joateko. Hautatu **Aurrekoa** aurreko diferentziara joateko.

Zereginen esleipenak dituzun baina erreserbarik ez duzun egoeretan, erreserba eskasia aukeratu dezakezu eta, ondoren, hautatu **Hedatu erreserba**. Baliabideen eskasiari aurre egiteko beharrezkoa den erreserba ikus dezakezu. Baliabideen erreserbak uneko proiektuan eta bestelako proiektuetan ere ikus ditzakezu. Hautatu **Ados** baliabidearen erreserba sortzeko uneko erabilgarritasuna kontuan hartu gabe. Orduan, proiektu-kudeatzaileak edo baliabide-kudeatzaileak antolaketa-panela erabil dezake baliabide batek gaitasunak gainditu eta erreserbak hedatzeagatik gainerreserbatuta dagoen egoerak kudeatzeko.

## <a name="managing-with-time-zones"></a>Ordu-eremuekin kudeatzea
Hedatu erreserba erabiliz emaitza zehatzak eta iragar daitezkeenak ziurtatzeko, bete beharreko bi aurrebaldintza nagusi daude:  

- Erabiltzaileak bere gailuaren ordu-eremua konfiguratu behar du sistemaren Pertsonalizazio-ezarpenetan zehaztutako ordu-eremuarekin bat etortzeko.
 
  ![Ordu-eremuaren ezarpenak Windows 10-en](media/reconcile-assignments-03.png)

  ![Ordutegi-eremuaren ezarpenak pertsonalizazio-ezarpenetan](media/reconcile-assignments-04.png)
 
- Baliabide erreserbagarriak eskatutako luzapena definitzeko erabilitako sarrerak gainjartzen den lanaldiko minutu bat izan behar du gutxienez. Adibidez, adibide honetan 09:00etatik 19:00etara lan egiten dutenen berrikusteko baliabideak erakusten dira. 

  ![Baliabideen sarrerak alderatzea](media/reconcile-assignments-05.png)

Taula honek hau erakusten du:

- Proiektuaren egutegi-txantiloi bat.
- A baliabidea: baliabide honek egutegi bera du eta proiektuaren ordu-eremu berean dago. Erreserbaren hasiera-ordua goizeko 09:00etan izango da.
- B baliabideak: baliabide hau ez dago proiektuaren ordu-eremu berean eta, beraz, goizeko 07:00etatik aurrera hasten da bere ordu-eremuan. Hala ere, erreserbak goizeko 09:00etan hasiko dira, esleipen-sarreraren hasiera-ordu goiztiarrena delako.
- C eta D baliabideak: baliabide hauek ere ordu-eremu desberdinetan daude, biek ordu-eremu desberdina dute bai elkarrekiko baita proiektuarekiko ere, eta euren erreserbak ez dira hasiko dagozkien hasiera-orduak baino lehenago.

|Entitatea  |Egutegia  |
|-|-|
|Proiektuaren egutegi-txantiloia   | ![proiektuaren egutegia](media/reconcile-assignments-06.png) |
|A baliabidea  | ![A baliabidearen egutegia](media/reconcile-assignments-06.png) |
|B baliabidea  |  ![B baliabidearen egutegia](media/reconcile-assignments-07.png) |
|C baliabidea  |  ![C baliabidearen egutegia](media/reconcile-assignments-08.png) |
|D baliabidea  | ![D baliabidearen egutegia](media/reconcile-assignments-09.png)  |
 
Bateratze-ikuspegira joatean, baliabideen esleipenak eta lotutako erreserba-eskasiak agertzen dira.
 ![Bateratze-ikuspegia hedapenaren aurretik](media/reconcile-assignments-10.png)

Baliabide bakoitzean Hedatu erreserba baliabidea exekutatu ostean, behar bezala hedatuko dira baliabide bakoitzaren erreserbak. Baliabide bakoitzaren lan-orduak gabeziaren eskasiaren sarrerekin gainjartzen direlako gertatzen da hori.
 ![Bateratze-ikuspegia erreserba luzatu ostean](media/reconcile-assignments-11.png) 

Hala ere, erreserben xehetasunei gertuagotik begiratuz gero erreserben hasiera-orduetako aldeak erakusten dira. Erreserbak ez dira hasi esleipen-sarreraren hasiera-ordua baino lehenago, ezta baliabidearen hasiera-ordu librea baino lehenago ere.
 ![Antolaketa-taulako baliabideen erreserba berriak](media/reconcile-assignments-12.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]