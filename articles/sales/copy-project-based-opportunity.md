---
title: Kopiatu proiektuetan oinarritutako abaguneak
description: Gai honek proiektuetan oinarritutako abaguneak kopiatzeari buruzko informazioa eskaintzen du Project Operations-en.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 89f5a63581f36b30634bdd302a6d360d6b5e75bd
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070975"
---
# <a name="copy-project-based-opportunities"></a>Kopiatu proiektuetan oinarritutako abaguneak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Proiektu aukerak erraz kopiatu daitezke proiektu aukera berriak sortzeko. 

1. Joan **Proiektu-aukerak** zerrendaren orria eta hautatu aukera bat zerrendatik. Edo ireki aukera zehatz baten xehetasunak. 
2. Orrialde bietatik aukeratu **Kopiatu**. Elkarrizketa-orri bat irekiko da eremuko informazio hau duena. Elkarrizketa honetan aukeratzen dituzun balioen arabera, kopia prozesua alda daiteke.

    | **Eremua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
    | --- | --- | --- |
    | Gaia | Idatzi xede-abagunearen dagokion gaia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko abagunearen gaia ezarriko du **kopia** erantsi zaio. | Ez dago alor honen beherako eraginik. |
    | Account | Bezeroaren enpresaren edo kontuaren erregistroari egiten dio erreferentzia. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko abaguneko kontuan ezarriko du. | Eremu hau abagunearen bezero nagusia da. |
    | Kontratatzailea | Akordio honekin lotutako proiektuak entregatzeaz arduratzen den Antolakuntza unitatea. Elkarrizketa-koadroa irekitzen denean, sistemak iturburuko abaguneko kontratazio-unitatea ezarriko du. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatzen dituen enpresaren banaketa da. Kontratazio unitate guztiek moneta bat dute, eta moneta hori proiektuan zehar egindako kostu estimatuen eta benetakoen berri emateko erabiltzen da. |
    | Moneta | Eskaintzaren transakzioa zein dibisatan egingo den. Elkarrizketa-orria irekitzen denean, sistemak iturburuko abaguneko moneta ezarriko du. | Moneta prezioen zerrenda lehenetsi eta aurrekontuaren finantza estimazioak sortzeko erabiltzen da. Azkenean, tratua irabazten denean bezeroari fakturatzeko erabiltzen da. |
    | Kopiatu prezioak | Aukeraren prezioa jatorrizko aukeratik kopiatu behar den adierazten duen Bai / Ez balioa. | **Bai** hautatuta badago, prezioen zerrendak iturburutik xede aukerara kopiatzen dira. **Ez** hautatuta badago, prezioen zerrendak lehenetsita daude ezarri ziren azken prezioen zerrendetan oinarrituta. |

3. Hautatu **Ados**. Sistemak aukeratutako parametroetan oinarrituta proiektuaren aukeraren kopia sortzen du eta proiektuaren aukera berria irekitzen da.