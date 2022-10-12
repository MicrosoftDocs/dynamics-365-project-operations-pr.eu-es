---
title: Zer berri 2022ko iraila - Baliabideetan/hornituta ez dauden agertokietarako proiektu-eragiketak
description: Artikulu honek Microsoft-en 2022ko iraileko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du Dynamics 365 Project Operations baliabideetan/ez hornituta oinarritutako eszenatokietarako.
author: ramagadu
ms.date: 09/28/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: ef8b4dd98d64dac1e2420f8e6a104258f126f112
ms.sourcegitcommit: a2d720ac6d7ddb20a0967fe87992a376b2478208
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/04/2022
ms.locfileid: "9621308"
---
# <a name="whats-new-september-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Zer berri 2022ko iraila - Baliabideetan/hornituta ez dauden agertokietarako proiektu-eragiketak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu hau Microsoft-en osagai eta bertsio hauei aplikatzen zaie Dynamics 365 Project Operations:

- Proiektuaren Eragiketak a Dataverse ingurunearen bertsioa 4.46.0.60
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunean 10.0.29 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

| Ezaugarrien eremua | Ezaugarriaren izena | Informazio gehiago |
| --- | --- | --- |
| Abaguneen kudeaketa | **Aurrekontuen berrikuspena eta aktibazioa**<br>Project Operations-ek salmenta-prozesuaren laguntza osoa dakar. Proiektuaren aurrekontuak aktibatu daitezke aurrekontua irakurtzeko soilik den eta berrikusten den egoera bat irudikatzeko. Aktibatutako komatxoak berrikus daitezke berrikuspen-zenbaki handitua duten komatxo berriak sortzeko. Aktibatutako proiektuen aurrekontuak edo aurrekontuen berrikuspenak irabazi edo galdu gisa itxi daitezke. | [Aktibatu eta berrikusi proiektuaren eskaintza](/dynamics365/project-operations/sales/activation-and-revision) |
| Fakturazioa eta prezioak | **Ordu-eremuaren prezio agnostikoa lehenetsita**<br>Project Operations-ek ordu-eremuaren data agnostiko baten kontzeptua sartu du proiektuaren erreal guztietan. Eremu berri bat, **Transakzio data**, orain eskuragarri dago aldizkari-lerroetan eta errealetan, eta transakzioa gertatu zeneko data gordetzeko erabiliko da, baina data hori Ordu Unibertsal Koordinatuan bihurtu gabe. Data hori beheranzko prozesuetarako erabiliko da, hala nola prezioen lehenetsia eta fakturak sortzeko. | <p>[Proiektuetan oinarritutako estimazioen eta errealen kostu-tasak zehaztea](/dynamics365/project-operations/pricing-costing/cost-price-resolution)</p><p>[Zehaztu proiektuetan oinarritutako estimazioen eta benetakoen salmenta-prezioak](/dynamics365/project-operations/pricing-costing/sales-price-resolution)</p> |
| Fakturazioa eta prezioak | **Data-eraginkorra den prezioen baliogabetzea Proiektuen Eragiketetan**<br>Data-eraginkorra den prezioen baliogabetzeak prezioen zerrendako prezio zehatzak aldatzeko edo aldatzeko modua eskaintzen du. | [Data-eraginkorra den prezioak gainidaztea](/dynamics365/project-operations/pricing-costing/dateffective_price_overrides) |
| Azpikontratazioa | **Azpikontratazioa eta saltzaileen fakturak bateratzea**<br>Ezaugarri honi esker, bezeroek proiektuko lanetarako erabiltzen diren baliabideen denbora, gastu kategoriak eta materialak erosteko azpikontratuak sortzeko aukera ematen du. Era berean, bezeroei proiektu-kudeatzaileentzako eskuragarri egongo diren saltzaileen fakturak erregistratzeko aukera ematen die finantza- eta eragiketa-aplikazioetan.Dataverse egiaztatzeko. | <p>[Azpikontratuen kudeaketa](/dynamics365/project-operations/pro/subcontracting/managing-subcontracts-overview)</p><p>[Sortu saltzailearen fakturak](/dynamics365/project-operations/procurement/vendor-invoicing-concept-and-creation)</p> |
| Denbora eta gastua | **Onartzaile globala**<br>Ezaugarri honek software hornitzaile independentea (ISV) eta onespen zentralizatua ahalbidetzen du, proiektuaren edo taldekideen egoera edozein dela ere. | [Segurtasuna eta onarpenak](/dynamics365/project-operations/approvals/approvals-security) |
| Gastuen kudeaketa | **Gastuen erantzukizuna saltzaileen monetan argitaratzeko gaitasuna**<br>Ezaugarri honek gastuen txostenak saltzaileen moneta batean argitaratzea ahalbidetzen du eskudirutan ordaintzeko metodorako. | [Gastuen erantzukizuna saltzaileen monetan argitaratzeko gaitasuna](/dynamics365/project-operations/expense/posting-expense-reports#enable-the-ability-to-post-expense-liability-in-vendor-currency-for-cash-payment-method-feature) |
| Proiektuen Kontratazioa | **Ordaindu saltzaileen ordainketak ordaintzean**<br>Eginbide honek ordaintzen denean ordaindu (PWP) funtzioa Project Operations stock gabeko inguruneekin erabiltzeko aukera ematen du. Horri esker, saltzaileen ordainketak blokeatu/atxiki daitezke, atxikipen-baldintzetan oinarrituta, ordainketa bezeroarengandik jaso arte. | [Ordaindu saltzaileen ordainketak ordaintzean](/dynamics365/project-operations/procurement/pay-when-paid) |
| Proiektuen Kontratazioa | **Proiektua erosteko eskariak**<br>Eginbide honi esker, erabiltzaileek proiektuei lotutako erosketa-aginduak sortzeko aukera ematen diete Dynamics 365 Customer Engagement integrazioan Project Operations gaituta dagoen pertsona juridikoetan. Proiektuaren erosketa-eskaerak hornituta ez dagoen materialaren kontratazioa proiektuaren aurka erregistratzeko erabil daitezke Kontratazio sailaren pertsonaren arabera. Proiektuaren erosketa-eskaerak ez dira sinkronizatuko Dataverse. Hala ere, entitate birtual bat erabil dezakezu Proiektuko erosketa-eskaeraren lerroak azaleratzeko Dataverse proiektuaren kudeatzailearen informaziorako. Proiektuarekin erlazionatutako hornitzaileen fakturaren kostua Project Actuals entitatearekin integratuta dago Dataverse. Proiektuaren kostua Proiektuaren azpiliburuan erregistratzen da Proiektuaren Eragiketen Integrazio aldizkaria erabiliz. | |

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ondorengo taulak 2022ko irailean Project Operations-en bertsioan aldatu edo gehitu diren idazketa bikoitzeko mapak erakusten ditu.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| -------------- | ------------------- | ------------|
| Project Operations-en integrazioaren benetako datuak (msdynactuals) | 1.0.0.15 | Mapa honek proiektuko eragiketekin azpikontratu errealak prozesatzea onartzen du baliabideetan oinarritutako eszenatokietarako. |
| Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices) | 1.0.0.2 | Mapa honek proiektuko eragiketekin azpikontratu errealak prozesatzea onartzen du baliabideetan oinarritutako eszenatokietarako. |
| Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn_projectvendorinvoicelines) | 1.0.0.5 | Mapa honek proiektuko eragiketekin azpikontratu errealak prozesatzea onartzen du baliabideetan oinarritutako eszenatokietarako. |

