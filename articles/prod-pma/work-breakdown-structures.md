---
title: Zereginen xehetasunen egituraren ikuspegi orokorra
description: Zereginen xehetasunen egitura (WBS) deskribapen bat da egina izango da proiektuarena. Zereginen hierarkia da, proiektuaren taldeak lanaren osaera eta osagai edo zeregin bakoitzaren tamaina, kostua eta iraupena ulertzea adierazten duena.
author: Yowelle
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjWorkBreakdownStructure
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23861
ms.assetid: 241a0464-0056-4a69-b468-0afbe2d5f3ae
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9dc4575f5b4b80e257e34e21980b0516e7c546e6
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287943"
---
# <a name="work-breakdown-structures-overview"></a>Zereginen xehetasunen egituraren ikuspegi orokorra

[!include [banner](../includes/banner.md)]

Zereginen xehetasunen egitura (WBS) deskribapen bat da egina izango da proiektuarena. Zereginen hierarkia da, proiektuaren taldeak lanaren osaera eta osagai edo zeregin bakoitzaren tamaina, kostua eta iraupena ulertzea adierazten duena. WBS batek hiru helburu nagusi ditu:

-   Atazetako lanen banaketa edo osaera deskribatzea.
-   Antolaketa proiektuaren lana.
-   Zeregin bakoitzaren kostua kalkulatu.

WBS baten xehetasun maila estimazioetan eskatzen den zehaztasun mailaren eta estimazio horien arabera behar den jarraipen mailaren araberakoa da. Ordutegian edo kostuan irristaketekiko oso tolerantzia txikia duten proiektuek normalean WBS zehatzagoa eskatzen dute eta lanaren aurrerapenaren eta kostuaren jarraipen zorrotza eskatzen dute WBSren aurka. Proiektu mota hau ohikoa da eraikuntzako eta ingeniaritzako industrietan. 

Aitzitik, komunikabideetan eta publizitatean, softwarean eta IT azpiegituretan bezalako industrietako proiektuak mota batekoak izan ohi dira, eta produktibitatea zeregina betetzen ari den norbanakoaren esperientziarekin eta gaitasunarekin alderatuta dago. Hori dela eta, industria horiek WBS bat erabiltzen dute proiektu baten tamainaren hurbilketa lortzeko, ez proiektu horren aurrerapena zehatz-mehatz jarraitzeko. 

WBS bat eraikitzea epe luzean egin ohi den prozesu intentsiboa da eta askotariko jendearen lankidetza eta informazioa eskatzen ditu. Gai honetan deskribatzen da WBS hobekuntzak nola erabil ditzakezun kalkuluen eta jarraipenaren baldintzak betetzeko.

## <a name="prerequisites-for-creating-a-wbs"></a>WBS bat sortzeko aurrebaldintzak
WBS bat sortzeko, lan egutegia sortu eta lanaren kostua kalkulatu behar duzu.

### <a name="prerequisites-for-creating-a-work-schedule"></a>Lan egutegia sortzeko aurrebaldintzak

WBS funtzioen programazio ahalmen guztiak erabiltzeko, osatu konfigurazio hau:

1.  Konfiguratu egutegi lehenetsia eta proiektuaren egutegia:
    1.  Egin klik **Proiektuen kudeaketa eta kontabilitatea** &gt; **Konfigurazioa** &gt; **Proiektuen kudeaketa eta kontabilitate parametroak** &gt; **Programazioa**. **Lan egutegi lehenetsia** eremuan, zehaztu egutegi lehenetsia. Hau izango da sortzen den proiektu berriaren lan egutegi lehenetsia.
    2.  Proiektu jakin baterako egutegi lehenetsia alda dezakezu. Egin klik proiektuaren xehetasunen orrian, eta gero, **Proiektu taldea eta programazioa** FastTab, eguneratu **Egutegia programatzea** eremua beste egutegi bat hautatuta.

2.  Konfiguratu lanegun eta lanaldi estandarrak. Zure proiektuaren lan egutegi gisa ezarri duzun egutegia WBSn erabiliko da informazio hau zehazteko:

-   Lanegunak eta oporrak
-   Eguneko lan ordu kopurua

Egutegi baterako lanegunak eta lan orduak konfiguratzeko edo egutegi berria sortzeko, egin klik **Erakundearen administrazioa** &gt; **Arrunta** &gt; **Egutegiak**.

### <a name="prerequisites-for-estimating-the-cost-of-work"></a>Lanaren kostua kalkulatzeko aurrebaldintzak

WBSren kostuen zenbatespen gaitasun osoa erabiltzeko, langileen kostuak eta salmenta prezioak, lan kategoriak, gastuak eta tasak eta artikuluak ezarri beharko zenituzke.

