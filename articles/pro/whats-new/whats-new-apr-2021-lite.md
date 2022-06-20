---
title: 2021eko apirileko berritasunak - Project Operations lite-n inplementazioa
description: Artikulu honek Project Operations lite inplementazioaren 2021eko apirileko bertsioan eskuragarri dauden kalitate eguneratzeei buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 04/07/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 987eeaf2e57659a6facae6b0a3688f15992e8bb9
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8931224"
---
# <a name="whats-new-april-2021---project-operations-lite-deployment"></a>2021eko apirileko berritasunak - Project Operations lite-n inplementazioa

_Honi aplikatzen zaio: Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu hau honako hauei aplikatzen zaie Dynamics 365 Project Operations osagaiak eta bertsioak:

  - Project Operations Dataverse ingurunearen 4.9.0.221 bertsioa 

## <a name="features-included-in-this-release"></a>Bertsioan sartzen diren eginbideak

Eginbide hauek sartzen dira bertsio honetan:

- Proiektuetarako materialik gabeko materiala. Gaitasun nagusiak honako hauek dira:
  - Proiektu baten salmenta-zikloan stockik gabeko materialak kalkulatzea eta preziatzea. Informazio gehiago lortzeko, ikusi [Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak - arina](../pricing-costing/set-up-cost-sales-rates-catalog-products.md).
  - Biltegiratu gabeko materialen erabileraren jarraipena egitea proiektuaren entrega garaian. Informazio gehiago lortzeko, ikusi [Erregistratu proiektuetako eta proiektu-zereginetako material-erabilera](../../material/material-usage-log.md).
  - Erabilitako materialik gabeko kostuen fakturazioa. Informazio gehiago lortzeko, ikusi [Kudeatu fakturazio atzeratua - arina](../proforma-invoicing/manage-billing-backlog-sales.md#product-billing-backlog).
  - API berriak Dynamics 365-en Dataverse baimendu eragiketak sortu, eguneratu eta ezabatzearekin **Programazio entitateak**. Informazio gehiagorako, ikusi [Erabili Programazio APIak Planifikazio entitateekin eragiketak egiteko](../../project-management/schedule-api-preview.md).

## <a name="quality-updates"></a>Kalitatearen eguneratzeak

| **Ezaugarrien eremua** | **Erreferentzia-zenbakia** | **Kalitatearen eguneratzea** |
| --- | --- | --- |
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
