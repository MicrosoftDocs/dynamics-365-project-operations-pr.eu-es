---
title: Konfiguratu kontratudun langileak eta azpikontratatutako ahalmena erakusteko Antolaketa-panela
description: Artikulu honetan, Schedule Boardek Microsoften Dynamics 365 Project Operations nola konfiguratu azaltzen du, azpikontratatutako baliabideen gaitasuna erakusteko, proiektuaren baliabide-betekizunei langileak ematean.
author: rumant
ms.date: 08/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: b965fd5011a575354f50c47081be198ab43248f9
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8919815"
---
# <a name="configure-schedule-board-to-show-contract-workers-and-subcontracted-capacity"></a>Konfiguratu kontratudun langileak eta azpikontratatutako ahalmena erakusteko Antolaketa-panela 

[!include [banner](../../includes/dataverse-preview.md)]

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Schedule BoardEk Microsoften Dynamics 365 Project Operations bi eratara erabil ditzake baliabideak:

- Baliabideen bilaketa orokorra, proiektuetan oinarritutako baliabideen betekizun espezifikorik gabe.
- Betekizunen berariazko baliabideak bilatzea, non proiektuaren betekizunak iradokitako baliabideetarako testuingurua emango duen.

Programazio-batzordeari azpikontratatutako baliabideen gaitasuna eta kontratatutako langileei jakinarazteko, eguneratzeak egin behar ditu programazio-batzarraren konfigurazioan. Eguneratze horien artean honako hauek sartzen dira: 
- Schedule Boarden konfigurazioa eguneratu baliabideak bilatzeko.
- Schedule Boarden konfigurazioa eguneratu, betekizunetan oinarritutako baliabideak bilatzeko.

## <a name="update-schedule-board-settings-for-general-resource-search"></a>Schedule Boarden konfigurazioa eguneratzea, baliabideak orokorrean bilatzeko
### <a name="update-filters-for-general-resource-search"></a>Baliabideen bilaketa orokorrerako iragazkiak eguneratzea
Baliabide bat bilatzean, programazio-taulan eskuragarri dauden iragazkiak eguneratu egin behar dira, kanpoko baliabideak ere bilatu ahal izateko, honako edozein edo guztiak zehaztuz:
  - Langile mota, erakutsitako baliabideak kontratatutako langileak edo langileak izan behar badira.
  - Baliabide bat izan behar duen enpresa hornitzailea.
  - Azpikontratu edo azpikontratu-lerro espezifiko batekoak diren baliabideak.
    
### <a name="update-retrieve-resource-query"></a>Baliabideen kontsulta berreskuratzea
Bilaketarako erabilitako kontsulta ere eguneratu egin behar da iragazki gehigarriko atributu horiek erabiltzeko. Erabili ondorengo urratsak Schedule Boarden konfigurazioa eguneratzeko, baliabideak oro har bilatzeko:  
1. Programazio-plaka espezifiko baterako programazio-plakaren **konfigurazioa irekitzea**.
2. Ireki **betile** orokorra eta beste konfigurazio batzuetaraino **deslazea**.
3. Atal honetako konfigurazio-aukeren zerrendan, eguneratu Project Operations Lite-rako aurrez zehaztutako filtro-diseinua **·** **.**
4. **Project Operations Lite-rako** aurrez zehaztutako baliabideak berreskuratzea kontsultarako **baliabideak** berreskuratzea.

![Schedule Boarden konfigurazioa eguneratzea, baliabideak orokorrean bilatzeko](../media/BoardSettings.png)  

## <a name="update-schedule-board-settings-for-requirementbased-resource-search"></a>Schedule Board-en konfigurazioa eguneratzea, betekizunetan oinarritutako baliabideak bilatzeko
### <a name="update-filters-for-requirement-specific-resource-search"></a>Betekizunen baliabide espezifikoak bilatzeko iragazkiak eguneratzea 
Baliabide bat bilatzean, programazio-taulan eskuragarri dauden iragazkiak eguneratu egin behar dira, kanpoko baliabideak ere bilatu ahal izateko, honako edozein edo guztiak zehaztuz:
 - Langile mota, erakutsitako baliabideak kontratatutako langileak edo langileak izan behar badira.
 - Baliabide bat izan behar duen enpresa hornitzailea.
 - Azpikontratu edo azpikontratu-lerro espezifiko batekoak diren baliabideak.

### <a name="update-retrieve-resource-query-for-requirement-specific-resource-search"></a>Betekizunen baliabide espezifikoak bilatzeko baliabideen kontsulta berreskuratzea eguneratzea 
Bilaketarako erabilitako kontsulta ere eguneratu egin behar da iragazki gehigarriko atributu horiek erabiltzeko. Erabili honako urrats hauek schedule board-aren konfigurazioa eguneratzeko, betekizunetan oinarritutako baliabideak bilatzeko:

1. Programazio-plaka espezifiko baterako programazio-plakaren konfigurazioa irekitzea **eta, ondoren, aurrez zehaztutako konfigurazioa** irekitzea, **betekizunen bilaketa espezifikoaren konfigurazioa irekitzeko.**
2. Ireki **betile** orokorra eta beste konfigurazio batzuetaraino **deslazea**.
3. Atal honetako konfigurazio-aukeren zerrendan, eguneratu Project Operations Lite-rako aurrez zehaztutako filtro-diseinua **·** **.**
4. **Project Operations Lite-rako** aurrez zehaztutako baliabideak berreskuratzea kontsultarako **baliabideak** berreskuratzea.
5. Ireki betilea **programazio motak** eta joan **Proiektura**.
6. Project-en konfigurazioan **,** Schedule Assistant Retrieve Resources Query **a** Default Retrieve Resources Query for Project Operations Lite **eta eguneratzea** Schedule Assistant Retrieve Constraints Query **to** Default Retrieve Constraints Query for Project Operations **Lite**.

![Schedule Board-en konfigurazioa eguneratzea, betekizunetan oinarritutako baliabideak bilatzeko](../media/SASettings.png)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
