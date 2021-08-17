---
title: 2021eko maiatzeko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Gai honek 2021eko maiatzeko Project Operations bertsioan baliabideetan/izakinik gabekoetan oinarritutako agertokietarako eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 26d4d9feb386075fec2b5c0854e0762604a74d36c90068e35d351e52d95165d4
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994666"
---
# <a name="whats-new-may-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko maiatzeko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dynamics 365 Dataverse inguruneko bertsioa 4.10.0.186
- Proiektuen kudeaketa eta kontabilitatea Finance and Operations aplikazioen inguruneak 10.0.18 bertsioa

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- [Programazio moduak](../project-management/scheduling-modes.md): Proiektuen kudeatzaileek proiektu bat iraupen finkoa, lan finkoa edo unitate finkoen programazio modua erabiliz kudeatu behar den zehaztu dezakete.
- [Konfiguratu kilometrajea kilometrajearen tasaren mailak erabiliz](../expense/set-up-mileage.md): Eguneratu kilometrajearen tasa mailak langileen gastuen txostenetarako.

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo zerrendan 2021eko maiatzeko Project Operations aldatu edo gehitu diren idazketa bikoitzeko mapak agertzen dira.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| --- | --- | --- |
| Proiektua finantzatzeko iturria (msdyn\_projectcontractsplitbillingrules) | 1.0.0.2 | Proiektuaren kontratuaren bezeroaren ordainketa baldintzak sinkronizatzea. |
| Proiektuaren faktura-proposamena V2 (fakturak) | 1.0.0.3 | Proforma fakturaren ordainketa baldintzak sinkronizatzea. |
| Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn\_projectvendorinvoicelines) | 1.0.0.1 | Kalitatearen eguneratzeak |
| Proiektuak V2 (msdyn\_projects) | 1.0.0.2 | Kalitatearen eguneratzeak |