-   Eskulanaren, gastuen eta kuoten kategorien kostua eta salmenta-prezioa konfiguratzeko, egin klik **Proiektuen kudeaketa eta kontabilitatea** &gt; **Konfigurazioa** &gt; **Prezioak**.
-   Artikuluen kostua eta salmenta prezioa konfiguratzeko, erabili **Merkataritza akordioak** fitxategiko elementu bakoitzaren orria **Kaleratutako produktuak** zerrenda orria Produktuen informazioaren kudeaketan.

## <a name="creating-a-wbs"></a>WBS bat sortu
WBS bat sortzeak hiru jarduera dakartza:

1.  **Lanaren deskonposizioa** - Sortu lanen banaketa manejagarriak diren zatietan edo zereginetan.
2.  **Lan egutegia** - Zeregin bat burutzeko behar den denbora kalkulatu, atazen arteko mendekotasunak ezarri eta atazen hasiera eta amaiera datak hautatu.
3.  **Kostuen zenbatespena** - Zeregin bakoitzaren kostuak kalkulatu.

Hurrengo ataletan WBS gaitasunek jarduera horietako bakoitzean nola lagun dezaketen eztabaidatzen da.

### <a name="work-decomposition"></a>Lanaren deskonposizioa

Lanaren matxura edo deskonposizioa sortzea normalean WBS bat sortzeko prozesuaren lehen pausoa da. WBS funtzionalitateak oinarrizko eraikuntza hauek onartzen ditu lana banatzeko edo deskonposatzeko. 

**Proiektuaren root zeregina** Proiektuaren erro zeregina proiektu baten goi mailako laburpen zeregina da. Gainerako proiektu-zereginak bere azpian sortzen dira. Erroko zereginaren izena ezartzen zaio proiektuaren izenari. Erro nodoaren esfortzuak, datak eta iraupenak erro zereginaren azpian dauden atazen balioak laburbiltzen ditu. Ezin dituzu aldatu propietateak erroko nodoa edo ezabatu hori.

**Laburpen edo edukiontzi lanak** Laburpen zeregina azpian zereginak edo zeregin osagarriak dituen zeregina da. Zeregin-laburpenak ez di lan-ahaleginik edo kosturik. Horren ordez, laburpen-zeregin baten lan-ahalegina eta kostua bere zereginen lan-ahaleginaren eta kostuaren batura dira. Lehenengo hasiera-data zeregin kideak erabiltzen dira hasiera-data laburpen zeregina, eta azkeneko amaiera-data zereginaren kideak erabiltzen dira amaiera-datan. Ezin duzu aldatu laburpen-zereginaren izena, baina ezin da aldatu antolaketa propietateak eskaintza, datak eta iraupena. Laburpen zeregin bat ezabatzen baduzu, bere zeregin kide guztiak ere ezabatuko dituzu. 

**Hosto nodo zereginak** Hosto nodo zereginak proiektuko lan paketerik zehatzena adierazten du. Hosto-nodoa estimatutako ahalegina, antolatutako baliabide kopurua, antolatutako hasiera- eta amaiera-data eta iraupena ditu. 

Ondorengo hierarkia eragiketak osa ditzakezu proiektu baterako lan hierarkia edo deskonposizioa sortzea ahalbidetzeko. 

**Zeregin berria** Sortzen duzun zeregin berria automatikoki erro-nodoaren azpian gehitzen da eta WBS zenbaki bat esleitzen zaio zereginari automatikoki. WBS zenbakiak atariaren maila hierarkian adierazten du. Proiektuaren erroko zereginaren azpian dagoen lehen mailan dauden zereginetarako, 1, 2, 3 eta abar zenbakizko eskema erabiltzen da. Lehen mailaren azpian dauden zereginetarako, 1.1, 1.2, 1.3 eta abar zenbakizko eskema erabiltzen da. Aurreko maila baten azpian gehitzen den maila bakoitzeko, puntuz osatutako zenbaki serie berri bat gehitzen da. 

Une honetan, ezin duzu WBS numerazioa pertsonalizatu. 

**Koska zeregina** Zeregin bat koskatzen duzunean, aurretik egiten den zereginaren seme-alaba bihurtzen da. Haur berriaren WBS zenbakia automatikoki birkalkulatzen da bere guraso berriaren WBS zenbakiaren arabera. Gurasoen zeregina orain laburpen edo edukiontzi zeregina da eta, beraz, bere osagai diren zereginen bilketa bihurtzen da. 

