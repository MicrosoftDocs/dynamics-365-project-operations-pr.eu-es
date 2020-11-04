---
title: Zehaztu proiektu baten kostuaren eta diru-sarreren aurreikuspenak
description: Nola zehaztu proiektu-kostua eta diru-sarreren estimazioak Project Service-n
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 1652b39b6c8a703bf198a990eb9047eff9dc9f4c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071044"
---
# <a name="determine-project-cost-and-revenue-estimates"></a>Zehaztu proiektu baten kostuaren eta diru-sarreren aurreikuspenak 

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Proiektua estimates finantza ikuspegi ematen lanerako estimatua eta proiektua-lana diren kanpaina-xehatzea egitura antolatu. Ikuspegia estimates-kostua eta diru-sarrerak elkartze antolatutako lan duzu informs. Ikusi informazioa neurriak dira aurretik zehaztutako ondoen buruzko proiektuan-finantza elkartze duzu kopurua tresna bat eskaintzen du estimates ikuspegia.  
  
## <a name="cost-and-sales-value-of-the-project"></a>Kostua eta proiektuan balio salmenta  
[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] prezio-zerrendak proiektuek erabiltzen dituzten kostuak eta fakturazio-zerrendak definitzen dituzte. Zereginak, proiektua lan diren kanpaina-xehatzea egitura lotutako funtzioak oinarrituta zehatz ditzakezu, kostua eta diru-sarrerak elkartze konexioarekin lan.  
  
## <a name="cost-price-defaulting"></a>Kostu-prezio lehenetsia  
Behin proiektua dagokion erakunde bat (adierazita **Jabetzadun Unitate** proiektuan aplikazioan). Zure erakundearen unitatearekin erlazionatutako prezio-zerrendaren unitatearen kostuen prezioa zehazten dute. [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)]ek funtzioen kostu-prezioak zehazten dituzte, kostuaren prezio-zerrendako funtzioaren, unitatearen eta erakunde-unitatearen konbinazioa bilatuta, kostuaren prezio zuzena lortzeko estimatutako lerroetako data eraginkorrerako.  
  
Baduzu konbinazioa funtzio-unitatea. eta zure unitatea prezio-zerrenda batetik kostua bat prezioa result ez antolakuntza unitatea, unitate-funtzioak eta antolakuntza unitatea konbinazio in favor of disregarded. Prezio hau bihurtzen kostua prezio bat bada, unitate-aukeratzen dagozkionak lerroan.  
  
Funtzio eta antolakuntza unitatea konbinazio kostua prezioa result ez antolakuntza unitatea funtzioa eta unitate konbinazio in favor of disregarded eta prezioa bihurketa edozein aplikatu ondoren defaulted da eskatuz gero.  
  
 Funtzio prezio ez, ondoren, kostua prezioa berez, eremu dauka 0,00 dagozkionak lerroan.  
  
 Kostua dagozkionak lineak proiektuen arabera kostu guztiak zenbatekoak zure antolakuntza unitatea monetan dira.  
  
## <a name="sales-price-defaulting"></a>Salmenta-prezio lehenetsia  
Salmenta-prezio-zerrenda proiektuan erantsita duen entitate salmenta oinarritzen da. Eskaintzarekin edo kontratuarekin lotutako salmenten prezio-zerrendak zehazten du unitateen salmenta-prezioa. Eskaintza edo kontratu pertsonalizatuak prezio-zerrenda bat badu, proiektua estimates-salmenta prezio-zerrenda lehenetsia da hau. Salmenta-unitateak, erlazioa ez bada, ondoren, konfiguratuta parametroak ezarpenak ataleko salmenta prezio-zerrenda lehenetsia izango proiektuan lehenetsitako salmenta prezio-zerrenda. Dagozkionak-linea bakoitzeko diren baliabideak izango booked zeregina osatzeko antolakuntza unitatea adierazteko erlazionatutako baliabide antolakuntza unitatea da. Lotutako funtzioekin lotutako salmenta-prezioak zehazteko, kostu-prezioak funtzioak bilatzea konbinazioa funtzioa, unitate eta antolakuntza unitatea kostua prezio-zerrendaren aplikazioa kostua prezioa zuzena data dagozkionak lineatan hasiera.  
  
Baduzu antolakuntza unitatea funtzioa, unitate eta baliabide-konbinazioa salmenta prezio-zerrenda batetik salmentako prezioan result ez du, sistema-unitatea eta antolakuntza unitatea funtzioak eta baliabide-konbinazioa bilatu disregard da. Salmenta-prezio bat aurkitzen bada, aukeratzen duzun salmenta-estimazio lerroko unitate bihurtuko da.  
  
Sistemak ez badu funtzioaren preziorik aurkitzen, salmenta-prezioak 0,00 izango da estimazio-lerroan lehenespenez.  
  
