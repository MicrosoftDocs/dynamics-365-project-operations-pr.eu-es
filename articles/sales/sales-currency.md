---
title: Moneta
description: Gai honek proiektuaren eragiketetan moneta motak nola gehitu eta kentzeari buruzko informazioa eskaintzen du.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: d53bae2f64e7b427f762161ff08917598217bb5a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898336"
---
# <a name="currency"></a>Moneta

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Monetek produktuen katalogoko produktuen prezioak eta transakzioen kostua zehazten dituzte, hala nola salmenta-eskaerak. Bezeroak toki askotan badituzu, gehitu diruak transakzioak kudeatzeko. Gehitu zure uneko eta etorkizuneko negozioaren beharretarako egokiak diren monetak.  

> [!NOTE]
> Zure ingurunea Common Data Service ingurumena, zu zara Power Platform administrazio-zentroa eta aukeratu duzu **Monetak** orria (**Inguruneak** > [hautatu ingurunea]> **Ezarpenak** > **Negozioa** > **Monetak**), orria hutsik egongo da. Hau moneta ezarrita ez dago onartzen delako Common Data Service nguruneak.

## <a name="add-a-currency"></a>Moneta bat gehitu  
Prozedura hau hasi aurretik, egiaztatu zure segurtasun-funtzio-k sistemaren administratzaile baimenak dituela. 

1. Power Platform administrazio-zentroan, hautatu ingurune bat. 
2. Hautatu **Ezarpenak** > **Negozioa**.
3. Hautatu **Moneta**.  
4. Hautatu **Berria**.  
5. Informazioa bete, behar bezala.  


   |          Eremua          |                                                                                                                                                                                                                                                                                                                                                                            Azalpena                                                                                                                                                                                                                                                                                                                                                                            |
   |-------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   |    **Moneta mota**    | - **Sistema**: hautatu aukera hau moneta erabilgarriak erabili nahi badituzu ereduetan oinarritutako Dynamics 365-ko aplikazioetan. Hautatu **Bilatu**, moneta bat bilatzeko. Monetaren kode bat hautatzen duzunean, hautatutako monetaren **Monetaren izena** eta **Moneta-ikurra** automatikoki gehituko dira.<br />- **Pertsonalizatu**: hautatu aukera hau erabilgarri ez dagoen moneta bat gehitzeko ereduetan oinarritutako Dynamics 365-ko aplikazioetan. Kasu honetan, eskuz idatzi behar dituzu balio hauek: **Monetaren kodea**, **Monetaren zehaztasuna**, **Monetaren izena**, **Moneta-ikurra** eta **Monetaren bihurketa**. |
   |    **Monetaren kodea**    |                                                                                                                                                                                                                                                                                                                                            Monetaren forma laburra. Adibidez, **USD** AEBetako dolarra.                                                                                                                                                                                                                                                                                                                                            |
   | **Monetaren zehaztasuna**  |                                                                                                                                                                                  Idatzi moneta gisa erabili nahi duzun hamartarren kopurua.  0 eta 4 arteko balio bat gehi dezakezu. **Oharra:**  Doitasun-balio bat ezarri baduzu **Sistemaren ezarpenak** elkarrizketa-koadroan, balio hori agertuko da hemen.                                                                                                                                                                                  |
   |    **Monetaren izena**    |                                                                                                                                                                                                                                         Ereduetan oinarritutako Dynamics 365-ko aplikazioetan erabilgarri dauden moneten zerrendatik moneta-kode bat hautatzen baduzu, hautatutako kodearen moneta-izena bistaratuko da hemen. **Pertsonalizatua** hautatu baduzu moneta mota gisa, idatzi monetaren izena.                                                                                                                                                                                                                                          |
   |   **Moneta-ikurra**   |                                                                                                                                                                                                                                                                      Erabilgarri dauden moneten zerrendatik moneta-kode bat hautatzen baduzu, hautatutako monetaren ikurra bistaratuko da hemen. **Pertsonalizatua** hautatu baduzu moneta mota gisa, idatzi moneta berriaren ikurra.                                                                                                                                                                                                                                                                       |
   | **Monetaren bihurketa** |                                                                                                                                                                                                                                     Idatzi hautatutako monetaren balioa AEBko dolar baten baldintzetan. Zenbatekoa burtsa hautatutako moneta bihurtzen oinarrizko moneta da. **Garrantzitsua:** Ziurtatu duzu eguneratu balioa gisa maiz zure transakzioetan kalkuluak zehatza edozein saihesteko behar bezala.                                                                                                                                                                                                                                      |


6. Amaitutakoan, komando-barran, aukeratu **Gorde** edo **Gorde eta itxi**.  

   > [!TIP]
   >  Moneta editatzeko, hautatu moneta eta, ondoren, sartu edo hautatu balio berriak.  

## <a name="delete-a-currency"></a>Ezabatu moneta  

1. Power Platform administrazio-zentroan, hautatu ingurune bat. 
2. Hautatu **Ezarpenak** > **Negozioa**.
3. Hautatu **Moneta**.  
4. Bistaratu tako moneten zerrendatik, hautatu ezabatzeko moneta.  
5. Hautatu **Ezabatu**.  
6. Berretsi ezabatzea.  

> [!IMPORTANT]
>  Beste erregistro batzuek erabiltzen dituzten monetak ezin dira ezabatu; desaktibatu soilik egin ditzakezu. Moneta-erregistroak desaktibatzean, ez da erregistroetan gordetako monetaren informazioa ezabatzen, esaterako, abaguneak edo eskaerak. Hala ere, ezingo duzu desaktibatutako monetarik hautatu transakzio berrietarako.  
