---
title: Aurreikuspen-proiektuen informazio orokorra
description: Gai honek Dynamics 365 Project Operations-eko aurreikuspenei buruzko informazioa ematen du.
author: ruhercul
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4ff73c6efd5b21b91a7772c3733734d8008e00a3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286863"
---
# <a name="estimate-projects-overview"></a>Aurreikuspen-proiektuen informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuetan oinarritutako eskaintzan, **Eskaintzaren lerroaren xehetasuna** entitatea erabil dezakezu proiektua entregatzeko behar den lana aurreikusteko. Aurreikuspen horiek bezeroarekin partekatu ditzakezu.

Proiektuan oinarritutako eskaintzaren lerroek zero edo hainbat eskaintzaren lerroren xehetasunak izan ditzake. Eskaintzaren lerroaren xehetasunak denbora, gastuak edo tasak aurreikusteko erabiltzen dira. Microsoft Dynamics 365 Project Operations-ek ez du eskaintzaren lerroaren xehetasunetan materialaren aurreikuspenik egiten. Hauek transakzio-klaseak deitzen dira. Aurreikusitako zergen zenbatekoak transakzio-klase batean ere sar daitezke.

Transakzio-klaseez gain, eskaintzaren lerroaren xehetasunek transakzio mota dute. Bi transakzio mota onartzen dira eskaintzaren lerroaren xehetasunak lortzeko: **Kostua** eta **Proiektu-kontratua**.

## <a name="estimate-by-using-a-contract"></a>Aurreikusi kontratua erabiliz

Proiektuan oinarritutako kontratua sortu zenuenean eskaintza erabili bazenuen, eskaintzaren lerro bakoitzeko egin zenuen aurreikuspena proiektu-kontratuan kopiatzen da. Proiektu-kontratuaren egitura, lerroak, lerro xehetasunak eta fakturen egutegiak dituzten proiektu-eskaintzaren egitura bezalakoa da.

Aurreikuspenak proiektu-kontratuan zuzenean egin daitezke, proiektu-eskaintzan bezala. Proiektu-eskaintza lortzeko, aurreikuspena kontratuaren lerroak eta kontratuaren linearen xehetasunak erabiliz egiten da. Kontratuaren lerroko xehetasunak behetik gorako kalkulu ikuspegia erabiliz sortutako proiektu-planetik ere sor daitezke.

Kontratuaren lerroaren xehetasunak denbora, gastuak edo tasak aurreikusteko erabil daitezke. Aurreikusitako zergen zenbatekoak kontratuaren lerroaren xehetasunean ere sar daitezke.

Kontratuaren lerroaren xehetasunetan ez da onartzen materialaren aurreikuspenik.

Proiektu-kontratu batean onartzen diren prozesuak fakturak sortzea eta berrestea dira. Fakturak sortzeak proiektuan oinarritutako fakturaren zirriborroa sortzen du, fakturatu gabeko salmenten kontu guztiak barne hartzen dituena orain arte.

Baieztapenak kontratua irakurtzeko soilik egiten du eta egoera aldatu egiten da **Zirriborroa** aukera **Baieztatuta** aukerara aldatuz. Ekintza hau egin ondoren, ezin duzu desegin. Ekintza hau iraunkorra denez, praktika onena da kontratua **Zirriborroa** egoeran mantentzea.

Kontratuen zirriborroen eta kontratu berrien arteko desberdintasun bakarrak dira haien egoera eta kontratuen zirriborroak editatu daitezkeela, baieztatutako kontratuetan hori egin ezin den bitartean. Fakturen sorrera eta jarraipen errealak egin daitezke bai zirriborroetan bai baieztatutako kontratuetan.

Proiektu-eragiketek ez dute onartzen kontratu edo proiektuen aldaketa-eskaerarik.

## <a name="estimating-projects"></a>Proiektuak aurreikusten

Proiektuetan denbora eta gastuak aurreikusi ditzakezu. Proiektu-eragiketek ez dute proiektuen gaineko materialen edo tasen aurreikuspenik onartzen.

Denboraren aurreikuspenak zeregin bat sortzen duzunean eta zeregina burutzeko beharrezkoa den baliabide generiko baten atributuak identifikatzen dira sortzen dira. Denboraren aurreikuspenak antolaketako zereginetatik sortzen dira. Denboraren aurreikuspenak ez dira sortzen taldeko kide generikoak sortzen badituzu egutegiaren antolaketatik kanpo.

Gastuen aurreikuspenak **Aurreikuspenak** orriko saretan sartzen dira.

## <a name="understanding-estimation"></a>Aurreikuspena ulertzea

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