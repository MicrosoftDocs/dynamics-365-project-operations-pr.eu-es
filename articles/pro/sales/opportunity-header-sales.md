---
title: Abagune-goiburua
description: Gai honek proiektuan oinarritutako eskaintzei eta proiektuetan oinarritutako aukera lerroei buruzko informazio orakorrari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2f08de54767f49c308d0ccc7f2e1c6ef880b7f99
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906055"
---
# <a name="opportunity-header"></a>Abagune-goiburua

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Abagunea goiburuak proiektuan oinarritutako aukera batean lerro guztiei aplikatzen zaien akordioari buruzko informazio orokorra jasotzen du.

Dynamics 365 Project Operations proiektuetan oinarritutako aukerak Dynamics 365 Sales-en aukeren luzapenak dira. Luzapen hauek funtzionalitate osagarriak eskaintzen dituzte, proiektuetan oinarritutako aukeretarako espezifikoak eta beharrezkoak direnak. Luzapen hauek proiektuetan oinarritutako aukeretan eskuragarri dauden eremu berriak eta zinta-ekintzak sar ditzakete. Salmentan eskuragarri dauden zenbait eremu, funtzionalitate eta lehenetsitako logika aurki ditzakezu Project Operations-etan ez daude erabilgarri.

Hurrengo taulan proiektuan oinarritutako aukera bateko eremuak biltzen dira, Project Operations-etarako bereziak direnak edo salmenten aukeren portaeran aldaketa garrantzitsuak dituztenak.

| **Eremua** | **Kokalekua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
| --- | --- | --- | --- |
| Mota | Fitxa orokorra (ezkutatuta) | Aukera multzo eremu honek aukera hauek ditu:</br>- Lanean oinarrituta (Project Operations-ekin soilik eskuragarri)</br>- Elementuetan oinarrituta (Project Operations eta Sales instalatuta badituzu soilik)</br>- Zerbitzua mantentze lanetan oinarrituta (Field Service instalatuta dagoenean eskuragarri) | Project Operations erabiltzen duzunean, eremuaren balio hau automatikoki ezartzen da **Lanean oinarrituta** Abagunea proiektuan oinarrituta sailkatzen duena. Abagunea proiektuan oinarrituta egon beharko litzateke akordio honetarako salmenta prozesuan proiektuaren berariazko luzapen eta funtzionalitate guztiak ahalbidetzeko. |
| Contact | Fitxa orokorra | Akordio honen bezeroaren lehen harremanetarako erreferentzia. | |
| Account | Fitxa orokorra | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. | |
| Kontu-kudeatzailea | Fitxa orokorra | Proiektuan oinarritutako aukera honen kontu kudeatzailearen izena. | Kontuaren kudeatzailea bezeroarekin harremana kudeatzeaz arduratzen da proiektu hau burutu bitartean. Kontuaren kudeatzaileari lotuta dagoen baliabide erreserbagarrien erregistroan oinarrituta, kontratazio unitatea lehenetsita dago. |
| Kontratatzailea | Fitxa orokorra | Akordio honekin lotutako proiektua edo proiektuak entregatzeaz arduratzen den Antolakuntza unitatea. | Kontratazio unitatea akordioa itxi ondoren proiektuak osatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek moneta bat dute, eta moneta hori proiektuan zehar egindako kostu estimatuen eta benetakoen berri emateko erabiltzen da. |

Abagunearen **Laburpena** fitxako gainerako eremuei eta sekzioei buruzko informazio gehiago lortzeko, ikusi [Sortu edo editatu abaguneak (Salmentak eta Salmenten atala)](https://docs.microsoft.com/dynamics365/sales-enterprise/create-edit-opportunity-sales)
