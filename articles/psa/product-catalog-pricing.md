---
title: Produktuen katalogoaren prezioak
description: Gai honek produktuen katalogoaren prezioek nola funtzionatzen duten informazioa eskaintzen du Dynamics 365 Project Service Automation-en (PSA).
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 6cf50a09226bd6fdb803fd1fd379fec80838be75
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8600635"
---
# <a name="product-catalog-pricing"></a>Produktuen katalogoaren prezioak 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


Prezio-zerrendak eta prezioen zerrendako entitateek produktuaren katalogoaren prezioei laguntza ematen diete. Gehienetan, funtzionalitate hau katalogoan oinarritutako ildoetarako erabiltzen da proiektuaren aurrekontuetan eta proiektuen kontratuetan.

Proiektuetan oinarritutako ildoetarako, kontratu batek akordioa irabazi ondoren adierazten du. Negoziazio prozesua irabazi aurretik, izan ere, aurrekontuari atxikitako prezioak beti kopiatzen dira prezioen zerrenda berri batean eta kontratuaren erantsita. Prezioen zerrenda berri hau ezin da aldatu kontratuaren eremutik kanpo. Muga horrek prezioen zerrenda nagusian gertatzen diren prezio aldaketetatik negoziatutako tasa txartela babesten laguntzen du.

Produktuak produktuen katalogoan kostu eta prezio zerrendak lehenetsi behar dira. Zerrenda prezioa, kostu estandarra eta uneko kostua erabili behar dituzu kostu lehenetsiak eta zerrenda prezioak konfiguratzeko. Lehenetsitako zerrenda-prezioak aurrekontu-lerro batean edo proiektu-kontratuaren lerroan erabiltzen dira sistemak ezin badu produktu horren prezio-lerro bat aurkitu produktuen prezioen zerrendan aurrekontuaren edo proiektuaren kontratuan.

Produktuen katalogoko lineen kostu prezioa aldatu egin daiteke aurrekontuen artean. Gaitasun hau garrantzitsua da, izan ere, kostuak zehatz-mehatz kontrolatzen ez badituzu, ezin dituzu proiektuen konpromisoetan etekin operatiboak zehaztu. Lehenespenez, kostua produktuaren unitate bakoitzeko, kostuaren prezioa da. Hala ere, aurrekontuaren kostu lehenetsia aurrekontuaren lerroan eguneratu daiteke aurrekontu horren kostu desberdina badago.

## <a name="price-list-items"></a>Prezio-zerrendako elementuak

Produktuen katalogoko produktuak prezioen zerrendetara gehitu ditzakezu. Produktuen prezioen zerrenda-lerroek unitate zehatz bat aipatzen dute beti. Prezioen zerrendako produktuen prezioa moneta kopuru gisa konfigura daiteke. Bestela, zerrenda prezioaren, uneko kostuaren edo estandar kostuaren funtzio gisa konfigura daiteke.

PSAk biribiltze aukera ugari onartzen ditu prezioak zerrenda prezioaren, kostu estandarraren edo uneko kostuaren funtzio gisa konfiguratutakoan. Prezio metodo ugari eta biribiltzeko aukerak aprobetxatzeaz gain, deskontu zerrendak prezioen zerrendako elementuekin lotu ditzakezu. 

> ![Produktuen katalogoko produktuak prezioen zerrendetara gehitu.](media/basic-guide-16.png)

Aurrekontuen zerrenda pertsonalizatuko zerrenda berria sortzen duzunean, hautatuta **Sortu pertsonalizatutako prezioak** orrian **Proiektuaren eskaintza** orrialdea, PSAk prezioen zerrendaren kopia egiten du eta **Erakundea** prezioen zerrenda berriaren goiburuko eremuan ezarrita dago **Salmenta-erakundea**. Prezioen zerrenda berriaren izena aurrekontuaren izenarekin eta marka-denborarekin eransten da. Prezioen zerrenda berriaren izena eta aurrekontuaren izena erabil ditzakezu laneko fluxu pertsonalizatuetan, berrikuspen eta onarpen osagarriak abiarazteko prezio pertsonalizatuak erabiltzen dituzten aurrekontuetarako.

 
## <a name="default-product-price-list"></a>Prezio-zerrenda lehenetsia
Bezeroen erregistro bakoitzak **Lehenetsitako prezioen zerrenda** eremua, non bezeroaren moneta bat datorren prezioen zerrenda zehaztu dezakezu. PSAn, balio lehenetsia ez da automatikoki sartuko eremu honetan. Bezero jakin batekin prezioen akordio pertsonalizatua dagoenean, eremu hau prezioen zerrenda bezero horrekin lotzeko erabil dezakezu.

Aukera, aurrekontua eta Proiektuen kontratuaren entitateek produktu honen prezioen zerrendetan lehenetsitako agindua erabiltzen dute. Eskaera bera erabiltzen da proiektuaren prezioen zerrendetan.

1.  Eskaintza
2.  Abagunea
3.  Bezeroa
4.  Ezarpen orokorrak PSAn

Berez, **Produktua** eskaintzaren lerroko eremuan produktuen prezioen zerrendako produktu aktibo guztiak agertzen dira. Produktu bat aktibatuta egon bada edo produktu zirriborroa bada, ez da zerrendatzen, nahiz eta prezioen zerrendan egon. 

Produktuen katalogoko lineak faktura-lerro gisa gehitzen dira proiektuko kontratu baterako sortzen den lehen fakturan. Zerga faktura batean, faktura lerro horiek ezaba daitezke. Kasu horretan, lerroak ondorengo faktura batean agertuko dira fakturatu arte edo faktura bezeroari bidali arte. PSAn, ezin duzu produktuen faktura-lerro bateko kantitate partziala fakturatu. Proiektuko kontratuaren produktu-lerroak fakturatzen direnean, errealak sortzen dira. Hala ere, egiazkoak ez daude lotuta proiektuaren entitatearekin. Alegia, produktuetan oinarritutako proiektuen kontratu-ildoak proiektuan oinarritutako edozein erabilerarekiko independentea dira. PSAk ez du materialen kontsumoa kontrolatzen proiektuetan.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
