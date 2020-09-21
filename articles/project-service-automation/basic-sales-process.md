---
title: Salmenta-prozesuak
description: Gai honek oinarrizko salmenta-prozesuei buruzko informazioa ematen du.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: a169dee5-f4a7-42c8-9bf1-7f0018cc25cb
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: eaaa4b8fe6577ff572489ac0c6abac3c4e970c63
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748878"
---
# <a name="sales-processes"></a>Salmenta-prozesuak

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Proiektuetan oinarritutako erakunde batean erabiltzen diren salmenta-prozesuak eta produktuetan oinarritutako erakunde batean erabiltzen diren salmenta-prozesuak desberdinak dira. Alde hori gertatzen da proiektuetan oinarritutako erakundeen salmenta-zikloak luzeagoak direlako eta aurreikuspen bakoitzarentzako eskaintzak aztertu eta kalkulatzeko teknika pertsonalizatuak behar dituztelako. Dynamics 365 Project Service Automation-ek Dynamics 365 Sales-en salmenta-prozesuan erabilitako funtzionaltasun bera erabiltzen du. Hona hemen zenbait adibideak:

- Erakunde nagusi bat salmenta-prozesuaren jarraipena egiteko erabiltzen da.
- Bezerogai kalifikatzaileak abagune gisa jarraitzen dira. Salmenta-prozesua abagunearekin ere has daiteke.
- Abagune baterako erlazionatutako artefaktu guztiak eskura daitezke. Artefaktu hauek salmenta-taldea, interes taldeak, probabilitatea, balorazioa, salmenta faseak eta negozio prozesuak dituzte.
- Eskaintza bat baino gehiagok abagunea sortzen dute.
- Eskaintza markatuta dago **Irabazi gisa itxita** moduan salmenta-eskaera sortzeko. PSAn, salmenta-eskaera pertsonalizatzen da eta proiektu-kontratua deitzen zaio.

Hurrengo irudian proiektuan oinarritutako erakunde bateko salmenta-prozesua erakusten da.

> ![Salmenta-prozesua proiektuan oinarritutako erakunde batean](media/basic-guide-1.png)

## <a name="estimating-a-sale"></a>Salmenta bat aurreikusten
Salmenta baten balioa aurretik entregatutako proiektuen eta proiektuen konplexutasunaren arabera aurreikusi daiteke. Aurreko proiektuetara hedapenak inplikatzen dituzten proiektuetarako edo saltzailearen espezializazioa handia den eta ezagunak diren lan-txantiloiak erabiltzen dituzten proiektuetarako, aurreikuspen prozesu sinpleagoa erabil dezakezu. Proiektu konplexuagoek normalean erosketa-prozesu luzeagoa izaten dute. Hori dela eta, fase gehiago daude salmenten aurreikuspen prozesuan. Prozesu hasieran, salmenta-taldeak kontu kudeatzaileen eta gaien adituek (ETEak) egiten duten ekarpena erabiltzen da kotizatzen den lan osagai bakoitzerako goi mailako aurreikuspena sortzen hasteko. Lan osagai hauek eskaintzaren lerroen bidez irudikatzen dira. 

Eskaintzaren goi mailako aurreikuspena sor dezakezu. Azkenean, goi-mailako aurreikuspen hau proiektuaren txantilo normalizatuak erabiliz sortutako proiektu-planean oinarritutako aurreikuspen zehatzagoa izango da. Txantiloi hauek ordutegi bat eraikitzen eta eskaintzen eta haren osagaien (eskaintzaren lerroak) dirua zehazten lagunduko dizute. 

Proiekturako hainbat eskaintza sor ditzakezu eta abagune bakarreko entitate motaren arabera taldeka ditzakezu. Azkenean, eskaintza horietako bat markatuta dago **Irabazi gisa itxita** moduan, eta proiektu-kontratua edo lanaren adierazpena (SOW) sortzen da. Proiektu-kontratuak bezeroak entragatzeko onartzen duen osagai bakoitzeko (kontratuaren lerroa) balio bat edukitzen du. SOW bat bezala sortzen da normalean Microsoft Word dokumentua. Proiektua entregatu bitartean bezeroari bidaltzen zaizkion faktura guztiek proiektuaren kontratua edo SOW aipatzen dute.

Abagune entitate mota baten pean ordezko eskaintzak sor ditzakezu edo sistema konfiguratu proiektu-kontratua eratzeko eskaintza bat irabazten denean. Kasu honetan, SOW ordezkatzen duen Word dokumentua erantsi diezaioke proiektuaren kontratuaren erregistroari.

![Eskaintza ixtea proiektu-kontratua sortzeko](media/basic-guide-2.png)

## <a name="configuring-the-sales-process"></a>Salmenta-prozesua konfiguratzea
Negozio-prozesuaren fluxuak (BPF) erabil ditzakezu Microsoft Dynamics 365 salmenta-prozesuan konfiguratzeko. BPFek salmentako langileei zure negozio tipikoa duten faseetan aurrerakuntzak egiteko erabil ditzaketen bisual interfaze gidatua eskaintzen diete.

Adibidez, zure enpresak hurrengo sei faseak izan ditzake salmenta-prozesuan:

1. Gaitu
2. Aurreikuspena
3. Barne-berrikuspena
4. Kontratua
5. Entregatu
6. Itxi

Sei fase hauek xebroien bidez irudikatzen dira (\>), sortu duzun abagune entitate mota bakoitzean zabaltzeko hautatzen dituzunak.

![Negozio-prozesuaren konfigurazioa Dynamics 365-en](media/basic-guide-3.png)
 
