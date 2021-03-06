---
title: Proiektuaren eskaintzako laburpen-informazioa
description: Gai honek proiektuaren aurrekontuei aplikatzen zaien eta ezartzen duen informazioari eta ezarpenei buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6dde5305f179e9a4454bf97c44f1ebdf9986dd43
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907827"
---
# <a name="summary-information-on-a-project-quote"></a>Proiektuaren eskaintzako laburpen-informazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_


Artikulu honetan proiektuaren aurrekontuari aplikatzen zaion informazioa azaltzen da. Honek aurrekontu lerro guztietan eragina duten ezarpenak eta proiektuaren aurrekontuaren KPIak gidatzeko lerro elementu guztietan laburbiltzen den aurrekontuari buruzko informazioa biltzen ditu.

Hurrengo taulan proiektuaren aurrekontuaren laburpeneko informazio eremuak zerrendatzen dira, Dynamics 365 Project Operations-erako bakarrak direnak edo Dynamics 365 Sales-en aurrekontuen portaera aldaketa garrantzitsuak dituztenak.

| **Eremua** | **Kokalekua** | **Garrantzia, xedea eta orientazioa** | **Downstream eragina** |
| --- | --- | --- | --- |
| Mota | Laburpen fitxa (ezkutatuta) | Aukera multzo eremu honek aukera hauek ditu:</br>- Lanean oinarrituta (Project Operations instalatuta dagoenean soilik eskuragarri)</br>- Elementuetan oinarrituta (Project Operations eta Sales instalatuta badituzu soilik)</br>- Zerbitzua mantentze lanetan oinarrituta (Dynamics 365 Field Service instalatuta dagoenean eskuragarri) | Project Operations aplikazioa erabiltzen duzunean, eremuaren balio hau automatikoki ezartzen da **Lanean oinarrituta** gisa. Honek aurrekontua proiektuan oinarritutako aurrekontu gisa sailkatzen du. Aurrekontuak proiektuan oinarrituta egon behar du proiektuaren berariazko luzapen eta funtzionalitate guztiak ahalbidetzeko. |
| Jabetzadun enpresa | Laburpena | Proiektu honetatik edo aurrekontu honekin lotutako proiektuetatik sortzen diren kostuak eta diru-sarrerak kontabilizatuko dituen pertsona juridikoa. Abagune batetik eskaintza bat sortzen denean, eremu hori Abagunean dagokion eremutik kopiatzen da. | Enpresa titularra pertsona juridikoaren kontzeptuarekin bat dator **Proiektuen kudeaketa eta kontabilitatea** proiektuaren eragiketen modulua. Proiektu honetatik sortzen diren kostu eta diru-sarrera guztiak enpresa jabearen liburu nagusian kontabilizatuko dira. |
| Balizko bezeroa | Laburpena fitxa | Bezeroaren enpresaren edo kontuaren erregistroaren erreferentzia. Baliozko bezero bat proiektuaren eskaintza batean erreferentzia egitean bezero gisa konfiguratu behar duenean, eskaintzaren jabe den enpresan. Enpresa titularra legezko entitatearen zerrenda erakusten du eta **Proiektuen kudeaketa eta kontabilitatea** proiektuaren eragiketen moduluan konfiguratzen dira. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Proiektuaren aurrekontuaren moneta lehenetsita dago bezeroaren monetan oinarrituta. Alabaina, hori ezin da aldatu eskaintza gorde baino lehen. |
| Kontu-kudeatzailea | Laburpena fitxa | Eskaintzaren kontu-kudeatzailearen izena. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Kontuaren kudeatzailea bezeroarekin harremana kudeatzeaz arduratzen da proiektu hau burutu bitartean. Kontuaren kudeatzaileari lotuta dagoen baliabide erreserbagarrien erregistroan oinarrituta, kontratazio unitatea lehenetsia da proiektuaren eskaintzan.|
| Kontratatzailea | Laburpena fitxa | Eskaintza honekin lotutako proiektua edo proiektuak entregatzeaz arduratzen den antolakuntza unitatea. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Kontratazio-unitatea akordioa itxi ondoren proiektuak exekutatuko dituen enpresaren banaketa da. Kontratazio unitate guztiek moneta bat dute, eta moneta hori proiektua exekutatzean egindako kostu estimatuen eta benetakoen berri emateko erabiltzen da. |
| Produktuaren prezio-zerrenda | Laburpena fitxa | Hau da produktuetan oinarritutako aurrekontu lerroetan lehenetsitako prezioetarako erabiltzen den prezio zerrenda. Eremu honetako aukeren zerrendan prezioen zerrenden zerrenda agertzen da, non prezioen zerrendako moneta aurrekontuaren monetara datorren. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. Aukerako eremu hau lehenetsita dago kontuaren erregistroan, baina alda daiteke. | Eskaintza irabazi denean, eremuaren balioa proiektuaren kontratuan kopiatu da. |
| Moneta | Laburpena fitxa | Honek akordioaren balioaren berri emateko erabiliko den moneta adierazten du. Hau da, bezeroari fakturatuko zaion moneta ere tratua irabaziz gero. Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. Aukerako eremu hau lehenetsita dago kontuaren erregistroan, baina erabiltzaileak alda dezake.  | Aurrekontua gorde ondoren, eremu hau jada ez da editagarria. Aurrekontuan produktuen eta proiektuen prezioen zerrendak lehenesteko erabiltzen da. Eskaintza prezio-zerrendako monetarekin bat etortzeko erabiltzen da. |
| Ez gainditzeko muga | Laburpena fitxa | Honek bezeroak akordio honetarako adosten duen azken balioaren negoziazioaren muga adierazten du. | Kapitulu hori exekuzioan zehar ebaluatzen da eta akordio honekin lotutako lineako elementu eta proiektu guztietan aplika daiteke. |
| Eskatutako entrega-data | Laburpena fitxa | Abagune batetik eskaintza bat sortzen denean, eremu hori abagunean dagokion eremutik kopiatzen da. | Data hori fakturen ordutegiak sortzeko amaierako data gisa erabiltzen da. |

Jarraian, proiektuaren aurrekontuetan eskuragarri dauden fitxak eta KPIak daude, proiektuaren eragiketetarako bakarrak direnak edo salmenten aurrekontuen portaeran aldaketa garrantzitsuak dituztenak:

| **Eremua** | **Kokalekua** | **Garrantzia, xedea eta orientazioa** |
| --- | --- | --- |
| Errentagarritasun-analisia | Eskaintzako fitxa | Fitxak neurketa hauek ditu:</br>- Kobra daitekeen kostua, guztira</br></br>- Kobra ezin daitekeen kostua, guztira</br>- Diru-sarrerak, guztira</br>- Diru-sarrerak, guztira (oinarrizkoa)</br>- Marjina gordina</br>- Marjina gordin doitua|
| Bezeroen aurreikuspenekiko konparazioa | Eskaintzako fitxa | Fitxa honek neurketa hauek ditu:</br>- Aurreikusitako osatze-data</br>- Eskatutako osatze-data</br>- Bezeroaren aurrekontua</br>- Eskainitako balioa |
| Eskaintzaren analisia | Eskaintzako fitxa | Fitxa honek proiektuaren aurrekontua lortzeko ondorengo KPI nagusiak laburbiltzen ditu</br>- Aurrekontuaren eta ordutegiaren bezeroen itxaropenekin alderatzea</br>- Marjina gordina</br>- Marjina gordin doitua |
