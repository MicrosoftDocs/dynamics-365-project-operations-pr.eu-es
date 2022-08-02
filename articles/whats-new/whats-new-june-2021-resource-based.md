---
title: 2021eko ekaineko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations
description: Artikulu honek 2021eko ekaineko Project Operations-en bertsioan eskuragarri dauden kalitate-egunerei buruzko informazioa eskaintzen du baliabideetan edo hornituta ez dauden agertokietarako.
author: sigitac
ms.date: 06/14/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: fd745107fa6d50882ebea302d3d2ae0de21b79ad
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028160"
---
# <a name="whats-new-june-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko ekaineko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu hau honako hauei aplikatzen zaie Dynamics 365 Project Operations osagaiak eta bertsioak:

- Project Operations Dynamics 365-en Dataverse inguruneko bertsioa 4.11.0.156 edo 4.11.0.164.
- Proiektuen kudeaketa eta kontabilitatea finantza eta eragiketa aplikazioen inguruneetan 10.0.19 bertsioa.

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- [Egokitzapen-egoeretarako proiektuaren faktura-proposamenak](../invoicing/correct-project-invoice-proposals.md) ezabatzeko gaitasuna.
- Partikulatutako gastu lerroek azpikategorien izenak islatzen dituzte gastuen txostenean [Gastuen txostenak berriro pentsatu-Ezaugarri berriak](../expense/expense-reports-reimagined.md#new-features).
- Ordainketa modua gastu berrien panelean eskuragarri dago gastu berria sortzerakoan.
- Proiektuak antolatzeko APIen erabilgarritasun orokorra. Funtzionalitate berri honi esker, bezeroek proiektuko zereginetan, baliabideen esleipenetan, atazen mendekotasunetan eta proiektuko taldekideen erregistroetan sortu, eguneratu eta ezabatzeko eragiketak programatikoki egin ditzakete. Informazio gehiagorako, ikusi [Erabili Proiektuak antolatzeko APIak antolaketa-entitateak dituzten eragiketak egiteko](../project-management/schedule-api-preview.md).

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. 

Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta finantza eta eragiketa aplikazioak irtenbide bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Idazketa bikoitza** orrialdean **Bertsioa** zutabean. Aktibatu maparen bertsio berria hautatuta **Taulen mapen bertsioak**, azken bertsioa hautatuz eta ondoren hautatutako bertsioa gordez. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa hastean arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan arazoa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) idazketa bikoitzeko arazoak konpontzeko gida atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2281417 | Faktura-egutegiaren bidez faktura automatikoki sortzeko ekintzaren hutsaren inguruko arazoa konpondu da. |
| Fakturazioa eta prezioak | 2287835 | Fakturen berrespena hobetu da. |
| Abaguneen kudeaketa | 2222555 | Materialen kalkuluen kargagarritasuna behar bezala kopiatu behar da **Inportatu proiektuaren zenbatespenetik** erabiltzen ari zarenean lerroaren xehetasunak aipatzeko. |
| Abaguneen kudeaketa | 2223427 | Pertsonalizazioak ekintzarako honetarako onartzen dira, **GenerateRetainersFromRetainerScheduleOptions**. |
| Abaguneen kudeaketa | 2277528 | Finkatutako fakturazio mugarriaren balioa kalkulatzea bezero anitzekin egindako proiektuen kontratu lerroetarako. |
| Proiektuaren antolaketa eta jarraipena | 2226110 | Aldizkako arazoa konpondu da **Sortu Eskakizuna** funtzioan **Proiektu taldea** saretan. |
| Proiektuaren antolaketa eta jarraipena | 2208109 | Erabiltzaileek ezin dute moneta batean proiektu bat sortu beste moneta bati lotutako egitekoekin. |
| Proiektuaren antolaketa eta jarraipena | 2258228 | Antolaketa APIa erabiliz **Programazioa** elementuarekin aldatzeko baimendutako eremuen zerrenda erabiltzen duten entitateak eguneratu dira. |
| Proiektuaren antolaketa eta jarraipena | 2293989 | Hizkuntza eta eskualde ezarpen zuzenak pasatu behar dira **Proiektuaren zereginak** saretara. |
| Baliabideen kudeaketa | 2220493 | Erabiltzaileen esperientzia konpondu da **Egitekoa** saretan baliabide eskaera azkar osatuta dagoela markatzean. |
| Baliabideen kudeaketa | 2330496 | Konpondu da **Antolaketa taula** kargatzearen arazoa. (Kalitatearen eguneratzea eskuragarri dago 4.11.0.164 bertsioan) |
| Denbora eta gastua | 2194431 | **Denbora sarrera** saretak aste hasieran errespetatu behar du **Sistemaren ezarpenetan**. |
| Denbora eta gastua | 2277311 | Gelaxka bateko balioa ezabatu ondoren **Denbora sarrera** saretan, kurtsorea saretan geratzen da. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance-en

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Proiektuaren kudeaketa eta kontabilitatea | [552976](https://fix.lcs.dynamics.com/Issue/Details/?bugId=552976) | **Inprimaki oharrak** eta **Inprimakiaren konfigurazioa** ez dago ikusgai Finantza entitate juridikoen **proiektuaren kudeaketaren konfigurazioan**, proiektuaren eragiketekin integratuta daudenetan. |
| Proiektuaren kudeaketa eta kontabilitatea | [527970](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527970) | Azalpen lehenetsia hutsik dago BEZean, **bidalketa motak** = **Salmenten gaineko zerga** denean proiektuaren fakturaren bonuetan. |
| Proiektuaren kudeaketa eta kontabilitatea | [565089](https://fix.lcs.dynamics.com/Issue/Details/?bugId=565089) | Transakzio bikoitz bat bi aldiz argitaratzen da zereginetan oinarritutako fakturazioa erabiltzen denean Dataverse-n Project Operations-en integrazioarekin. |
| Proiektuaren kudeaketa eta kontabilitatea | [566869](https://fix.lcs.dynamics.com/Issue/Details/?bugId=566869) | Diru sarrerak hautemateko ehunekoa ez da zuzena Project Operations-en integrazioa erabiltzean. |
| Proiektuaren kudeaketa eta kontabilitatea | [568107](https://fix.lcs.dynamics.com/Issue/Details/?bugId=568107) | Diru sarreren metaketa bikoiztu egiten da Project Operations-en integratutako agertoki batean saltzailearen faktura pendiente bat erabiltzen duzunean. |
| Proiektuaren kudeaketa eta kontabilitatea | [572370](https://fix.lcs.dynamics.com/Issue/Details/?bugId=572370) | Integrazio egunkaria ezin da argitaratu diru-sarreren profileko araua honela ezarrita badago: **Taldearen** konfigurazioa. |
| Proiektuaren kudeaketa eta kontabilitatea | [573596](https://fix.lcs.dynamics.com/Issue/Details/?bugId=573596) | Ezin da erosketa fakturarik bidali neurri unitate anitzeko lerroak dituen proiektuaren erosketa eskaeretarako. |
| Proiektuaren kudeaketa eta kontabilitatea | [573637](https://fix.lcs.dynamics.com/Issue/Details/?bugId=573637) | Proiektu baten finantza dimentsio lehenetsia ezin da eguneratu proiektuak **V2** datu entitatea erabiliz. |
| Proiektuaren kudeaketa eta kontabilitatea | [577211](https://fix.lcs.dynamics.com/Issue/Details/?bugId=577211) | Proiektua kalkulatzeko sortze sorta prozesuak denbora gehiegi behar du burutzeko. |
| Proiektuaren kudeaketa eta kontabilitatea | [582329](https://fix.lcs.dynamics.com/Issue/Details/?bugId=582329) | Kontratua ezabatzen duzunean, bezeroarekin lotutako helbidea ere ezabatzen da. |
| Bidaia eta gastua | [514930](https://fix.lcs.dynamics.com/Issue/Details/?bugId=514930) | Gastuen txostena onartzeko lan-fluxuaren egoera ez da behar bezala ebaluatzen. |
| Bidaia eta gastua | [519304](https://fix.lcs.dynamics.com/Issue/Details/?bugId=519304) | Gastuen txostenaren gidalerroak ez du proiektuaren IDa behar bezala ebaluatzen. |
| Bidaia eta gastua | [522463](https://fix.lcs.dynamics.com/Issue/Details/?bugId=522463) | **Enpresen arteko gastuen transakzioen banatu pertsonalera** ekintzak ez du ondo funtzionatzen. |
| Bidaia eta gastua | [534702](https://fix.lcs.dynamics.com/Issue/Details/?bugId=534702) | Batzuetan, gastuen berri emateko lerroaren justifikazioak ezabatzen dira bidaia eskaerak ezabatzen direnean. Hori gertatzen da gastuen txostenaren berreskurapena eta bidaia-eskaera berdinak direnean. |
| Bidaia eta gastua | [544368](https://fix.lcs.dynamics.com/Issue/Details/?bugId=544368) | Gastuen mugikorretarako aplikazioarekin arazo bat dago **Proiektuaren IDa** eremua beharrezkoa denean gastuen txostenen gidalerroetarako. |
| Bidaia eta gastua | [545331](https://fix.lcs.dynamics.com/Issue/Details/?bugId=545331) | Ezin dira editatu proiektu batekin lotutako enpresa arteko gastuak. Horren ordez, honako errore-mezu hau agertzen da: "Objektuaren erreferentzia ez da objektu baten instantzia gisa ezarri". |
| Bidaia eta gastua | [548659](https://fix.lcs.dynamics.com/Issue/Details/?bugId=548659) | Okerreko moneta eta zenbatekoa banku azpiegituran agertzen da, gastuen txostena argitaratu ondoren. |
| Bidaia eta gastua | [558336](https://fix.lcs.dynamics.com/Issue/Details/?bugId=558336) | Hobetu da *Ezabatu kreditu txartelaren transakzioak* eginbidea.  |
| Bidaia eta gastua | [525070](https://fix.lcs.dynamics.com/Issue/Details/?bugId=525070) | Gastu-txostenean jasotako salmenten gaineko zerga ez da koherentziaz kalkulatzen pertsona juridiko batean beste moneta berri bat zehazten denean. |
| Bidaia eta gastua | [527779](https://fix.lcs.dynamics.com/Issue/Details/?bugId=527779) | Errendimenduak eragina du eskudiruzko bidaia gastu berri bat gehitzean. |
| Bidaia eta gastua | [537841](https://fix.lcs.dynamics.com/Issue/Details/?bugId=537841) | Gastu-politikaren araua ez da gastu-txostenean abiarazten. |
| Bidaia eta gastua | [566386](https://fix.lcs.dynamics.com/Issue/Details/?bugId=566386) | Datuen kudeaketa-esparrua erabiliz partekatutako kategoria berri bat kargatzeak partekatutako kategoria guztietako azpikategoria guztiak kentzen ditu. |
| Bidaia eta gastua | [574131](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574131) | Gastu lerro bat sortu eta kategoria bat hautatzen duzunean, errore-mezu hau bistaratzen da: "Salmenten gaineko zergen DOM eta elementuen salmenten gaineko zerga taldearen STD konbinazioak ez du balio". |
| Bidaia eta gastua | [574900](https://fix.lcs.dynamics.com/Issue/Details/?bugId=574900) | Gastu mugikorretarako aplikazioan sinkronizazio arazoak daude. |