> [!NOTE] 
> Koska eragiketaren aurretik hosto nodo bat zen ataza baten barruan zereginak kosmetzen dituzunean, sortu berri den laburpen atazak bere datak, ahalegina eta baliabide kopurua galtzen ditu. Orain osatzen dituen zeregin berrien balioen laburpena erabiltzen du. 

**Outdent zeregina** Zeregin bat gainditzen duzunean, jada ez da bere gurasoen zeregin osagarria. Ataza honen WBS zenbakia automatikoki birkalkulatzen da atazaren hierarkian maila berria islatzeko. Aurreko zeregin nagusiaren esfortzua, kostua eta datak berriro kalkulatuko dira kanpo uzteko zeregina. 

**Mugitu gora eta behera** Klik egitean **Mugitu gora** eta **Mugitu behera**, zeregin baten posizioa aldatu egiten duzu gurasoen hierarkiaren barruan. Posizioaren zereginak ez du eragin zereginaren esfortzua, kostua, datak edo iraupena. Hala ere, WBS kopurua zereginaren automatikoki kalkulatuko da berriz islatzeko zereginaren posizio berria.

### <a name="schedule-estimation"></a>Antolaketa-balioztatzea

Ordutegien estimazioa normalean WBS bat sortzeko bigarren urratsa izan ohi da. Praktika egoki gisa, eginkizunak sortu ondoren ordutegiaren estimazioa osatu beharko zenuke. Finance-ko **Lanen matxuren egitura** orriak bi atal ditu. Goiko panela ordutegiak kalkulatzeko pentsatuta dago, eta beheko panelak an **Aurreikusitako kostuak eta diru-sarrerak** kostua kalkulatzeko erabil dezakezu fitxa. 
**Zereginen mendekotasunak** WBS batean, aurreko lanen arteko harremana sor dezakezu. Zeregin bati aurrenekoen balioak esleitzean, zeregina aurreko zeregin guztiak osatu direnean soilik abiarazi daiteke. Zereginaren hasierako data automatikoki ezartzen da aurreko guztien azken data. 

**Zereginen programazioa** Hurrengo faktoreek zehazten dute hosto-nodoen atazen antolaketa:

-   Aurrekoak
-   Ahalegina
-   Baliabide kopurua
-   Hasiera- eta amaiera-datak

Arauen antolaketa Hosto-nodoaren hasiera-data, aurrekaririk ez duten automatikoki ezarri proiektuaren antolatzeko hasiera-data. Hosto-nodoaren zereginaren iraupena hasiera- eta amaiera-datuen arteko lan-egun kopuru gisa kalkulatzen da beti. 

*<strong><em>Programazio arauak</em></strong>* Programazio automatikoaren laguntza aktibatuta dagoenean, arau hauek aplikatzen zaizkie hosto nodoetako zereginen planifikazioari:

-   Zereginen hasiera- eta amaiera-datek lanegunak izan behar dute, proiektuaren antolaketa-egutegiaren arabera.
-   Hasiera-data zereginaren aurrekariak automatiko ezarriko da azkeneko amaiera-data horien aurrekarienak.
-   Zeregin baterako ahalegina honela kalkulatzen da automatikoki:

Jende kopurua × Iraupena × Proiektuaren egutegian lanegun estandarraren ordu-kopurua. 

Zenbait kasutan, baliteke arau horiek desbideratu behar izatea. Programazio automatikoa desaktiba dezakezu Finantzak hosto nodoen zereginen propietateak automatikoki ezartzea edo zuzentzea ekiditeko. Edozein antolaketa-arau haustea eragiten duen zeregin bati buruzko informazioa idazten duzunean, planifikazio-errore ikono bat agertzen da zereginerako. Programazio akatsak bistaratzea nahi ez baduzu, egin klik **Programazio akatsak agertzen dira** funtzioa desaktibatzeko. 

> [!NOTE] 
> Laburpen edo edukiontzi ataza baten balioak osatutako atazen balioen batura gisa kalkulatzen jarraitzen dute, antolaketa automatikoaren laguntza aktibatuta edo desaktibatuta dagoen ala ez kontuan hartu gabe. 

**Programazio akatsak konpontzea** Programazio automatikoaren laguntza aktibatuta dagoenean, ez dira programazio akatsak gertatuko. Hala ere, programazio automatikoaren laguntza desaktibatzen baduzu eta gero berriro aktibatzen baduzu, akatsen ikonoak ager daitezke WBSn. 

**Programazio akatsak atazaren arabera konpontzea** Zeregin zehatz baten programazio erroreen ikonoan bi aldiz klik egitean, elkarrizketa-koadro batean ataza horren antolaketa errore guztiak bistaratuko dira. Zereginerako zein ordutegi-akats konpondu erabaki dezakezu. 

