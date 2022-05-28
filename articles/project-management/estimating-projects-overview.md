---
title: Aurreikuspen ekonomikoaren kontzeptuak
description: Gai honek proiektuen aurreikuspen ekonomikoaren inguruko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 03/22/2021
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 338d2924f0e2a4a7fb943686eaad421a892dce70
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8597737"
---
# <a name="financial-estimation-concepts"></a>Aurreikuspen ekonomikoaren kontzeptuak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Dynamics 365 Project Operations-en, ekonomikoki zure proiektuak bi etapatan kalkula ditzakezu: 
1. Aurre-salmenta fasean tratua irabazi aurretik. 
2. Proiektua kontratua sortu ondorengo exekuzio fasean. 

Proiektuetan oinarritutako lanen aurrekontu ekonomikoa sor dezakezu 3 orrialde hauetakoren bat erabiliz:
- **Eskaintzaren lerroa** orrialdea, aurrekontuaren lerroaren xehetasunak erabiliz.  
- **Proiektuaren kontratuaren lerroa** orrialdea, kontratuaren lerroaren xehetasunak erabiliz. 
- **Proiektua** orrialdean, **Zereginak** edo **Gastuen aurrekontuak** fitxa orriak.

## <a name="use-a-project-quote-to-create-an-estimate"></a>Erabili proiektuaren aurrekontua aurrekontua sortzeko
Proiektuetan oinarritutako eskaintzan, **Eskaintzaren lerroaren xehetasuna** entitatea erabil dezakezu proiektua entregatzeko behar den lana aurreikusteko. Aurreikuspen horiek bezeroarekin partekatu ditzakezu.

Proiektuan oinarritutako eskaintzaren lerroek zero edo hainbat eskaintzaren lerroren xehetasunak izan ditzake. Eskaintzaren lerroaren xehetasunak denbora, gastuak edo tasak aurreikusteko erabiltzen dira. Microsoft Dynamics 365 Project Operations-ek ez du eskaintzaren lerroaren xehetasunetan materialaren aurreikuspenik egiten. Hauek transakzio-klaseak deitzen dira. Aurreikusitako zergen zenbatekoak transakzio-klase batean ere sar daitezke.

Transakzio-klaseez gain, eskaintzaren lerroaren xehetasunek transakzio mota dute. Bi transakzio mota onartzen dira eskaintzaren lerroaren xehetasunak lortzeko: **Kostua** eta **Proiektu-kontratua**.

## <a name="use-a-project-contract-to-create-an-estimate"></a>Erabili proiektuaren kontratua aurrekontua sortzeko

Proiektuan oinarritutako kontratua sortu zenuenean eskaintza erabili bazenuen, eskaintzaren lerro bakoitzeko egin zenuen aurreikuspena proiektu-kontratuan kopiatzen da. Proiektu-kontratuaren egitura, lerroak, lerro xehetasunak eta fakturen egutegiak dituzten proiektu-eskaintzaren egitura bezalakoa da.

Aurreikuspenak proiektu-kontratuan zuzenean egin daitezke, proiektu-eskaintzan bezala. Proiektu-eskaintza lortzeko, aurreikuspena kontratuaren lerroak eta kontratuaren linearen xehetasunak erabiliz egiten da. Kontratuaren lerroko xehetasunak behetik gorako kalkulu ikuspegia erabiliz sortutako proiektu-planetik ere sor daitezke.

Kontratuaren lerroaren xehetasunak denbora, gastuak edo tasak aurreikusteko erabil daitezke. Aurreikusitako zergen zenbatekoak kontratuaren lerroaren xehetasunean ere sar daitezke.

Kontratuaren lerroaren xehetasunetan ez da onartzen materialaren aurreikuspenik.

## <a name="use-a-project-to-create-an-estimate"></a>Erabili proiektua aurrekontua sortzeko 

Proiektuetan denbora eta gastuak aurreikusi ditzakezu. Project Operations-en eragiketek ez dituzte onartzen proiektuen materialen edo tasen estimazioak.

Denboraren aurreikuspenak zeregin bat sortzen duzunean eta zeregina burutzeko beharrezkoa den baliabide generiko baten atributuak identifikatzen dira sortzen dira. Denboraren aurreikuspenak antolaketako zereginetatik sortzen dira. Denboraren aurreikuspenak ez dira sortzen taldeko kide generikoak sortzen badituzu egutegiaren antolaketatik kanpo.

Gastuen aurreikuspenak **Gastuen aurreikuspenak** orriko saretan sartzen dira.

Proiektu baterako aurrekontua sortzea praktika egokitzat jotzen da, proiektuaren planeko zeregin bakoitzaren eskuineko lanaren edo denboraren eta gastuen kalkulu zehatzak behetik gora egin ditzakezu. Ondoren, estimazio zehatz hau erabil dezakezu aurrekontu lerro bakoitzerako estimazioak sortzeko eta bezeroarentzako aurrekontu sinesgarriagoa eraikitzeko. Proiektuaren plana erabiliz aurrekontuaren lerroan aurrekontu zehatza inportatzen edo sortzen duzunean, Project Operations-ek inportatzen dituzte salmenten balioak eta kalkulu horien kostuak. Inportatu ondoren, errentagarritasuna, marjinak eta bideragarritasun metrikak ikus ditzakezu proiektuaren aurrekontuan.

