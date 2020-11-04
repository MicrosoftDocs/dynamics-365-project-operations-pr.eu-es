---
title: Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak
description: Gai honek produktuen katalogoan dauden elementuen kostua eta salmenta tasak konfiguratzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5178a9143536bf4b2573403125325017861cdd5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071103"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products"></a>Konfiguratu katalogoko produktuen kostu- eta salmenta-tasak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_


Produktuen katalogoko elementuen prezioak konfiguratzea Dynamics 365 Project Operations-en Dynamics 365 Sales-en bezalakoa da.

Produktuak Project Operations-en proiektuetan ezin direnez kalkulatu edo erabili, ez da beharrezkoa produktuen katalogoaren prezioak finkatzea proiektuen prezioen zerrendetan aurrekontu eta kontratuetarako.

Produktuen katalogoaren prezioak atalean ezarri behar dira **Produktuaren prezioa** aurrekontu, kontratu edo kontu baten eremua. Ez ezarri produktu horien katalogoaren prezioak proiektu horietako entitateen prezioen zerrendetan. Project Operations-en zerrendak proiektuaren eragiketetarako soilik dira. Aplikazio espezifikoen negozio logika dago, prezioen zerrendak aurrekontu batetik kontratu batera kopiatzen dituena. Emaitza kontratuaren araberako proiektuaren prezio-zerrenda da. Kopiatze eragiketak aurrekontua irabazteko prozesua atzeratu dezake aurrekontuaren proiektuaren prezio zerrenda handiegia bada. Produktuen prezioen zerrendak ez dira kopiatzen kontratuetako prezioen zerrenda pertsonalizatuak sortzeko. Horrek esan nahi du produktuen prezioen zerrendek ez dutela aurrekontua irabazteko prozesuaren errendimenduan eraginik.
