---
title: Proiektuetan oinarritutako kontratuak kopiatzea
description: Artikulu honek Microsoft-en proiektu-kontratuak kopiatzeari buruzko informazioa eskaintzen du Dynamics 365 Project Operations.
author: rumant
ms.date: 09/01/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 21994ef6d8f6e6cdf321599d107cc80368c96ecc
ms.sourcegitcommit: 16c9eded66d60d4c654872ff5a0267cccae9ef0e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/07/2022
ms.locfileid: "9410357"
---
# <a name="copy-project-based-contracts"></a>Proiektuetan oinarritutako kontratuak kopiatzea

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektu-kontratu berriak erraz sor ditzakezu lehendik dauden kontratuak bi modu hauetako batean kopiatuz:

- Gainean **Proiektu Kontratuak** zerrenda orria, hautatu proiektu-kontratua eta, gero, hautatu **Kopiatu**.
- **Proiektuaren kontratua** xehetasunen orrian, hautatu **Kopiatu**.

Bi kasuetan, elkarrizketa-koadro bat agertzen da, non kopiatutako kontratuaren parametroak ezar ditzakezun. Elkarrizketa-koadroak honako eremu hauek ditu. Hautatzen dituzun balioen arabera, kopia-prozesua alda daiteke.

| Eremua | Deskribapenak | Downstream eragina |
| --- | --- | --- |
| Gaia | Sartu helburuko kontratuaren gaia. Elkarrizketa-koadroa irekitzen denean, sistemak eremua iturburu-kontratuaren izena ezartzen du, baina "kopia" hitza eransten zaio. | Ez dago alor honen beherako eraginik. |
| bezero hori | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. Elkarrizketa-koadroa irekitzen denean, sistemak eremua ezartzen du iturburu-kontratuko kontuarekin. | Eremu hau kontratuaren bezero nagusia da. |
| Jabetzadun enpresa | Akordio honekin lotutako proiektuak entregatzeaz arduratzen den enpresa. Elkarrizketa-koadroa irekitzen denean, sistemak iturburu-kontratuaren enpresa jabeari ezartzen dio eremua. | Enpresa jabea tratua itxi ondoren proiektua gauzatuko duen pertsona juridikoa da. Enpresa jabearen moneta kontratazio-unitateko diruarekin bat etorri behar da. |
| Kontratatzailea | Akordio honekin lotutako proiektuak emateaz arduratzen den antolakuntza-unitatea. Elkarrizketa-koadroa irekitzen denean, sistemak eremua ezartzen du iturburu-kontratuaren kontratazio-unitatean. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek dute moneta bat. Moneta hau proiektuan zehar sortutako kostu estimatuak eta errealak jakinarazteko erabiltzen da. |
| Moneta | Eskaintzaren transakzioa zein dibisatan egingo den. Elkarrizketa-koadroa irekitzen denean, sistemak eremua iturburu-kontratuaren moneta ezartzen du. Ezin da aldatu moneta. Hala bada, **Kopiatu prezioak** eremua beti dago ezarrita **Ez**, iturri-kontratuko prezio-zerrendak jada ez direlako garrantzitsuak. | Moneta hau prezioen zerrenda lehenetsietarako erabiltzen da, kontratuaren finantza-estimazioak sortzeko eta bezeroari fakturatzeko akordioa irabazten denean. |
| Eskatutako entrega-data | Bezeroak eskatzen duen entrega-data. | Data hau amaiera data gisa erabiltzen da fakturazio-datak maiztasun zehatz batean sortzen dituzunean. |
| Kopiatu prezioak | Kontratuaren prezioa iturriko kontratutik kopiatu behar den ala ez adierazten duen balioa. | Eremua ezarrita badago **Bai**, proiektuaren eta produktuen prezioen zerrendako erreferentziak sorburu-kontratutik xede-kontratura kopiatzen dira. Ezarrita badago **Ez**, prezio-zerrenda lehenetsiak erabiltzen dira, kontuaren edo proiektuaren parametroetako azken prezio-zerrendetan oinarrituta. |

Hautatzen duzunean **Ados** elkarrizketa-koadroan, sistemak kontratuaren kopia bat sortzen du, zuk ezarritako parametroen balioetan oinarrituta. Ondoren, kontratu berria irekitzen da.

Hurrengo informazioa da **ez** sorburu-kontratutik xede-kontratura kopiatu da, kontratu bakoitzari berariazkoa baita:

- Fakturazio-antolaketak
- Kontratua eta kontratuaren lerroaren bezeroak
- Proiektuaren erreferentzia proiektuan oinarritutako kontratu lerroetan
- Bezeroaren aurrekontu-informazioa

Proiektu eta produktuen kontratu-lerroak, kontratu-lerroen xehetasunetan estimazioak eta kontratu mailan gainditu beharreko balioak kopiatzen dira. Lehenetsitako prezioak eta kostu-tasak sartzea aukeraketaren araberakoa da **Kopiatu prezioa** eremuan **Kopiatu Parametroak** elkarrizketa-koadroa.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
