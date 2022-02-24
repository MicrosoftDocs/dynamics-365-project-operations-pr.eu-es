---
title: Antolaketa proiektua atazen xehapenaren egiturarekin
description: Nola antolatu proiektua zereginen xehetasunen egiturarekin Project Service-n
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: cf12cc3bcf061e1daffafb248cfd76809c6444ec
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149798"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a>Antolaketa proiektua zereginen xehetasunen egiturarekin (Project Service)

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Proiektu-antolaketak zein lan egin behar den komunikatzen du, zein baliabidek gauzatuko duen lana eta zein denbora-tartetan egingo den lana. Proiektu-antolaketak proiektua garaiz entregatzearekin lotutako lan guztia islatzen du. Proiektuaren hasierako faseko lehen urratsetako bat proiektuaren antolaketa izatea da. Proiektu-antolaketa zehazteko, atazen xehapenaren egitura sortu behar duzu.  
  
 Sortu proiektu-egitura atazen xehapenaren egiturarekin, eta honetan lagunduko dizu:  
  
- Lana zeregin kudeagarritan zatitzen  
  
- Zeregina osatzeko beharrezko denbora kalkulatzen  
  
- Mendeko zereginak eta zereginen iraupena ezartzen  
  
- Zeregin bakoitza gauzatzeko beharrezko funtzioak zehazten  
  
  Atazen xehapenaren egiturako proiektu-antolaketak itxura ezaguna du, Gantt taula interaktibo batekin lagunduta.  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a>Sortu proiektuaren atazen xehapenaren egitura  
 Sortu proiektuan zereginen sekuentzia adierazten duen atazen xehapenaren egitura. Atazen xehapenaren egiturak zereginak, zeregin bakoitzerako eskakizunak eta irabaziei eta kostuei buruzko informazioa ditu. Atazen xehapenaren egituran gehi ditzakezu:  
  
-   Hierarkiako zereginen sekuentzia  
  
-   Zeregina hasi ahal izateko, egin behar diren beste zeregin batzuk, baldin badaude  
  
-   Hasiera-data, amaiera-data eta zereginaren iraupena  
  
-   Zeregina egiteko behar den ordu kopurua  
  
-   Langileek behar dituzten trebakuntzak eta heziketa  
  
-   Zereginera esleitutako langileak  
  
-   Gutxi gorabeherako diru-sarrerak eta kostuak  
  
## <a name="task-types"></a>Zeregin motak  
Zeregin mota hauek erabiliko dituzu atazen xehapenaren egitura sortzean:  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| **Proiektuaren erroko nodoa** | Proiektuaren goi-mailako laburpen-zeregina. Gainerako proiektu-zereginak bere barnean sortzen dira. Erroko zereginaren izena proiektuaren izena da. Erroko nodoaren ahalegina, datak eta iraupena bere azpiko hierarkiako balioetan oinarritzen dira. Ezin duzu erroko nodoaren propietaterik editatu edo erroko nodoa ezabatu. | 
| **Laburpena edo edukiontzi-zereginak** | Zeregin-laburpena azpizereginak konbinatzeko zeregina da. Zeregin-laburpenak ez di lan-ahaleginik edo kosturik. Lan-ahalegina eta kostua azpizereginetan bateratzen dira. Laburpen-zereginaren izena alda dezakezu, baina ezin duzu aldatu ahalegina, datak edo iraupena, automatikoki kalkulatzen baitira. Laburpen-zeregin bat ezabatzen baduzu, zereginak eta azpizeregin guztiak ezabatuko dituzu.|  
| **Hosto-nodoaren zereginak** | Hosto-nodoaren zereginak proiektuaren lan xehatuena adierazten du. Estimatutako ahalegina, antolatutako baliabide kopurua, antolatutako hasiera- eta amaiera-datak eta iraupena ditu.|

  
## <a name="task-hierarchy"></a>Zeregin-hierarkia  
 Aukera hauek dituzu zeregin-hierarkia sortzeko:  
  
- **Gehitu zeregina**.   Zeregin bat gehi dezakezu zeregin-hierarkian aukeratu duzun posizioan. Ez baduzu posiziorik hautatzen, zeregin berria amaieran agertuko da.  
  
- **Jarri koska zereginari**.   Jarri koska zeregin bati, zereginaren bigarren mailako bat sortzeko bere gainean.  
  
- **Kendu koska zereginari**.   Kendu koska zereginari zeregin nagusiaren azpizeregina izateari utz diezaion.  
  
- **Eraman gora eta behera**.   Eraman zereginak gora eta behera zeregin nagusiaren hierarkian. Zereginak gora edo behera eramateak ez du eragiten ahaleginean, kostuan, datetan edo iraupenean.  
  
## <a name="task-attributes"></a>Zeregin-atributuak  
 Zeregin-izenak egin beha den lana deskribatzen du. Erabili hainbat zeregin-atributu antolaketa azaltzeko eta zereginaren eskakizunak gehitzeko.  
  
### <a name="schedule-attributes"></a>Antolaketa-atributuak

 - Esleitu balioak **Ahalegin-orduak**, **Baliabide kopurua**, **Hasiera-data**, **Amaiera-data** eta **Iraupena** aukerei, zereginaren antolaketa zehazteko. 
 - **Ahalegina** zeregina egiteko behar den orduen estimazioa da.
 - **Baliabide kopurua** ahalik eta antolaketa onena lortzen laguntzeko proiektu-kudeatzaileak jartzen duen estimazioa da. 
 - **Iraupena** (egunetan), zeregina egiteko behar diren egun kopurua adierazten du.  
  