Erakundeak hainbat entitate erabil ditzake eboluzionatu duen akordio bera irudikatzeko. Salmenta-prozesuan hasieran, tratua Abagunea entitatearen bidez adierazten da. Denbora igaro ahala eta xehetasun gehiago azaltzen diren heinean, baliteke goi mailako aurreikuspenak erabil daitezkeela eskaintza bat edo gehiago sortzeko. Eskaintza horietako bat barneko bezeroen eta interes taldeek berrikusten badute, Eskaintza entitateak tratua adierazten du. Bezeroak eskaintza onartu ondoren, proiektu-kontratuak edo SOWk tratua adierazten du. Jokabide hori onartzeko, BPFak egituratzen dira, prozesuko fase bakoitza datu baseko taula desberdin batekin lotuta egon dadin.

**Gaitu** fasean salmenta-prozesuan Abagunea entite batek babestu dezake. **Aurreikuspena** eta **Barne-berrikuspena** faseak Eskaintza entitate batek babestu ditzake. **Kontratua**, **Entrega**, eta **Itxi** faseak Proiektu-kontratua entitate batek babestu ditzake.

Tratuak faseetan zehar mugitzen dituzunean, prozesuan zehar laguntzeko eta gidatzeko entitate erregistro egokia sortzeko eskatuko zaizu. Faseak baldintzatuak izan daitezke. Adibidez, eskaintzaren barne-berrikuspena behar baduzu eskaintzak prezio-zerrenda pertsonalizatua erabiltzen badu soilik, baldintza hori konfigura dezakezu negozio prozesuaren fase egokian. **Barne-berrikuspena** fasea, ondoren, pertsonalizatutako prezio-zerrenda erabiltzen duten eskaintzetarako bakarrik erakutsiko da. Gainerako tratu eta eskaintzetarako, **Aurreikuspena** fasearen ostean **Kontratua** fasea izango da.

> [!NOTE]
> PSAk orrialde espezifikoak ditu Abagunea, Eskaintza, Eskaera eta Faktura entitateetarako. Project Service abaguneak, eskaintzak, eskaerak eta fakturak sortu behar dituzu entitate horien proiektuaren informazio orriak erabiliz. Erregistro bat sortzeko beste orri bat erabiltzen baduzu, ezin izango duzu erregistroa ireki **Proiektuaren informazioa** orrian. Erregistro bat ireki nahi baduzu **Proiektuaren informazioa** orrian, erregistroa ezabatu eta birsortu egin behar duzu **Proiektuaren informazioa** orrian. **Proiektuaren informazioa** orrialdean, negozioen logika entitate mota bakoitzerako **Mota** erregistroaren eremua behar bezala finkatuta dagoela ziurtatzen du, eta nahitaezko kontzeptu guztiak behar bezala hasi direla.

> ![Eskaera berri bat egiteko proiektuaren informazioa](media/basic-guide-4.png)
 
## <a name="differences-between-project-service-automation-and-sales"></a>Project Service Automation eta Sales-en arteko desberdintasunak
Salmenta-prozesuak PSAn Sales-en erabilitako salmenta-prozesuaren oinarrizko gaitasunak erabiltzen baditu ere, funtsezko desberdintasunak ditu proiektuan oinarritutako erakundeen negozio praktiken aldaketengatik. Hona hemen zenbait adibideak:

- **Proiektuaren aurrekontuak**: ,Project Service Automation-en eskaintza itxi egiten da proiektu-kontratua eskaintza batetik sortu ondoren. Sales-en, eskaintza irekita mantendu dezakezu irabazi ondoren. Alde horren arrazoia da eskaintzaren eta proiektu-kontratu baten arteko partida hobea dela proiektuan oinarritutako erakundeentzat. 
- **Aktibazioa eta berrikuspenak**: PSAn, aktibazioa eta berrikuspenak ez dira onartzen proiektuen eskaintzetarako. Sales-en, eskaintza blokeatu daiteke, aldaketa gehigarriak ekiditeko.
- **Eskaintza itxi galduta edo irabazita moduan**: PSAn, proiektuaren eskaintza irabazita edo galduta moduan itxita dagoenean, abaguneak irekia izaten jarraitzen du. Abaguneko gainerako eskaintza guztiak galduta moduan daude itxita. Sales-en, eskaintza irabazita edo galduta moduan itxita dagoenean, erabiltzaileari abaguneari buruzko ekintza bat eskatzen zaio. Erabiltzailearen sarreren arabera, azpiko abagunea itxita edo irekita egon liteke.

## <a name="tracking-revisions-to-quotes-and-project-plans-in-the-sales-cycle"></a>Salmenta-zikloko eskaintzen eta proiektu-planen berrikuspenak jarraitzea
PSAn, ezin duzu eskaintzetan egiten diren berrikuspenik egin. Horren ordez, lehendik dagoen eskaintza markatu behar duzu **Galdu bezala itxita** moduan eta sortu eskaintza berria. Eskaintza kopiatu edo proiektuan oinarritutako eskaintza kopiatu dezakezu PSA erabiliz.

## <a name="tracking-comments-and-approvals-of-quotes-and-project-contracts"></a>Eskaintzen eta proiektu-kontratuen iruzkinak eta onespenak jarraitu
Eskaintzen eta proiektu-kontratuen berrikuspena eta onespena kudeatu ahal izango dituzu erregistroen horma eta mezuak erabiliz. Erakundeak lan-fluxuak eta plugin pertsonalizatuak sor ditzake, berrikusteko eta onesteko lan-elementuen jakinarazpenak kudeatzeko.
