---
title: Proiektuaren kostuak eta diru-sarrerak
description: Gai honek proiektuaren kostuak eta dir-sarrerak aurreikusteari buruzko informazioa eskaintzen du.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: fe51af8adb7c3831a57494b8359def2a0176b552efe16feb53a2a265f5ffcb0c
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7002541"
---
# <a name="project-costs-and-revenue"></a>Proiektuaren kostuak eta diru-sarrerak

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuaren aurreikuspenek proiektuaren antolaketan aurreikusitako eta antolatutako lanaren finantza ikuspegia eskaintzen dute. **Aurreikuspenak** fitxak, **Proiektuak** orrialdean, antolatzen ari zaren lanaren kostuaren eta diru-sarreren eragina erakusten du. Aurrez definitutako dimentsio ugariri buruzko informazioa ere ematen du. 

> ![Aurreikuspenen fitxa.](media/project-5.png)

## <a name="cost-and-sales-values-of-the-project"></a>Proiektuaren kostuen eta salementen balioak

Prezio-zerrendek proiektuko funtzioen kostuak eta fakturazio-zerrendak definitzen dituzte. Laneko kostuaren eta diru-sarreren eragina zehaztu dezakezu, zeregin bati esleitzen zaion lanpostuaren izenarekin eta zereginari esleitutako izendatutako baliabidearekin esleitutako funtzioen arabera. Eslepenik ez duten zereginak badira (orokorrak edo izendatuak), ezin duzu kostuen edo salmenten estimaziorik jaso. Kostuen eta salmenten balioek prezio-zerrendetan zehazten den data hartzen dute kontuan.

### <a name="default-cost-price"></a>Kostuaren prezio lehenetsia  

Proiektu oro erakunde batekoa da. Erakunde hori **Kontratazio-unitatea** eremuan agertzen da proiektuan. Kontratazio-unitatearekin lotzen den prezio-zerrenda unitateko kostuaren prezioa zehazteko erabiltzen da. Funtzioen kostuen prezio zuzena zehazteko aurreikusitako lerroetan zehaztutako datarako, bilatu kostuaren prezio-zerrendako funtzioaren, unitatearen eta erakunde-unitatearen konbinazioa. 

Haien kostuen prezioak kalkulatu ahal izateko, zeregin guztiak baliabide bati esleitu behar zaizkio. Esleitu gabeko zeregin guztien kostuaren prezioa 0,00 izango da.

Funtzioaren, unitatearen eta antolaketa unitatearen konbinazioak unitate kontratatuen prezioen zerrendatik kostua itzultzen ez badu, sistemak ez dio kasurik egingo unitateari. Horren ordez, funtzio justuaren eta antolaketa unitatearen konbinazioa bilatzen du. Kostuen prezioa aurkitzen bada, bihurketa-faktoreak erabiliko dira aurreikuspenaren lerroan hautatu duzun unitatera bihurtzeko.

Funtzioaren eta antolaketa unitatearen konbinazioak kostuaren prezioa itzultzen ez badu, sistemak ez dio kasurik egingo antolaketa unitateari. Horren ordez, funtzioaren eta unitatearen konbinazioa bilatzen du prezio lehenetsia ezartzeko (edozein bihurketa aplikatu ondoren).

Sistemak ez badu aurkitzen funtzioaren preziorik, aurreikuspenaren lerroko kostuaren prezioak **0,00** balio lehenetsia izango du. Proiektuaren kostuaren aurreikuspenaren lerroko kostu kopuru guztiak unitate kontratatzailearen moneta berean erregistratuko dira.

> [!NOTE]
> Modu lehenetsian, Microsoft Dynamics 365 aplikazioak kostuen kopuruak zure oinarrizko monetan gordetzen ditu. Hala ere, **Aurreikuspenak** fitxan erakusten diren kostuen zenbatekoak kontratazio unitatearen monetan daude.  

### <a name="default-sales-price"></a>Salmenten prezio lehenetsia 

Salmenten prezio-zerrenda proiektua lotuta dagoen salmenta-erakundeak edo proiektuaren bezeroak zehazten du. Salmenta-erakunde bat, hala nola abagunea, eskaintza edo kontratua, proiektuarekin lotzen denean, salmenta-entitatearen salmenta-prezioa eskaintzarekin edo kontratuarekin lotzen den prezio-zerrendaren arabera zehazten da. Eskaintzak edo kontratuak prezio-zerrenda pertsonalizatu bat badu, prezio-zerrenda hori proiektuaren aurreikuspenetarako salmenten prezio-zerrenda lehenetsi gisa erabiltzen da. Salmenta-entitateekin loturarik ez badago, parametroetako salmenten prezio-zerrenda lehenetsia erabiltzen da proiektuaren lehenetsitako salmenten prezio-zerrenda gisa proiektuan definitzen den bezeroaren monetaren arabera.

Aurreikuspeneko lerro bakoitzak berarekin lotzen den baliabide-unitate bat du. Baliabide-unitateak zeregina burutzeko baliabideak erreserbatzen diren antolaketa-unitatea adierazten du. Esleitutako funtzioen salmenta-prezioa zehazteko, bilatu salmenten prezio-zerrendan funtzioaren, unitatearen eta baliabide unitateen konbinazioa. Zereginean esleipenik ez badago, zereginaren salmenta-prezioa 0,00 da.

Funtzioaren, unitatearen eta baliabide unitatearen konbinazioak salmenten kontratatuen prezioen zerrendatik salmentak itzultzen ez badu, sistemak ez dio kasurik egingo unitateari. Horren ordez, funtzio justuaren eta baliabide unitatearen konbinazioa bilatzen du. Salmenten prezioa aurkitzen bada, bihurketa-faktoreak erabiliko dira salmenten aurreikuspenaren lerroan hautatu duzun unitatera bihurtzeko. 

