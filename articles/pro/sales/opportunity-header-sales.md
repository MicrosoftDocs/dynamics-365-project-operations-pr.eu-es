---
title: Abagunearen ezarpenak - arina
description: Gai honek proiektuan oinarritutako eskaintzei eta proiektuetan oinarritutako aukera lerroei buruzko informazioa eskaintzen du.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6a9a1ea9dacdb3aa2dbc8a0500481b204ff14eddfc1138e3db43ff568d7cd48b
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6994441"
---
# <a name="header-details-for-project-opportunities"></a>Proiektuko abaguneen goiburuaren xehetasunak

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Abagunea goiburuak proiektuan oinarritutako aukera batean lerro guztiei aplikatzen zaien akordioari buruzko informazio orokorra jasotzen du.

Dynamics 365 Project Operations-eko proiektuan oinarritutako aukerak Dynamics 365 Sales-eko abaguneen luzapenak dira. Luzapen hauek funtzionalitate osagarriak eskaintzen dituzte, proiektuetan oinarritutako aukeretarako espezifikoak eta beharrezkoak direnak. Luzapen hauek proiektuetan oinarritutako aukeretan eskuragarri dauden eremu berriak eta zinta-ekintzak sar ditzakete. Salmentan eskuragarri dauden zenbait eremu, funtzionalitate eta lehenetsitako logika aurki ditzakezu Project Operations-etan ez daude erabilgarri.

Hurrengo taulan proiektuan oinarritutako aukera bateko eremuak biltzen dira, Project Operations-etarako bereziak direnak edo salmenten aukeren portaeran aldaketa garrantzitsuak dituztenak.

| **Eremua** | **Kokalekua** | **Azalpena** | **Downstream eragina** |
| --- | --- | --- | --- |
| Idatzi | Fitxa orokorra (ezkutatuta) | Aukera multzo eremu honek aukera hauek ditu:</br>- Lanean oinarrituta (Project Operations-ekin soilik eskuragarri)</br>- Elementuetan oinarrituta (Project Operations eta Sales instalatuta badituzu soilik)</br>- Zerbitzua mantentze lanetan oinarrituta (Field Service instalatuta dagoenean eskuragarri) | Project Operations erabiltzen duzunean, eremuaren balio hau automatikoki ezartzen da **Lanean oinarrituta** Abagunea proiektuan oinarrituta sailkatzen duena. Abagunea proiektuan oinarrituta egon beharko litzateke akordio honetarako salmenta prozesuan proiektuaren berariazko luzapen eta funtzionalitate guztiak ahalbidetzeko. |
| Contact | Fitxa orokorra | Akordio honen bezeroaren lehen harremanetarako erreferentzia. | |
| Account | Fitxa orokorra | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. | |
| Kontu-kudeatzailea | Fitxa orokorra | Proiektuan oinarritutako aukera honen kontu kudeatzailearen izena. | Kontuaren kudeatzailea bezeroarekin harremana kudeatzeaz arduratzen da proiektu hau burutu bitartean. Kontuaren kudeatzaileari lotuta dagoen baliabide erreserbagarrien erregistroan oinarrituta, kontratazio unitatea lehenetsita dago. |
| Kontratatzailea | Fitxa orokorra | Akordio honekin lotutako proiektua edo proiektuak entregatzeaz arduratzen den Antolakuntza unitatea. | Kontratazio unitatea akordioa itxi ondoren proiektuak osatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek moneta bat dute, eta moneta hori proiektuan zehar egindako kostu estimatuen eta benetakoen berri emateko erabiltzen da. |

Abagunearen **Laburpena** fitxako gainerako eremuei eta sekzioei buruzko informazio gehiago lortzeko, ikusi [Sortu edo editatu abaguneak (Salmentak eta Salmenten atala)](/dynamics365/sales-enterprise/create-edit-opportunity-sales)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
