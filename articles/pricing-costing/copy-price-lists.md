---
title: Kopiatu prezio-zerrendak
description: Gai honek prezio-zerrendak kopiatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 10/13/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 9e4f4eeda019f2af11a0d7a4469c41ee450eb03b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001411"
---
# <a name="copy-price-lists"></a>Kopiatu prezio-zerrendak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Prezio zerrenden kopiak hemen sor ditzakezu Dynamics 365 Project Operations-en. Adibidez, hurrengo urteko prezioen zerrendak sor ditzakezu uneko urteko prezioen zerrenda erabiliz.  Edo, fakturen tasen eta salmenta prezioen prezioen zerrenda kopiatu dezakezu kostuaren prezioen zerrendetatik. 

Prezioen zerrendaren kopia bat egiteko, jarraitu urrats hauek.

1. Ireki kopia bat egin nahi duzun prezio zerrenda eta hautatu **Kopiatu**.
2. Sartu beharrezko informazioa prezioen zerrenda kopiatzeko. Hurrengo taulan informazioa sartzerakoan kontuan hartu beharreko gogoetak agertzen dira.

| Eremua | Deskribapena | Downstream eragina |
| --- | --- | --- |
| Eman izena | Iturriaren prezioen zerrendaren izena **kopia** erantsita. | Prezioen zerrendak balio hori zerrendako orrialde eta goitibeherako aukera guztietan biltzen du. |
| Testuingurua | Idatzi helburuko prezioen zerrendarako nahi duzun testuingurua. | Testuingurua ezarrita duen prezio zerrenda **Kostua** kalkulatzeko eta kostuen benetako prezioa bilatzeko erabiltzen da. Testuingurua ezarrita duen prezio zerrenda **Salmenta** kalkulatzeko eta salmenten benetako prezioa bilatzeko erabiltzen da. Testuingurua ezarrita duten prezioen zerrendak soilik **Salmentak** bezeroaren, aurrekontuen edo kontratuaren proiektuen prezioen zerrendara erants daiteke. |
| Hasiera-data | Prezioen zerrenda dagoen aldiaren hasiera-data eraginkorra da. | **Amaiera-data** eremuarekin batera, eremu hau estimazio jakin baterako edo benetako lerro baterako zein prezio-zerrenda aplikagarri den jakiteko erabiltzen da. |
| Amaiera-data | Prezioen zerrenda dagoen aldiaren amaiera-data eraginkorra da. | **Hasiera-data** eremuarekin batera, eremu hau estimazio jakin baterako edo benetako lerro baterako zein prezio-zerrenda aplikagarri den jakiteko erabiltzen da. |
| Moneta | Iturburu prezioen zerrendaren moneta. Hori alda daiteke. | Hori aldatzen denean, eskulanaren, gastuaren eta produktuen katalogoaren ondoriozko prezio lerro guztiak kopiatzerakoan helburuko prezioen zerrendako monetara bihurtuko dira. |
| Denbora-unitatea | Iturburu prezioen zerrendaren moneta. Hori alda daiteke. | Hori aldatzen denean, eskulanaren ondoriozko prezio lerro guztiak kopiatzerakoan helburuko prezioen zerrendako unitatera bihurtuko dira. Unitatearen konfigurazioko iturburuko prezioen zerrendako denbora unitatearen eta helburu prezioen zerrendaren denbora unitatearen bihurketa erabiltzen da. |
| Deskribapena | Iturriaren prezioen zerrendaren deskribapena **kopia** erantsita. Testu eremua da eta prezio zerrendaren lerro anitzeko deskribapena egiteko aukera ematen du. | Eremu hau **Elkartua** erlazionatutako prezio zerrendak dituzten hainbat erakundetako prezioen zerrendari buruzko ikuspegiak. |

3. Gorde prezio-zerrenda. 

## <a name="update-a-price-list-by-applying-a-mark-up-to-all-the-prices"></a>Eguneratu prezioen zerrenda prezio guztiei marka gehituz

1. **Funtzioa**, **Kategoria** eta **Prezioen zerrendako elementua** prezioen zerrenda baten fitxak, hauta ditzakezu **Eguneratu prezioak** azpisareko prezio guztiei marka bat aplikatzeko. 
2. Irekitzen den elkarrizketa-orrian, sartu marka bat. Halaber, ehuneko negatiboa gehi dezakezu prezioak ehuneko jakin batean jaisteko. 
3. Aukeratu **Ados** elkarrizketa-orrian eta egiaztatu azpisareko prezioek egindako aldaketak islatzen dituztela.


[!INCLUDE[footer-include](../includes/footer-banner.md)]