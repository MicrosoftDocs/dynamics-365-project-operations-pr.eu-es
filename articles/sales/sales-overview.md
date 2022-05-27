---
title: Salmenta-prozesuaren informazio orokorra
description: Gai honek oinarrizko salmenta-prozesuei buruzko informazioa ematen du.
author: rumant
ms.date: 10/29/2020
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: e99035798f775de5cd59724a9fe0d7ea6de40034
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8578463"
---
# <a name="sales-process-overview"></a>Salmenta-prozesuaren informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuetan oinarritutako erakunde batean erabiltzen diren salmenta-prozesuak eta produktuetan oinarritutako erakunde batean erabiltzen diren salmenta-prozesuak desberdinak dira. Alde hori gertatzen da proiektuetan oinarritutako erakundeen salmenta-zikloak luzeagoak direlako eta aurreikuspen bakoitzarentzako eskaintzak aztertu eta kalkulatzeko teknika pertsonalizatuak behar dituztelako. Dynamics 365 Project Operations-ek salmenta prozesu batean erabiltzen diren funtzionalitate hauetako batzuk erabiltzen ditu:

- Erregistro nagusi bat salmenta-prozesuaren jarraipena egiteko erabiltzen da.
- Bezerogai kalifikatzaileak abagune gisa jarraitzen dira.
- Abagune baterako erlazionatutako artefaktu guztiak eskura daitezke. Artefaktu hauek salmenta-taldea, interes taldeak, probabilitatea, balorazioa, salmenta faseak eta negozio prozesuak dituzte.
- Eskaintza bat baino gehiagok abagunea sortzen dute.
- Egoera jakin bateko eskaintza bat **Irabazi gisa itxita** moduan salmenta-eskaera sortzeko. Project Operations-en, salmenta-eskaera pertsonalizatzen da eta proiektu-kontratua deitzen zaio.

## <a name="estimate-a-sale"></a>Salmenta bat aurreikuspena
Salmenta baten balioa aurretik entregatutako proiektuen eta proiektuen konplexutasunaren arabera aurreikusi daiteke. Aurreko proiektuetara hedapenak inplikatzen dituzten proiektuetarako edo saltzailearen espezializazioa handia den eta ezagunak diren lan-txantiloiak erabiltzen dituzten proiektuetarako, aurreikuspen prozesu sinpleagoa erabil dezakezu. Proiektu konplexuagoek normalean erosketa-prozesu luzeagoa izaten dute. Hori dela eta, fase gehiago daude salmenten aurreikuspen prozesuan. Prozesu hasieran, salmenta-taldeak kontu kudeatzaileen eta gaien adituek (ETEak) egiten duten ekarpena erabiltzen da kotizatzen den lan osagai bakoitzerako goi mailako aurreikuspena sortzeko. Lan osagai hauek eskaintzaren lerroen bidez irudikatzen dira. 

Eskaintzaren goi mailako aurreikuspena sor dezakezu. Azkenean, goi-mailako aurreikuspen hau proiektuaren txantilo normalizatuak erabiliz sortutako proiektu-planean oinarritutako aurreikuspen zehatzagoa izango da. Txantiloi hauek ordutegi bat eraikitzen eta eskaintzen eta haren osagaien (eskaintzaren lerroak) dirua zehazten lagunduko dizute. 

Proiekturako hainbat eskaintza sor ditzakezu eta abagune bakarreko erregistroaren arabera taldeka ditzakezu. Azkenean, eskaintzetako bat markatuta dago **Irabazi gisa itxita** moduan, eta proiektu-kontratua edo lanaren adierazpena (SOW) sortzen da. Proiektu-kontratuak bezeroak entragatzeko onartzen duen osagai bakoitzeko (kontratuaren lerroa) balio bat edukitzen du. SOW bat bezala sortzen da normalean Microsoft Word dokumentua. Proiektua entregatu bitartean bezeroari bidaltzen zaizkion faktura guztiek proiektuaren kontratua edo SOW aipatzen dute.

Abagune-erregistro mota baten pean ordezko eskaintzak sor ditzakezu edo sistema konfiguratu proiektu-kontratua eratzeko eskaintza bat irabazten denean. Kasu honetan, SOW ordezkatzen duen Word dokumentua erantsi diezaioke proiektuaren kontratuaren erregistroari.

