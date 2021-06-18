---
title: Kudeatu proiektuetan oinarritutako abaguneak
description: Gai honek proiektuekin erlazionatutako aukerekin lan egiteko moduari buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: aebff4d3a94735e76bcb9cafd25a058207dae846
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996326"
---
# <a name="manage-project-based-opportunities"></a>Kudeatu proiektuetan oinarritutako abaguneak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuetan oinarritutako konpainiek herrialde eta geografi anitzetan banatzeko eragiketak izaten dituzte. Proiektuaren exekuzioaren eta entregaren kostua alda daiteke banaketa kudeatzen duen geografiaren edo sailaren arabera. Aldiz, horrek akordioaren marjinetan eragina izan dezake. Proiektuetan oinarritutako zerbitzuak emateak giza baliabideen denbora kopuru handia, bidaiatzeko gastu handiak, kostu materialak eta bestelako gastuak dakartza normalean.

Dynamics 365 Project Operations-eko proiektuan oinarritutako abaguneak Dynamics 365 Sales-erako luzapenekin diseinatuta daude. Gaiak proiektuetan oinarritutako enpresek proiektuetan oinarritutako aukerak kudeatzeko eskatzen duten funtzionalitate osagarriaren barne dauden arlo eta negozio logikari buruzko xehetasunak eskaintzen ditu.

## <a name="view-all-project-based-opportunities"></a>Ikusi proiektuetan oinarritutako abagune guztiak

Proiektuetan oinarritutako aukera guztien zerrenda ikus daiteke **Abagunea** zerrenda orria. 

1. Joan **Salmentak** > **Abaguneak** atalera.
2. Erabili **Ikusi aldatzailea** aukeren iragazitako beste ikuspegi batzuk hautatzeko. Ikuspegi propioak sor ditzakezu iragazki pertsonalizatuko irizpideekin ikuspegi eta nabigazio aukera hauek konfiguratzeko.

Proiektuaren abaguneak zerrenda edo orrialde honetatik sortu edo ezabatu daitezke.

## <a name="business-process-flow-for-project-based-deals"></a>Negozio-prozesuaren fluxu proiektuetan oinarritutako akordioetarako

Ondorengo negozio-prozesuen fluxuak onartzen dira proiektuetan oinarritutako Project Operations-en:

- Bezerogaitik abagunerako negozio-prozesua
- Abagune-salmenten prozesua

### <a name="lead-to-opportunity-business-process"></a>Bezerogaitik abagunerako negozio-prozesua 
Bezerogaitik abagunerako negozio-prozesuak fase hauek onartzen ditu:

| Fasea | Esleitutako entitatea | Funtzioa |
| --- | --- | --- |
| Gaitu | Bezerogaia | Gaitu bezerogaia kontu, kontaktu eta abagune bat sortzeko. |
| Garatu | Abagunea | Garatu aukera inplikatutako lanari, funtsezko eragileei eta lehiari buruzko informazio gehiago gehitzeko. |
| Proposatu | Abagunea | Garatu proposamena eta lortu barne ebaluazio taldearen onespena. |
| Itxi | Abagunea | Irabazi abagunea mahuka ixteko. |

### <a name="opportunity-sales-process"></a>Abagune-salmenten prozesua
Project Operations-en Aukera salmenta prozesua Salmenta aplikazioko Aukera salmenta prozesuaren negozio fluxuaren luzapena da. Negozio prozesu hau premiazko diseinatuta dago proiektuan oinarritutako aukera batean hurrengo faseak laguntzeko.

| Fasea | Esleitutako entitatea | Funtzioa |
| --- | --- | --- |
| Gaitu | Abagunea | Gaitu bezerogaia kontu, kontaktu eta abagune bat sortzeko. |
| Proposatu | Eskaintza | Garatu proposamena proiektuaren eskaintzak erabiliz, eta lortu barne ebaluazio taldearen onespena. |
| Kontratua | Proiektu-kontratua | Irabazi aurrekontua kontratua sortzeko eta proiektuaren exekuzioa eta entrega ematen hasteko. |
| Itxi | Proiektu-kontratua | Amaitu lana ongi eta itxi proiektuaren kontratua. |

> [!NOTE]
> Zure proiektuan oinarritutako akordioa Bezerogai batekin hasi bada, Bezerogaitik Abagunera negozio prozesuak lehentasuna du.
>
> Zure proiektuan oinarritutako akordioa Abagune batekin hasi bada, Bezerogai-salmenten negozio prozesuak lehentasuna du.

Negozio-prozesuaren fluxu produktua editatu edo zure negozio prozesuen fluxuak sor ditzakezu zure salmenta prozesua behar bezala jarraitzeko. Negozio-prozesuaren fluxuari buruz gehiago jakiteko, ikusi [Negozio-prozesuaren fluxu informazio orokorra](/dynamics365/customerengagement/on-premises/customize/business-process-flows-overview).


[!INCLUDE[footer-include](../includes/footer-banner.md)]