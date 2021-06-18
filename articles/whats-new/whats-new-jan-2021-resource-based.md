---
title: 2021eko urtarrileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Gai honek informazioa eskaintzen du 2021eko urtarrilean Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruz, baliabideetan / stockean oinarritutako egoeretarako.
author: sigitac
ms.date: 01/13/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c600c30acd5e07e6370459928e33033a6ba418d6
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995741"
---
# <a name="whats-new-january-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko urtarrileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

  - Project Operations Dataverse ingurunearen 4.6.0.154 bertsioa
  - Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.16 bertsioa

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| **Inplementazioa eta konfigurazioa** | 2106818 | Orrialde bat pertsonalizatzearekin lotutako arazoak sortzen ari zen web baliabidearen izena aldatu zen. |
| **Fakturazioa eta prezioak** | 2091908 | Fitxategiaren ikusgaitasuna konpondu da **Blokeatu prezioak** eta **Erabili uneko prezioak** aukerak **Faktura** orrialdea Project Operations Dynamics 365 Field Service-rekin batera instalatzen denean. |
| **Fakturazioa eta prezioak** | 2103058 | Freskatutako **Proiektuaren guztirakoak** zeregin batean benetako kostuaren balio baliogarriak kudeatzeko. |
| **Fakturazioa eta prezioak** | 2116100 | Funtzionaltasunarekin erabilitako errore mezuak hobetu dira, **Zuzendu sarrera egunkarietan**. |
| **Fakturazioa eta prezioak** | 2116129 | Gastuen hobekuntzak ikusgarritasuna kalkulatzen du **Aurrekontuak** fitxan **Proiektuak** orrialdean. |
| **Fakturazioa eta prezioak** | 2119112 | Benetako salmenten eta benetako kostuaren batuketa finkoa truke-tasa desberdinak erabiltzen direnean. |
| **Fakturazioa eta prezioak** | 2134705 | Akatsa konpondu da "Ezin da propietatea irakurri **getResourceString** "zehaztu gabeko" **Faktura** orria ireki eta Field Service instalatuta dago. |
| **Abaguneen kudeaketa** | 2022195 | Zereginetan oinarritutako fakturazio sareta **Proiektua** orrialdeak zeregin horrekin loturiko kontratu edo aurrekontu lerroa dagoela adierazten duen ikonoa dauka. |
| **Abaguneen kudeaketa** | 2029135 | Erabiltzaile batek fakturatutako lerro bat irekitzen ahalegintzen denean fakturatutako linea aurreratua duen faktura berretsi batean gertatzen den negozio-prozesuko errorea konpondu da. |
| **Abaguneen kudeaketa** | 2040713 | Kontratu batetik faktura bat sortzerakoan gertatzen den script errorea konpondu da eta Field Service instalatuta dago. |
| **Proiektuaren antolaketa eta jarraipena** | 2090202 | Jada erabiltzen ez diren negozio-arauak **Zaharkituta** gisa markatuta. |
| **Denbora eta gastua** | 2091249 | Estutu kontrolak erabiltzaileek zeregina ezin aldatzeko bidalitako edo onartutako denbora-sarrera batean. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Dynamics 365 Finance-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| **Proiektuaren kudeaketa eta kontabilitatea** | [478667](https://fix.lcs.dynamics.com/Issue/Details/?bugId=478667) | Kontratuaren zenbateko okerra **Kontuan** finantzaketa iturri anitz dituen prezio finko baterako proiektuaren orria. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [480260](https://fix.lcs.dynamics.com/Issue/Details/?bugId=480260) | **Faktura-proposamena.PSAnfRefProjId** leku-markak ez du proiektuaren IDa erakusten lan-fluxurako, **Proiektuen fakturen proposamenak berrikusi**. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [481227](https://fix.lcs.dynamics.com/Issue/Details/?bugId=481227) | Eskudirua deskontatzeko data okerra erabiltzen da proiektuaren fakturen proposamenak argitaratzerakoan. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [482558](https://fix.lcs.dynamics.com/Issue/Details/?bugId=482558) | Project Operations-en baliabideen esleipenak kendu eta irakurtzeak bikoiztu egiten ditu proiektuen aurreikuspenen sarrerak Finance-n. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [484468](https://fix.lcs.dynamics.com/Issue/Details/?bugId=484468) | Project Operations-en, ezin duzu proiektuaren kalkuluak sortu Dataverse-n proiektuan kontratu linearik izan gabe. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [485871](https://fix.lcs.dynamics.com/Issue/Details/?bugId=485871) | Proiektuaren gastuen transakzioaren dimentsio finantzarioa ez dago erlazionatutako bonuarekin eta gastuen txostenaren kontabilitate banaketarekin kostuak Saldoan kontabilizatzen direnean. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [488382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488382) | Prezio finkoetarako proiektuen transakzioetan **Fakturatutako egoera** iragazkiak ez du funtzionatzen. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [491941](https://fix.lcs.dynamics.com/Issue/Details/?bugId=491941) | Alderantzizko kalkuluen ezabaketak ez du funtzionatzen **Aldizkakoa** atala. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [509989](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509989) | Faktura proposamenen lerroak ezaba daitezke Project Operations-en Dataverse-rekin integratzean. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [510041](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510041) | Saihestu kontratu lerro anitzen eginbidea gaitzea Dataverse integraziorik gabe. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [510527](https://fix.lcs.dynamics.com/Issue/Details/?bugId=510527) | Kontuko fakturazioa irabazien eta galeren berdina denean, fakturatutako diru sarrerak zero gisa azaltzen dira Aurrekontuak orrialdea. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [514167](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514167) | Fakturen zuzenketak ez dira funtzionatzen ingurune integratuetan. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [514364](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514364) | Enpresen arteko proiektuen fakturazioko WIP salmenten balioa argiataatzean, kontu okerra aukeratzen da. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [514385](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514385) | Project Operations-en, estimazioko atazen mendekotasunak Dataverse-n ezin da eguneratu. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [515258](https://fix.lcs.dynamics.com/Issue/Details/?bugId=515258) | Finantzetan Project Operations integrazio aldizkariak behin eta berriro ezabatzeak datuen galera dakar. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [519716](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519716) | Proiektuaren faktura proposamen bat argitaratzean errore hau gertatzen da: "Transakzio bat ez da orekatzen txosteneko monetan kendutako faktura aurreratua berriro gehitzen denean". |
| **Proiektuaren kudeaketa eta kontabilitatea** | [521807](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521807) | Proiektuaren ID okerra sartzen da kenketetan, lehenetsitako proiektuaren kontratua Project Operations-en eguneratu ondoren. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [522799](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522799) | Aurrekontua eta diru-sarreren aitorpena ezin dira osatu Project Operations gaituta dagoenean. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [527319](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527319) | Project Operations-en, proiektu bat kontratu batetik kentzeak ez du kontratuko lehenetsitako proiektua berrezarri. |
| **Proiektuaren kudeaketa eta kontabilitatea** | [528212](https://fix.lcs.dynamics.com/Issue/Details/?bugId=528212) | Project Operations-en, enpresen arteko fakturan, okerreko gastu lerroak agertzen dira **Gehitu lerroa** zerrenda. |
| **Bidaia eta gastua** | [515334](https://fix.lcs.dynamics.com/Issue/Details/?bugId=515334) | Gastu lerroak ezin dira argitaratu kontratu lerroan ordu konfigurazioa falta delako. |
| **Bidaia eta gastua** | [437673](https://fix.lcs.dynamics.com/Issue/Details/?bugId=437673) | Proiektua / kategoria baliozkotzea derrigorrezkoa denean, proiektuarekin lotutako gastuen kategoriak ez dira gastuen txostenean ikusgai. |
| **Bidaia eta gastua** | [441256](https://fix.lcs.dynamics.com/Issue/Details/?bugId=441256) | Diru-aurrerakinaren saldoa ez da eguneratzen gastuen txostena lerro bidez argitaratzen denean. |
| **Bidaia eta gastua** | [465396](https://fix.lcs.dynamics.com/Issue/Details/?bugId=465396) | **Eguneratu ordainketaren informazioa** lanak huts egiten du fakturak ordainketa bi transakzio edo gehiagorekin likidatu diren likidazioak alderantzikatu ondoren. |
| **Bidaia eta gastua** | [472892](https://fix.lcs.dynamics.com/Issue/Details/?bugId=472892) | Arazo bat izan da azken eguneko otordua murrizteko kalkuluarekin arazoa eguneko gastu kategorian. |
| **Bidaia eta gastua** | [477714](https://fix.lcs.dynamics.com/Issue/Details/?bugId=477714) | **Langile bakoitzeko gastu mota** txostenak ez ditu gastu xehatuak erakusten erabiltzailearen lehen konexioa es-MX hizkuntzan izan bada. |
| **Bidaia eta gastua** | [487516](https://fix.lcs.dynamics.com/Issue/Details/?bugId=487516) | Saltzaileak gastuen txostenaren faktura baten ordainketa okerreko laburpen-kontua erabiltzen ari da likidazioa argitaratzeko. |
| **Bidaia eta gastua** | [487531](https://fix.lcs.dynamics.com/Issue/Details/?bugId=487531) | Urtean argitaratutako gastuen txostena **Baimendu ordainketen ordainketa-kontuan oinarritutako transakzioen multzokatzea** eta **Kontabilitate data zuzentzea argitaratzean** aukerekin gaituta dagoenean, kontabilitate datak ez daude taldean **Kontabilitate banaketa** taula, salmenten gaineko zergen erregistroetan eragina duena. |
| **Bidaia eta gastua** | [488292](https://fix.lcs.dynamics.com/Issue/Details/?bugId=488292) | Gastuen azpikategoriaren mapaketa kendu egiten da Erabilera gastuan kontrol laukia garbitu eta berriro hautatuko da. |
| **Bidaia eta gastua** | [506175](https://fix.lcs.dynamics.com/Issue/Details/?bugId=506175) | Enpresen arteko gastuen txostena ezin da sortu proiektuaren IDa goiburuko mailan gehitzen bada. |
| **Bidaia eta gastua** | [509491](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509491) | Gastuen ordainketekin arazo bat izan da, gastuaren zenbatekoa dirua aurreratzea baino handiagoa denean. |
| **Bidaia eta gastua** | [509556](https://fix.lcs.dynamics.com/Issue/Details/?bugId=509556) | Enpresen arteko gastuen txosteneko **Proiektuaren IDa** eremua hutsik dago erabiltzailearen rola erakunde jakin bati esleitzen bazaio. |
| **Bidaia eta gastua** | [518186](https://fix.lcs.dynamics.com/Issue/Details/?bugId=518186) | Gastu kategoria blokeatuta dago gastu lerro berria gehitzean. |
| **Bidaia eta gastua** | [520914](https://fix.lcs.dynamics.com/Issue/Details/?bugId=520914) | Jadanik zatituta dauden gastuen txostenen lerroak zehaztuz gero, osatu gabeko kontuak ordaindu behar dira \ Liburu orokorreko bonua. **TRVEXPTRANS.SOURCEDOCUMENTLINE** parametroa bikoiztuta dagoelako, Kontabilitate-iturriaren esploratzailea ere hautsita dago. |
| **Bidaia eta gastua** | [521768](https://fix.lcs.dynamics.com/Issue/Details/?bugId=521768) | Bezeroak bikoiztuak dituen **TRVREQUISITIONLINE** taulan gehitutako aurkibideak errore bat sortzen du bertsio berritzean. |
| **Bidaia eta gastua** | [525106](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525106) | Project Operations-en, denbora enpresen arteko zereginetan Dataverse ezin da sortu edo onartu. |

## <a name="regulatory-updates"></a>Araudiaren eguneratzeak

Eguneratze arautzaileei buruzko informazioa lortzeko Finance and Operations aplikazioak, ikusi [Araudiaren eguneratzeak](/dynamics365/finance/localizations/regulatory-updates). LCS-en saioa hasi eta aurreikusitako arauzko eguneratzeak ikus ditzakezu Arazoak bilatzeko tresna erabiliz. Arazoen bilaketak herrialdearen, eginbide motaren eta askapenaren arabera bilatzeko aukera ematen du.


[!INCLUDE[footer-include](../includes/footer-banner.md)]