## <a name="understanding-estimates"></a>Aurreikuspenak ulertzea

Erabili ondorengo taula enpresa-logika aurreikuspen-fasean ulertzeko gida gisa.

| Egoera                                                                                                                                                                                                                                                                                                                                          | Entitatearen erregistroa                                                                                                                                                                                                       | Transakzio mota | Transakzio-klasea | Informazio gehigarria                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------|-------------|-----------------------------------------------------------------------------------|
| Denboraren salmenten balioa eskaintza batean aurreikusi behar duzunean                                                                                                                                                                                                                                                                                    | Eskaintzaren lerroaren xehetasunaren (QLD) erregistroa sortu da                                                                                                                                                                               | Proiektu-kontratua | Time        | Salmenta-aldeen transakzioen jatorriaren eremua QLD errenkadak kostuaren alboko QLD aipatzen du |
|                                                                                                                                                                                                                                                                                     | Sistemak bigarren QLD erregistroa sortzen du, dagozkion kostu-balioak gordetzeko. Dirua ez den eremu guztiak sistemaren arabera kopiatzen dira salmenten QLD eta kostuaren QLDra.                                                                                                                                                                               | Kostua | Time        | Salmenta-aldeen eskaintzaren lerroaren xehetasunak (QLD) eremuko transakzioen jatorriaren errenkadak kostuaren alboko QLD aipatzen du |
| Denboraren salmenten balioa kontratu batean aurreikusi behar duzunean                                                                                                                                                                                                                                                                                 | Proiektuaren lerroaren xehetasunaren (CLD) erregistroa sortu da                                                                                                                                                                    | Proiektu-kontratua | Time        | Salmenta-aldeen transakzioen jatorriaren eremua CLD errenkadak kostuaren CLD aipatzen du      |
|                                                                                                                                                                                                                                                                                  | Sistemak bigarren CLD erregistroa sortzen du, dagozkion kostu-balioak gordetzeko. Dirua ez den eremu guztiak sistemaren arabera kopiatzen dira salmenten CLD eta kostuaren QLDra.                                                                                                                                                                    | Kostua | Time        | Salmenta-aldeen transakzioen jatorriaren eremua CLD errenkadak kostuaren CLD aipatzen du      |
| Erabiltzaileak proiektuaren zeregin batean baliabidea deskribatzen duenean                                                                                                                                                                                                                                                                                            | Aurreikusitako lerroaren erregistroa zereginaren salmenta balioa erakusteko zereginak beharrezko prezioen dimentsio guztiekin sortzean sortzen da. Funtzio- eta antolaketa-unitateak prezio-dimentsioak dira | Proiektu-kontratua | Ordua        |                                                                                   |
|     | Aurreikusitako lerroaren erregistroa zereginaren salmenta kostua erakusteko zereginak beharrezko prezioen dimentsio guztiekin sortzean sortzen da. Dirua ez den eremu guztiak sistemaren arabera kopiatzen dira salmenten aurreikuspenaren lerrotik kostuaren aurreikuspenaren lerrora. Funtzio- eta antolakuntza-unitatea prezio-dimentsioak dira, kostu- eta faktura-tasetan.                                                                                                                                                                                                                | Kostua             | Ordua           |                                                                                   |



## <a name="customize-the-quote-line-detail-and-contract-line-detail-entities"></a>Eskaintzaren lerroaren xehetasunak eta kontratuaren lerroaren xehetasun entitateak pertsonalizatu

Eskaintzaren lerroaren xehetasunean eremu pertsonalizatu bat gehitu baduzu eta sistemak sortzen duen erlazionatutako kostuaren lerroaren eremuaren balioa lehenetsi gisa sartu nahi baduzu, erabili **PreOperationContractLineDetailUpdate** eta **PreOperationQuoteLineDetailUpdate** pluginak erregistratzeko tresnak. Plugin horiek berriro erregistratu behar dira eskaintzaren lerroaren xehetasunak edo kontratuaren lerroaren xehetasunak aldatu ondoren. Prozesua amaitzeko, jarraitu urrats hauei:

1. Ireki PluginRegistrationTool eta konektatu zure lineako instantziara.
2. Hautatu **Bilatu** aukera eta bilatu eguneratu behar den plugina.
3. Hautatu plugina eta, ondoren, sakatu orri nagusian **Aukeratu** aukera.
4. Hautatu eguneratzeko pluginaren urratsa, egin klik eskuineko botoiarekin eta, ondoren, hautatu **Eguneratu**.
5. **Eguneratu dagoen urratsa** elkarrizketa-koadroan **Atributuak iragaztea** eremuan, hautatu elipsi botoia (**...**):
6. **Hautatu atributuak** elkarrizketa-koadroan, hautatu atributu pertsonalizatuen kontrol-koadroak.
7. Hautatu **Ados** aukera elkarrizketa-koadroa ixteko eta, ondoren, hautatu **Eguneratu urratsa**.
8. Errepikatu 1-7. urratsak bigarren pluginerako.
9. Itxi **PluginRegistrationTool** tresna.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
