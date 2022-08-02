---
title: 2021eko apirileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Artikulu honek Project Operations-en 2021eko apirileko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du baliabideetan edo hornituta ez dauden agertokietarako.
author: sigitac
ms.date: 04/22/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 490b7aa38bfdfbcdce21a21e582296e4ce15aeeb
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029233"
---
# <a name="whats-new-april-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko apirileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu hau honako hauei aplikatzen zaie Dynamics 365 Project Operations osagaiak eta bertsioak:

- Project Operations Dataverse ingurunearen 4.9.0.221 bertsioa
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.17 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- Proiektuetarako materialik gabeko materiala. Gaitasun nagusiak honako hauek dira:
  - Proiektu baten salmenta-zikloan stockik gabeko materialak kalkulatzea eta preziatzea. Informazio gehiago lortzeko, ikusi [Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak - arina](../pro/pricing-costing/set-up-cost-sales-rates-catalog-products.md).
  - Biltegiratu gabeko materialen erabileraren jarraipena egitea proiektuaren entrega garaian. Informazio gehiago lortzeko, ikusi [Erregistratu proiektuetako eta proiektu-zereginetako material-erabilera](../material/material-usage-log.md).
  - Erabilitako materialik gabeko kostuen fakturazioa. Informazio gehiago lortzeko, ikusi [Kudeatu fakturazio atzeratua](../proforma-invoicing/manage-billing-backlog.md).
  - Ezaugarri hau nola konfiguratu jakiteko, ikusi [Konfiguratu ez dauden materialak eta zain dauden saltzailearen fakturak](../procurement/configure-materials-nonstocked.md)
- Zereginetan oinarritutako fakturazioa: proiektuaren zereginak proiektuko kontratu lerroekin lotzeko gaitasuna gehitu zen eta, horrela, fakturazio metodo, faktura maiztasun eta kontratu lerroan dauden bezero berberak ezarriko zaizkie. Elkarte honek fakturazio zehatza, kontabilitatea, diru-sarreren estimazioa eta aitorpena bermatzen ditu proiektuaren zereginetan konfigurazio honen arabera lan egiteko.
- API berriak Dynamics 365-en Dataverse baimendu eragiketak sortu, eguneratu eta ezabatzearekin **Programazio entitateak**. Informazio gehiagorako, ikusi [Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko](../project-management/schedule-api-preview.md).

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo zerrendan 2021eko apirileko Project Operations aldatu edo gehitu diren idazketa bikoitzeko mapak agertzen dira.

| **Entitate-esleipena** | **Eguneratutako bertsioa** | **Iruzkinak** |
| --- | --- | --- |
| Project Operations-en integrazioaren benetako datuak (msdyn\_actuals) | 1.0.0.14 | Mapa aldatu da proiektuaren egiazkoak sinkronizatzeko. |
| Project Operations-ek integratzeko entitatea gastuen kalkuluen arabera (msdyn\_estimateslines) | 1.0.0.2 | Proiektu-kontratu-lerroen sinkronizazioa gehitu da finantza- eta eragiketa-aplikazioetan zereginetan oinarritutako fakturazio-laguntzarako. |
| Project Operations-ek integratzeko entitatea orduen kalkuluen arabera (msdyn\_resourceassignments) | 1.0.0.5 | Proiektu-kontratu-lerroen sinkronizazioa gehitu da finantza- eta eragiketa-aplikazioetan zereginetan oinarritutako fakturazio-laguntzarako. |
| Project Operations integrazioaren taula materialen kalkuluen arabera (msdyn\_estimatelines) | 1.0.0.0 | Taula-mapa berria materialaren estimazioak sinkronizatzeko Dataverse finantzaketa eta eragiketa aplikazioetarako. |
| Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn\_projectvendorinvoices) | 1.0.0.0 | Taula-mapa berria saltzaileen fakturen goiburuak finantza eta eragiketa aplikazioetatik sinkronizatzeko Dataverse. |
| Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn\_projectvendorinvoicelines) | 1.0.0.0 | Taula-mapa berria saltzaileen faktura-lerroak finantza- eta eragiketa-aplikazioetatik sinkronizatzeko Dataverse. |

