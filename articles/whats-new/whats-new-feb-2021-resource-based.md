---
title: 2021eko otsaileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations
description: Gai honek informazioa eskaintzen du 2021eko otsailean Project Operations bertsioan eskuragarri dauden kalitate-eguneratzeei buruz, baliabideetan / stockean oinarritutako egoeretarako.
author: sigitac
ms.date: 02/08/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 41d7d7133652069ca3899db7f12e67e9ba531bcd3e36d67c3686a6b637b077d3
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986791"
---
# <a name="whats-new-february-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>2021eko otsaileko berrikuntzak - Baliabideetan edo izakinik gabeko produktuetan oinarritutako adibideen Project Operations

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai hau Dynamics 365 Project Operations osagai eta bertsio hauei aplikatzen zaie:

- Project Operations Dataverse ingurunean 4.7.0.95
- Proiektuen kudeaketa eta kontabilitatea Dynamics 365 Finance ingurunearen 10.0.16 bertsioa 

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

### <a name="project-operations-on-dataverse"></a>Project Operations Dataverse-n

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
| **Fakturazioa eta prezioak** | 2053736 | Faktura-lerroaren xehetasunak **Faktura** > **Lotutako informazioa** aukeran daude orain. |
| **Fakturazioa eta prezioak** | 2122613 | **Aktibatu** eta **Desaktibatu** ekintzak kendu ziren **Prezioen zerrenda** elkarteko entitateak. |
| **Fakturazioa eta prezioak** | 2128606 | Arazoa konpondu da **ullReferenceException** parametroarekin **GetEstimatesForProject** pluginean. |
| **Inplementazioa eta konfigurazioa** | 2139346 | Arazoa konpondu da kudeatu gabeko inportazioarekin **Dynamics365ProjectOperationsDualWrite** irtenbidea. |
| **Inplementazioa eta konfigurazioa** | 2140569 | Proiektu-soluzioa ez da instalatu behar Dataverse Teams inguruneetan. |
| **Inplementazioa eta konfigurazioa** | 2086991 | Web baliabideen lokalizazio pertsonalizatua mugatua. |
| **Abaguneen kudeaketa** | 2136794 | Bistaratu errore mezu zuzena **Berretsi faktura** edo **Markatu faktura ordainduta** prozesuak huts egiten du. |
| **Abaguneen kudeaketa** | 2139330 | Proiektuaren kudeatzailea proiektu batean aldatzeak ez du enpresa jabea lehenetsitako balioera berrezarri behar. |
| **Abaguneen kudeaketa** | 2146376 | Kobratu gabeko benetako zergaren zenbatekoa fakturaren baieztapenetik sortzen da. |
| **Proiektuaren antolaketa eta jarraipena** | 2099879 | Dataverse ingurunearen inplementazioak transakzio kategoria lehenetsia sortu behar du ID estatikoarekin eta ez du ausaz sortu ingurune bakoitzeko bat. |
| **Proiektuaren antolaketa eta jarraipena** | 2128577 | Project Service-ren erabiltzaile pribilegioak konpondu dira transakzio kategoria baliabideen esleipenean eguneratzeko. |
| **Proiektuaren antolaketa eta jarraipena** | 2164035 | Arazoak konpondu dira **Kopiatu proiektua** funtzioa. |
| **Denbora-sarrera** | 2129161 | Murrizketa estuagoak aplikatzen dira erabiltzaileek bidalitako edo onartutako denbora sarrera aldatu eta eguneratu ezin dutela ziurtatzeko. |
| **Denbora-sarrera** | 2103572 | Proiektuak ez diren denbora-sarreren denbora onartzeak ez du proiektua onartzeko eginkizunik bilatu behar. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Proiektuaren kudeaketa eta kontabilitatea Dynamics 365 Finance-n 

Dynamics 365 Finance-ko proiektuen kudeaketari eta kontabilitateari buruzko informazio gehiago lortzeko, ikusi [2021eko urtarrileko berrikuntzak - Baliabideen/Stockik gabekoan oinarritutako eszenatokietarako Project Operations](whats-new-jan-2021-resource-based.md).


## <a name="regulatory-updates"></a>Araudiaren eguneratzeak

Eguneratze arautzaileei buruzko informazioa lortzeko Finance and Operations aplikazioak, ikusi [Araudiaren eguneratzeak](/dynamics365/finance/localizations/regulatory-updates). Araudi-eguneratzeak ezagutzeko beste modu bat Lifecycle Services (LCS) saioa hastea da eta aurreikusitako erregulazio-eguneratzeak ikustea arazoa bilatzeko tresna erabiliz. Arazoen bilaketak herrialdearen, eginbide motaren eta askapenaren arabera bilatzeko aukera ematen du.


[!INCLUDE[footer-include](../includes/footer-banner.md)]