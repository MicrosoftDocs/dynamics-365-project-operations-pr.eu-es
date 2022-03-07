---
title: 2021eko abuztuko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations
description: Gai honek 2021eko abuztuko Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruzko informazioa eskaintzen du baliabideetan / ez-ekoizpenean oinarritutako eszenatokietarako.
author: sigitac
ms.date: 08/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 26861472d3af20c58b3d01142b834d535cf99715
ms.sourcegitcommit: 083e3d219cd5126eecb74debb1b70b361680b1f6
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/18/2021
ms.locfileid: "7501356"
---
# <a name="whats-new-august-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko abuztuko berrikuntzak - Balabideetan edo ekoizpenean oinarritutako egoeretarako Project Operations

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

   - Project Operations Microsoft Dataverse inguruneko bertsioan 4.13.0.152.
   - Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.20 bertsioan.

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- **Onarpen multzoak**: Onarpenak taldearen denbora, gastua edo materialaren erabilera onartzeko eskaerak eragiketa azpimultzo txikiagoetan biltzen ditu. Multzo horri esker, onarpenak proiektuen arabera orden zehatz batean prozesatu daitezke eta berriro saiatzea eta sekuentziatzea ahalbidetzen du. Eskaerak multzokatzeak homologazioen prozesuen fidagarritasuna eta trazabilitatea hobetzen ditu homologazio kopuru handietan. Informazio gehiago lortzeko, ikusi [Onarpen ezarpenak](../approvals/approval-sets.md).

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik.

Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Idazketa bikoitza** orrialdean **Bertsioa** zutabean. Aktibatu maparen bertsio berria hautatuta **Taulen mapen bertsioak**, azken bertsioa hautatuz eta ondoren hautatutako bertsioa gordez. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa hastean arazoren bat baduzu, jarraitu argibideak [Taulen zutabeak falta dira mapetan arazoa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) idazketa bikoitzeko arazoak konpontzeko gida atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Fakturazioa eta prezioak | 2295625 | Mugarriaren izena fakturaren egitarautik fakturaren lerroaren xehetasunera kopiatu behar da. |
| Fakturazioa eta prezioak | 2316323 | Deskontua ez da Project Operations proforma fakturan editatu behar baliabideetan oinarritutako eszenatokietan. |
|   Abaguneen kudeaketa | 2338619 | **Aukera** eta **Aurrekontua** negozio arauak orrialdeetan soilik deitu behar dira. |
| Baliabideen kudeaketa | 2316523 | Erabiltzen **Bidali eskaera** rola erantsita duen baliabide eskakizunetik ez luke akatsik erakutsi behar. |
| Baliabideen kudeaketa | 2326885 | Baliabideen eskakizuna proiektu baten bidez sortzeak ez luke akatsik erakutsi behar. |
| Denbora eta gastua | 2335584 | Zaharkitako zereginak denbora sarreran isurtzen dira. |
| Denbora eta gastua | 2336884 | **Kopiatu Astea** denbora sartzeko botoiak uneko erabiltzailea baino gehiagorako funtzionatu behar du. |


### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Dynamics 365 Finance-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Bidaia eta gastua | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | Saltzailearen transakzioaren eta salmenten gaineko zergaren transakzioen zenbateko okerrak kreditu txartelaren transakzio batetik gastua sortzen denean erregistratzen dira. |
| Bidaia eta gastua | [4620366](https://fix.lcs.dynamics.com/Issue/Details?kb=4620366&amp;bugId=579485&amp;dbType=3&amp;qc=e864789bd95505ea624c537d585bf113c2de60b97c88439d44693dbd85aa8e92) | Okerreko likidazioa ordainketa egunkaria sortzen denean sortutako lerroak dira. |
| Bidaia eta gastua | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | Salmenten gaineko zergaren transakzioen zenbateko okerrak kreditu txartelaren transakzio batetik gastua sortzen denean erregistratzen dira. |
| Bidaia eta gastua | [4621765](https://fix.lcs.dynamics.com/Issue/Details?kb=4621765&amp;bugId=587306&amp;dbType=3&amp;qc=6fbfad0123d4e95eaf8d5a5a2f6c354577c991b7905c852ab02d1f94e728a876) | Gastu lerro bat ezabatzeak denbora asko behar izan dezake. |
| Proiektuaren kontabilitatea | [4623737](https://fix.lcs.dynamics.com/Issue/Details?kb=4623737&amp;bugId=598109&amp;dbType=3&amp;qc=4101fc5865201e21815299f2ff11ae46d5d5370510868df86c25ee09a8ca1a0c) | Sistemak ez du onartzen zenbaki sekuentziazio jarraia konfiguratzea aurrekontua KB 4619395 aplikatu ondoren argitaratzen duzunean. |
| Proiektuaren kontabilitatea | [4623332](https://fix.lcs.dynamics.com/Issue/Details?kb=4623332&amp;bugId=586034&amp;dbType=3&amp;qc=2f64bb1977c4a9c9dd2ce9de7e72230b86eca14b6295c5bbfb614ea97ad81caf) | Saltzailearen fakturak bidaltzeak akats mezuarekin huts egin dezake. "Bonoaren transakzioak ez dira orekatzen 2021/05/17 arabera. (kontabilitate moneta: 0,00 - txosten moneta: 0,01)" |
