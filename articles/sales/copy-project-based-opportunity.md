---
title: Kopiatu proiektuetan oinarritutako abaguneak
description: Gai honek proiektuetan oinarritutako abaguneak kopiatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
ms.date: 10/09/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 3ca48125d90ee50c5621780be19bd4ceb2130d2d
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8577773"
---
# <a name="copy-project-based-opportunities"></a>Kopiatu proiektuetan oinarritutako abaguneak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_


Proiektu aukerak erraz kopiatu daitezke proiektu aukera berriak sortzeko. 

1. Joan **Proiektu-aukerak** zerrendaren orria eta hautatu aukera bat zerrendatik. Edo ireki aukera zehatz baten xehetasunak. 
2. Orrialde bietatik aukeratu **Kopiatu**. Elkarrizketa-orri bat irekiko da eremuko informazio hau duena. Elkarrizketa honetan aukeratzen dituzun balioen arabera, kopia prozesua alda daiteke.

    | **Eremua** | **Azalpena** | **Downstream eragina** |
    | --- | --- | --- |
    | Gaia | Idatzi xede-abagunearen dagokion gaia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko abagunearen gaia ezarriko du **kopia** erantsi zaio. | Ez dago alor honen beherako eraginik. |
    | Account | Bezeroaren enpresaren edo kontuaren erregistroari egiten dio erreferentzia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko abaguneko kontuan ezarriko du. | Eremu hau abagunearen bezero nagusia da. |
    | Kontratatzailea | Akordio honekin lotutako proiektuak entregatzeaz arduratzen den Antolakuntza unitatea. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko abaguneko kontratazio-unitatea ezarriko du. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatzen dituen enpresaren banaketa da. Kontratazio unitate guztiek moneta bat dute, eta moneta hori proiektuan zehar egindako kostu estimatuen eta benetakoen berri emateko erabiltzen da. |
    | Moneta | Eskaintzaren transakzioa zein dibisatan egingo den. Elkarrizketa-orria irekitzen denean, sistemak iturburuko abaguneko moneta ezarriko du. | Moneta prezioen zerrenda lehenetsi eta aurrekontuaren finantza estimazioak sortzeko erabiltzen da. Azkenean, tratua irabazten denean bezeroari fakturatzeko erabiltzen da. |
    | Kopiatu prezioak | Aukeraren prezioa jatorrizko aukeratik kopiatu behar den adierazten duen Bai / Ez balioa. | **Bai** hautatuta badago, prezioen zerrendak iturburutik xede aukerara kopiatzen dira. **Ez** hautatuta badago, prezioen zerrendak lehenetsita daude ezarri ziren azken prezioen zerrendetan oinarrituta. |

3. Hautatu **Ados**. Sistemak aukeratutako parametroetan oinarrituta proiektuaren aukeraren kopia sortzen du eta proiektuaren aukera berria irekitzen da.


[!INCLUDE[footer-include](../includes/footer-banner.md)]