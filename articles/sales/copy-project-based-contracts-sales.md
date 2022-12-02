---
title: Kopiatu proiektuetan oinarritutako kontratuak
description: Artikulu honek proiektu kontratuak kopiatzeari buruzko informazioa eskaintzen du Microsoft Dynamics 365 Project Operations-en.
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
# <a name="copy-project-based-contracts"></a>Kopiatu proiektuetan oinarritutako kontratuak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Proiektuen kontratu berriak erraz sor ditzakezu lehendik dauden kontratuen kopiak bi modu hauetako batean eginez:

- **Proiektuen kontratuak** zerrenda-orrian, hautatu proiektu-kontratua eta ondoren hautatu **Kopiatu**.
- **Proiektuaren kontratua** xehetasunen orrian, hautatu **Kopiatu**.

Elkarrizketa-orria irekiko da eta bertan kopiatutako kontratuaren parametroak hauta ditzakezu. Eremu hauek izango dira elkarrizketa-koadroan. Aukeratzen dituzun balioen arabera, kopia prozesua alda daiteke.

| Eremua | Deskribapenak | Downstream eragina |
| --- | --- | --- |
| Gaia | Sartu helburuko kontratuaren gaia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko kontratuaren izenaren eremuari "kopia" erantsi dio. | Ez dago alor honen beherako eraginik. |
| bezero hori | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko kontratuko kontuan ezarriko du. | Eremu hau kontratuaren bezero nagusia da. |
| Jabetzadun enpresa | Akordio honekin lotutako proiektuak entregatzeaz arduratzen den erakundea. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko kontratuko jabetza erakundean ezarriko du. | Jabetza erakundea akordioa itxi ondoren proiektuak exekutatuko dituen entitate legala. Jabetza erakundearen kostu monetak bat etorri behar du kontratu-unitatearekin. |
| Kontratatzailea | Akordio honekin lotutako proiektuak entregatzeaz arduratzen den Antolakuntza unitatea. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko kontratu-unitatea erakundean ezarriko du. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek dute moneta bat. Moneta proiektuan zenbatetsitako eta benetako kostuen berri emateko erabiltzen da. |
| Moneta | Eskaintzaren transakzioa zein dibisatan egingo den. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko kontratuko moneta ezarriko du. Ezin da aldatu moneta. Hala bada, **Kopien prezioak** eremua beti **Ez** izango da iturburu-kontratuko prezioen zerrendak ez direlako garrantzitsuak. | Moneta prezioen zerrendak lehenesteko erabiltzen da, kontratuaren finantza-estimazioa eraikitzeko eta bezeroari faktura egiteko akordioa irabazten denean. |
| Eskatutako entrega-data | Bezeroak eskatutako entrega-data. | Fakturazio datak maiztasun zehatz batean sortzerakoan amaierako data gisa erabiltzen da. |
| Kopiatu prezioak | Balioak kontratuaren prezioa iturburuko kontratutik kopiatu behar den adierazten du. | Eremua **Bai** gisa ezartzen bada, proiektuaren prezioen zerrenda eta produktuen prezioen zerrenda erreferentziak jatorrizko kontratutik xedekora kopiatzen dira. **Ez** ezarrita badago, prezioen zerrendak lehenetsia erabiliko da,kontuan edo proiektuaren parametroetan ezarritako prezioen zerrendetan oinarrituta. |

**Ados** hautatzen duzunean elkarrizketa-koadroan, sistemak kontratuaren kopia bat sortzen du ezarritako parametroetan oinarrituta. Kontratu berria irekiko da.

Hurrengo informazioa da **ez** sorburu-kontratutik xede-kontratura kopiatu da, kontratu bakoitzari berariazkoa baita:

- Fakturazio-antolaketak
- Kontratua eta kontratuaren lerroaren bezeroak
- Proiektuaren erreferentzia proiektuan oinarritutako kontratu lerroetan
- Bezeroaren aurrekontu-informazioa

Proiektuen eta produktuen kontratu lerroak, kontratuaren lerroaren xehetasunen inguruko kalkuluak eta kontratu-mailan ez gainditzeko balioak kopiatzen dira. Hautapeneko prezioaren eta kostuaren tasaren sarrera arabera **Kopiatu prezioak** eremuan hautatutako aukera **Kopiatu parametroak** elkarrizketa-koadroan.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
