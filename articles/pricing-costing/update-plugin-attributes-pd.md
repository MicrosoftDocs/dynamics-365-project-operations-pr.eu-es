---
title: Plugin-atributuak prezio-dimentsio berriak gehitzeko eguneratzen
description: Gai honek prezio-dimentsioetarako plugin atributuak eguneratzeko informazioa eskaintzen du.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 2ae502fea533d9f199ef5ee1cc85b623f08cbd84
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8919999"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a>Eguneratu plugin-atributuak prezio-dimentsio berriak gehitzeko

Gai honek prezio-dimentsioetarako plugin atributuak eguneratzeko informazioa eskaintzen du.

> [!NOTE]
> Gai hau aurrekontuaren eta kontratuaren ezaugarriei soilik aplikatzen zaie Dynamics 365 Project Operations.

## <a name="prerequisites"></a>Aurrebaldintzak
Gai honetako pausoak bete aurretik, gai hauetako prozedurak bete beharko dituzu:

  - [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities-pricing-dimensions.md) 
  - [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan ](add-custom-fields-price-setup-transactional-entities.md)
  - [Konfiguratu eremu pertsonalizatuak prezio-dimentsio gisa](set-up-custom-fields-pricing-dimensions.md). 
  
Prozedura horiek bete ez badituzu, bete itzazu eta, ondoren, itzuli gai honetara.

## <a name="register-a-plug-in"></a>Erregistratu plugina
Aurrekontuaren lerroaren xehetasuna sortzen denean **Aipatu lerroa** proiektuaren aurrekontu lerroaren orrialdea, sistemak bi estimazio lerro sortzen ditu. Lerro bat aurrekontuaren kostuaren aldekoa da eta beste lerroa salmenten aldekoa. Gauza bera gertatzen da proiektuaren kontratuaren lerroarekin.

Kostuaren aldeko kopuruari edo eremuari aldaketaren bat egiten diozunean, aldaketa hori salmenten aldean ere egiten da. Hori posible da, Quotelinedetaileko eta kontratatutako xehetasun entitateetako PreOperation plug-inek kostu aldetik atributu espezifikoak transakzioaren salmenten aldera konektatzen dituztelako. Salmenten aldetik prezioen dimentsio balioetan egindako aldaketak kostuaren aldetik ere egin behar badituzu, honako plug-in hauek berriro erregistratu beharko dira prezioen dimentsioan aldaketak egin ondoren.

Hauek dira eguneratzeko eta berriro erregistratzeko pluginak:

- PreOperationContractLineDetailUpdate - **Eguneratu msdyn_orderlinetransaction**
- PreOperationQuoteLineDetailUpdate - **msdyn_quotelinetransaction eguneratzen du**.

Osatu urrats hauek pluginak eguneratzeko eta berriro erregistratzeko.

1. Ireki **PluginRegistrationTool** eta konektatu zure Project Operations-en Dataverse ingurunea.
2. Aukeratu **Bilatu**, eta idatzi eguneratu beharreko pluginaren lehen hizkiak.
3. Plugina aurkitu ondoren, hautatu eta hautatu **Hautatu Inprimaki nagusian**.
4. Hautatu **Eguneratu msdyn_orderlinetransaction** urratsa, egin klik eskuineko botoiarekin eta, ondoren, hautatu **Eguneratu**.
5. **Eguneratu** elkarrizketa-leihoan, sakatu elipsia (**...**) iragazkiaren atributuetan.
6. Iragazteko atributuak leihoa ireki eta entitatearen atributu guztien zerrenda eta prezioen dimentsioak eskaintzen ditu. Hautatu prezioen dimentsio atributuen kontrol laukiak.
7. Hautatu **Ados** aukeran orria ixteko eta, ondoren, hautatu **Eguneratu urratsa**.
8. Errepikatu 2-7. urratsak bigarren pluginerako, **PreOperationQuoteLineDetail**. Plugin honetarako, **Eguneratu msdyn_quotelinetransaction** urratsa eguneratu behar duzu.
9. Itxi **PluginRegistrationTool**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]