**Programazio akats guztiak konpontzen** Finantzak WBS programazioko errore guztiak konpontzea nahi baduzu, egin klik Ekintza panelean **Konpondu programazio desadostasun guztiak**. 

> [!NOTE] 
> Ezaugarri honek aldaketa garrantzitsuak sor ditzake WBSn. Akatsak hurrenkera honetan zuzentzen dira:

1.  Eginkizun guztietan kalkulatutako ahalegina aldatu egiten da, proiektuaren egutegian definitutako gaitasunaren berdina izan dadin.
2.  Zeregin bakoitzaren hasiera-data aldatu egiten da, aurreko zeregin guztiak amaitu ondoren zeregina abiarazteko.
3.  Zeregin bakoitzaren hasiera-data aldatu egiten da aurreko lanen hasiera-datetan hutsuneak kentzeko.

### <a name="cost-estimation"></a>Kostuen estimazioa

Dokumentu honetan lehen aipatu bezala, hosto nodo zeregin bakoitzaren kostuen zenbatespena sartzen duzu **Aurreikusitako kostuak eta diru-sarrerak** fitxa beheko panelean **Lanen matxuren egitura** orrialdea. 

> [!NOTE] 
> Ezin duzu aldatu laburpen edo edukiontzi zereginen kostuen zenbatespena. Laburpen zeregin baten kostuen estimazioa bere hosto nodoen zereginen kostuaren estimazioaren batura da. Zeregin bakoitzaren guztizko kostua kalkulatzen da transakzio mota hauetarako zenbatetsitako kostuen zenbatekoen batura gisa:

-   Lana
-   Elementua edo materiala
-   Gastuak

**Kuota** transakzio mota kuoten araberako diru-sarrerak kalkulatzeko erabiltzen da. Transakzio mota honek ez du kostu osagairik eta, beraz, ez da kontuan hartzen kostuak zenbatetsitakoan. 

**Konturako** transakzio mota balio finkoko proiektu mota batean kontratatutako salmenten balioa erregistratzeko erabiltzen da. Transakzio mota hau ere ez da kontuan hartzen kostuak kalkulatzen direnean. 

Zeregin bakoitzeko eskulanaren, materialaren eta gastuen kostuak kalkulatzen dituzunean, proiektuaren kategoria esleitu beharko diozue zenbatetsitako kostuari. 

**Lan kostuak kalkulatzea** Hosto nodo zeregin bakoitzerako, lan esfortzua orduetan eta kategoria lehenetsi batean esleitzen duzu. Hori dela eta, zeregin baterako programazioa konfiguratzen duzunean, zeregin horren kostuaren kalkulua automatikoki gehitzen da eskulanaren kategoria lehenetsian. Kostuen aurrekontu hau **Aurreikusitako kostuak eta diru-sarrerak** fitxan **Lerroaren xehetasunak** zeregin horretarako sareta. Eskulanaren kostuen kalkulu gehiago behar izanez gero, fitxa honetan gehi ditzakezu. Eskulanaren kostuaren kalkuluak orduak handitzen edo murrizten badituzu, zereginaren egutegia automatikoki kalkulatuko da berriro. 

**Gastua eta material kostuak kalkulatzea** hurrengoa **Aurreikusitako kostuak eta diru-sarrerak** fitxak zeregin baterako gastuak eta material kostuak kalkulatzeko aukera ematen du, aurrekontuak behar izanez gero. 

Eskulanaren edo gastuen kalkuluen lerro bakoitzaren kostua eta salmenta-prezioa kategoria bakoitzeko prezioen tauletan zehazten den konfigurazioan oinarritzen dira **Proiektuen kudeaketa eta kontabilitatea** &gt; **Konfigurazioa** &gt; **Prezioak**. Elementuetarako, kostua eta salmenta-prezioa gehitzeko lehenespenez elementu edo merkataritza akordioetatik hurrengoan **Argitaratutako produktuak** zerrenda-orrian Produktuaren informazio-kudeaketa.

## <a name="tracking-progress-on-the-wbs"></a>WBSen aurrerapenaren jarraipena
Zenbait industriak proiektu baten aurrerapenen jarraipena egiten du WBS baten aurka, oso maila pikorrean, beste batzuek, berriz, WBSaren maila altuago batean. Atal honetan WBS jarraipena zure proiektuaren eskakizunetarako nola erabil dezakezu deskribatzen da. 

Finantzak hiru ikuspegi ditu proiektu baten WBSrako: Plangintza ikuspegia, Esfortzuaren jarraipena ikuspegia eta Kostuen jarraipena ikuspegia.

### <a name="planning-view"></a>Plangintza ikuspegia