### <a name="staffing-attributes"></a>Betetze-atributuak

 - **Funtzioa**, **Baliabideen antolakuntza-unitatea**, **Baliabide kopurua** eta **Baliabideak** aukerek zereginaren betetze-eskakizunak deskribatzen dituzte. 
 - **Funtzioa**, zeregina egiteko behar den baliabide mota azaltzen du. 
 - **Baliabideen antolakuntza-unitatea** aukerak zeregina egiteko baliabideak hartu behar diren erakunde-unitatea adierazten du; zereginaren kostuari eta salmentei ere eragiten die, baliabidearen unitatearen salmenta-prezioa zehaztean kontatzen baita. 
 - **Baliabideak** baliabide orokorra adierazten du edo bat izendatzen du aurkitzen duenean.  
  
## <a name="task-dependencies"></a>Zeregin-mendekotasunak  
 Aurrekoen harremanak sor ditzakezu atazen xehapenaren egiturako zeregin baten edo gehiagoren artean. Zereginen aurrekari-eremuan balio bat edo gehiago ezar ditzakezu mendeko izango zaren zereginak adierazteko. Aurreko balio bat esleitzen duzunean, zeregina hasteko aurreko zeregin guztiak osatu direnean abiaraziko dira. Zereginean mendekotasun hori ezarrita, zereginaren planeatutako hasiera-data berriro kalkulatuko da aurreko zereginen azken amaiera gisa. Antolaketako aurrekoekin lotutako inpaktu guztiak ez daude zeregin bidez mugatuta.  
  
## <a name="task-mode"></a>Zeregin modua  
 Zeregin modua antolaketako hosto-nodoaren zereginak zehazten dituen faktore garrantzitsuetako bat da. Zeregin bakoitzak bi zeregin modu ditu: automatikoki antolatzeko modua eta eskuz antolatzeko modua.  
  
-   **Antolaketa automatikoa**.   Automatikoki antolatzea Zeregin modua Automatikoki antolatuta gisa ezartzen duzunean, zeregina antolatzeko motorrak antolaketa-arauak erabiltzen ditu zeregin-atributu hauetan, zereginaren antolaketa zehazteko:  
  
    -   Aurrekoak  
  
    -   Ahalegina  
  
    -   Baliabide kopurua  
  
    -   Hasiera- eta amaiera-datak  
  
-   **Nire antolaketa-arauak**.   Arauen antolaketa Hosto-nodoaren hasiera-data, aurrekaririk ez duten lehenetsiak proiektuaren antolatzeko hasiera-data. Hosto-nodoaren zereginaren iraupena hasiera- eta amaiera-datuen arteko lan-egun kopuru gisa kalkulatzen da beti. Zeregina automatikoki antolatzen denean, antolaketa-motorrak arau hauei jarraitzen die:  
  
    -   Zereginen hasiera- eta amaiera-datek lanegunak izan behar dute, proiektuaren antolaketa-egutegiaren arabera  
  
    -   Bere aurrekarien azken amaiera-dataren aurrekariak dituzten zereginen hasiera-data  
  
    -   Ahalegina = pertsona kopurua * Iraupena * orduak proiektu-egutegiaren lanegun estandarrean  
  
-   **Eskuzko antolaketa**.   Zenbait kasutan, baliteke arau horiek desbideratu behar izatea. Kasu horietan, eskuz antolatzeko zereginen zeregin modua ezar dezakezu. Beste antolaketa-atributu batzuek balioak kalkulatzea eragozten dio antolaketa-motorrari. Zereginetan aurrekariak ezartzeak mendeko zereginen hasiera-datari eragiten die.  
  
## <a name="create-a-work-breakdown-structure"></a>Sortu atazen xehapenaren egitura  
  
1.  Joan **Project Service > Proiektuak**.  
  
2.  Sakatu landu nahi duzun proiektua.  
  
3.  Pantailaren goialdean dagoen barran, hautatu proiektuaren izenaren alboan dagoen beherako gezia eta sakatu Atazen xehapenaren egitura.  
  
4.  Zeregina gehitzeko, sakatu **Gehitu zeregina**. Bete zereginaren eremuak eta, ondoren, klikatu **Gorde**.  
  
5.  Jarraitu zereginak gehitzen, atazen xehapenaren egitura bete arte. Atazen xehapenaren egitura sortzen ari zaren bitartean, zera egin dezakezu zereginak antolatzeko:  
  
    -   Hautatu zeregin bat eta sakatu **Ezarri koska** beste zeregin baten mende jartzeko edo sakatu Kendu koska mailaz igotzeko.  
  
    -   Hautatu zeregina eta sakatu **Eraman gora** edo **Eraman behera** zerrendan gora edo behera eramateko.  
  
    -   Sakatu **Ezkutatu Gantt** Gantt diagrama ezkutatzeko eta sakatu **Erakutsi Gantt** berriro bistaratzeko.  
  
    -   Hautatu beste denbora-tarte bat Gantt diagraman, **Ordu-eskala** aukeran.  
  
6.  Atazen xehapenaren egituran zehaztu dituzun funtzioak gehitzeko proiektuaren taldekideetan, sakatu **Sortu proiektu-taldea**.  
  
7.  Aldaketak egiten amaitzean, sakatu **Gorde** pantailaren behe-eskuineko izkinan.  
  
### <a name="see-also"></a>Ikusi baita ere  
 [Proiektu-kudeatzailearen gida](../psa/project-manager-guide.md)
