---
title: Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko
description: Gai honek prezio-dimentsioetarako plugin atributuak eguneratzeko informazioa eskaintzen du.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: dynamics-365-customerservice
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: f215555dd7b29444e00499c0e731624e51057250
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071119"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a>Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko

> [!NOTE]
> Project Service Automation-en (PSA) Aurrekontua eta Kontratazioa eginbidea erabiltzen ari ez bazara, gai hau salta dezakezu.

Gai honek honako gai hauetan azaldutako prozedurak bete dituzula suposatzen du: [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities.md), [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan](field-references.md), eta [Ezarri eremu pertsonalizatuak prezioen dimentsio gisa](set-up-pricing-dimensions.md). Prozedura horiek bete ez badituzu, itzuli, bete itzazu eta, ondoren, itzuli gai honetara.

Eskaintzaren lerroaren xehetasunak sortzen direnean **Eskaintzaren lerroa** orrialdean proiektu baten eskaintzaren lerro baterako, sistemak bi estimazio lerro sortzen ditu atzeko planoan: lerro bat kostuen aldeko estimaziorako eta, bestea, salmenten aldeko estimaziorako. Gauza bera gertatzen da proiektuaren kontratuaren lerroarekin.

Kostuaren aldeko kopuruari edo eremuari aldaketaren bat egiten diozunean, aldaketa hori salmenten aldera hedatzen da. Jarraian agertzen diren pluginen ondorioz gertatzen da hori, zeina berriro erregistratu behar den prezio-dimentsioei aldaketaren bat egin ondoren.

- PreOperationContractLineDetailUpdate - Eguneratzeak **msdyn_orderlinetransaction**.
- PreOperationQuoteLineDetailUpdate - Eguneratzeak **msdyn_quotelinetransaction**.

Hurrengo urratsek pluginak erregistratzeko prozesua azaltzen dute.

1. Ireki **PluginRegistrationTool** eta konektatu zure lineako instantziara.
2. Egin klik **Bilatu** aukeran eta bilatu eguneratu behar den plugina.

 ![Bilaketa zuhaitzaren pantaila-argazkia](media/PRT-1.png)

3. Plugina aurkitu ondoren, hautatu eta egin klik **Hautatu Inprimaki nagusian**.

4. Hautatu eguneratu beharreko pluginaren urratsa, egin klik eskuineko botoiarekin eta, ondoren, hautatu **Eguneratu**.

 ![Eguneratu beharreko pluginaren pantaila-argazkia](media/PRT-2.png)
 
5. Eguneratze leihoan, sakatu elipsia ( **...** ) iragazkiaren atributuetan.

 ![Eguneratzeko lehendik dagoen urratsaren konfigurazioaren informazioa](media/PRT-3.png)
 
6. Hautatu prezioaren atributuaren kontrol-laukiak.

 ![Prezio-atributuetarako kontrol-laukien hautaketa erakusten duen pantaila-argazkia](media/PRT-4.png)

7. Egin klik **Ados** aukeran orria ixteko eta, ondoren, hautatu **Eguneratu urratsa**.

 !["Eguneratu urratsa" botoia erakusten duen pantaila-argazkia](media/PRT-5.png)
 
8. Errepikatu prozesu hori bigarren pluginarekin, **PreOperationQuoteLineDetail - msdyn_quotelinetransaction eguneratzea**.

9. Itxi plugina erregistratzeko tresna.
