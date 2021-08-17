---
title: Proposatu proiektuaren baliabideak
description: Gai honek proiektuaren baliabideak proposatzeari buruzko informazioa ematen du.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 9fe63f424735f22dc6b525631287e7ff36db17f37aad8e14e926f5cc9be39136
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6995026"
---
# <a name="propose-project-resources"></a>Proposatu proiektuaren baliabideak

[!include [banner](../includes/psa-now-project-operations.md)]

Baliabide-kudeatzaileek baliabide bat proposatu diezaiokete proiektu-kudeatzaileari baliabide-eskaera erabiliz.

1. Eskaera saretan edo eskaeran bertan, hautatu **Bilatu baliabideak**.
2. **Antolaketa-laguntzailea** orrialdean, hautatu baliabidea eta, ondoren, **Sortu baliabideen erreserba** panelean, **Erreserbaren egoera** eremuan, hautatu **Erreserbatu**.

    ![Hautatutako proposatutako baliabideak.](media/Resource-Management-image62.png)

Hurrengo egoeraren eguneratzeak gertatzen dira:

- **Antolaketa-laguntzailea** orrian, egoeraren adierazleak eguneratu egiten dira erreserba proposatu dela adierazteko, ez behin betiko erreserba.

    ![Antolaketa-laguntzailearen orrian proposatutako erreserben egoeraren adierazleak.](media/Resource-Management-image63.png)

- Baliabide-eskaeran, egoera aldatu egingo da **Berrikusi behar da** egoerara.

    ![Baliabide-eskaeraren egoera aldatu da "Berrikusi behar da" egoerara.](media/Resource-Management-image64.png)

- Proiektuaren **Taldea** fitxan, taldeko kide orokorraren **Eskaeraren egoera** balioa **Berrikusi behar da** baliora aldatu da.

    ![Proiektuko kide orokorraren eskaera-egoera aldatu egin da "Berrikusi behar da" baliora Taldea fitxan.](media/Resource-Management-image48.png)

Proiektu-kudeatzaileak proposamena onartu edo baztertu dezake.

Baliabide-kudeatzaileek baliabide-eskaerak prozesatzen dituztenean, honako ikuspegi hauetakoren bat erabil dezakete:

- Eskaria asetzeko hainbat baliabide proposatzea beharrezko orduak betetzeko baliabiderik ez badago eskuragarri. Proposatutako orduak behar diren orduak asetzeko baliabide ugarien artean banatzen dira. Egoera horretan, orduak ezin dira gainjarri.
- Behar direnak baino baliabide gutxiago proposatzea. Egoera horretan, proposatutako baliabideen ahalmena eskatzaileak zehaztutako beharrezko orduak baino txikiagoa da. Beraz, eskatzaileak proposatutako baliabideak onartzen dituenean, bete gabeko baliabide-eskakizuna sortzen da geratzen den eskaria harrapatzeko.
- Erreserbatu eskaria asetzeko hainbat baliabide lana osatzeko baliabiderik ez badago eskuragarri.
- Behar direnak baino baliabide gutxiago erreserbatzea. Egoera horretan, erreserbatutako orduak eskatutako orduak baino txikiagoak dira. Sistemak erreserbatu beharrean baliabideak proposatzeko gidatzen zaitu, eskatzaileak gainerako eskaerak egiaztatu eta jarrai ditzan.

## <a name="billable-utilization"></a>Erabilera fakturagarria

Baliabideek xede erabilera fakturagarria izan dezakete. Xede-erabilera hori baliabidearen funtzio lehenetsiko atributu gisa definitzen da edo erreserbatu daitekeen baliabide indibidualaren erregistroan ezartzen da. Erabileraren kalkuluak baliabideek onartutako denbora-sarrerak erabilita jakinarazi dituzten orduetan oinarritzen dira.

Erabilera kalkulatzeko honako formula hauek erabiltzen dira:

- Erabilera fakturagarria = Kobratu daitezkeen benetako orduak ÷ Baliabidearen ahalmena
- Erabilera ez fakturagarria = ID motako fakturaziodun denbora erreala = Kobratu ezin dena, osagarria edo eskuragarri ez dagoena ÷ Baliabidearen ahalmena
- Barnekoa = Salmenta kontraturik gabeko denbora erreala ÷ Baliabideen ahalmena
- Baliabideen ahalmena = Baliabideen lan orduak – Bulegotik kanpo – Lanik gabeko egunak

**Baliabideen erabilera** ikuspegia **Baliabideak** panelean aurkituko duzu.

