---
title: Nola egin ditzaket Proiektua Faseak negozio-prozesuaren fluxua?
description: Proiektua faseen negozio-prozesuaren fluxua pertsonalizatzeko ikuspegi orokorra.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
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
ms.openlocfilehash: 0f95677c56b745bf7900ad503596c93f1e722281
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286143"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a>Nola egin ditzaket Proiektua Faseak negozio-prozesuaren fluxua?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

Muga ezagun bat dago Project Service-ren aplikazioan eta negozio-prozesuaren fluxuko Proiektu-faseek bat etorri behar dute ingelesezko izenekin (**Quote**, **Plan**, **Close**). Bestela, eta negozio-logika, relies izenak Ingelesez fasea arabera, zer ez du funtzionatzen bezala. Why dagoen bai ekintzak esaterako ikusten ez **modura Aldaketa Prozesu** edo **Editatu Prozesua** proiektua inprimakian erabilgarri, eta pertsonalizatu negozio-prozesuaren fluxua encouraged ez dago. 

Muga honi 2.4.5.48 bertsioan edo berriagoan ekin zaio. Artikulu honek iradokitako konponbideak ematen ditu, bertsio berriagoen negozio-prozesuaren fluxu lehenetsia pertsonalizatu nahi baduzu.  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a>Negozio-logika Ingelesez fasea izenekin bat etor zehatzak behar du

Proiektua Faseak negozio-prozesuaren fluxua drives hurrengo ditzake aplikazioan negozio-logika ditu:
- Proiektuan eskaintza batekin erlazionatuta dagoenean, kodea ezartzen negozio-prozesuaren fluxua, **Quote** fasea.
- Proiektuan kontratu batekin erlazionatuta dagoenean, kodea ezartzen negozio-prozesuaren fluxua, **Plan** fasea.
- Negozio-prozesuaren fluxua aurreratuaren duzunean, **Close** fasea proiektua erregistroa den desaktibatutako. Proiektuan desaktibatzen denean, proiektu-inprimakia eta zereginen xehetasunen egitura (WBS) irakurtzeko soilik dira, izena duten baliabideen erreserbak argitaratuta daude, eta erlazionatutako prezio-zerrendak desaktibatuta daude.

Negozio logikoak ingelesezko izenetan oinarritzen dira proiektu-faseetarako. Hau izenak Ingelesez fasea atalean mendekotasunarekin zergatik Proiektua Faseak negozio-prozesuaren fluxua pertsonalizazio ez encouraged, zergatik ez ikusi, ohiko negozio-prozesuaren fluxuaren ekintzak bezala bezalaxe nagusian arrazoia **modura Aldaketa Prozesu** edo **Editatu Prozesua** proiektua entitatean.

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a>Fase izenak Ingelesez izenekin bat ez baduzu gertatzen dena?

Aplikazioa bertsioan Project Service 8.2 plataforma, 1.x fasea izenak aplikazioan negozio-prozesuaren fluxua duzunean ez izenekin bat datoz Ingelesez fasea negozio-logika ezartzen eskaintzak edo kontratuak fasea eskuineko edo ixten proiektua, zehazki, egin. Ez dago errore-mezuak bistaratuko dira. Beraz agertzen dela Proiektua Faseak negozio-prozesuaren fluxua pertsonaliza ditzakezu. Hala ere, eskaintza, kontratuak, lanean prozesu automatikoen ikusi ez eta proiektua itxi.

Project Service aplikazioa bertsioan 2.4.4.30 edo aurrekoa 9.0 plataforma, gertatu da bat asko arkitekturala aldatu negozio-prozesuaren fluxuak, eskatzen bat berriro idatzi negozio prozesuaren fluxu negozioen logikan. Ondorioz, prozesu-fasearen izenak aurreikusitako izenak Ingelesez ez badatoz bat, jasotzen errore-mezu bat. 

Beraz, Proiektua Faseak negozio-prozesuaren fluxua proiektua entitate pertsonalizatu nahi badituzu soilik gehi ditzakezu brand berria faseak lehenetsia negozio-prozesuaren fluxua proiektua entitaterako, zu, **Eskaintza**, **Plana** eta **Itxi** gisa faseak-da. Murrizketa hau kontutan duzun duzun ez lortu erroreak negozio-prozesuaren fluxua izenak Ingelesez fasea expects negozio-logika ziurtatzen.

2.4.5.48 bertsioan edo berriagoan, artikulu honetan azaldutako negozio-logika negozio-prozesuaren fluxu lehenetsitik kendu da proiektu-entitaterako. Horren bertsioa edo berriagoa bertsioa berritzen ahalko dituzu pertsonalizatu edo ordezkatu lehenetsitako negozio-prozesuaren fluxua bat izatea. 

## <a name="workarounds-for-earlier-versions"></a>Aurreko bertsioetarako konponbideak