Planifikazio ikuspegian, ordutegiaren eta kostuen informazioaren aurreikusitako edo oinarrizko estimazioa bistaratzen da. Proiektuaren WBS baten bertsioaren eta oinarrizko lerroaren jarraipena egiteko ezaugarririk ez badago ere, ikuspegi honetako balioak oinarrizko lerroaren bertsioa irudikatzeko pentsatuta daude. Gai honetako Ordutegien estimazioa eta Kostuen estimazioa atalek ikuspegi hau eta WBS bat sortzeko nola erabiltzen den deskribatzen dute.

### <a name="effort-tracking-view"></a>Ahaleginen segimenduaren ikuspegia

Saiakera jarraipenaren ikuspegia bistaratzen da jarraipenaren garapena zereginerako WBS-en. Eginkizun baterako metatutako benetako esfortzu orduak aurreikusitako esfortzu orduekin alderatzen ditu. Ondorengo formulek Ahaleginaren jarraipen ikuspegian ematen dituzte balioak:

-   Garapenaren ehunekoa = Orain arte egindako egiazko ahalegina ÷ Zereginerako aurreikusitako ahalegina
-   Gainerako ahalegina (Burutzeko-osatzeko gisa ere ezagutzen da \[ETC\]) = Aurreikusitako ahalegina - Orain arteko ahalegina
-   Burutzean egindako estimazioa (EAC) = Geratzen den ahalegina + Orain arte ahalegina
-   Proiektatutako ahaleginaren bariantza = Aurreikusitako ahalegina - EAC

Ahaleginaren jarraipena ikuspegiak zereginaren esfortzuaren bariantzaren proiekzioa erakusten du, EAC aurreikusitako ahalegina baino gehiago edo txikiagoa den oinarrituta:

-   EAC aurreikusitako ahalegina baino handiagoa bada, zereginak hasieran aurreikusitakoa baino denbora gehiago beharko duela aurreikusten da eta antolaketaren atzean dago.
-   EAC aurreikusitako ahalegina baino gutxiago bada, zereginak hasieran aurreikusitakoa baino denbora gutxiago beharko duela aurreikusten da eta antolaketaren aurrean dago.

**Proiektuaren zuzendariaren ahalegina berriro proiektatzea** Batzuetan, proiektuaren zuzendariak edo proiektu baten aurrerapenaren jarraipena egiten duen beste pertsona batek zeregin baten jatorrizko kalkuluak berrikusi beharko ditu. Zeregina hasieran aurreikusitakoa baino azkarrago edo mantsoago mugitzen ari da hainbat arrazoirengatik. Adibidez, esparrua murriztu da edo langileek hasieran aurreikusitakoa baino esperientzia gutxiago dute. Proiekzioak proiektuaren kudeatzailearen pertzepzioaren balioztatzea, oinarrituz uneko egoeraren proiektuan. Orokorrean, ez zenuke aldatu behar oinarrizko zenbakiak, argitaratutako dokumentuak ordezkatzen duen oinarrizko proiektua proiektuaren antolaketa kosturako balioztatzen du interes talde guztiak onartutako proiekturako. 

Proiektu-kudeatzaileak bi modutara alda ditzake zereginetako ahaleginak:

-   Aldatu automatikoki ezartzen den gainerako ahalegina, zereginean geratzen den ahalegina eguneratzeko.
-   Aldatu automatikoki ezartzen den garapenaren ehunekoa zereginean egiazko garapena.

Bi Planteamendu zereginaren ETC, EAC eta garapenaren ehunekoa eta zeregin baten proiektatutako ahaleginaren bariantza berriro kalkulatzea eragiten du. Laburpen zereginetan EAC, ETC eta garapenaren ehunekoa ere berriro kalkulatzen dira eta haien proiektatutako ahaleginen aldaketa eguneratuta dago. 

**Laburpen zereginetan ahalegina aldatu da** Laburpen edo edukiontzi zereginetan ahalegina alda dezakezu. Zuk balio horiek aldatzen badituzu edo ez gainerako ahalegina erabiliz edo garapenaren ehunekoa laburpenaren zereginak, kalkuluak gertatuko dira automatikoki hurrengo ordenean:

1.  Zeregineko EAC, ETC eta garapenaren ehunekoa kalkulatzen dira.
2.  EAC berria bigarren mailako zereginetan banatzen da jatorrizko zereginean zegoen EAC proportzio berean.
3.  Hosto-nodo bakoitzaren EAC berria kalkulatzen da.
4.  Gainerako ahalegina eta aurrerapen portzentajea kaltetutako haurraren zeregin guztietarako birkalkulatzen da, EAC balio berrian oinarrituta. Zereginen esfortzu-bariantza ere berriro kalkulatzen da.
5.  Laburpen zereginen EAC orri-nodoetatik berriro kalkulatzen da.