Exekutatu beti maparen azken bertsioa zure ingurunean, eta gaitu erlazionatutako taula-mapa guztiak zure proiektuaren eragiketak eguneratzen dituzun bitartean.Dataverse irtenbidea eta Finantza irtenbidearen bertsioa. Baliteke eginbide eta gaitasun batzuk behar bezala ez funtzionatzea maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taula-mapa bat pertsonalizatu baduzu, aplikatu berriro aldaketak. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztean arazoren bat aurkitzen baduzu, jarraitu argibideei [Mapetan taulako zutabeak falta dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa bikoitzeko arazoak konpontzeko gidaliburuaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2754422 | Material eta gastuen estimazioak ez dira Finantzara iristen proiektuak kopiatzen direnean Dataverse. |
| Denbora eta gastua | 2787409 | Balio ez duen onartzaile batek proiektua ez den denbora-sarrera onar dezake. |
| Abaguneen kudeaketa | 2788907 | Errore-mezu eguneratua, banderak dituzten eskaera-lerroen esklusibotasuna baliozkotzeko. |
| Denbora eta gastua | 2842253 | Denbora onartzeko salbuespen nulua kudeatzea. |
| Fakturazioa eta prezioak | 2844181 | Korrelazio IDa ez lortzeak blokeatzen du faktura sortzea. |
| Fakturazioa eta prezioak | 2876628 | QLD, CLD - Estimazio-prezio-zerrendaren ebazpenak prezio-zerrendako data-tarte-eremuak erabili behar ditu. |
| Azpikontratazioa | 2893222 | Azpikontratazio-lerro baterako rolik ez bada zehazten, posible izan beharko litzateke lerro hori hautatzea taldekide batean edozein roltarako. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuen kudeaketa eta kontabilitatea Finantzetan

Eguneratze honetan sartzen diren akatsen konponketei buruzko informazioa lortzeko, hasi saioa hemen Microsoft Dynamics Bizitza zikloko zerbitzuak eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=726559).