## <a name="configure-the-sales-process"></a>Salmenta-prozesua konfiguratu
Negozio-prozesuaren fluxuak erabil ditzakezu salmenta-prozesua konfiguratzeko. Fluxu hauek interfaze bisual gidatua eskaintzen dute salmentak prozesuaren faseak aurrera eramateko.

Adibidez, zure enpresak hurrengo sei faseak izan ditzake salmenta-prozesuan:

1. Gaitu
2. Aurreikuspena
3. Barne-berrikuspena
4. Kontratua
5. Entregatu
6. Itxi
 
Erakundeak hainbat entitate erabil ditzake eboluzionatu duen akordio bera irudikatzeko. Salmenta-prozesuan hasieran, tratua Abagunea entitatearen bidez adierazten da. Denbora igaro ahala eta xehetasun gehiago azaltzen diren heinean, baliteke goi mailako aurreikuspenak erabil daitezkeela eskaintza bat edo gehiago sortzeko. Eskaintza horietako bat barneko bezeroen eta interes taldeek berrikusten badute, Eskaintza entitateak tratua adierazten du. Bezeroak eskaintza onartu ondoren, proiektu-kontratuak edo SOWk tratua adierazten du. Jokabide hori onartzeko, BPFak egituratzen dira, prozesuko fase bakoitza datu baseko taula desberdin batekin lotuta egon dadin.

**Gaitu** fasean salmenta-prozesuan Abagunea entite batek babestu dezake. **Aurreikuspena** eta **Barne-berrikuspena** faseak Eskaintza entitate batek babestu ditzake. **Kontratua**, **Entrega**, eta **Itxi** faseak Proiektu-kontratua entitate batek babestu ditzake.

Tratuak faseetan zehar mugitzen dituzunean, prozesuan zehar laguntzeko eta gidatzeko entitate erregistro egokia sortzeko eskatuko zaizu. Faseak baldintzatuak izan daitezke. Adibidez, eskaintzaren barne-berrikuspena behar baduzu eskaintzak prezio-zerrenda pertsonalizatua erabiltzen badu soilik, baldintza hori konfigura dezakezu negozio prozesuaren fase egokian. **Barne-berrikuspena** fasea, ondoren, pertsonalizatutako prezio-zerrenda erabiltzen duten eskaintzetarako bakarrik erakutsiko da. Gainerako tratu eta eskaintzetarako, **Aurreikuspena** fasearen ostean **Kontratua** fasea izango da.

> [!NOTE]
> Project Operations-ek orrialde zehatzak ditu Aukera, aurrekontua, eskaera eta faktura entitateen erregistroetarako. Erregistro horiek entitate horien proiektuaren informazio orriak erabiliz sortu behar dituzu. Bestela, ezin izango dituzu erregistroak ireki **Proiektuaren informazioa** orrialdea. Erregistroa fitxategitik ireki nahi baduzu **Proiektuaren informazioa** orrialdea, erregistroa ezabatu eta birsortu behar duzu **Proiektuaren informazioa** orrialdea non entitate mota horietako bakoitzaren negozio logikak ziurtatzen duen **Mota** erregistroaren eremua behar bezala ezarrita dago, eta derrigorrezko kontzeptu guztiak behar bezala hasieratuta daude.


## <a name="track-revisions-to-quotes-and-project-plans-in-the-sales-cycle"></a>Salmenta-zikloko eskaintzen eta proiektu-planen berrikuspenak jarraitu
Project Operations-en, ezin duzu eskaintzetan egiten diren berrikuspenik egin. Horren ordez, lehendik dagoen eskaintza markatu behar duzu **Galdu bezala itxita** moduan eta sortu eskaintza berria. Eskaintza kopiatu edo proiektuan oinarritutako eskaintza kopiatu dezakezu.

## <a name="track-comments-and-approvals-of-quotes-and-project-contracts"></a>Eskaintzen eta proiektu-kontratuen iruzkinak eta onespenak jarraitu
Eskaintzen eta proiektu-kontratuen berrikuspena eta onespena kudeatu ahal izango dituzu erregistroen horma eta mezuak erabiliz. Erakundeak lan-fluxuak eta plugin pertsonalizatuak sor ditzake, berrikusteko eta onesteko lan-elementuen jakinarazpenak kudeatzeko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]