Funtzioaren eta baliabide unitatearen konbinazioak salmenten kontratatuen prezioen zerrendatik salmentak itzultzen ez badu, sistemak ez dio kasurik egingo baliabide unitateari. Horren ordez, funtzioaren eta unitatearen konbinazioa bilatzen du prezio lehenetsia ezartzeko (edozein bihurketa aplikatu ondoren).

Sistemak ez badu aurkitzen funtzioaren preziorik, aurreikuspenaren lerroko salmenten prezioak **0,00** balio lehenetsia izango du.

**Aurreikuspenak** fitxak aurreikuspenen lerroak erakusten dituen sareta ikuspegi bat du. Saretak unitateko zutabeak, kostuaren prezio osoa eta salmenten prezio osoa ditu, hurrengo irudian erakusten den moduan. 

> ![Gelaxka-ikuspegia Aurreikuspenak fitxan.](media/project-6.png)

## <a name="time-phased-view-of-project-estimates"></a>Ikuspegi ordua phased proiektua estimates

Proiektuen estimazioen denbora-fasea ikuspegiak saretaren ikuspegiko denbora-lerroan aurreikusitako datuak erakusten ditu, zuk aukeratutako denbora-eskalan. Modu lehenetsian, aurreikusitako datuak **Funtzioa** dimentsioan aktibatzen dira.

> ![Proiektuen aurreikuspenetarako denbora-fasea ikuspegia.](media/project-7.png)

## <a name="allocating-estimated-effort-based-on-the-task-mode"></a>Esleitu zereginaren moduan oinarritutako aurreikusitako ahalegina

Denbora-fasea ikuspegian, banatu zereginerako aurreikusita dagoen ahalegin guztia ahalegin-orduak unitataren denbora tarte bakoitzerari esleituz hautatutako denbora-eskalan. Zereginaren moduak zehazten du zeregina iraupena zehar ahalegina nola esleitutzen den. Bi esleipen mota daude: **Uniformea** eta **Lanorduetan oinarritutakoa**.

### <a name="work-hours-based-allocation"></a>Lanorduetan oinarritutako esleipena
 
Automatikoki programatutako zeregin moduan, zereginen baliabideen eguneroko lehenetsitako orduak laneko ordu osoko tasan ezartzen dira. Jarrera hori ahalegina zereginaren iraupenean zatituta esleitzen denean aplikatzen da denora-fasearen ikuspegian. Adibidez, zeregin bat **Eguna** denbora-eskalako baliabide batekin osatuko dela aurreikusten baduzu, egunaren esleitutako ahaleginak ez du gaindituko proiektua egutegian zehaztutako eguneko lanordu kopurua. Beraz, ahaleginaren esleipenak beti ziurtatzen du baliabideak egun osoan erabiltzeko aurreikusita daudela.

### <a name="even-allocation"></a>Esleipen uniformea

Eskuz programatutako zeregin moduan, ez dira erabiltzen proiektuaren egutegiko lan orduak. Horren ordez, zereginaren antolaketa erabiltzailearen sarreretan oinarritzen da. Zeregin horietarako, hautatutako denbora-eskalako unitatearen denbora tarte bakoitzeko esleitutako ahalmenak ez du mugatzen duen faktorerik. Zeregineko guztizko ahalegina zati berdinetan zatitzen da eta unitatearen denbora tarte bakoitzari esleitzen zaio hautatutako denbora-eskalan. Beraz, zereginean zehaztutako zeregin moduak ahaleginaren banaketa edo aurreikusitako denbora-faseko unitatearen denbora tarte bakoitzeko esleitutako ahalegina zehazten du.

## <a name="grouping-and-time-phasing-options"></a>Taldekatzea eta denbora phasing aukerak

Denbora-fasearen ikuspegiak ahaleginaren, kostuen eta aurreikusitako salmenten banaketa erakusten du egunean, astean,hilabetean edo urtean oinarrituta. Modu lehenetsian, aurreikusitako datuak **Funtzioa** dimentsioan aktibatzen dira. Hala ere, **Taldekatu honela:** aukera erabil dezakezu beste bi dimentsiotan nabigatzeko: **Kategoria** eta **Baliabidea**.

Bai saretaren ikuspegian, bai denbora-fasearen ikuspegian, erakusten diren eremuak hauta ditzakezu. Denbora bloke bakoitzeko balio osoak proiektuaren behealdean agertzen dira. Eguneko, asteko, hileko edo urteko aurreikusitako ahalegina, kostua eta salmentak erakusten dituzte. Lehenetsitako kostuaren prezioa eta salmenten prezioa data barruan daude. Bestela esanda, baliabide bakoitzerako aldatzen dira, zuk aukeratutako denbora-fasearen ikuspegian oinarrituta.

## <a name="expense-estimates"></a>Expense estimates

Sareko ikuspegiko **Gehitu gastuen aurreikuspen berria** botoiak proiektuan sor daitezkeen gastuak erregistratzeko aukera ematen dizu, baina lanarekin zerikusirik ez dutenak. Zeregin jakin baterako edo proiektu osorako gastuen aurreikuspenak erregistratu ditzakezu. Aukeratu gastuen kategoriak eta gastua jasotzea espero duzun behin-behineko data. Lotuta dauden kostuen prezio-zerrendak eta salmenten prezio-zerrendak prezio lehenetsiak badituzte (edo gainprezioaren ehunekoak diren gastuen kategoriarako zehaztuta badaude), automatikoki gehituko dira aurreikuspenen lerroan esleipena egitean.


[!INCLUDE[footer-include](../includes/footer-banner.md)]