## <a name="features-turned-on-by-default-in-upcoming-release"></a>Eginbideak lehenespenez aktibatuta daude hurrengo bertsioan

Hurrengo taulan 10.0.30 bertsioan lehenespenez aktibatuta dauden funtzioak zerrendatzen dira. Automatikoki aktibatu diren eginbide gehienak bertan desaktibatu daitezke [Ezaugarrien kudeaketa](/dynamics365/fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview). Etorkizunean, baliteke automatikoki aktibatu diren eginbide batzuk Eginbideen kudeaketatik kendu eta derrigorrezko bihurtzea. Aldaketa honek bezeroek egungo funtzionalitateak erabiltzen dituztela ziurtatzen du, hobekuntzak gehitu ahala uneko funtzionalitatean oinarritu daitezen. Eginbideak ez dira inoiz automatikoki gaituta urtebete baino gutxiagoan, ezinbestekoak direla erabakitzen ez bada.

| Ezaugarriaren izena | Gaitu data | Eginbidea gehitu da | Eginbidearen egoera | Modulua |
| --- | --- | --- |--- |--- |
| Gaitu asinkronizazio eragiketa erabiltzaileak sinkronizazio eta asinkronizazio eragiketa batetik bestera aldatu behar duenean | 2022ko urriaren 21a | 2021eko apirilaren 9a | Lehenespenez aktibatuta | Gastuen kudeaketa |
| Beharrezko ordainagirien gastu-politikaren ebaluazioa | 2022ko urriaren 21a | 2021eko abenduaren 20a | Lehenespenez aktibatuta | Gastuen kudeaketa |
| Langileen eskuordetzak sortutako gastu-txostenen zerrenda-ikuspegia | 2022ko urriaren 21a | 2020ko otsailaren 19a | Lehenespenez aktibatuta | Gastuen kudeaketa |
| Kilometrajearen guztizkoen kalkulua urte fiskal arabera | 2022ko urriaren 21a | 2022ko maiatzaren 10a | Lehenespenez aktibatuta | Gastuen kudeaketa |