Egin klik **Zabaldu mailara** esfortzuaren jarraipena ikuspegian zure WBSen jarraipena eta mantentze-maila zehazteko. WBS automatikoki maila horretara zabaltzen da Esfortzuaren jarraipena ikuspegian irekitzen duzun bakoitzean.

### <a name="cost-tracking-view"></a>Kostuen jarraipenaren ikuspegia

Kostuen jarraipena ikuspegiak ataza baterako kostuen kontsumoaren jarraipena erakusten du. Ikuspegi honen arabera, orain arte zeregin baten aurka gastatu den kostua zereginerako aurreikusitako kostuarekin alderatzen da. Ondorengo formulek Kostuaren jarraipen ikuspegian ematen dituzte balioak:

-   Kontsumitutako kostuaren ehunekoa = Orain arteko kostua ÷ Zereginerako aurreikusitako kostua
-   Burutzeko kostua (CTC) = Aurreikusitako kostua - Orain arteko kostua
-   Estimazioa osatuta (EAC) = CTC + Orain arteko kostu erreala
-   Proiektatutako kostuaren bariantza = Aurreikusitako kostua - EAC

Kostuaren jarraipena ikuspegiak zereginaren kostuaren bariantzaren proiekzioa erakusten du, EAC aurreikusitako kostua baino gehiago edo txikiagoa den oinarrituta:

-   EAC aurreikusitako kostua baino handiagoa bada, zereginak hasieran aurreikusitakoa baino diru gehiago erabiliko duela aurreikusten da eta aurrekontuaren gainetik dago.
-   EAC aurreikusitako kostua baino txikiagoa bada, zereginak hasieran aurreikusitakoa baino diru gutxiago erabiliko duela aurreikusten da eta aurrekontuaren azpitik dago.

**Proiektuaren zuzendariaren kostua berriro proiektatzea** Proiektuen kudeatzaileek CTC erabili behar dute zeregin baten kostuaren aurrekontua berrikusteko. Proiektuaren kudeatzaileak CTC balioa alda dezake zeregina betetzeko behar den kostura. CTC balioa aldatzen baduzu, zereginaren CTC, EAC eta kontsumitutako kostuaren ehunekoa eta zeregin batean aurreikusitako kostuen bariantza berriro kalkulatuko dira. Laburpen zereginetan EAC, ETC eta kostua kontsumitua ehunekoa ere berriro kalkulatzen dira eta haien proiektatutako kostuaren aldaketa eguneratuta dago. 

> [!NOTE] 
> Esfortzuaren jarraipena ikuspegian WBS zeregin baterako ahalegina berrikusten duzunean, atazaren CTC, EAC, kontsumitutako kostuaren ehunekoa eta aurreikusitako kostuen bariantza berriro kalkulatzen dira Kostuen jarraipena ikuspegian. Hala ere, kostuen berrikuspenek ez dute Ahaleginaren jarraipena ikuspegiko balioetan eragiten, kostua transakzio motaren arabera (eskulana, materiala edo gastua) edo proiektuaren kategoria ez delako berrikusten. 

**Laburpen zereginetan kostuen proiekzioa berrikustea** Laburpen zereginetan kostuak berrikusi ditzakezu eta kalkuluak automatikoki egiten dira hurrenkera honetan:

1.  EAC, CTC eta zereginean kontsumitutako kostuaren ehunekoa berriro kalkulatzen dira.
2.  EAC berria bigarren mailako zereginetan banatzen da jatorrizko zereginetan zegoen EAC proportzio berean.
3.  Ataza bakoitzaren EAC berria kalkulatzen da.
4.  CTS eta kontsumitutako kostuaren portzentajea kaltetutako haurraren zereginetarako birkalkulatzen dira, EAC balioan oinarrituta. Kostua esfortzu-bariantza ere berriro kalkulatzen da.
5.  Laburpen zeregin guztien EAC birkalkulatzen da aldaketa horren arabera.

Egin klik **Zabaldu mailara** kostuaren jarraipena ikuspegian zure WBSen jarraipena eta mantentze-maila zehazteko. WBS maila horretara zabaltzen da Kostuaren jarraipena ikuspegian irekitzen duzun bakoitzean.

### <a name="earned-value-management"></a>Irabazitako balioaren kudeaketa

