---
title: Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko
description: Artikulu honetan, osagarriaren atributuak prezio-dimentsioetarako nola eguneratu behar diren ematen da.
author: Rumant
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 459aefb510cc9a9ec55a86ca7e362db98ccabb70
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8913191"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a>Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko

[!include [banner](../includes/psa-now-project-operations.md)]

> [!NOTE]
> Project Service Automation (PSA) kotizazio- eta kontratazio-ezaugarriak erabiltzen ari ez bazara, artikulu hau ez du eman.

Artikuluen prozedurak osatu ditu artikuluen prozedurak, [eremu eta erakunde](create-custom-fields-entities.md) pertsonalizatuak sortu ditu, [erakunde transakzionalei eremu pertsonalizatuak gehitu eta prezioak konfiguratu](field-references.md) ditu, eta [eremu pertsonalizatuak prezio-dimentsio gisa konfiguratu ditu](set-up-pricing-dimensions.md). Prozedura horiek bete ez badituzu, joan atzera eta osatu eta, ondoren, itzuli artikulu honetara.

Eskaintzaren lerroaren xehetasunak sortzen direnean **Eskaintzaren lerroa** orrialdean proiektu baten eskaintzaren lerro baterako, sistemak bi estimazio lerro sortzen ditu atzeko planoan: lerro bat kostuen aldeko estimaziorako eta, bestea, salmenten aldeko estimaziorako. Gauza bera gertatzen da proiektuaren kontratuaren lerroarekin.

Kostuaren aldeko kopuruari edo eremuari aldaketaren bat egiten diozunean, aldaketa hori salmenten aldera hedatzen da. Jarraian agertzen diren pluginen ondorioz gertatzen da hori, zeina berriro erregistratu behar den prezio-dimentsioei aldaketaren bat egin ondoren.

- PreOperationContractLineDetailUpdate - Eguneratzeak **msdyn_orderlinetransaction**.
- PreOperationQuoteLineDetailUpdate - Eguneratzeak **msdyn_quotelinetransaction**.

Hurrengo urratsek pluginak erregistratzeko prozesua azaltzen dute.

1. Ireki **PluginRegistrationTool** eta konektatu zure lineako instantziara.
2. Egin klik **Bilatu** aukeran eta bilatu eguneratu behar den plugina.

 ![Bilaketa zuhaitzaren pantaila-argazkia.](media/PRT-1.png)

3. Plugina aurkitu ondoren, hautatu eta egin klik **Hautatu Inprimaki nagusian**.

4. Hautatu eguneratu beharreko pluginaren urratsa, egin klik eskuineko botoiarekin eta, ondoren, hautatu **Eguneratu**.

 ![Eguneratu beharreko pluginaren pantaila-argazkia.](media/PRT-2.png)
 
5. Eguneratze leihoan, sakatu elipsia (**...**) iragazkiaren atributuetan.

 ![Eguneratzeko lehendik dagoen urratsaren konfigurazioaren informazioa.](media/PRT-3.png)
 
6. Hautatu prezioaren atributuaren kontrol-laukiak.

 ![Prezio-atributuetarako kontrol-laukien hautaketa erakusten duen pantaila-argazkia.](media/PRT-4.png)

7. Egin klik **Ados** aukeran orria ixteko eta, ondoren, hautatu **Eguneratu urratsa**.

 !["Eguneratu urratsa" botoia erakusten duen pantaila-argazkia.](media/PRT-5.png)
 
8. Errepikatu prozesu hori bigarren pluginarekin, **PreOperationQuoteLineDetail - msdyn_quotelinetransaction eguneratzea**.

9. Itxi plugina erregistratzeko tresna.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