Maparen azken bertsioa beti zure ingurunean exekutatu behar duzu eta erlazionatutako taulako mapa guztiak gaitu Project Operations eguneratzen dituzunean Dataverse konponbidea eta Finance and Operations aplikazioen irtenbide bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management.md).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades.md#missing-table-columns-issue-on-maps) Idazketa Dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2227635 | Fitxategiko balioak **Unitate taldea** eta **Unitatea** eremuak lehenetsitako produktuan **Materialen aurrekontuak** sareta. |
| Fakturazioa eta prezioak | 2234127 | **Ataza IDa** eremua orain ondo integratzen da Dataverse proiektuaren egileak saltzailearen faktura argitaratzen denean. |
| Fakturazioa eta prezioak | 2235564 | Aldizkariaren lerroa gordetzean, egunkariaren lerroan agertzen den moneta moneta lehenetsia lerroarekin bat datorrela ziurtatzen da gorde ondoren. |
| Fakturazioa eta prezioak | 2246671 | Fakturazioan transakzio bat kobratu gabe egiteak jatorrizko fakturazio gabeko salmenten erregistroa alderantzikatzen du eta fakturatu gabeko salmenten erregistro berria sortzen du kobratu gabe. |
| Fakturazioa eta prezioak | 2264042 | Faktura zuzenketa zuzena ez da blokeatu behar ingurunean baliozkoa ez den faktura zuzentzeko xehetasunik badago. |
| Fakturazioa eta prezioak | 2146367 | Proiektuaren fakturen goiburua idazketa bikoitzeko mapak ordainketa baldintzak barne hartzen ditu. |
|   Abaguneen kudeaketa | 2086888 | Ez gehitu aurrekontua kopiatu aurretik desaktibatuta dauden rolak eta kategoriak kopiatu berri den aurrekontuaren kargagarriak diren rol eta kategorietan. |
|   Abaguneen kudeaketa | 2234376 | Irakurtzeko soilik diren eremuak grisean daude **Materialen aurrekontuak** sareta. |
|   Abaguneen kudeaketa | 2238337 | Kontaktu batean oinarritutako aurrekontua gorde daiteke proiektuaren prezioen zerrendarekin lotzen ez bada ere. |
|   Abaguneen kudeaketa | 2239810 | Aurrekontua galdu ahala ixteak lotutako proiektua itxi eta erreserbak bertan behera uzten ditu. |
| Proiektuaren antolaketa eta jarraipena | 2099559 | Sistemaren osasunaren baliozkotzeak gehitu dira **Proiektuaren zereginak** sareta irekitzen da. |
| Proiektuaren antolaketa eta jarraipena | 2178987 | Aukeratzean gertatzen zen errore iragankorra konpondu zen **Hurrengo etapa** **Proiektua** orrialdean. |
| Baliabideen kudeaketa | 2224817 | Erreserbak luzatzeko funtzionaltasunak lehenespenez erreserba-egoera zuzena du. |
| Denbora-sarrera | 2202476 | **Denbora Sarrera** orrialdeak orain erreakzionatzeko sarearen kontrola erabiltzen du eta saretaren lerrokatzea kentzea bezalako arazoak konpontzen ditu. |
| Denbora-sarrera | 2223377 | Denbora sarrera ezkutatuta dago **Lotua** atala **Erreserbatzeko Baliabidea** orrialdea erabilgarritasunarekin nahastea ekiditeko. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Dynamics 365 Finance-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [545878](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545878) | Egoeretan oinarritutako baliabideen Project Operations: ezin duzu aurrekontua irabazi integrazio-errore bat dela-eta. |
| Proiektuaren kudeaketa eta kontabilitatea | [546604](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546604) | Project Operations: errore-mezu bat gertatzen da kontratu-lerroa Proiektuaren IDarekin lotzen saiatzen zarenean, kontratu-lerroak eta transakzio motak gainjartzen diren egiaztatzeagatik. |
| Proiektuaren kudeaketa eta kontabilitatea | [547440](https://fix.lcs.dynamics.com/Issue/Details/?bugId=547440) | **ProjCDSProjectContractEntity** beste bezero baten finantzazio iturriaren faktura helbidea ezartzen ditu. |
| Bidaia eta gastua | [480451](https://fix.lcs.dynamics.com/Issue/Details/?bugId=480451) | Kilometrajearen konfigurazioarekin lotutako errore bat gerta daiteke. |
| Bidaia eta gastua | [522084](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522084) | **Banatu pertsonalera** funtzionalitateak ez du funtzionatzen atzerriko monetan gastuen transakzioetarako. |
| Bidaia eta gastua | [523938](https://fix.lcs.dynamics.com/Issue/Details/?bugId=523938) | Gastuen kategoria goitibeherako balioek kategoria okerrak erakusten dizkie ordezkariei, baliabideak dauden kontuan hartu gabe. |
| Bidaia eta gastua | [539266](https://fix.lcs.dynamics.com/Issue/Details/?bugId=539266) | Ezin duzu enpresen arteko gastuen txostena gorde **Baliabideen/Kategoria baliozkotzea** akats bat delako. |
| Bidaia eta gastua | [532610](https://fix.lcs.dynamics.com/Issue/Details/?bugId=532610) | Gastuen txostenak bidaltzean egindako kilometrajearen tasa kalkulatzeak lerro zatituak ditu. |
| Bidaia eta gastua | [537404](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537404) | Ezin duzu konpainien arteko gastuen txostena bidali salmenten gaineko zerga sartuta dagoenean eta ordainketa-metodoaren kontu konpentsatu mota dagoenean **Langilea**. |
| Bidaia eta gastua | [542927](https://fix.lcs.dynamics.com/Issue/Details/?bugId=542927) | Leheneratu **TrvRequisitionLine** datu-entitatea eta lotutako indize bakarra. |
| Bidaia eta gastua | [543239](https://fix.lcs.dynamics.com/Issue/Details/?bugId=543239) | Gastuen txostenak iturburuko dokumentu lerroak sortu eta eguneratzea onartzen du. |
| Bidaia eta gastua | [544323](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544323) | Azpiliburu nagusi okerra erakusten da enpresen arteko agertokian salmenten gaineko zerga helmugako pertsona juridikoari bidaltzen bazaio. |
| Bidaia eta gastua | [546877](https://fix.lcs.dynamics.com/Issue/Details/?bugId=546877) | Project Operations: gastuen kalkulua ez da Finantzatik ezabatzen, ezabatzen denean Dataverse-tik. |
| Bidaia eta gastua | [550575](https://fix.lcs.dynamics.com/Issue/Details/?bugId=550575) | Gastu kategoria proiektua ez den kategoria bat denean, **Gastuak** orria ez da gastuen txostenean kopiatzen. |
