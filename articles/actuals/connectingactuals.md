---
title: Transakzioaren konexioak - Lotu transakzio mota desberdinen benetako datuak
description: Artikulu honek transakzio-konexio bat nola erabiltzen den azaltzen du mota ezberdinetako errealak lotzeko errentagarritasuna, fakturazio-atzerapena eta fakturatutako eta fakturatu gabeko diru-sarreren kalkuluak egiten laguntzeko.
author: rumant
ms.date: 03/25/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 19a78336099f54c5d6b36a963a90b9fd77e3d0af
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8926071"
---
# <a name="transaction-connections---link-actuals-of-different-transaction-types"></a>Transakzioaren konexioak - Lotu transakzio mota desberdinen benetako datuak

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Transakzio-konexio-erregistroak mota ezberdinetako errealak lotzeko sortzen dira, denbora, gastua edo materialaren erabilera bere bizitza-zikloan mugitzen den heinean aurrekontua edo salmenta-aurreko fasetik kontratuaren fasera, onarpenak eta/edo berreskuratzeak, fakturazioak eta baliteke kreditu edo faktura zuzentzaileak. .

Hurrengo adibidean Project Operations proiektuaren bizi-zikloko denbora sarreren prozesaketa tipikoa erakusten da.

> ![Proiektuaren Eragiketetan denbora-sarrerak prozesatzea.](media/basic-guide-17.png)

Project Operations proiektuaren bizi-zikloko denbora-sarrerak prozesatzeko urrats hauek jarraitzen ditu: 

1. Denbora-sarrera bidaltzeak bi aldizkari-lerro sortzea eragiten du: kosturako bat eta fakturatu gabeko salmenterako. 
2. Denbora-sarreren behin-behinean onartzeak bi erreal sortzen ditu: kosturako bat eta fakturatu gabeko salmentetarako. 2 erreal hauek transakzio-konexioak erabiliz lotzen dira.
3. Erabiltzaileak proiektuaren faktura sortzen duenean, fakturen lerroko transakzioa fakturatu gabeko salmenten egiazko datuak erabiliz sortzen da.
4. Faktura berresten denean, bi erreal berri sortzen dira: fakturatu gabeko salmenten itzulketa eta fakturatutako salmenta erreal bat. Fakturatu gabeko salmenten itzulketa eta fakturatu gabeko jatorrizko salmenta errealak alderantzizko transakzio konexioak erabiliz konektatzen dira. Fakturatutako salmentak eta fakturatu gabeko jatorrizko salmenten errealak ere konektatzen dira garai batean atzerapena edo lan egiten ari zirenaren (WIP) diru-sarreren eta orain fakturatutako diru-sarreren arteko loturak erakusteko.   

Prozesatzeko lan-fluxuko gertaera bakoitzak erregistroak sortzea abiarazten du **Transakzio-konexioa** mahaia. Honek denbora-sarreran, egunkari-lerroan, benetako eta faktura-lerroaren xehetasunetan sortzen diren erregistroen arteko erlazioen arrastoa eraikitzen laguntzen du.

Hurrengo taulan erregistroak erakusten ditu **Transakzio-konexioa** aurreko lan-fluxurako entitatea.

|Gertaera                   |1. transakzioa                 |1. transakzioaren funtzioa |1. transakzioaren mota       |2. transakzioa          |2. transakzioaren funtzioa |2. transakzioaren mota |
|------------------------|------------------------------|---------------|-----------------------------|-----------------------------|-------------------|-------------------|
|Denbora-sarreraren bidalketa   |Kutxako liburuaren lerroa GUIDA (salmentak)     |Fakturatu gabeko salmentak |msdyn_journalline            |Kutxako liburuaren lerroa GIDA (kostua)     |Kostua            |msdyn_journalline  |
|Orduaren onarpena           |Fakturatu gabeko benetakoak (salmentak) GIDA  |Fakturatu gabeko salmentak |msdyn_actual                 |Benetako kostua (kostua) GIDA       |Kostua            |msdyn_actual       |
|Faktura sortzea        |Fakturaren lerroaren xehetasunak GIDA      |Fakturatutako salmentak   |msdyn_invoicelinetransaction |Fakturatu gabeko benetakoak GIDA   |Fakturatu gabeko salmentak  |msdyn_actual       |
|Faktura berrespena    |Benetako GIDA itzultzea         |Itzultzea      |msdyn_actual                 |Jatorrizko fakturatu gabeko salmentak GIDA |Jatorrizkoa        |msdyn_actual       |
|                        |Fakturatutako salmentak GIDA             |Fakturatutako salmentak   |msdyn_actual                 |Fakturatu gabeko benetakoak GIDA   |Fakturatu gabeko salmentak  |msdyn_actual       |
|Faktura-zirriborroen zuzenketa |Fakturaren lerroaren transakzioak GIDA|Ordezkapena      |msdyn_invoicelinetransaction |Fakturatutako salmentak GIDA            |Jatorrizkoa        |msdyn_actual       |
|Berretsi faktura zuzenketa|Fakturatutako salmenten itzulera GIDA  |Itzultzea      |msdyn_actual                 |Fakturatutako salmentak GIDA            |Jatorrizkoa        |msdyn_actual       |
|                        |Fakturatu gabeko Salmenten GUID berria |Ordezkapena            |msdyn_actual                 |Fakturatutako salmentak GIDA            |Jatorrizkoa        |msdyn_actual       |


Ondorengo ilustrazioak hainbat gertaeratan erreal mota ezberdinen artean sortzen diren estekak erakusten ditu Proiektu Eragiketetako denbora-sarreren adibidea erabiliz.

> ![Mota desberdinetako errealak nola lotzen diren proiektuen eragiketetan.](media/TransactionConnections.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
