---
title: Zer berri 2022ko iraila - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Artikulu honek 2022ko iraileko baliabideetan/izakinik ezan oinarritutako egoeretarako Microsoft Dynamics 365 Project Operations bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: ramagadu
ms.date: 09/28/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 04b5f2f8223cdc80028860dd880dde314be244eb
ms.sourcegitcommit: b3a70bc4f2850cff5c2b7114cff7bd61ec298143
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/06/2022
ms.locfileid: "9634790"
---
# <a name="whats-new-september-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>Zer berri 2022ko iraila - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Microsoft Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse inguruneko bertsioan 4.46.0.60
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.29 bertsioan

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

| Ezaugarrien eremua | Eginbidearen izena | Informazio gehiago |
| --- | --- | --- |
| Abaguneen kudeaketa | **Eskaintzen aktibazioa eta berrikuspenak**<br>Project Operations-ek salmenta-prozesuaren laguntza osoa dakar. Proiektuaren eskaintzak aktibatu daitezke eskaintza irakurtzeko soilik den eta berrikusten den egoera bat irudikatzeko. Aktibatutako eskaintzak berrikus daitezke berrikuspen-zenbaki handitua duten eskaintza berriak sortzeko. Aktibatutako proiektuaren eskaintzak edo eskaintzen berrikuspenak irabazi edo galduta gisa itxi daitezke. | [Aktibatu eta berrikusi proiektuaren eskaintza](/dynamics365/project-operations/sales/activation-and-revision) |
| Fakturazioa eta prezioak | **Ordu-eremuaren prezio agnostikoa lehenetsita**<br>Project Operations-ek ordu-eremuaren data agnostiko baten kontzeptua sartu du proiektuaren erreal guztietan. Eremu berri bat, **Transakzio data**, orain egunkari-lerroetan eta errealetan eskuragarri dago, eta transakzioa gertatu zeneko data gordetzeko erabiliko da, baina data hori Ordu Unibertsal Koordinatuan bihurtu gabe. Data hori beheranzko prozesuetarako erabiliko da, hala nola prezioen lehenetsia eta fakturak sortzeko. | <p>[Erabaki proiektuetan oinarritutako estimazio eta benetako datuen salmenta-prezioak](/dynamics365/project-operations/pricing-costing/cost-price-resolution)</p><p>[Erabaki proiektuetan oinarritutako aurreikuspenen eta benetako datuen salmenta-prezioak](/dynamics365/project-operations/pricing-costing/sales-price-resolution)</p> |
| Fakturazioa eta prezioak | **Datarekin eraginkor bihurtzen den prezioen gainidazketa Project Operations-en**<br>Data-eraginkorra den prezioak gainidaztea prezioen zerrendan prezio zehatzak gainidazteko edo aldatzeko modu bat eskaini. | [Dataren araberako prezioen gainidazketak](/dynamics365/project-operations/pricing-costing/dateffective_price_overrides) |
| Azpikontratazioa | **Azpikontratazioa eta saltzaileen fakturak bateratzea**<br>Ezaugarri honi esker, bezeroek proiektuko lanetarako erabiltzen diren baliabideen denbora, gastu kategoriak eta materialak erosteko azpikontratuak sortzeko aukera ematen du. Era berean, egiaztatzeko Dataverse-eko proiektu-kudeatzaileentzako eskuragarri egongo diren saltzaileen fakturak erregistratzeko aukera ematen die bezeroei finantzen eta eragiketen aplikazioetan. | <p>[Azpikontratatuen kudeaketa](/dynamics365/project-operations/pro/subcontracting/managing-subcontracts-overview)</p><p>[Sortu saltzailearen fakturak](/dynamics365/project-operations/procurement/vendor-invoicing-concept-and-creation)</p> |
| Denbora eta gastua | **Onartzaile globala**<br>Ezaugarri honek software hornitzaile independentea (ISV) eta onespen zentralizatua ahalbidetzen du, proiektuaren edo taldekideen egoera edozein dela ere. | [Segurtasuna eta onarpenak](/dynamics365/project-operations/approvals/approvals-security) |
| Gastuen kudeaketa | **Gastuen erantzukizuna saltzaileen monetan argitaratzeko gaitasuna**<br>Ezaugarri honek gastuen txostenak saltzaileen moneta batean argitaratzea ahalbidetzen du eskudirutan ordaintzeko metodorako. | [Gastuen erantzukizuna saltzaileen monetan argitaratzeko gaitasuna](/dynamics365/project-operations/expense/posting-expense-reports#enable-the-ability-to-post-expense-liability-in-vendor-currency-for-cash-payment-method-feature) |
| Proiektuen Kontratazioa | **Ordaindu ordaintzean saltzailearen ordainketak**<br>Eginbide honek ordaintzen denean ordaindu (PWP) funtzioa Project Operations-eko stock gabeko inguruneekin erabiltzeko aukera ematen du. Horri esker, saltzaileen ordainketak blokeatu/atxiki daitezke, atxikipen-baldintzetan oinarrituta, ordainketa bezeroarengandik jaso arte. | [Ordaindu ordaintzean saltzailearen ordainketak](/dynamics365/project-operations/procurement/pay-when-paid) |
| Proiektuen Kontratazioa | **Proiektuaren erosketa-eskakizunak**<br>Eginbide honi esker, erabiltzaileek proiektuarekin lotutako erosketa-aginduak sortzeko aukera ematen dute Project Operations on Dynamics 365 Customer Engagement integrazioa gaituta dagoen pertsona juridikoetan. Proiektuaren erosketa-eskaerak hornituta ez dagoen materialaren kontratazioa proiektuaren aurka erregistratzeko erabil daitezke Kontratazio sailaren pertsonaren arabera. Proiektuaren erosketa-eskaerak ez dira sinkronizatuko Dataverse-n. Hala ere, entitate birtual bat erabil dezakezu Proiektuko erosketa-eskaeraren lerroak azaleratzeko Dataverse-n proiektuaren kudeatzailearen informaziorako. Proiektuarekin erlazionatutako hornitzaileen fakturaren kostua Proiektuaren beetako datuak entitatearekin integratuta dago Dataverse-n. Proiektuaren kostua erregistratzen da bigarren mailako liburu nagusian Project Operations integrazio-egunkaria erabiliz. | |
|Proiektuaren antolaketa eta jarraipena|**Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko** </br> </br>Baliabideen esleipenaren sestra editatzeko APIari esker, garatzaileek programatikoki zehazten dute zereginen esleipendun baten esfortzua onartzen den edozein data-barrutitan, denbora-mailako esfortzuen planifikazio zehatzagoa lortzeko.|[Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko](/dynamics365/project-operations/project-management/schedule-api-preview)|

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Hurrengo taulan 2022ko iraileko Project Operations aldatu edo gehitu diren idazketa bikoitzeko mapak agertzen dira.

| Entitate-esleipena | Eguneratutako bertsioa | Iruzkinak |
| -------------- | ------------------- | ------------|
| Project Operations-en integrazioaren benetako datuak (msdynactuals) | 1.0.0.15 | Mapa honek Project Operations-ekin azpikontratu errealak prozesatzea onartzen du baliabideetan oinarritutako eszenatokietarako. |
| Project Operations integrazioa proiektuaren saltzailearen faktura esportatzeko entitatea (msdyn_projectvendorinvoices) | 1.0.0.2 | Mapa honek Project Operations-ekin azpikontratu errealak prozesatzea onartzen du baliabideetan oinarritutako eszenatokietarako. |
| Project Operations integrazioa proiektuaren saltzailearen faktura-lerroa esportatzeko entitatea (msdyn_projectvendorinvoicelines) | 1.0.0.5 | Mapa honek Project Operations-ekin azpikontratu errealak prozesatzea onartzen du baliabideetan oinarritutako eszenatokietarako. |

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Bertsioa** zutabea **Idazketa bikoitza** orrialdean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa abiaraztearen arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2754422 | Material eta gastuen estimazioak ez dira Finantzara iristen proiektuak kopiatzen direnean Dataverse-n. |
| Denbora eta gastua | 2787409 | Balio ez duen onartzaile batek proiektua ez den denbora-sarrera onar dezake. |
| Abaguneen kudeaketa | 2788907 | Errore-mezu eguneratua, markak dituzten eskaera-lerroen esklusibotasuna baliozkotzeko. |
| Denbora eta gastua | 2842253 | Denbora onartzeko salbuespen nulua kudeatzea. |
| Fakturazioa eta prezioak | 2844181 | Korrelazio IDa ez lortzeak blokeatzen du faktura sortzea. |
| Fakturazioa eta prezioak | 2876628 | QLD, CLD - Estimazio-prezio-zerrendaren ebazpenak prezio-zerrendako data-tarte-eremuak erabili behar ditu. |
| Azpikontratazioa | 2893222 | Azpikontratazio-lerro baterako rolik ez bada zehazten, posible izan beharko litzateke lerro hori hautatzea taldekide batean edozein roltarako. |

### <a name="project-management-and-accounting-in-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Finantzan

Eguneratze honetan jasotako arazoen konponketen inguruko informazioa lortzeko, hasi saioa Microsoft Dynamics Lifecycle Services-en eta ikusi [KB artikulua](https://fix.lcs.dynamics.com/Issue/Details?bugId=726559).

## <a name="features-turned-on-by-default-in-upcoming-release"></a>Eginbideak lehenespenez aktibatuta daude hurrengo bertsioan

Hurrengo taulan 10.0.30 bertsioan lehenespenez aktibatuta dauden funtzioak zerrendatzen dira. Automatikoki aktibatu diren eginbide gehienak desaktibatu daitezke [Ezaugarrien kudeaketan](/dynamics365/fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview). Etorkizunean, baliteke automatikoki aktibatu diren eginbide batzuk Eginbideen kudeaketatik kendu eta derrigorrezko bihurtzea. Aldaketa honek bezeroek egungo funtzionalitateak erabiltzen dituztela ziurtatzen du, hobekuntzak gehitu ahala uneko funtzionalitatean oinarritu daitezen. Eginbideak ez dira inoiz automatikoki gaituko urtebete baino gutxiagoan, ezinbestekoak direla erabakitzen ez bada.

| Eginbidearen izena | Gaitu data | Eginbidea gehitu da | Eginbidearen egoera | Modulua |
| --- | --- | --- |--- |--- |
| Gaitu asinkronizazio eragiketa erabiltzaileak sinkronizazio eta asinkronizazio eragiketa batetik bestera aldatu behar duenean | 2022ko urriak 21 | 2021eko apirilaren 9a | Lehenespenez aktibatuta | Gastuen kudeaketa |
| Beharrezko ordainagirien gastu-politikaren ebaluazioa | 2022ko urriak 21 | 2021eko abenduaren 20 | Lehenespenez aktibatuta | Gastuen kudeaketa |
| Langile ordezkariek sortutako gastu-txostenen zerrenda-ikuspegia | 2022ko urriak 21 | 2020ko otsailaren 19a | Lehenespenez aktibatuta | Gastuen kudeaketa |
| Kilometrajearen guztizkoen kalkulua urte fiskal arabera | 2022ko urriak 21 | 2022ko maiatzaren 10a | Lehenespenez aktibatuta | Gastuen kudeaketa |
