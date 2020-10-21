---
title: Proiektuaren eskaintzako laburpen-informazioa (salmentak)
description: Gai honek proiektuaren aurrekontuei aplikatzen zaien eta ezartzen duen informazioari eta ezarpenei buruzko informazioa eskaintzen du. (Sales)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d050258ae457bb4392d5fa761442cfc7a444feb0
ms.sourcegitcommit: f6509f7d50de4d4ebb92c1bf2cfcdf09f17458eb
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/06/2020
ms.locfileid: "3966725"
---
# <a name="summary-information-on-a-project-quote-sales"></a>Proiektuaren eskaintzako laburpen-informazioa (salmentak)

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Artikulu honetan proiektuaren aurrekontuari aplikatzen zaion informazioa azaltzen da. Honek aurrekontu lerro guztietan eragina duten ezarpenak eta proiektuaren aurrekontuaren KPIak gidatzeko lerro elementu guztietan laburbiltzen den aurrekontuari buruzko informazioa biltzen ditu.

Hurrengo taulan proiektuaren aurrekontuaren laburpeneko informazio eremuak zerrendatzen dira, Dynamics 365 Project Operations-erako bakarrak direnak edo Dynamics 365 Sales-en aurrekontuen portaera aldaketa garrantzitsuak dituztenak.

| **Eremua** | **Kokalekua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
| --- | --- | --- | --- |
| Mota | Laburpen fitxa (ezkutatuta) | Aukera multzo eremu honek aukera hauek ditu:</br>- Lanean oinarrituta (Project Operations instalatuta dagoenean soilik eskuragarri)</br>- Elementuetan oinarrituta (Project Operations eta Sales instalatuta badituzu soilik)</br>- Zerbitzua mantentze lanetan oinarrituta (Dynamics 365 Field Service instalatuta dagoenean eskuragarri) | Project Operations aplikazioa erabiltzen duzunean, eremuaren balio hau automatikoki ezartzen da **Lanean oinarrituta** gisa. Honek aurrekontua proiektuan oinarritutako aurrekontu gisa sailkatzen du. Aurrekontuak proiektuan oinarrituta egon behar du proiektuaren berariazko luzapen eta funtzionalitate guztiak ahalbidetzeko. |
| Balizko bezeroa | Laburpena fitxa | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Proiektuaren aurrekontuaren moneta lehenetsita dago bezeroaren monetan oinarrituta. Alabaina, hori ezin da aldatu eskaintza gorde baino lehen. |
| Kontu-kudeatzailea | Laburpena fitxa | Eskaintzaren kontu-kudeatzailearen izena. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Kontuaren kudeatzailea bezeroarekin harremana kudeatzeaz arduratzen da proiektu hau burutu bitartean. Kontuaren kudeatzaileari lotuta dagoen baliabide erreserbagarrien erregistroan oinarrituta, kontratazio unitatea lehenetsia da proiektuaren eskaintzan. |
| Kontratatzailea | Laburpena fitxa | Eskaintza honekin lotutako proiektua edo proiektuak entregatzeaz arduratzen den antolakuntza unitatea. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek moneta bat dute, eta moneta hori proiektua exekutatzean egindako kostu estimatuen eta benetakoen berri emateko erabiltzen da. |
| Produktuaren prezio-zerrenda | Laburpena fitxa | Hau da produktuetan oinarritutako aurrekontu lerroetan lehenetsitako prezioetarako erabiltzen den prezio zerrenda. Eremu honetako aukeren zerrendan prezioen zerrenden zerrenda agertzen da, non prezioen zerrendako moneta aurrekontuaren monetara datorren. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. Aukerako eremu hau lehenetsita dago kontuaren erregistroan, baina alda daiteke. | Eskaintza irabazi denean, eremuaren balioa proiektuaren kontratuan kopiatu da. |
| Moneta | Laburpena fitxa | Honek akordioaren balioaren berri emateko erabiliko den moneta adierazten du. Hau da, bezeroari fakturatuko zaion moneta ere tratua irabaziz gero. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. Aukerako eremu hau lehenetsita dago kontuaren erregistroan, baina erabiltzaileak alda dezake. | Aurrekontua gorde ondoren, eremu hau jada ez da editagarria. Aurrekontuan produktuen eta proiektuen prezioen zerrendak lehenesteko erabiltzen da. Eskaintza prezio-zerrendako monetarekin bat etortzeko erabiltzen da. |
| Ez gainditzeko muga | Laburpena fitxa | Honek bezeroak akordio honetarako adosten duen azken balioaren negoziazioaren muga adierazten du. | Kapitulu hori exekuzioan zehar ebaluatzen da eta akordio honekin lotutako lineako elementu eta proiektu guztietan aplika daiteke. |
| Eskatutako entrega-data | Laburpena fitxa | Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Data hori fakturen ordutegiak sortzeko amaierako data gisa erabiltzen da. |

Jarraian, proiektuaren aurrekontuetan eskuragarri dauden fitxak eta KPIak daude, proiektuaren eragiketetarako bakarrak direnak edo salmenten aurrekontuen portaeran aldaketa garrantzitsuak dituztenak:

| **Eremua** | **Kokalekua** | **Garrantzia, xedea eta orientazioa** |
| --- | --- | --- |
| Errentagarritasun-analisia | Eskaintzako fitxa | Fitxak neurketa hauek ditu:</br>- Kobra daitekeen kostua, guztira</br></br>- Kobra ezin daitekeen kostua, guztira</br>- Diru-sarrerak, guztira</br>- Diru-sarrerak, guztira (oinarrizkoa)</br>- Marjina gordina</br>- Marjina gordin doitua|
| Bezeroen aurreikuspenekiko konparazioa | Eskaintzako fitxa | Fitxa honek neurketa hauek ditu:</br>- Aurreikusitako osatze-data</br>- Eskatutako osatze-data</br>- Bezeroaren aurrekontua</br>- Eskainitako balioa |
| Eskaintzaren analisia | Eskaintzako fitxa | Fitxa honek proiektuaren aurrekontua lortzeko ondorengo KPI nagusiak laburbiltzen ditu</br>- Aurrekontuaren eta ordutegiaren bezeroen itxaropenekin alderatzea</br>- Marjina gordina</br>- Marjina gordin doitua |
