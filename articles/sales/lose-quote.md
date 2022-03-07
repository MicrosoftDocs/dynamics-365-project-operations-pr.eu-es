---
title: Kopiatu proiektuetan oinarritutako eskaintzak
description: Gai honek proiektuetan oinarritutako eskaintzak kopiatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 247f9d33bc2e7b0bcbeae8114bb436ed237efce660d0840e58d536d2a290639e
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6992146"
---
# <a name="copy-project-based-quotes"></a>Kopiatu proiektuetan oinarritutako eskaintzak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuaren aurrekontu berri bat erraz sor dezakezu lehendik dagoen bat kopiatuz. 

- Proiektuaren aurrekontua kopiatzeko,**Proiektuaren aurrekontuak** zerrendaren orria edo **Proiektuaren aurrekontua** xehetasunen orria, hautatu kopiatu nahi duzun proiektuaren aurrekontua eta, ondoren, hautatu **Kopiatu**.

Elkarrizketa-orria irekiko da eta bertan kopiaren parametroak sar ditzakezu. Hurrengo taulan elkarrizketa-orrian agertzen diren eremuak zerrendatzen dira. Aukeratzen dituzun balioen arabera, kopia prozesua alda daiteke.

| **Eremua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- |
| Gaia | Idatzi xede-aurrekontuaren dagokion gaia edo izena. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko aurrekontuaren gaia ezarriko du **-kopia** erantsi zaio. | |
| Balizko bezeroa | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko aurrekontuko kontuan ezarriko du. | Eremu hau aurrekontuaren bezero nagusia da. |
| Kontratatzailea | Akordio honekin lotutako proiektuak entregatzeaz arduratzen den Antolakuntza unitatea.
Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko aurrekontuko kontratazio-unitatea ezarriko du. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek dute moneta bat. Moneta proiektua gauzatzerakoan zenbatetsitako eta benetako kostuen berri emateko erabiltzen da. |
| Moneta | Eskaintzaren transakzioa zein dibisatan egingo den. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko aurrekontuko dibisa ezarriko du. Hau alda daiteke eta aldatu bada, **Kopien prezioak** eremua beti ezarrita dago **Ez**. Hori gertatzen da iturburuko aurrekontuko prezioen zerrendak jada ez direla garrantzitsuak. | Moneta prezioen zerrenda lehenesteko erabiltzen da, aurrekontuaren finantza-estimazioa eraikitzeko eta, azkenean, bezeroari faktura egiteko akordioa irabazten denean. |
| Eskatutako entrega-data | Bezeroak eskatutako entrega eguna da. | Fakturazio datak maiztasun zehatz batean sortzerakoan amaierako data gisa erabiltzen da. |
| Kopiatu prezioak | Bai / Ez balio batek aurrekontuaren prezioa iturburuko aurrekontutik kopiatu behar den adierazten du. | **Bai** hautatzen bada, proiektuaren prezioen zerrenda eta produktuen prezioen zerrenda erreferentziak jatorrizko aurrekontutik xede aurrekontura kopiatzen dira. **Ez** hautatuta badago, prezioen zerrendak lehenetsita daude kontuan edo proiektuaren parametroetan ezarri ziren azken prezioen zerrendetan oinarrituta. |

**Ados** hautatzen duzunean elkarrizketa-orrian, sistemak proiektuaren aurrekontuaren kopia bat sortzen du elkarrizketan hautatutako parametroetan oinarrituta. Proiektuaren aurrekontu berria irekiko da. 

> [!NOTE]
> Informazio hau ez da Iturritik Xede aurrekontutik kopiatuta:
>
> - Fakturazio-antolaketak
> - Eskaintza eta eskaintzaren lerroaren bezeroak
> - Proiektuaren erreferentzia proiektuan oinarritutako aurrekontu lerroetan -Bezeroaren aurrekontuaren informazioa
>
>Informazio hau aurrekontu bakoitzerako oso zehatza denez, eremu eta erregistro horiek ez dira kopiatzen. Proiektuen eta produktuen aurrekontu lerroak, aurrekontu lerroaren xehetasunen inguruko kalkuluak eta aurrekontu mailan ez gainditzeko balioak kopiatzen dira. Prezioaren eta kostuaren tasaren lehenespenen arabera **Kopiatu prezioak** aukeran hautatutako aukera **Kopiatu parametroak** elkarrizketa-orria.


[!INCLUDE[footer-include](../includes/footer-banner.md)]