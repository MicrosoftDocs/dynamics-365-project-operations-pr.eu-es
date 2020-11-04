---
title: Eman proiektu bateko lanaren aurreikuspenak salmenta-prozesuan
description: Nola eman proiektu bateko lanen gutxi gorabeherakoak salmenta-prozesuan Project Service-n
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
ms.openlocfilehash: ddb7f8c0ff8c7fd7e51edb42f9d227f2b91a811b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071086"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a>Eman proiektu bateko lanen gutxi gorabeherakoak salmenta-prozesuan (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

Salmenta-prozesuan zehar, salmenten gutxi gorabeherakoak kalkula ditzakezu eskaintza-lerroetatik. [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] aplikazioko [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ahalmenek salmenten gutxi gorabeherako zientifikoagoa eta zehatzagoa ematen dizu, laneko elementuak zatituz eta atazen xehapenaren egituran proiekturako kalkulatzen laguntzen duten atributuekin lotuz.  
  
 Salmenta irabazi ostean, proiektu-planean lotutako atazen xehapenaren egitura erabil dezakezu, proiektua gauzatzeko behar den bezala zehaztuz.  
  
## <a name="link-a-project-to-a-quote-line"></a>Estekatu proiektua eskaintza-linea bati  
 Proiektuan oinarritutako eskaintza-lerro bat sortzean, beste proiektu bat sor dezakezu eskaintza-lerrotik. Proiektu-txantiloiak erabil ditzakezu (aurrekonfiguratutako proiektu estandarreko planak eta zure erakundearekin bat datorren finantza-kalkuluak) edo proiektu-plan eta lehengo proiektu baten kalkuluen kopia. Proiektu bat sortzen duzunean, proiektu-txantiloi bat aukeratzen baduzu, proiektu-plana, kalkuluak eta funtzio-eskakizunak fintzeko oinarri bat ematen dizu. Proiektu bat eskaintza batetik sortzean, proiektua automatikoki lotuko da eskaintza-lerroarekin.  
  
## <a name="project-estimate-components"></a>Proiektuaren gutxi gorabeherako osagaiak  
 Proiektuko atazen xehapenaren egiturak lanak zereginetan apurtzeko, zereginen hierarkia mantentzeko eta zeregin bakoitza gauzatzeko behar diren esfortzuen gutxi gorabeherako esleitzeko modua eskaintzen dizu. Zeregin bati funtzioak ere lotu diezazkiozuke zeregin bat eta antolaketa bat osatzeko behar diren baliabide moten kalkulua adierazteko.  
  
 Atazen xehapenaren egiturak gutxi gorabeherako lan-esfortzua eta antolaketa zehazten laguntzen du. Modu lehenetsian, proiektuak lehenago definitu dituzun lehenetsitako prezio-zerrendak erabiltzen ditu. Prezio-zerrendetan zehaztutako kostuak eta salmenta-prezioek proiektuko atazen xehapenen gutxi gorabeherako finantzak zehazten laguntzen dute.  
  
 Proiektua eskaintza batekin erlazionatuta badago, eta eskaintzak beste prezio-zerrenda bat badu lehenetsi gisa, eskaintzaren prezio-zerrenda erabiltzen da finantzak kalkulatzeko.  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a>Inportatu kalkuluak proiektu batetik eskaintza batera  
 Proiektuaren aurreikuspenak dituzunean proiektuan, aurreikuspen horiek eskaintza-lerrora inporta ditzakezu:  
  
-   **Eskaintza-lerroaren xehetasunak** aukeran, sakatu **Inportatu kalkuluetatik**. 

-   Hautatu proiektu-kalkuluak laburtuta inportatu nahi ote dituzun, motaren, funtzioaren edo atazen xehapenaren egituraren nodo-mailaren arabera.  
  
### <a name="see-also"></a>Ikusi baita ere  
 [Proiektu-kudeatzailearen gida](../psa/project-manager-guide.md)
