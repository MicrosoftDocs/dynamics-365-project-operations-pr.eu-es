---
title: Produktuaren prezio-zerrendak
description: Gai honek proiektuen aurrekontuetarako eta kontratuetarako erabilitako katalogoko prezioen zerrendei buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 504aa90bfb478207059b5e2894a3990f9a4a5e9e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071104"
---
# <a name="product-price-lists"></a>Produktuaren prezio-zerrendak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Prezio-zerrendak eta prezioen zerrendako entitateek produktuaren katalogoaren prezioei laguntza ematen diete. Gehienetan, funtzionalitate hau katalogoan oinarritutako ildoetarako erabiltzen da proiektuaren aurrekontuetan eta proiektuen kontratuetan.

Proiektuetan oinarritutako ildoetarako, kontratu batek akordioa irabazi ondoren adierazten du. Negoziazio prozesua irabazi aurretik, izan ere, aurrekontuari atxikitako prezioak beti kopiatzen dira prezioen zerrenda berri batean eta kontratuaren erantsita. Prezioen zerrenda berri hau ezin da aldatu kontratuaren eremutik kanpo. Muga horrek prezioen zerrenda nagusian gertatzen diren prezio aldaketetatik negoziatutako tasa txartela babesten laguntzen du.

Produktuak produktuen katalogoan kostu eta prezio zerrendak lehenetsi behar dira. Erabili zerrenda prezioa, kostu estandarra eta uneko kostua kostu lehenetsiak eta zerrenda prezioak konfiguratzeko. Lehenetsitako zerrenda-prezioak aurrekontu-lerro batean edo proiektu-kontratuaren lerroan erabiltzen dira sistemak ezin badu produktu horren prezio-lerro bat aurkitu produktuen prezioen zerrendan aurrekontuaren edo proiektuaren kontratuan.

Produktuen katalogoko lineen kostu prezioa aldatu egin daiteke aurrekontuen artean. Gaitasun hau garrantzitsua da, izan ere, kostuak zehatz-mehatz kontrolatzen ez badituzu, ezin dituzu proiektuen konpromisoetan etekin operatiboak zehaztu. Lehenespenez, kostua produktuaren unitate bakoitzeko, kostuaren prezioa da. Hala ere, aurrekontuaren kostu lehenetsia aurrekontuaren lerroan eguneratu daiteke aurrekontu horren kostu desberdina badago.

## <a name="price-list-items"></a>Prezio-zerrendako elementuak

Produktuen katalogoko produktuak prezioen zerrendetara gehitu ditzakezu. Produktuen prezioen zerrenda-lerroek unitate zehatz bat aipatzen dute beti. Prezioen zerrendako produktuen prezioa moneta kopuru gisa konfigura daiteke. Bestela, zerrenda prezioaren, uneko kostuaren edo estandar kostuaren funtzio gisa konfigura daiteke.

PSAk biribiltze aukera ugari onartzen ditu prezioak zerrenda prezioaren, kostu estandarraren edo uneko kostuaren funtzio gisa konfiguratutakoan. Prezio metodo ugari eta biribiltzeko aukerak aprobetxatzeaz gain, deskontu zerrendak prezioen zerrendako elementuekin lotu ditzakezu. 

Aurrekontuen zerrenda pertsonalizatuko zerrenda berria sortzen duzunean, hautatuta **Sortu pertsonalizatutako prezioak** orrian **Proiektuaren eskaintza** orrialdea, prezioen zerrendaren kopia egiten du eta **Erakundea** prezioen zerrenda berriaren goiburuko eremuan ezarrita dago **Salmenta-erakundea**. Prezioen zerrenda berriaren izena aurrekontuaren izenarekin eta marka-denborarekin eransten da. Prezioen zerrenda berriaren izena eta aurrekontuaren izena erabil ditzakezu laneko fluxu pertsonalizatuetan, berrikuspen eta onarpen osagarriak abiarazteko prezio pertsonalizatuak erabiltzen dituzten aurrekontuetarako.

 
## <a name="default-product-price-list"></a>Prezio-zerrenda lehenetsia
Bezeroen erregistro bakoitzak **Lehenetsitako prezioen zerrenda** eremua, non bezeroaren moneta bat datorren prezioen zerrenda zehaztu dezakezu. Balio lehenetsia ez da automatikoki sartuko eremu honetan. Bezero jakin batekin prezioen akordio pertsonalizatua dagoenean, eremu hau prezioen zerrenda bezero horrekin lotzeko erabil dezakezu.

Aukera, aurrekontua eta Proiektuen kontratuaren entitateek produktu honen prezioen zerrendetan lehenetsitako agindua erabiltzen dute. Eskaera bera erabiltzen da proiektuaren prezioen zerrendetan.

1.  Eskaintza
2.  Abagunea
3.  Bezeroa
4.  Ezarpen orokorrak 

Berez, **Produktua** eskaintzaren lerroko eremuan produktuen prezioen zerrendako produktu aktibo guztiak agertzen dira. Produktu bat aktibatuta egon bada edo produktu zirriborroa bada, ez da zerrendatzen, nahiz eta prezioen zerrendan egon. 

Produktuen katalogoko lineak faktura-lerro gisa gehitzen dira proiektuko kontratu baterako sortzen den lehen fakturan. Zerga faktura batean, faktura lerro horiek ezaba daitezke. Kasu horretan, lerroak ondorengo faktura batean agertuko dira fakturatu arte edo faktura bezeroari bidali arte. Ezin duzu produktuen faktura-lerro bateko kantitate partziala fakturatu. Proiektuko kontratuaren produktu-lerroak fakturatzen direnean, errealak sortzen dira. Hala ere, egiazkoak ez daude lotuta proiektuaren entitatearekin. Alegia, produktuetan oinarritutako proiektuen kontratu-ildoak proiektuan oinarritutako edozein erabilerarekiko independentea dira. Ez da materialen kontsumoa kontrolatzen proiektuetan.