Irabazitako balioaren metodoa (EVM) erabil dezakezu proiektu baten garapenaren jarraipena egiteko. Irabazitako balioaren metrikak proiektuaren kudeatzailearen rolen zentroan ikus ditzakezu. Irabazitako balio-taulako osagaiak aurreikusitako balioaren eta benetako kostuaren denbora-faseko balioak erakusten ditu. Irabazitako balioa uneko datatik puntu gisa erakusten da. Irabazitako balioaren denborazko datuak ez daude erabilgarri une honetan. 

Irabazitako balio-taulako denbora fasea astez edo hilabetez bistaratzen da. Atal honetan EVMren hiru zutabeak deskribatzen dira: aurreikusitako balioa, irabazitako balioa eta benetako kostua. 

**Aurreikusitako balioa** EVM teoriaren arabera, aurreikusitako balioaren lursailak proiektuaren taldeak proiektuan balioa irabazteko asmoa zuen abiadura adierazten du. 

Finantzak 0: 100 irabazteko araua erabiltzen du aurreikusitako balioa adierazten duenean. Arau honen arabera, atazaren balioa ataza bertan amaitzen den egunetik aurrera argitaratzen da. Ez da baliorik ataza ehuneko 100 bete arte. 

Proiektuen kudeaketa eta kontabilitatea atalean, hosto nodoen amaiera data eta horretarako aurreikusitako kostua sartzen dituzu. Aurreikusitako balioaren grafikoa astero bistaratzen denean, aurreikusitako balioa astero laburbiltzen da hosto nodoaren eginkizun guztietarako proiektuak iraun bitartean. 

**Jasotako balioa** EVM teoriaren arabera, irabazitako balioaren lursailak proiektuaren taldeak proiektuan balioa irabazteko unean zuen abiadura adierazten du. 

Finantzak 0: 100 irabazteko araua erabiltzen du irabazitako balioa adierazten duenean. Arau honen arabera, atazaren balioa ataza bertan amaitzen den egunetik aurrera argitaratzen da. Ez da baliorik ataza ehuneko 100 bete arte. 

Irabazitako balioa kalkulatzen denean, ataza bakoitzaren aurrerapen portzentajea kontuan hartzen da. 0: 100 irabazteko arauaren arabera, epe jakin batean burututako zereginak soilik hartzen dira kontuan irabazitako balioa kalkulatzeko epe hori amaitu zenetik aurrera. Proiektuan lortutako balioa grafikoa sortzerakoan burututako zeregin guztietarako kalkulatzen da. 

> [!NOTE] 
> Gaur egun, WBS jarraipena egiteko sistemak ez du zeregin bakoitzean aurrerapen portzentaje historikoak gordetzeko datu egiturarik. Hori dela eta, irabazitako balioa kuboa prozesatzen den unetik aurrera bakarrik eman daiteke. Prozesatu kuboa aldizka Role Center-en agertzen diren irabazitako balioen datuak eguneratzeko. 

**Benetako kostua** EVM teoriaren arabera, benetako kostuaren lursailak dirua proiektuan gastatzen den tasa adierazten du. 

Proiektu batean argitaratzen diren eragiketak benetako kostu lerroa marrazteko erabiltzen dira. Kostuak dataren arabera laburbiltzen dira. Datu horiek gero irabazitako balio-taulan kostuen benetako kostuak astean edo hilean grafikatzeko erabiltzen dira.

### <a name="how-to-use-the-concepts-of-planned-value-earned-value-and-actual-cost"></a>Nola erabili aurreikusitako balioaren, irabazitako balioaren eta benetako kostuaren kontzeptuak

**Programatu bariantza** Planifikazioan zehar, kronograman lan egiteko aurreikuspenak sortzen dituzu. Hori dela eta, aurreikusitako balioa proiektuaren antolatzaileek proiektuan lanak amaituko zirela pentsatzen duten tasa da. Proiektu bat martxan dagoenean, lanak amaitu eta proiektuak balioa irabazten du. Aurreikusitako balioa irabazitako balioarekin alderatuz gero, proiektu bateko lanak nola aurrera doazen ikus dezakezu. Konparazio horren emaitzari ordutegi bariantza deritzo. 

Aldi baterako aurreikusitako balioa irabazitako balioa baino handiagoa bada, proiektu batean egindako lan kopurua aurreikusitakoa baino txikiagoa da. Hori dela eta, proiektua atzeratu egin da. Aurreikusitako balioa eta irabazitako balioa dirutan adierazten direnez, proiektuaren atzerapen-denborari ere diru-balioa ematen zaio. 

Aldi baterako aurreikusitako balioa irabazitako balioa baino gutxiago bada, proiektu batean egindako lan kopurua aurreikusitakoa baino gehiago da. Hori dela eta, proiektua aurreratu egin da. Berunezko denbora horri diru balioa ere ematen zaio.