![Baliabideen erabileren ikuspegia.](media/Resource-Management-image65.png)

Saretako gelaxka bakoitzak baliabidearen erabilera fakturagarriaren ehunekoa adierazten du aldi batean, hala nola, egun batean, astean edo hilean. Gelaxkei kolorea emateko honako formula hauek erabiltzen dira:

- **Berdea:** Erabilera fakturagarria \>= Baliabidearen helburuko erabilera
- **Horia:** Helburuko erabilera – 20 \<= Erabilera fakturagarria \< Helburuko erabilera
- **Gorria:** Erabilera fakturagarria \< Helburuko erabilera – 20

**Baliabide-erabilera** ikuspegia antolaketa-panelean oinarrituta dagoenez, antolaketa paneleko iragazkien ahalmenak erabil ditzakezu emaitzak iragazteko.

Saretak helburuko erabilera ezartzea eskatzen du, bai funtzioan, bai baliabide indibidualean. Konfigurazio hori egiteko, joan **Baliabideak** \> **Baliabideen funtzioak** atalera.

Gainera, eginkizun lehenetsi bat esleitu behar zaio erreserbatu daitekeen baliabide bakoitzari. Joan **Baliabideak** \> **Baliabideak** atalera. **Project Service** fitxan, egiaztatu baliabide funtzioa definituta dagoela, eta **Lehenetsia da** eremua **Bai** gisa ezarrita dagoela. Funtzio osagarriak gehi ditzakezu **Lehenetsia da = Ez** den tokian. **Lehenetsia da = Bai** aukeran erabiltzen den funtzioa baliabidearen erabilera ebaluatzeko erabiltzen da funtzioaren helburuarekin alderatuz.

![Funtzio lehenetsien multzoa.](media/Resource-Management-image67.png)

**Project Service** fitxan, helburuko erabilera indibiduala ere ezar dezakezu baliabiderako. Ondoren, erabileraren kalkuluak helburuko erabilera hori erabiltzen du baliabidearen helburua ebaluatzeko, baliabidearen funtzio lehenetsiaren helburua ebaluatu beharrean.

Erabilera baliabide gisa erakusten da baliabideak saretan agertzen den aldian kobratu daitekeen denbora onartu badu soilik.

## <a name="resource-availability"></a>Baliabide-erabilgarritasuna

Garrantzitsua da baliabide-kudeatzaileak baliabideen erabilgarritasuna eta erreserben eguneratzeak ikusteko gai izatea. Zenbait kasutan, ez dago eskari formalik (baliabide-eskaera), baina baliabide-kudeatzaileak mezu elektronikoak, telefono-deiak edo berehalako mezuak bezalako kanalen bidez iristen den ezusteko eskaera bati erantzun behar dio. Baliabide-kudeatzaileek antolaketa-panela erabiltzen dute baliabideak eta erreserbak eguneratzeko.

Baliabideen lan orduak baliabide baten erabilgarritasuna kalkulatzeko oinarri gisa erabiltzen dira. Baliabideen erreserbak baliabideen ahalmena kontsumitzen du.

![Antolaketa-panela.](media/Resource-Management-image68.png)

Antolaketa-panelak koloreak eta itzalak erabiltzen ditu erreserbetarako, erabilgarritasunerako, gainditutako erreserbetarako eta erreserben egoerarako. Antolaketa-paneleko ezarpenetako batek legenda erakusten du.

Eskuinera gezi bat agertzen bada erreserbatzeko baliabide indibidualaren ondoan antolaketa-panelean, baliabidea hedatu egin daiteke baliabidea erreserbatuta dagoen lanaren xehetasunak erakusteko.

![Antolaketa-panelean hedatuta dagoen baliabide erreserbagarria.](media/Resource-Management-image69.png)

Dynamics 365 Project Service Automation aplikazioak Universal Resource Scheduling motorra erabiltzen duenez, Dynamics 365 Field Service instalatuta baduzu, proiektu, lan-eskaera eta antolatzeko hedatu duzun beste edozein entitateren baliabideen erreserben xehetasunak ikus ditzakezu.

![Proiektuetarako eta lan-eskaeretarako baliabideen erreserbaren xehetasunak.](media/Resource-Management-image70.png)

Baliabide indibidualei buruzko xehetasun gehiago ikusteko, egin klik eskuineko botoiarekin gainean baliabide-txartela irekitzeko.

![Baliabide-txartela.](media/Resource-Management-image71.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]