Ikuspegia estimates unitate eta guztizko kostua eta salmentako prezioan dagozkionak lineak sareta prezio bistaratzen dituen sareta-ikuspegia da.  
  
## <a name="time-phased-view-of-project-estimates"></a>Ikuspegi ordua phased proiektua estimates  
Ordua phased ikuspegiak proiektua estimates, sareta-ikuspegia estimates datuak da pivoted lehenespenez funtzioaren eta aukeratutako timescale aplikazioan timeline zehar dagozkionak datuen spread erakusten du.  
  
## <a name="effort-estimate-allocation-based-on-task-mode"></a>Ahalegina dagozkionak kopuruan oinarrituta zeregina modua  
Ordua phased ikuspegian, zeregina estimatuak guztira ahalegina banatzen arabera allocating ahalegina ordu unitateko denbora-tarte aukeratutako timescale-zenbaki bat. Project Service zeregina modua zehazten zeregina iraupena zehar ahalegina nola esleituta dago. Esleipen mota bi baita guztirako baldintza kopuruak dira eta kopuruan oinarrituta lanorduekin lan egin  
  
## <a name="work-hours-based-allocation"></a>Lanorduak kopuruan oinarrituta  
Antolaketa-zereginak zeregina modua automatikoki governs duzun zeregina estimatua baliabide-kopuruaren, duten dira estimatua osoa lanorduak eguneko-utilized. Aplikatzen duzunean ikuspegi ere phased allocating ahalegina, iraupena ordua zeregin zehar zatikatzea arabera. Instance, bat 'Egun' timescale, zeregin bat estimatua, baliabide bat osatu, egunaren esleitutako ahalegina lanorduak, proiektua egutegian zehaztutako egunaren ezin dira. Beraz, ahalegina guztirako baldintza kopuruak beti ziurtatzen diren baliabideak egun horretarako antolatzen utilized, estimatua dira.  
  
## <a name="even-distribution"></a>Banaketa berdina  
Zeregina antolatutako eskuz modua lanorduak, proiektua egutegi edo zeregin entitate nagusian zehaztutako baliabideak gutxieneko denboraz ez du. Zeregina antolaketa oinarritutako erabiltzailea. Zeregin horrelako, ahalegina guztirako baldintza kopuruak unitateko aukeratutako timescale-denbora-tarte duelako garrantzitsuak limiting edozein. Zereginean guztira ahalegina tratatzen da zatitzea eta esleitutako unitate bakoitzarentzako aukeratutako timescale denbora-epea.  
  
Modu honetan, zeregin entitate nagusian zehaztutako zeregina modua zehazten ahalegina banaketa edo guztirako baldintza kopuruak unitateko alderatuta ordua phased estimates aldiko ordua.  
  
## <a name="grouping-and-time-phasing-options"></a>Taldekatzea eta denbora phasing aukerak  
Ikuspegi hau laguntzen ulertzen ahalegina, kostua eta estimates salmenta banaketa atalean bat eguneko, asteko, hilabeteko edo urte oinarri bakoitzeko. Elkartu aukera ematen bi beste neurriak dira estimates datuen pivoting: kategoria eta baliabideak. Sareta-ikuspegia, eta denbora phased ikuspegia eremuak bistaratuko diren hauta dezakezu. Denbora-tarteen bakoitzeko guztizkoak, guztira estimatutako ahalegina, kostua adierazten beheko bistaratuko da. eta salmentak eguneko, asteko, hilabeteko edo urte.  
  
Data efektiboak da prezioa egiten defaulting kostua eta salmenta — duzunean funtzioak aldaketa-tasak izango da gehiago ordua phased ikuspegian 'Baliabide' aukeran pivoted dagozkionak datuak ikusten duzunean transparent eta denbora-phased astearen arabera.  
  
## <a name="expense-estimates"></a>Expense estimates  
Izango da incurred ez zuzenean erlazionatuta dagoen kontratuan expended da proiektua expense edozein sareta ikuspegian proiektua estimates aplikazioan erregistratzen dira. Erabiliz, **Gehitu expense dagozkionak** aukera sareta ikuspegian duzu dezakezu lortzeko hau. Expense estimates zeregina jakin baterako edo osoa proiektua; erregistratu da aukera horiek lineatan expense kategoriak eta duzunean, expense bezerogaitik incurred da momentuaren data bat hautatu. Baldin lotutako kostua eta salmenta-prezio-zerrenda prezio lehenetsien ordez edo prezio-igoeraren ehunekoak diren zehaztutako expense kategoriak, hori izango da defaulted erlazioaren atalean dagozkionak ilaran.  
  
### <a name="see-also"></a>Ikusi baita ere  
 [Proiektu-kudeatzailearen gida](../psa/project-manager-guide.md)
