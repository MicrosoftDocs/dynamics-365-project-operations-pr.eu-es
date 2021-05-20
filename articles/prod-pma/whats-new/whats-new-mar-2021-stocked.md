---
title: 2021eko martxoko Project Operations-eko berrikuntzak edo aldaketak- Izakinen edo ekoizpenean oinarritutako egoeretarako
description: Gai honek 2021eko martxoko Project Operations bertsioan eskuragarri dauden/ekoizpenean oinarritutako agertokietarako eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: andchoi
manager: tfehr
ms.date: 03/22/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: andchoi
ms.openlocfilehash: 804b5d1cc3392349fb6bcc81a91d69d0d9dc51da
ms.sourcegitcommit: 386921f44f1e9a8a828b140206d52945de07aee7
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/22/2021
ms.locfileid: "5701905"
---
# <a name="whats-new-or-changed-in-project-operations-march-2021-for-stockedproduction-based-scenarios"></a>2021eko martxoko Project Operations-eko berrikuntzak edo aldaketak- Izakinen edo ekoizpenean oinarritutako egoeretarako

_**Honi aplikatzen zaio:** Izakinen edo ekoizpenean oinarritutako egoeretarako Project Operations_

Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.17 bertsioa

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak
Eginbide hauek sartzen dira bertsio honetan:

  - [Proiektuko faktura-proposamenen errendimendua](../project-invoice-proposal-performance.md)
 
### <a name="quality-updates"></a>Kalitatearen eguneratzeak

