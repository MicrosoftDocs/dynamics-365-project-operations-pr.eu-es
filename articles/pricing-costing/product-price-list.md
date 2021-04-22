---
title: Produktuaren prezio-zerrendak
description: Gai honek proiektuen aurrekontuetarako eta kontratuetarako erabilitako katalogoko prezioen zerrendei buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 04/05/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e37f0bf9eef946ab4ebd658cef4e1269cbaf686d
ms.sourcegitcommit: ac90be6106592f883a0de39a75836fb40255d65a
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/09/2021
ms.locfileid: "5877475"
---
# <a name="product-price-lists"></a>Produktuaren prezio-zerrendak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

 Project Operations-en, **Produktuen prezioen zerrendak** eta erlazionatutako prezioen zerrendako elementu entitateek produktuak oinarritutako aurrekontu eta kontratu lerroetan produktuak tasatzeko funtzionalitatea onartzen dute. Proiektuetan erabilitako produktuetarako, proiektuen prezio zerrendetako prezioen zerrendako elementuen erregistroak erabiltzen dira. 

Produktuak produktuen katalogoan kostu eta prezio zerrendak lehenetsi behar dira. Erabili zerrenda prezioa, kostu estandarra eta uneko kostua kostu lehenetsiak eta zerrenda prezioak konfiguratzeko. Lehenetsitako zerrenda-prezioak aurrekontu-lerro batean edo proiektu-kontratuaren lerroan erabiltzen dira sistemak ezin badu produktu horren prezio-lerro bat aurkitu produktuen prezioen zerrendan aurrekontuaren edo proiektuaren kontratuan.

Produktuen katalogoko lineen kostu prezioa aldatu egin daiteke aurrekontuen artean. Gaitasun hau garrantzitsua da, izan ere, kostuak zehatz-mehatz kontrolatzen ez badituzu, ezin dituzu proiektuen konpromisoetan etekin operatiboak zehaztu. Lehenespenez, kostua produktuaren unitate bakoitzeko, kostuaren prezioa da. Hala ere, aurrekontuaren kostu lehenetsia aurrekontuaren lerroan eguneratu daiteke aurrekontu horren kostu desberdina badago.

## <a name="price-list-items"></a>Prezio-zerrendako elementuak

Produktuen katalogoko produktuak prezioen zerrendetara gehitu ditzakezu. Produktuen prezioen zerrenda-lerroek unitate zehatz bat aipatzen dute beti. Prezioen zerrendako produktuen prezioa moneta kopuru gisa konfigura daiteke. Bestela, zerrenda prezioaren, uneko kostuaren edo estandar kostuaren funtzio gisa konfigura daiteke.

Prezioen funtzionalitateak biribiltze aukera ugari onartzen ditu produktu-prezioak zerrenda prezioaren, kostu estandarraren edo uneko kostuaren funtzio gisa konfiguratutakoan. Prezio metodo ugari eta biribiltzeko aukerak aprobetxatzeaz gain, deskontu zerrendak prezioen zerrendako elementuekin lotu ditzakezu. 

 
## <a name="default-product-price-list"></a>Prezio-zerrenda lehenetsia
Bezeroen erregistro bakoitzak **Lehenetsitako prezioen zerrenda** eremua, non bezeroaren moneta bat datorren prezioen zerrenda zehaztu dezakezu. Balio lehenetsia ez da automatikoki sartuko eremu honetan. Bezero jakin batekin prezioen akordio pertsonalizatua dagoenean, eremu hau prezioen zerrenda bezero horrekin lotzeko erabil dezakezu.

Aukera, aurrekontua eta Proiektuen kontratuaren entitateek produktu honen prezioen zerrendetan lehenetsitako agindua erabiltzen dute. Eskaera bera erabiltzen da proiektuaren prezioen zerrendetan.

1.  Eskaintza
2.  Abagunea
3.  Bezeroa
4.  Ezarpen orokorrak 

Berez, **Produktua** eskaintzaren lerroko eremuan produktuen prezioen zerrendako produktu aktibo guztiak agertzen dira. Produktu bat aktibatuta egon bada edo produktu zirriborroa bada, ez da zerrendatzen, nahiz eta prezioen zerrendan egon. 

Produktuen katalogoko lineak faktura-lerro gisa gehitzen dira proiektuko kontratu baterako sortzen den lehen fakturan. Zerga faktura batean, faktura lerro horiek ezaba daitezke. Kasu horretan, lerroak ondorengo faktura batean agertuko dira fakturatu arte edo faktura bezeroari bidali arte. Ezin duzu produktuen faktura-lerro bateko kantitate partziala fakturatu. Proiektuko kontratuaren produktu-lerroak fakturatzen direnean, errealak sortzen dira. Hala ere, egiazkoak ez daude lotuta proiektuaren entitatearekin. Alegia, produktuetan oinarritutako proiektuen kontratu-ildoak proiektuan oinarritutako edozein erabilerarekiko independentea dira. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
