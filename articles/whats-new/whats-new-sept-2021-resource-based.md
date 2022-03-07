---
title: Zer berri 2021eko iraila - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Gai honek 2021eko iraileko baliabideetan/izakinik ezan oinarritutako egoeretarako Project Operations bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 09/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 842ea95892fa4f7a29a778cfd2c33a66e84f676c
ms.sourcegitcommit: 74a7e1c9c338fb8a4b0ad57c5560a88b6e02d0b2
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/23/2021
ms.locfileid: "7547139"
---
# <a name="whats-new-september-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>Zer berri 2021eko iraila - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

*Honi aplikatzen zaio: Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations*

Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

   - Project Operations Microsoft Dataverse inguruneko bertsioan 4.14.0.99.
   - Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.20 bertsioan.

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations zerbitzuaren idazketa dualeko esleipenen eguneratzeak

Ez dago bertsio honetan Project Operations idazketa bikoitzeko mapen eguneratzerik. Project Operations idazketa bikoitzeko mapen uneko zerrenda eta bertsioak ikusteko, ikusi [Project Operations idazketa bikoitzeko mapen bertsioak](../environment/resource-dual-write-maps.md).

Exekutatu beti maparen azken bertsioa zure ingurunean eta gaitu erlazionatutako taula-mapa guztiak eguneratzen dituzunean Project Operations Dataverse irtenbidea eta Finantza soluzioaren bertsioa. Zenbait eginbide eta gaitasunek agian ez dute behar bezala funtzionatuko maparen azken bertsioa aktibatuta ez badago. Maparen bertsio aktiboa helbidean ikus dezakezu **Idazketa bikoitza** orrialdean **Bertsioa** zutabean. Maparen bertsio berria aktibatzeko, hautatu **Taula maparen bertsioak**, hautatu azken bertsioa, eta ondoren, gorde hautatutako bertsioa. Kutxaz kanpoko taulako mapa pertsonalizatu baduzu, aldaketak berriro aplikatu. Informazio gehiago lortzeko, ikusi [Aplikazioaren bizi-zikloaren kudeaketa](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

Mapa hasten duen arazoren bat aurkitzen baduzu, jarraitu argibideak [Falta diren taulako zutabeak mapetan agertzen dira](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) Idazketa Dualaren arazoak konpontzeko gidaren atalean.

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| Denbora eta gastua | 1811407 | Segurtasun-funtzio proiektuaren onartzailea egokitu da gastuak sartzeko onarpenetarako. |
| Denbora eta gastua | 1811438 | Denbora-sarrerako onespenaren baliogabetzerako segurtasun-funtzio proiektuaren onartzailea egokitu da gastuak sartzeko onarpenetarako. |
| Denbora eta gastua | 2370126 | Eguneratu da **Proiektuaren zeregina** eta **Funtzioa** ikonoak **Denbora-sarrera** entitatean. |
| Denbora eta gastua | 2379879 | Zuzendu da **Kopiatu astea** funtzioa denbora sartzean telefonoa Dynamics 365 erabiltzean. |
| Fakturazioa eta prezioak | 2371906 | Proforma fakturaren zenbateko osoa ezin da erregulatu Project Operations baliabideetan oinarritutako inplementazioetarako. |
| Fakturazioa eta prezioak | 2385802 | Proiektuen guztizkoak freskatzen direnean benetako ordu negatiboekin gertatzen den akatsa konpondu da. |
| Fakturazioa eta prezioak | 2389675 | Proformaren faktura berresteko portaera hobetu da. Iraupen luzeko lanpostuen entitateak kontabilitate berrespen emaitzak idazteko behar den jarduera kontuan hartu behar du. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Dynamics 365 Finance-n

| Ezaugarrien eremua | Erreferentzia-zenbakia | Kalitatearen eguneratzea |
| --- | --- | --- |
| Bidaia eta gastua | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | Kreditu txartelaren transakzio batetik sortutako gastu batetik erregistratutako saltzaileen eta salmenten gaineko zergaren transakzioen zenbatekoak ez dira zuzenak. |
| Bidaia eta gastua | [4620366](https://fix.lcs.dynamics.com/Issue/Details?kb=4620366&amp;bugId=579485&amp;dbType=3&amp;qc=e864789bd95505ea624c537d585bf113c2de60b97c88439d44693dbd85aa8e92) | Ordainketa egunkaria sortzen denean okerreko likidazio lerroak sortzen dira. |
| Bidaia eta gastua | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | Kreditu txartelaren transakzio batetik sortutako gastu batetik erregistratutako salmenten gaineko zergaren transakzioen zenbatekoak ez dira zuzenak. |
| Bidaia eta gastua | [4621765](https://fix.lcs.dynamics.com/Issue/Details?kb=4621765&amp;bugId=587306&amp;dbType=3&amp;qc=6fbfad0123d4e95eaf8d5a5a2f6c354577c991b7905c852ab02d1f94e728a876) | Gastu lerro bat ezabatzeak denbora asko behar izan dezake. |
| Proiektuaren kontabilitatea | [4623737](https://fix.lcs.dynamics.com/Issue/Details?kb=4623737&amp;bugId=598109&amp;dbType=3&amp;qc=4101fc5865201e21815299f2ff11ae46d5d5370510868df86c25ee09a8ca1a0c) | KB 4619395 aplikatu ondoren, zenbaki sekuentzia honetara aldatu **Etengabea** ez da onartzen eta aurrekontua bidaltzen duzunean, errore hau gertatzen da: "Sistemak ez du Proj_X zenbaki sekuentziaren 'etengabeko' konfigurazioa onartzen". |
| Proiektuaren kontabilitatea | [4623332](https://fix.lcs.dynamics.com/Issue/Details?kb=4623332&amp;bugId=586034&amp;dbType=3&amp;qc=2f64bb1977c4a9c9dd2ce9de7e72230b86eca14b6295c5bbfb614ea97ad81caf) | Saltzailearen faktura bidaltzeak huts egin dezake honako errore mezu honekin: "Bonoaren transakzioak ez dira orekatzen 2021/05/17en arabera. (kontabilitate moneta: 0,00 - txosten moneta: 0,01)." |