| Ezaugarrien eremua                        | Erreferentzia-zenbakia | Kalitatearen eguneratzea                                                                                                                                                                                                                                                   |
|-------------------------------------|------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Proiektuaren kudeaketa eta kontabilitatea | [420064](https://fix.lcs.dynamics.com/Issue/Details/?bugId=420064) | Bidalitako proiektuen transakzio negatiboak ez dira eguneratzen inbentarioa berriro kalkulatu ondoren.                                                                                                                      |
| Proiektuaren kudeaketa eta kontabilitatea | [438692](https://fix.lcs.dynamics.com/Issue/Details/?bugId=438692) | Finantziazio iturria ezabatzea posible izan beharko litzateke finantzaketa iturrirako transakziorik edo fakturarik ez badago.                                                                                                           |
| Proiektuaren kudeaketa eta kontabilitatea | [439470](https://fix.lcs.dynamics.com/Issue/Details/?bugId=439470) | Benetako estimazio transakzioek ez dituzte aurreko aldiko gastuen eta elementuen transakzioak erakusten.                                                                                                       |
| Proiektuaren kudeaketa eta kontabilitatea | [452710](https://fix.lcs.dynamics.com/Issue/Details/?bugId=452710) | Liburuaren deskribapenaren balioa ez da zuzena proiektuaren elementuen eskakizunen ontzirako agirian.                                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [455602](https://fix.lcs.dynamics.com/Issue/Details/?bugId=455602) | Aldizkariak proiektu baten aurka argitaratzen direnean, dimentsio ekonomikoak ez dira langilearen eta bonoaren elementuen artean aukeratzen.                                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [472988](https://fix.lcs.dynamics.com/Issue/Details/?bugId=472988) | Linearen zenbateko garbia proiektuaren fakturaren guztizkoan eguneratzen denean, salmenten zenbatekoa argitaratutako transakzioan doitutako zenbatekoarekin betetzen da.                                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [477969](https://fix.lcs.dynamics.com/Issue/Details/?bugId=477969) | Fakturan ez da proiektuaren IDaren erreferentzia hautatzen saltzailearen faktura lerroak aztertzerakoan **Saltzailearen fakturak ordaintzen direnean ordaintzen dute** orrialdea.                                                                                                   |
| Proiektuaren kudeaketa eta kontabilitatea | [478667](https://fix.lcs.dynamics.com/Issue/Details/?bugId=478667) | Kontratuaren zenbatekoa ez da zuzena **Konturako** finantzaketa iturri anitz dituen prezio finko baterako proiektuaren orria.                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [481443](https://fix.lcs.dynamics.com/Issue/Details/?bugId=481443) | Prezio finkoaren proiektuan jasotako diru-sarrerak ez dira doitzen ezabaketa argitaratu ondoren ere.                                                                                                                                |
| Proiektuaren kudeaketa eta kontabilitatea | [483209](https://fix.lcs.dynamics.com/Issue/Details/?bugId=483209) | Kredituaren gutuna ez da eguneratzen proiektuaren salmenta eskaera faktura proposamen baten bidez fakturatzen denean.                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [484274](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484274) | Erosketa eskaera fakturatzen denean eta fakturak kontratazio kategoria eta elementu bat biltzen dituenean, bezeroak okerreko kontuaren informazioa jasoko du.                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [484817](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484817) | Behin-behineko aldizkako lanen bidez sortzen diren proiektuen faktura proposamenek transakzio bikoitzak dituzte zero zenbatekoarekin.                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [486817](https://fix.lcs.dynamics.com/Issue/Details/?bugId=486817) | Kendu akatsen muga egiaztatzea proiektuaren irabazien eta galeren txostenak exekutatzen ari zaren bitartean.                                                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [488076](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488076) | Enpresen arteko kargaren bidez argitaratzen diren gastuek ez dute irabazien eta galeren sarrera erakusten **Bidalketa kostuak** funtzionalitatea **Denbora eta materiala proiektuaren kodea**.                                                         |
| Proiektuaren kudeaketa eta kontabilitatea | [488382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488382) | **Fakturaren egoera** iragazkiak prezio finkoko proiektuetarako argitaratutako proiektuen transakzioetan ez du funtzionatzen.                                                                                                   |
| Proiektuaren kudeaketa eta kontabilitatea | [488783](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488783) | Ordutegiaren sarrerak bikoiztu egiten dira delegatuen erregistro bikoitzak direlako.                                                                                                                                           |
| Proiektuaren kudeaketa eta kontabilitatea | [491941](https://fix.lcs.dynamics.com/Issue/Details/?bugId=491941) | Alderantzizko kalkuluen ezabaketak ez du funtzionatzen **Aldizkakoa**.                                                                                                                                                 |
| Proiektuaren kudeaketa eta kontabilitatea | [498010](https://fix.lcs.dynamics.com/Issue/Details/?bugId=498010) | Ezin dira datu egokiak hautatu **Doitu transakzioak** **Proiektuen kudeaketa eta kontabilitatea** modulua barruti gehigarri bat gehitzen denean. **Gehigarria** iragazkia ez da kontuan hartzen.                      |
| Proiektuaren kudeaketa eta kontabilitatea | [508494](https://fix.lcs.dynamics.com/Issue/Details/?bugId=508494) | Lan bat grabatu ondoren, ezin duzu produkzio eskaeraren egoera berrezarri.                                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [509716](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509716) | Proiektu batetik datozen erreserba automatikoa eta agintzeko gai diren (CTP) elementuak ez dira erreserbatzen.                                                                                                                      |
| Proiektuaren kudeaketa eta kontabilitatea | [509773](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509773) | **Kontabilitate doikuntza** Ezaugarriak arazo bat sortzen du kontabilitate kontuekin **Ez utzi eskuz sartzea** hautatuta.                                                                     |
| Proiektuaren kudeaketa eta kontabilitatea | [510079](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510079) | Ez da balio bistaratu behar **Sarrerak irabazi - salmenten balioa** proiektuaren adierazpenen eremua estimazioa ezabatzen denean.                                                                                 |
| Proiektuaren kudeaketa eta kontabilitatea | [510607](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510607) | Kostua eta salmenta prezioak okerrak dira eginkizunen prezioarekin egindako doikuntza batean.                                                                                                                        |
| Proiektuaren kudeaketa eta kontabilitatea | [10728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=10728) | Project Operations-en, atxikipen zuzentzeko fakturak ez du funtzionatzen atxikipen zuzentze partzial baten ondoren.                                                                                                                   |
| Proiektuaren kudeaketa eta kontabilitatea | [510743](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510743) | **Kendu esteka** Aukera gaituta egon beharko litzateke enpresen arteko erosketa eskaera bat bertan behera uzten baduzu.                                                                                                                                          |
| Proiektuaren kudeaketa eta kontabilitatea | [514364](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514364) | Enpresen arteko proiektuen fakturazioko WIP salmenten balioaren argitalpenak ustekabeko kontu bat aukeratzen du.                                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [514432](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514432) | Fakturazio arau bateko kuota ez da berriro kalkulatzen faktura proposamenak kreditu oharrentzako hautatutako lerroak dituenean.                                                                                            |
| Proiektuaren kudeaketa eta kontabilitatea | [515820](https://fix.lcs.dynamics.com/Issue/Details/?bugId=515820) | Sari Federalen Kontsultaren Gastuen egutegiak ordainagiriaren zenbatekoak erakusten ditu proiektuaren faktura proposamena gastu transakzio baterako exekutatu ez denean.                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [516301](https://fix.lcs.dynamics.com/Issue/Details/?bugId=516301) | WIP kostua ez da zuzena proiektuaren adierazpenean zerbitzu bat duen **Saldoa** proiektu taldea.                                                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [516553](https://fix.lcs.dynamics.com/Issue/Details/?bugId=516553) | Ezin dira zuzenketak egin proiektuarekin lotutako testu libreko fakturari.                                                                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [517074](https://fix.lcs.dynamics.com/Issue/Details/?bugId=517074) | Proiektuaren transakzioa zero salmentako preziora egokitzen duzunean, fakturatutako egoera duen transakzio egokitu berria **Kargagabea** sortu da.                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [517414](https://fix.lcs.dynamics.com/Issue/Details/?bugId=517414) | Arazo bat dago proiektuaren doikuntza bat argitaratzerakoan aldi berean lerro ugari doitzen ari zarenean.                                                                                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [518001](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518001) | Doikuntza bat kostu kopuru oker batekin argitaratzen da, baldin eta produktuaren kostuaren prezioa eta elementuaren eskakizunaren kopurua aldatzen badira ontzirako agiria bidali ondoren.                                                                   |
| Proiektuaren kudeaketa eta kontabilitatea | [518092](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518092) | Zuzeneko entrega erosketa eskaera baten finantza neurriak okerrak dira eta salmenta eskaera finantza dimentsioek ordezkatu dituzte.                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [518605](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518605) | Kopuru negatiboaren proiektuaren egunkari lerroak ez du iragarpena eguneratuko aurreikuspen kopurua zero denean.                                                                                        |
| Proiektuaren kudeaketa eta kontabilitatea | [518657](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518657) | Elementuen eskakizunak inportatu nahian Microsoft Excel emaitzek ordainagiriaren datako errorea sortzen dute.                                                                                                                                                    |
| Proiektuaren kudeaketa eta kontabilitatea | [519200](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519200) | Saltzailearen faktura transakzioari buruzko proiektuaren transakzioaren erreferentzia ez da eguneratzen faktura argitaratzen denean.                                                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [519716](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519716) | Proiektuaren faktura proposamena argitaratzen duzunean, errore hau gerta daiteke: "Transakzioa ez da orekatzen moneta jakinaraztean kendutako faktura aurreratua gehitzen denean".                                                                    |
| Proiektuaren kudeaketa eta kontabilitatea | [520268](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520268) | Proiektuaren IDa eta Proiektuaren izena ez daude **Saltzailearen ordainketa atxikitzea** jakinarazi proiektuaren diseinua erabiltzen baduzu.                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [520872](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520872) | Proiektu bat datu-entitate baten bidez sortzen denean, liburuaren argitaratze-liburuaren lehentasuna okerra da.                                                                                                                      |
| Proiektuaren kudeaketa eta kontabilitatea | [521150](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521150) | Kostuaren zenbatekoa ez da zuzena saltzailearen atxikipena duten erosketa eskaera baten arabera sortzen diren argitaratutako proiektuen transakzioetan. Horren ondorioz proiektuaren adierazpenetan balio okerrak sortzen dira eta prezio finkoetako proiektuen kostuen kontrola. |
| Proiektuaren kudeaketa eta kontabilitatea | [521374](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521374) | Proiektuaren salmenten aurrekontuak oker eguneratzen du goiburua eguneratzen denean unitateko prezioa.                                                                                                                    |
| Proiektuaren kudeaketa eta kontabilitatea | [521807](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521807) | Project Operations-en atxikitzaileekin lan egitean, aurreordainketak fakturatu ondoren kontratuaren lehenetsitako proiektua aldatzeak sarrerako kenkariekin arazoak sortzen ditu.                                                                        |
| Proiektuaren kudeaketa eta kontabilitatea | [521857](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521857) | Saltzailearen fakturen faktura-data eguneratzea eta proiektuen salmenta-prezioak aldatu dira.                                                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [522897](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520872) | Arazoak truke-tasa desberdinak dituzten enpresen arteko transakzioak doitzen dituzunean gertatzen dira.                                                                                                                |
| Proiektuaren kudeaketa eta kontabilitatea | [522983](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522983) | Artikuluaren eskakizunarekin eta erosketa-eskaerarekin konprometitutako kostuak okerrak dira erosketa-eskaeraren faktura prozesuan produktuaren ordainagiri partzialarekin eta fakturazio partzialarekin.                                                |
| Proiektuaren kudeaketa eta kontabilitatea | [523960](https://fix.lcs.dynamics.com/Issue/Details/?bugId=523960) | Balio okerrak estimazio bat truke-tasarekin alderantzikatzen denean gertatzen dira.                                                                                                                                             |
| Proiektuaren kudeaketa eta kontabilitatea | [524242](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524242) | Orduko ahalegina automatikoki garbitzen da ataza mailan lanaren banakako egitura txantiloian.                                                                                                                         |
| Proiektuaren kudeaketa eta kontabilitatea | [524911](https://fix.lcs.dynamics.com/Issue/Details/?bugId=524911) | Aurrekontuaren egoera eguneratzen duzunean **Galdua**, hasitako komatxo guztien egoera **Sortu** edo **Bidalita** eguneratu dira **Galdua**.                 |
| Proiektuaren kudeaketa eta kontabilitatea | [525182](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525182) | Salmenten faktura ez dago faktura proposamenean ikusgai bidalketa data etorkizunean bada.                                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [526180](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526180) | Enpresa logikaren aldaketa dago **Proiektuaren item egunkariaren lerroak** entitatea.                                                                                                                                          |
| Proiektuaren kudeaketa eta kontabilitatea | [526522](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526522) | Enpresen arteko bezeroen fakturetan jasotako diru-sarrerak ez datoz bat denbora-orrialdearekin eta atzerriko moneten birbalorazioarekin.                                                                                 |
| Proiektuaren kudeaketa eta kontabilitatea | [526650](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526650) | Konpromisoko kostua gaizki kalkulatzen da proiektuaren erosketa eskaera lerroan entregatzeko abisua proiektuaren erosketa eskaera batetik edo proiektu batetik sortu ondoren.                    |
| Proiektuaren kudeaketa eta kontabilitatea | [526812](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526812) | Proiektu bat doitzen duzunean, errore hau gerta liteke, "Inbentario-unitatean ez da datu ekonomikorik eguneratzen ari".                                                                                                             |
| Proiektuaren kudeaketa eta kontabilitatea | [527319](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527319) | Project Operations-en, proiektu bat kontratu batetik kentzeak kontratuaren lehenetsitako proiektua berrezarri beharko luke, behar izanez gero.                                                                                       |
| Proiektuaren kudeaketa eta kontabilitatea | [527945](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527945) | Proiektuaren gastuaren salmenta prezioa okerra da erabilera zerga aplikatzen denean.                                                                                                                                         |
| Proiektuaren kudeaketa eta kontabilitatea | [528020](https://fix.lcs.dynamics.com/Issue/Details/?bugId=528020) | Okerreko kantitatea proiektuaren elementuaren eskakizunean agertzen da proiektuaren erosketa eskaera lerroa faktura osagarriekin eguneratzen denean.                                                                                                 |
| Proiektuaren kudeaketa eta kontabilitatea | [528212](https://fix.lcs.dynamics.com/Issue/Details/?bugId=528212) | Project Operations-en, gastu lerro okerrak erakusten dira **Gehitu lerroa** enpresa arteko fakturan zerrenda.                                                                                                |
| Proiektuaren kudeaketa eta kontabilitatea | [529887](https://fix.lcs.dynamics.com/Issue/Details/?bugId=529887) | **Saltzailearen kontua** eremua hutsik dago **Proiektuak egindako transakzioa** orria, transakzioak faktura erregistroa eta faktura onarpena erabiliz argitaratzen direnean.                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [530008](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530008) | Proiektuaren jatorrizko data ez da kontuan hartzen errore bat eragiten duen doikuntza batean **Erabili doikuntza data proiektuaren data berri gisa** **Ez** ezarrita dagoenean.                                                                     |
| Proiektuaren kudeaketa eta kontabilitatea | [530241](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530241) | Egitasmoarekin lotutako aldizkari orokorreko eta gastu-egunkariko salmenta-prezioa gaizki kalkulatzen da transakzioaren moneta konpainiaren monetatik desberdina denean.                                     |
| Proiektuaren kudeaketa eta kontabilitatea | [530658](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530658) | Salmenta transakzioak ez dira proiektuaren erosketa eskaera baten faktura partzialaren bonuak agertzen.                                                                                                                          |
| Proiektuaren kudeaketa eta kontabilitatea | [530883](https://fix.lcs.dynamics.com/Issue/Details/?bugId=530883) | Proiektuaren kontulari eta proiektuaren kudeatzaile rolek ezin dituzte ordu-aldizkariak sortu onarpen taldea konfiguratuta.                                                                                                         |
| Proiektuaren kudeaketa eta kontabilitatea | [531974](https://fix.lcs.dynamics.com/Issue/Details/?bugId=531974) | Ezin da erabili inportatutako gastuen txostena Microsoft Excel.                                                                                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [532106](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532106) | Ezin da denbora-orrien gidalerroa sortu **Mezua** eremua ez dago aktibo.                                                                                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [532548](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532548) | Arazo bat dago konpainien arteko eszenatokietan saltzailearen transakzioa aldatzea onartzen denean. Hori bai saltzailearen fakturei eta gastuen txostenei dagokie.                                                                                 |
| Proiektuaren kudeaketa eta kontabilitatea | [532692](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532692) | Onartutako ordu-orriko banaketak ezin dira berrezarri.                                                                                                                                                     |
| Proiektuaren kudeaketa eta kontabilitatea | [532843](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532843) | Balio okerrak estimazio bat alderantzikatzean orduko eta artikuluetako aldizkarien truke-tasarekin alderantzikatzean gertatzen dira.                                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [533426](https://fix.lcs.dynamics.com/Issue/Details/?bugId=533426) | Proiektuaren doikuntzak ez du salmenten zenbatekoa behar bezala eguneratzen zeharkako kostuekin.                                                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [534597](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534597) | Orduko egunkaria argitaratzean, errore mezu hau agertzen da: "Ez da zehaztu dimentsioaren balioa".                                                                                                                                  |
| Proiektuaren kudeaketa eta kontabilitatea | [535428](https://fix.lcs.dynamics.com/Issue/Details/?bugId=535428) | Beste moneta batekin egindako proiektuaren kontratuak ez du bonoan kontabilitateko moneta behar bezala kalkulatzen.                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [535652](https://fix.lcs.dynamics.com/Issue/Details/?bugId=535652) | Salmenten WIP kontu okerra konpainien arteko orri WIP argitaratzeko erabiltzen da.                                                                                                                                     |
| Proiektuaren kudeaketa eta kontabilitatea | [536536](https://fix.lcs.dynamics.com/Issue/Details/?bugId=536536) | Proiektuaren aurrekontua deskontua kalkulatzen da, beherapena aplikatzen denean eta biltegia eguneratzen denean.                                                                                                       |
| Proiektuaren kudeaketa eta kontabilitatea | [537905](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537905) | Elementu kostuen doikuntza proiektuaren transakzio batean erabili ondoren birkalkulatzea exekutatzen duzunean, errore-mezu hau agertzen da, "Akats baten ondorioz birkalkulatzea pausatzen ari da".                                                               |
| Proiektuaren kudeaketa eta kontabilitatea | [540622](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540622) | Ez da liburuki orokorreko sarrerarik sortzen fakturagarriak direnetik fakturagabeak diren diru-sarrerak pilatzerakoan.                                                                                              |
| Proiektuaren kudeaketa eta kontabilitatea | [540633](https://fix.lcs.dynamics.com/Issue/Details/?bugId=540633) | Proiektuaren saltzailearen faktura atxikitzeko funtzioak, **Gaitu kostuaren zenbatekoaren kalkulua** aktibatuta dago, **ProjTrans** ez da soldata ordaintzen denean sortzen.                                             |
| Proiektuaren kudeaketa eta kontabilitatea | [541421](https://fix.lcs.dynamics.com/Issue/Details/?bugId=541421) | Arazo ugari daude **Sortu faktura proposamena** orrialdea.                                                                                                                                                     |
| Proiektuaren kudeaketa eta kontabilitatea | [543968](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543968) | Project Operations-en **Erosketa-hitzarmena** orria ez dago ikusgai Project Operations-ekin integratuta dauden Finantza entitate juridikoetan.                                                                                             |
| Proiektuaren kudeaketa eta kontabilitatea | [544132](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544132) | Aldizkari aurreratuak ezin dira kontabilitate-data batekin itxita egon, nahiz eta **Ezarri automatikoki kontabilitate data irekitako hurrengo aldira** aukera aktibatuta dago.                                                |
| Proiektuaren kudeaketa eta kontabilitatea | [545878](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545878) | Dataverse integrazioaren errore bat dagoelako, ezin duzu aurrekontua irabazi bihurtu Project Operations-en.                                                                                                                                       |
| Proiektuaren kudeaketa eta kontabilitatea | [546604](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546604) | Project Operations-en, errore-mezu bat gertatzen da kontratu-lerroa proiektuaren IDarekin lotzen saiatzen zarenean, kontratu-lerroak eta transakzio motak gainjartzen diren egiaztatzeagatik.                                                |
| Proiektuaren kudeaketa eta kontabilitatea | [547440](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547440) | **ProjCDSProjectContractEntity** beste bezero baten finantziazio iturriaren faktura helbidea ezar dezake.                                                                                                             |
| Proiektuaren kudeaketa eta kontabilitatea | [547606](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547606) | Baliabideen orrialdeetako bilaketa estandarra ez dago eskuragarri 10.0.15 eguneratu ondoren.                                                                                                                    |
| Proiektuaren kudeaketa eta kontabilitatea | [547831](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547831) | Liburu-kontua eta bidalketa mota okerrak dira liburu nagusiko bonuan eta bidalketa mota okerra da stock gabeko zerbitzu-elementu baten erosketa-eskaeraren bonuan proiektu-taldea ezarrita dagoenean **Saldoa**.                                 |
| Proiektuaren kudeaketa eta kontabilitatea | [550030](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550030) | Jardueraren zenbakia ez da saltzaileen faktura pendiente batean agertzen, nahiz eta **Blokeatu gurasoen jarduera hautatzea** Ezarrita dago                                                                    |
| Proiektuaren kudeaketa eta kontabilitatea | [557376](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557376) | Project Operations-en, ez da dimentsiorik hautatzen transakzio baten fakturazio bat bidaltzen duzunean.                                                                                                                   |
| Proiektuaren kudeaketa eta kontabilitatea | [442814](https://fix.lcs.dynamics.com/Issue/Details/?bugId=442814) | Proiektuen kudeaketan eta kontabilitatean, transferentziaren prezioaren lehentasuna ez da zehazki islatzen enpresen arteko orrietan.                                                                            |
| Proiektuaren kudeaketa eta kontabilitatea | [533530](https://fix.lcs.dynamics.com/Issue/Details/?bugId=533530) | Oinarrizko lanaren banaketa egitura (WBS) klase metodoa, **ProjWBSUpdateController::updateOutlineNumbersAndPublishInPreOrder** zaharkituta dago.                                                                                                   |

### <a name="regulatory-updates"></a>Araudiaren eguneratzeak
Eguneratze arautzaileei buruzko informazioa lortzeko Finance and Operations aplikazioak, ikusi [Araudiaren eguneratzeak](https://docs.microsoft.com/dynamics365/finance/localizations/regulatory-updates). LCS-en saioa hasi eta aurreikusitako arauzko eguneratzeak ikus ditzakezu Arazoak bilatzeko tresna erabiliz. Arazoen bilaketak herrialdearen, eginbide motaren eta askapenaren arabera bilatzeko aukera ematen du.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]