Aukera ez bertsio-berritzen, Proiektua Faseak negozio-prozesuaren fluxua bi moduetan bateko proiektua entitate pertsonaliza dezakezu:

1. Gehitu faseak gehigarria lehenetsia konfigurazioa, izenak Ingelesez fasea retaining da **Eskaintza**, **Antolatu**, eta **Itxi**.


![Lehenetsitako konfigurazio-fluxuari faseak gehitzeak-Eginbideei](media/FAQ-Customize-BPF-1.png)
 
2. Zure negozio-prozesuaren fluxua sortzeko eta egin nagusia negozio-prozesuaren fluxua entitaterako proiektua, nahi dituzun fase guztiak izenak duzu lezake. Hala ere, estandarra proiektua faseak bera erabili nahi baduzu **Eskaintza**, **Antolatu**, eta **Itxi**, zenbait pertsonalizazio izen pertsonalizatuak fasea desaktibatu driven egin behar duzu. Konplexu logika duzu oraindik batzuek eragin bakarrik desaktibatu proiektua erregistroa zein, proiektua ixten da.

![BPF pertsonalizazioa](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a>Project Service aplikazioa bertsioa 2.4.4.30 edo aurrekoa plataforma 9.0 considerations gehigarria

Project Service 2.4.4.30 edo aurrekoa plataforma 9.0, pertsonalizatutako negozio-prozesuaren fluxuko batekin, **Fasearen Izena** erabilitako entitatearen proiektua eremua, **Proiektua Fasea** diagrama eta proiektua zerrenda-ikuspegietako ez eguneratu delako coupled Proiektua Faseak negozio prozesuaren fluxu lehenetsia. Urrats hauekin arazoarekin bideratuko dira:

- Uneko negozio prozesu-fluxuaren fasearen erabiltzailearen advances pertsonalizatutako negozio-prozesuaren fluxua bidez gisa eguneratu diren islatzeko eremu pertsonalizatu bat gehitu.

- Aldatu, **Proiektua Fasea** ordez lehenetsitako konfigurazio-eremu pertsonalizatua zure lan egin nahi duzun diagrama.

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a>Urratsak sortzeko zure negozio-prozesuaren fluxu proiektua entitate

Proiektu-entitatearen negozio-prozesuaren fluxua sortzeko, egin hau:

1. Joan **Ezarpenak** > **Prozesu-zentroak** atalera. Ez da negozio-prozesuaren fluxu ere kopiatzen Project Service-ren negozio-logika duen delako Proiektua Faseak kopiatu.

  ![Sortu prozesua](media/FAQ-Customize-BPF-3.png)

2. Prozesu-Diseinatzailea sortzeko erabili nahi dituzun fase izenak. Funtzionalitate bera fase lehenetsi gisa nahi duzun **Eskaintza**, **Antolatu**, eta **Itxi**, zure pertsonalizatutako negozio-prozesuaren fluxu baten fasearen izenak oinarrituta sortu behar duzu.

   ![Eginbideei-Prozesua Diseinatzailea erabiltzen BPF pertsonalizatu](media/FAQ-Customize-BPF-4.png) 

3. Prozesu-Diseinatzailea, sakatu **Ordenatu Prozesu-Fluxua** pertsonalizatutako negozio-prozesuaren fluxua nagusia negozio-prozesuaren fluxua proiektua entitate batek da Proiektua Faseak negozio-prozesuaren fluxua gaineko batera mugituz, zerrendaren goiko aldean jartzeko.


   [Eskaera-Prozesuaren Fluxu erabiliz-Eginbideei](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a>Jarraitu urrats hauek Proiektua Zerbitzu aplikazioa 2.4.4.30, edo aurrekoa 9.0 plataforma aplikatu

4. Pertsonalizatutako negozio-prozesuaren fluxu pertsonalizatuak faseak islatzeko proiektua entitateetan eremu pertsonalizatu berri bat gehitzeko. Negozio-logika (plugin edo lan-fluxuaren) pertsonalizatutako negozio-prozesuaren fluxua fasea eguneratzen eremua eguneratzeko, gehitu behar duzu.

   ![Pertsonalizatu Proiektua entitate-Eginbideei](media/FAQ-Customize-BPF-6-720.png)

5. Aldatu, **Proiektua Fasea** eremu pertsonalizatu berri zure faseak erabili nahi duzun diagrama.

   ![Eginbideei erabiltzearen arriskua Proiektua Fasea diagrama](media/FAQ-Customize-BPF-7-720.png)

6. Eremu pertsonalizatu berri zure faseak gehitzeko proiektua entitatearentzat ikuspegiak edozein aldatu.

   ![Aldatu entitate Proiektua ikuspegiak Eginbideei](media/FAQ-Customize-BPF-8-720.png)



[!INCLUDE[footer-include](../includes/footer-banner.md)]