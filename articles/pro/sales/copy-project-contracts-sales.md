---
title: Proiektu-kontratuak kopiatzea
description: Gai honek proiektu-kontratuak kopiatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6da8e3ba8e062f3e06dc7f440caebdd93e496c65
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070941"
---
# <a name="copying-project-contracts"></a>Proiektu-kontratuak kopiatzea

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuen kontratu berriak erraz sor ditzakezu lehendik dauden kontratuen kopiak bi modu hauetako batean eginez: 

  - **Proiektuen kontratuak** zerrenda-orrian, hautatu proiektu-kontratua eta ondoren hautatu **Kopiatu**.
  - **Proiektuaren kontratua** xehetasunen orrian, hautatu **Kopiatu**.

Elkarrizketa-orria irekiko da eta bertan kopiatutako kontratuaren parametroak hauta ditzakezu. Eremu hauek izango dira elkarrizketan. Elkarrizketa honetan aukeratzen dituzun balioen arabera, kopia prozesua alda daiteke.

| **Eremua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
| --- | --- | --- |
| Gaia | Sartu helburuko kontratuaren gaia. Elkarrizketa-orria irekitzen denean, sistemak iturburuko kontratuaren izenaren eramuari **kopia** erantsi dio. | Ez dago alor honen beherako eraginik. |
| Bezeroa | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko kontratuko kontuan ezarriko du. | Eremu hau kontratuaren bezero nagusia da. |
| Kontratatzailea | Akordio honekin lotutako proiektuak entregatzeaz arduratzen den Antolakuntza unitatea. Elkarrizketa-orria irekitzen denean, sistemak iturburuko kontratuko kontratazio-unitatea ezarriko du. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek dute moneta bat. Moneta proiektuan zenbatetsitako eta benetako kostuen berri emateko erabiltzen da. |
| Moneta | Eskaintzaren transakzioa zein dibisatan egingo den. Elkarrizketa-orria irekitzen denean, sistemak iturburuko kontratuko moneta ezarriko du. Ezin da aldatu moneta. Hala bada, **Kopien prezioak** eremua beti **Ez** izango da iturburu-kontratuko prezioen zerrendak ez direlako garrantzitsuak. | Moneta prezioen zerrendak lehenesteko erabiltzen da, kontratuaren finantza-estimazioa eraikitzeko eta bezeroari faktura egiteko akordioa irabazten denean. |
| Eskatutako entrega-data | Bezeroak eskatutako entrega-data. | Fakturazio datak maiztasun zehatz batean sortzerakoan amaierako data gisa erabiltzen da. |
| Kopiatu prezioak | Kontratuaren prezioa iturburuko kontratutik kopiatu behar den adierazten du. | Eremua **Bai** gisa ezartzen bada, proiektuaren prezioen zerrenda eta produktuen prezioen zerrenda erreferentziak jatorrizko kontratutik xedekora kopiatzen dira. **Ez** hautatuta badago, prezioen zerrendak lehenetsita daude kontuan edo proiektuaren parametroetan ezarritako prezioen zerrendetan oinarrituta. |

**Ados** hautatzen duzunean elkarrizketa-orrian, sistemak kontratuaren kopia bat sortzen du hautatutako parametroetan oinarrituta. Kontratu berria irekiko da.

Informazio hau ez da **Iturritik** **Xede kontratutik** kopiatuta:

  - Fakturazio-antolaketak
  - Kontratua eta kontratuaren lerroaren bezeroak
  - Proiektuaren erreferentzia proiektuan oinarritutako kontratu lerroetan
  - Bezeroaren aurrekontu-informazioa

Informazio hau kontratu bakoitzerako zehatza denez, eremu eta erregistro horiek ez dira kopiatzen. Proiektuen eta produktuen kontratu lerroak, kontratuaren lerroaren xehetasunen inguruko kalkuluak eta kontratu-mailan ez gainditzeko balioak kopiatzen dira. Hautapeneko prezioaren eta kostuaren tasaren lehenespenen arabera **Kopiatu prezioak** eremuan hautatutako aukera **Kopiatu parametroak** elkarrizketa-orria.