Beti exekutatu behar duzu maparen azken bertsioa zure ingurunean eta erlazionatutako taula-mapa guztiak gaitu zure Proiektuaren Eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta finantza eta eragiketen irtenbidearen bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktiba dezakezu hautatuta **Taula maparen bertsioak**, azken bertsioa hautatuta, eta ondoren hautatutako bertsioa gorde. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa Dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-in-dynamics-365-dataverse"></a>Project Operations Dynamics 365 Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2124532 | **Faktura zuzena** botoia proforma fakturan bistaratzen da atxikipenaren zenbatekoa edo aplikatutako atxikipenaren zenbatekoa jatorrizko fakturan agertzen denean. Botoia Finantza 10.0.19 bertsioa edo berriagoa duten inguruneetan bakarrik bistaratzen da. |
| Fakturazioa eta prezioak | 2224568 | Gehitu da logika fakturaren baieztapen plugina deitzea dakarten pertsonalizazioak gaitzeko. |
| Fakturazioa eta prezioak | 2101098 | Eremu lehenetsien logika hobetu da proforma fakturan: **Fakturaziorako helbidea**, **Izena faktura** eta **Ordainketa baldintzak** orain dagokion proiektuaren kontratuaren bezeroaren erregistroa lehenetsita dago. |
| Fakturazioa eta prezioak | 2021413 | Eguneratu da **Benetako kostua** eta **Salmentak** eremuak **Egitekoa** entitateak fakturatutako eta fakturatutako gastuen salmenten balioak sartzeko zereginetan. |
| Fakturazioa eta prezioak | 2182110 | Proiektuaren kontratua kopiatzerakoan, kontratu lerroaren IDa helmugako proiektuaren kontratuan birsortzen da bakarra dela ziurtatzeko. |
| Abaguneen kudeaketa | 2186741 | Gehitu balidazioak ziurtatzeko **Jatorria** eremua eta **Transakzio mota** ezin da eguneratu aurrekontuaren lerroaren xehetasunetan. |
| Abaguneen kudeaketa | 2191353 | Mugarriak ez dira denbora eta material kontratu lerro batean sortu behar. |
| Abaguneen kudeaketa | 2216956 | Arazoak konpondu dira **Eguneratu prezioak**. |
| Antolaketa eta jarraipena | 2182979 | Proiektuaren kopia funtzioa hobetu da, gastuen estimazio lerroak jatorrizko proiektuaren kopiatuko direla ziurtatzeko. |
| Antolaketa eta jarraipena | 2184144 | Proiektuaren kopia funtzioa hobetu da, baliabidearen posizioaren izena jatorrizko proiektuaren kopiatuko dela ziurtatzeko. |
| Antolaketa eta jarraipena | 2184799 | Proiektuaren kopia: kontrol estua, aurreikusitako hasiera-data aldatu ezin dela ziurtatzeko, kopia egiten ari den bitartean. |
| Antolaketa eta jarraipena | 2185134 | Proiektuaren kopia: Helmugako proiektuaren hasierako data gaurko egunean ezarrita dago. |
| Antolaketa eta jarraipena | 2196373 | Proiektuaren kopia: ziurtatu proiektuaren zuzendaria eta taldekideen erregistroak ez direla proiektuan taldean bikoizten. |
| Antolaketa eta jarraipena | 2211833 | Proiektuaren kopia: baliabideen esleipenak jatorrizko proiektuaren zereginetik helmugako proiektuan kopiatzen dira. |
| Antolaketa eta jarraipena | 2186541 | Arazoak konpondu dira **Aurrekontuak** sareta baliabideen arabera multzokatzean. |
| Antolaketa eta jarraipena | 2166906 | Ataza bateko transakzio kategoria fitxategian kopiatu behar da **Baliabideen esleipena** entitatea. |
| Baliabideen kudeaketa | 2125362 | Taldekide generiko bat sortzerakoan arazoak konpondu dira orduetan oinarritutako esleipen metodoaren bidez. |
| Denbora eta gastua | 2113603 | Pertsonalizazioarekin lotutako arazoa konpondu da **Denbora-sarrera** orrialdea. Sistemak orain atributua orrian dagoen egiaztatzen du script horietara sartu aurretik. |
| Denbora eta gastua | 2204377 | Kopiatutako ordu-orriak automatikoki erakutsi behar dira hautatzen duzunean **Kopiatu astea** denbora sartzean. |
| Denbora eta gastua | 2209059 | **Egoera** eremua editatu daiteke Dynamics 365 Field Service denbora sarrerak. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance-en

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [491941](https://fix.lcs.dynamics.com/Issue/Details/?bugId=491941) | Alderantzizko kalkuluen ezabaketak ez du funtzionatzen **Aldizkakoa** atala.  |
| Proiektuaren kudeaketa eta kontabilitatea | [509773](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509773) | **Kontabilitate doikuntza** Ezaugarriak arazo bat sortzen du kontabilitate kontuekin **Ez utzi eskuz sartzea** hautatuta. |
| Proiektuaren kudeaketa eta kontabilitatea | [510728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=5109728) | Enpresa logika gehitu da zuzenketa fakturak prozesatzeko, atxikipenaren zenbatekoa edo aplikatutako atxikipenaren zenbatekoa barne. |
| Proiektuaren kudeaketa eta kontabilitatea | [514364](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514364) | Enpresen arteko proiektuen fakturazioko WIP salmenten balioaren argitalpenak ustekabeko kontu bat aukeratzen du. |
| Proiektuaren kudeaketa eta kontabilitatea | [521807](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521807) | Project Operations-en atxikitzaileekin lan egitean, aurreordainketak fakturatu kontratuaren lehenetsitako proiektua aldatzeak sarrerako kenkariekin arazoak sortzen ditu. |
| Proiektuaren kudeaketa eta kontabilitatea | [527319](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527319) | Project Operations-en, proiektu bat kontratu batetik kentzeak kontratuaren lehenetsitako proiektua berrezarri beharko luke, behar izanez gero. |
| Proiektuaren kudeaketa eta kontabilitatea | [528212](https://fix.lcs.dynamics.com/Issue/Details/?bugId=528212) | Project Operations-en, gastu lerro okerrak erakusten dira **Gehitu lerroa** enpresa arteko fakturan zerrenda. |
| Proiektuaren kudeaketa eta kontabilitatea | [543968](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543968) | Project Operations-en **Erosketa-hitzarmena** orria ez dago ikusgai Project Operations-ekin integratuta dauden Finantza entitate juridikoetan. |
| Proiektuaren kudeaketa eta kontabilitatea | [545878](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545878) | Dataverse integrazioaren errore bat dagoelako, ezin duzu aurrekontua irabazi bihurtu Project Operations-en. |
| Proiektuaren kudeaketa eta kontabilitatea | [547440](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547440) | **ProjCDSProjectContractEntity** beste bezero baten finantziazio iturriaren faktura helbidea ezar dezake.  |
| Proiektuaren kudeaketa eta kontabilitatea | [557376](https://fix.lcs.dynamics.com/Issue/Details/?bugId=557376) | Project Operations-en, ez da dimentsiorik hautatzen transakzio baten fakturazio bat bidaltzen duzunean. |
| Bidaia eta gastua | [441256](https://fix.lcs.dynamics.com/Issue/Details/?bugId=441256) | Diru-aurrerakinaren saldoa ez da eguneratzen gastu-txosten baterako, lineaz lerro onartzen bada eta argitaratzen bada. |
| Bidaia eta gastua | [482041](https://fix.lcs.dynamics.com/Issue/Details/?bugId=482041) | Enpresen arteko gastuen txosten zehatzen zergak ez dira behar bezala kalkulatzen. |
| Bidaia eta gastua | [483469](https://fix.lcs.dynamics.com/Issue/Details/?bugId=483469) | Proiektuekin lotutako eremu osagarriak berriro imajinatzen dira **Enpresen arteko gastuen txostenak** orrialdea. |
| Bidaia eta gastua | [486592](https://fix.lcs.dynamics.com/Issue/Details/?bugId=486592) | Okerreko mezu bat gertatzen da gastuen txostenen goiburuko ordainagirietan. |
| Bidaia eta gastua | [487971](https://fix.lcs.dynamics.com/Issue/Details/?bugId=487971) | Gastuen txostena gaizki argitaratzen da enpresen arteko agertokian salmenten gaineko zerga helmugako pertsona juridikoari bidaltzen bazaio. |
| Bidaia eta gastua | [505696](https://fix.lcs.dynamics.com/Issue/Details/?bugId=505696) | Txostenak bidaltzeko datak ez daude onartutako gastuen txostenetan inprimatuta. |
| Bidaia eta gastua | [508726](https://fix.lcs.dynamics.com/Issue/Details/?bugId=508726) | **Onartutako data** eta **Baztertutako data** eremuak ez dira betetzen gastu bat onartu ondoren. |
| Bidaia eta gastua | [509913](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509913) | Langile batek sortutako bidaia eskaera beste langile baten gastuen txostenean erabil daiteke. |
| Bidaia eta gastua | [518186](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518186) | Gastu kategoriak blokeatuta daude gastu lerro berria gehitzean. |
| Bidaia eta gastua | [520914](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520914) | Dagoeneko zatitutako gastuen txosten lerroak zerrendatzeak Ordaindu beharreko kontuak \ Liburu Nagusiaren bonua argitaratzea osatu gabe lortzen du eta Kontabilitate Iturriaren arakatzailea hausten duelako **TRVEXPTRANS.SOURCEDOCUMENTLINE** bikoiztu egiten da. |
| Bidaia eta gastua | [521943](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521943) | Bidaia eskatzeko gidalerroak ez du espero bezala funtzionatzen. |
| Bidaia eta gastua | [522567](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522567) | Saltzailearen kontuaren izena ez da argitaratutako proiektuaren transakzioetan agertzen gastuen txostenetarako. |
| Bidaia eta gastua | [525106](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525106) | Project Operations-en, ezin duzu denbora onartu enpresen arteko proiektu baterako zeregin batekin. |
| Bidaia eta gastua | [526336](https://fix.lcs.dynamics.com/Issue/Details/?bugId=526336) | Dirua aurreratzeko itzulketaren kategoria ez da dirua aurreratzeko saldoak eguneratzen argitaratutakoan. |
| Bidaia eta gastua | [527218](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527218) | Salmenta-prezioa gaizki kalkulatzen da inportatutako kreditu txartelarekin egindako transakzioen bidez atzerriko monetan sortu ziren eta proiektu batekin lotutako gastuen txostenetan. |
| Bidaia eta gastua | [542927](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542927) | Leheneratu **TrvRequisitionLine** datu-entitatea eta lotutako indize bakarra. |
| Bidaia eta gastua | [543239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543239) | Tresneria gehitu da **SOURCEDOCUMENTLINE** belaunaldia. |
| Bidaia eta gastua | [544323](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544323) | Azpiliburu nagusi okerra erakusten da enpresen arteko agertokian salmenten gaineko zerga helmugako pertsona juridikoari bidaltzen bazaio. |
| Bidaia eta gastua | [546877](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546877) | Project Operations-en, gastuen kalkuluak ez dira Finantzatik ezabatzen, ezabatzen direnean Dataverse. |
| Bidaia eta gastua | [550575](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550575) | Gastu kategoria proiektua ez den kategoria bat denean, **Gastua** orria ez da gastuen txostenean kopiatzen. |
