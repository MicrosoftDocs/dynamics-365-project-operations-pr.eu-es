---
title: Project Operations idazketa dualeko esleipen-bertsioak
description: Gai honek idazketa bikoitzeko mapen zerrenda eskaintzen du Dynamics 365 Project Operations.
author: sigitac
ms.date: 04/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c8bc389c83eaf2a7720ef3fa969c677eed11e7959199b5f0083df5bf3b43ea43
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7003801"
---
# <a name="project-operations-dual-write-map-versions"></a>Project Operations idazketa dualeko esleipen-bertsioak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Dynamics 365 Project Operations baliabideetarako / hornitu gabeko eszenatokietarako idazketa bikoitzeko mapen multzoa ingurunean exekutatzeko behar da. 

## <a name="prerequisite-maps-dual-write-orchestration-solution"></a>Aurrebaldintzen mapak: Idazketa dualaren antolaketa-soluzioa

Ondorengo mapak Project Operations soluziorako ezinbesteko baldintzak dira. Ziurtatu hurrengo taulan zerrendatutako mapak eta zure inguruneko erlazionatutako taulako mapak exekutatzen dituzula.

| Taula-esleipena | Hasierako sinkronizazioa |
| --- | --- |
| Liburua (msdyn_ledgers) | Taularen maparen eta aurrebaldintza guztien hasierako sinkronizazioa eskatzen du. Hasierako sinkronizazioaren eredua Finance and Operations aplikazioak dira. |
| Legezko entitateak (cdm_companies) | Ez da beharrezkoa. Sistemak entitate hau automatikoki betetzen du inguruneak idazketa bikoitzaren bidez lotzen direnean. |
| Bezeroak V3 (kontuak) | Ez da hornidura egiteko beharrezkoa. |
| Saltzaileak V2 (msdyn_vendors) | Ez da hornidura egiteko beharrezkoa. |

1. Mapen zerrendan, hautatu Liburua **(msdyn\_ledgers)** mapa aurrebaldintza guztiekin eta hautatu **Hasierako sinkronizazioa** kontrol-laukia. **Hasierako sinkronizaziorako maisua** eremua, hautatu **Finance and Operations aplikazioak** bai liburutegi maparako, bai aurrebaldintzako mapa guztietarako. Hautatu **Exekutatu**.

![Liburuaren esleipenaren sinkronizazioa.](media/DW6.png)

2. Jarrai itzazu urrats berberak goiko taulan zerrendatutako gainerako taula-mapa guztietan. Ez hautatu **Hasierako sinkronizazioa** kontrol laukia mapa horiek exekutatzean.

## <a name="project-operations-dual-write-maps"></a>Project Operations zerbitzuaren idazketa dualeko esleipenak

Ondorengo mapak Project Operations soluziorako behar dira. Idazketa bikoitzeko mapen bertsioak zerrendatzen dira Project Operations 2021eko maiatzaren bertsioarekin hasita, 4.10.0.186 bertsioa.

| **Entitate-esleipena** | **Azken bertsioa** | **Hasierako sinkronizazioa** |
| --- | --- | --- |
| Proiektuen transakzio harremanetarako integrazio entitatea (msdyn\_transactionconnections) | 1.0.0.0 | Ez da hornidura egiteko beharrezkoa. |
| Proiektuen kontratuen goiburuak (salmenta aginduak) | 1.0.0.1 | Ez da hornidura egiteko beharrezkoa. |
| Proiektuetako kontratuaren lerroak (salesorderdetails) | 1.0.0.0 | Ez da hornidura egiteko beharrezkoa. |
| Proiektua finantzatzeko iturria (msdyn_projectcontractsplitbillingrules) | 1.0.0.2 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations integrazioaren taula materialen kalkuluen arabera (msdyn\_estimatelines) | 1.0.0.0 | Ez da hornidura egiteko beharrezkoa. |
| Proiektuaren faktura-proposamenak V2 (fakturak) | 1.0.0.3 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations-en integrazioaren benetako datuak (msdynactuals) | 1.0.0.14 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations-ek integratzeko kontratu lerroaren mugarriak (msdyn_contractlinesscheduleofvalues) | 1.0.0.4 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations-ek integratzeko entitatea gastuen kalkuluen arabera (msdyn_estimateslines) | 1.0.0.2 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations-ek integratzeko entitatea orduen kalkuluen arabera (msdyn_resourceassignments) | 1.0.0.5 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations-ek integratzeko proiektuaren gastuak kategoriak esportatzeko entitatea (msdyn_expensecategories) | 1.0.0.1 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations-ek integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn_expenses) | 1.0.0.2 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices) | 1.0.0.0 | Ez da hornidura egiteko beharrezkoa. |
| Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn_projectvendorinvoicelines) | 1.0.0.1 | Ez da hornidura egiteko beharrezkoa. |
| Enpresa guztientzako proiektuaren baliabideen eginkizunak (bookableresourcecategories) | 1.0.0.1 | Taulako maparen hasierako sinkronizazioa eskatzen du Dynamics 365 Dataverse ingurunean betetzen diren Project Manager eta Taldeko kideen baliabide rolak sinkronizatzeko horniduran zehar. Dataverse hasierako sinkronizazioaren iturri nagusia da. |
| Proiektuaren zereginak (msdyn_projecttasks) | 1.0.0.4 | Ez da hornidura egiteko beharrezkoa. |
| Proiektuen transakzio kategoriak (msdyn_transactioncategories) | 1.0.0.0 | Ez da hornidura egiteko beharrezkoa. |
| Proiektuak V2 (msdyn_projects) | 1.0.0.2 | Ez da hornidura egiteko beharrezkoa. |

Osatu urrats hauek zerrendatutako mapak exekutatzeko.

1. Gaitu proiektuaren baliabide rolak **enpresa guztiak (bookableresourcecategories)** taula mapa mapa honek hasierako sinkronizazioa behar du. **Hasierako sinkronizaziorako maisua** eremua, hautatu **Datu zerbitzu arrunta**. 

 ![Baliabideen rolen taulen maparen sinkronizazioa.](media/6ResourceInitialSync.jpg)

 Itxaron maparen egoera izan arte **Korrika** hurrengo urratsera pasa aurretik.

2. Aukeratu beharrezko gainerako mapa guztiak. Idazketa bikoitzeko mapen zerrendan iragazi ditzakezu gako-hitza erabiliz, **Proiektua** bila goiko eskuineko izkinan. Mapa guztiak hauta ditzakezu eta gero exekutatu. Informazio gehiagorako, ikusi [Kudeatu taula-mapa anitz](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/multiple-entity-maps). Ziurtatu erlazionatutako entitate mapak ere gaitu eta exekutatzen dituzula.

### <a name="project-operations-dual-write-map-versions"></a>Project Operations idazketa dualeko esleipen-bertsioak

Exekutatu beti maparen azken bertsioa zure ingurunean. Baliteke zenbait eginbide eta gaitasunek behar bezala ez funtzionatzea baldintza hauetakoren bat baldin badago:

- Mapa ez dago aktibatuta.
- Maparen azken bertsioa ez dago aktibatuta. 
- Lotutako taulako mapak ez daude aktibatuta.

Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktiba dezakezu hautatuta **Taula maparen bertsioak**, azken bertsioa hautatuta, eta ondoren hautatutako bertsioa gorde. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu beharko dituzu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).