**Kostuen bariantza** Lortutako balioak kostuaren prezioa biderkatzaile gisa erabiltzen duenez, irabazitako balioak proiektu batean egiten den lanaren kostua adierazten du. Proiektuak aurrera egin ahala, transakzioen erregistroak proiektu horretan benetan gastatzen den diruaren erregistroa eskaintzen du. Irabazitako balioa benetako kostuarekin alderatuz gero, gastatzen den diru kopurua eta irabazitako balioa ikus ditzakezu. Konparazio horren emaitzari kostuaren bariantza deritzo. 

Epe baterako gastatutako benetako kostua irabazitako balioa baino handiagoa bada, irabazitakoa baino diru gehiago gastatu da. Hori dela eta, proiektuak aurrekontua gainditu du. 

Epe baterako gastatutako benetako kostua irabazitako balioa baino gutxiago bada, gastatutakoa baino diru gehiago irabazi da. Hori dela eta, proiektuak aurrekontua azpian du.

## <a name="wbs-templates"></a>WBS txantiloiak
WBS txantiloien funtzionalitatea erabil dezakezu proiektuetarako txantiloi estandarrak sortzeko. Zure enpresak eskaintzen dituen proiektuek lan errepikakor asko suposatzen badute, WBS txantiloia sortzea pentsatu beharko zenuke. 

Lehendik zegoen proiektu baten WBS-tik WBS txantiloia sor dezakezu, proiektu horren plangintzan bildu zenituen ezagutzak eta praktika onak antzeko proiektuetan berrerabili ahal izateko etorkizunean. Hala ere, batzuetan, agian ez luke zentzurik WBS osoa txantiloi gisa gordetzea. Hori dela eta, proiektu baterako WBSaren zati batzuetatik txantiloiak sor ditzakezu.

### <a name="saving-a-projects-wbs-as-a-template"></a>Proiektu baten WBS txantiloi gisa gordetzea

Txantiloi bat sortu ondoren, proiektu berriaren WBSra inporta dezakezu erro nodoaren azpian edo proiektuaren WBSeko edozein zereginetan.

### <a name="importing-a-wbs-template-into-a-projects-wbs"></a>WBS txantiloia proiektu baten WBSra inportatzea

Zereginak inportatzen dituzunean, txantiloiko zereginak azpian inportatzen diren zereginaren hasierako dataren arabera antolatzen dira. Inportazioan zehar, txantiloi atazen aurreko harremanak erabiltzen dira inportatutako atazen hasiera datak kalkulatzeko. Helmugako proiektuaren lan egutegi estandarra inportatutako zereginen amaiera datak kalkulatzeko aplikatzen da, uneko proiektuaren lan egutegian definitutako lanegunak eta lanaldi estandarrak mantendu ahal izateko. 

Aurrekontu-lerroetako kostuen zenbatekoak eta salmenta-prezioak aplikatzen dira proiektuari edo proiektuaren kontratuari dagozkion prezioek baliozko datak dituztela bermatzeko.

### <a name="differences-between-a-projects-wbs-and-a-wbs-template"></a>Proiektu baten WBS eta WBS txantiloien arteko desberdintasunak

-   WBS txantiloietako zereginek ez dute hasiera datarik eta amaiera datarik.

Laneguneko eta laneguneko egunak ez daude zehaztuta WBS txantiloietan.

-   WBS txantiloiek proiektu guztietarako egutegi lehenetsi gisa ezarrita dagoen antolaketa egutegia erabiltzen dute beti.

Programazio egutegi lehenetsia lanegun estandar bateko orduak jakiteko soilik erabiltzen da.

-   Aurreko harremanak ez dira WBS txantiloian kopiatzen.

WBS txantiloiek datarik ez dutenez, ez da beharrezkoa aurrekoaren amaiera datan oinarritutako hasiera dataren logika.

-   Lan kostuen estimazio lerroa automatikoki sortzen da ataza bat WBS txantiloian sortzen denean. Salmenta prezioa eta kostuaren zenbatekoa hautatutako langilearengandik kopiatzen dira.

Gastuen eta elementuen kostuak eskuz sor daitezke, proiektu baten WBSean egin dezaketen moduan.

-   Programazio akatsak bistaratzen dira formula honetatik desbideratzeak daudenean:

Esfortzua = Baliabide kopurua × Iraupena × Lanaldi estandar bateko ordu kopurua 

Programazio akats guztiak aldi berean zuzendu ditzakezu klik eginez **Konpondu programazio akats guztiak**. 

Bestela, planifikazio akatsak banan-banan zuzendu ditzakezu zeregin bakoitzerako abisu ikonoan klik eginez.





[!INCLUDE[footer-include](../includes/footer-banner.md)]