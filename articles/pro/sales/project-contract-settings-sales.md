---
title: Proiektu-kontratuaren ezarpenak - arina
description: Gai honek kontratu-lerroetan eragina duten eremuei buruzko informazioa eskaintzen du eta kontratuari buruzko informazioa lerro-elementu guztietan laburbilduta dago.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 28dfb256eb75ca9484161f053969c205fcd60965
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180897"
---
# <a name="project-contract-settings---lite"></a>Proiektu-kontratuaren ezarpenak - arina

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Gai honek proiektuaren kontratu osoari aplikatzen zaizkion eremuei buruzko informazioa eskaintzen du, kontratu lerro guztietan eragina duten ezarpenak barne. Proiektuaren kontratuaren KPIak gidatzeko lerro-elementu guztietan laburbiltzen den kontratuari buruzko informazioa ere sartzen da.

Hurrengo taulan proiektuaren kontratuaren eremuak zerrendatzen dira, Dynamics 365 Project Operations-erako bakarrak direnak edo Dynamics 365 Sales-en salmenta-eskaeren aldaketa garrantzitsuak dituztenak.

| Eremua | Kokapena | Deskribapena | Downstream eragina |
| --- | --- | --- | --- |
| Idatzi | **Laburpena** fitxa (ezkutatuta) | Aukera multzo eremu honek aukera hauek ditu:</br>- - **Lanean oinarrituta** (Project Operations instalatuta dagoenean soilik eskuragarri)</br>- **Elementuetan oinarrituta** (Project Operations eta Sales instalatuta badituzu soilik)</br>- **Zerbitzua mantentze lanetan oinarrituta** (Dynamics 365 Field Service instalatuta dagoenean eskuragarri) | Project Operations-en, eremu honen balioa lehenetsia da **Lanean oinarrituta** eta kontratua proiektuetan oinarritutako kontratu gisa sailkatzen du. Kontratuak proiektuan oinarrituta egon behar du proiektuaren berariazko luzapen eta funtzionalitate guztiak ahalbidetzeko. |
| Balizko bezeroa | **Laburpena** fitxa | Bezeroen enpresaren edo kontuaren erregistroaren erreferentzia. Eskaintza batetik kontratua bat sortzen denean, eremu hori eskaintzaren erregistroan dagokion eremutik kopiatzen da. | Proiektuaren kontratu lehenetsiko moneta dago bezeroaren monetan oinarrituta. Hori ezin da aldatu kontratua gorde baino lehen. |
| Kontu-kudeatzailea | **Laburpena** fitxa | Eskaintzaren kontu-kudeatzailearen izena. Eskaintza batetik kontratua bat sortzen denean, eremu hori eskaintzaren erregistroan dagokion eremutik kopiatzen da. | Kontuaren kudeatzailea bezeroarekin harremana kudeatzeaz arduratzen da proiektu hau burutu bitartean. Kontuaren kudeatzaileari lotuta dagoen baliabide erreserbagarrien erregistroan oinarrituta, kontratazio unitatea lehenetsia da proiektuaren kontratuan. |
| Kontratatzailea | **Laburpena** fitxa | Kontratu honekin lotutako proiektuak entregatzeaz arduratzen den Antolakuntza unitatea. Eskaintza batetik kontratua bat sortzen denean, eremu hori eskaintzaren erregistroan dagokion eremutik kopiatzen da. | Kontratazio-unitatea proiektuak exekutatzen dituen enpresaren banaketa da. Kontratazio unitate guztiek moneta bat dute, eta moneta hori proiektuan zehar egindako kostu estimatuen eta benetakoen berri emateko erabiltzen da. |
| Produktuaren prezio-zerrenda | **Laburpena** fitxa | Hau da produktuetan oinarritutako kontratuaren lerroetan lehenetsitako prezioetarako erabiltzen den prezio zerrenda. Eremu honetako goitibeherako aukeren zerrendan prezioen zerrenden zerrenda agertzen da, non prezioen zerrendako moneta kontratuaren monetara datorren. Eskaintza batetik kontratua bat sortzen denean, eremu hori eskaintzaren erregistroan dagokion eremutik kopiatzen da. Proiektuaren kontratuan, eremu hau lehenetsita dago kontuaren erregistroan, baina alda daiteke. | Ez dago behe-errendimendurik eremu honetarako. |
| Moneta | **Laburpena** fitxa | Akordio honen balioa eta bezeroari fakturatuko zaion moneta jakinarazteko erabilitako moneta. Eskaintza batetik kontratua bat sortzen denean, eremu hori eskaintzaren erregistroan dagokion eremutik kopiatzen da. Proiektuaren kontratuan, eremu hau lehenetsita dago kontuaren erregistroan, baina alda daiteke. | Kontratua gorde ondoren, eremu hau jada ez da editagarria. Kontratuan produktuen eta proiektuen prezioen zerrendak lehenesteko erabiltzen da eremua. Kontratua prezio-zerrendako monetarekin bat etortzeko erabiltzen da. |
| Ez gainditzeko muga | **Laburpena** fitxa | Eremu honek bezeroak akordio honetarako adosten duen azken balioaren negoziazioaren muga adierazten du. | Kapitulua exekuzioan zehar ebaluatzen da eta akordio honekin lotutako lineako elementu eta proiektu guztietan aplika daiteke. |
| Eskatutako entrega-data | **Laburpena** fitxa | Proiektuaren eskaintza batetik kontratua bat sortzen denean, eremu hori proiektuaren eskaintzan dagokion eremutik kopiatzen da. | Data hori fakturen ordutegiak sortzeko amaierako data gisa erabiltzen da. |

Ondorengo KPIak eskuragarri daude **Kontratuaren gauzatzea** proiektuaren kontratuaren fitxa.

| Eremua | Kokapena | Deskribapena |
| --- | --- | --- |
| Kontratuaren balioa | Kontratu orokorra | Proiektuaren kontratuaren guztizko balioa. |
| Fakturatutako zenbatekoa | Kontratu orokorra | Kontratu honen aurkako faktura guztien zenbatekoen batura. |
| Egindako kostua | Kontratu orokorra | Kontratuaren arabera mapatutako proiektu guztietan erregistratutako kostu erreal guztien batura. |
| Marjina gordina | Kontratu orokorra | Fakturatutako zenbatekoa - Orain arte sortutako kostua / Fakturatutako zenbatekoa |
| Aurreikusitako marjina | Kontratu orokorra | (Kontratuaren balioa - Kalkulatutako kostuak) / Kontratuaren balioa Kalkulatutako kostuak = Kontratuarekin mapatutako proiektu guztietan kalkulatutako kostu guztien batura.|
| Kontratuaren balioa | Proiektuetan oinarritutako lerroak | Kontratuaren lerroaren balioa. |
| Fakturatutako zenbatekoa | Proiektuetan oinarritutako lerroak | Prezio finkoko kontratu lerroarentzat: fakturatutako salmenten mugarri guztien zenbatekoen batura kontratu lerro honen aurka kontratu honetarako sortutako hainbat fakturatan. Denbora eta materialaren kontratu lerroarentzat: fakturatutako salmenta kargagarri guztien zenbatekoen batura kontratu lerro honen aurka kontratu honetarako sortutako hainbat fakturatan. |
| Egindako kostua | Proiektuetan oinarritutako lerroak | Kontratuaren lerroaren arabera mapatutako proiektu guztietan erregistratutako kostu erreal guztien batura. |
| Marjina gordina | Proiektuetan oinarritutako lerroak | (Fakturatutako zenbatekoa - Orain arte sortutako kostua) / Fakturatutako zenbatekoa |
| Aurreikusitako marjina | Proiektuetan oinarritutako lerroak | (Kontratuaren linearen zenbatekoa oinarrizko monetan - Kontratuaren linearen zenbatekoak oinarrizko monetan) / Kontratuaren linearen zenbatekoa oinarrizko monetan |
| Egindako kostua | Proiektuetan oinarritutako linea baten xehetasuna | Denbora: eginkizun honetarako kontratuaren lerroan mapatutako proiektuan erregistratutako denboraren kostuaren zenbatekoaren batura. Gastuak: kategoria honetarako kontratuaren lerroan mapatutako proiektuan erregistratutako gastu guztien kostuaren zenbatekoaren batura. |
| Erregistratutako kopurua | Proiektuetan oinarritutako linea baten xehetasuna | Denbora: eginkizun baterako kontratuaren lerro honetan mapatutako proiektuan erregistratutako denbora-kostuaren guztizko zenbatekoa. Gastuak: Proiektuko gastuen benetako datuetako gastuen kategoria honetarako kopuru guztiak kontratuaren lerroan mapatzen dira. |
| Fakturatutako zenbatekoa | Proiektuetan oinarritutako linea baten xehetasuna | Prezio finkoko kontratu lineari dagokionez, eremu hau hutsik geratzen da xehetasun mailan eta kontratu lerro mailan bakarrik erakusten da. Denbora eta material kontratu lerro baterako, kalkuluak xehetasun mailan burutzen dira. Xehetasunek fakturatutako diru-sarrera lerro guztietan kobratu beharreko zenbatekoaren batura erakusten dute. |
| Fakturatutako kopurua | Proiektuetan oinarritutako linea baten xehetasuna | Prezio finkoko kontratu lineari dagokionez, eremu hau hutsik geratzen da xehetasun mailan eta kontratu lerro mailan bakarrik erakusten da. Denbora eta material kontratu lerro baterako, kalkuluak denboraren eta gastuen xehetasun mailan burutzen dira. Denbora: Funtzio honen fakturatutako diru-sarreren lerro guztietako orduen batura zenbatekoaren batura erakusten dute. Gastuak: Proiektuko gastuen benetako datuetako gastuen kategoria honetarako kopuru guztiak kontratuaren lerroan mapatzen dira. |
| Kontratuaren balioa | Produktuetan oinarritutako lerroak | Produktuan oinarritutako kontratu lerro honen kontratu lerroaren balioa. |
| Fakturatutako zenbatekoa | Produktuetan oinarritutako lerroak | Produktuan oinarritutako kontratu lerro honen aurkako faktura lerro guztietako zenbatekoen batura kontratu honetarako sortzen diren hainbat fakturetan. |
| Egindako kostua | Produktuetan oinarritutako lerroak | Kontratuaren lerroan oinarritutako erregistratutako kostu erreal guztien batura. |
| Marjina gordina | Proiektuetan oinarritutako lerroak | Fakturatutako zenbatekoa - Orain arte sortutako kostua / Fakturatutako zenbatekoa |
| Aurreikusitako marjina | Produktuetan oinarritutako lerroak | (Kontratuaren lerroko balioa - Kontratuaren lerrorako aurreikusitako kostuak) / Kontratuaren lerroaren balioa |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]