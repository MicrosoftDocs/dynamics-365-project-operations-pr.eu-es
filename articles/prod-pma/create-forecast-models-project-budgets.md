---
title: Sortu proiektuaren aurrekontuen aurreikuspen ereduak
description: Gai honetan gainerako aurrekontuetarako aurreikuspen eredua nola sortu deskribatzen da.
author: Yowelle
manager: AnnBe
ms.date: 04/24/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 5a3b9d3c154a85b50536a67ae0eb45d9b4f25f15
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271023"
---
# <a name="create-forecast-models-for-project-budgets"></a>Sortu proiektuaren aurrekontuen aurreikuspen ereduak 

[!include [banner](../includes/banner.md)]

Gai honetan gainerako aurrekontuetarako aurreikuspen eredua nola sortu deskribatzen da. Aurrekontuen kontrolpean dagoen proiektuak bi aurrekontu mota erabiltzen ditu: jatorrizkoak eta gainerakoak. Proiektuaren aurrekontua sortzen duzunean, jatorrizko eta gainerako aurrekontuen aurreikuspen ereduak zehaztu behar dituzu **Iragarpen ereduak** orrialdea. Zehaztutako ereduetan oinarritutako proiektuen aurrekontuak proiektuaren aurrekontua konprometitzen duzunean sortzen dira.

> [!NOTE]
> Aurrekontuen kontrolerako erabiltzen den iragarpen ereduak ezin du azpimodelarik izan edo azpimodel gisa erabili.

1. Aukeratu **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Iragarpenak**  > **Iragarpen ereduak**.
2. Aukeratu **Berria** iragarpen eredu berria sortzeko eta, ondoren, idatzi modelo berriaren ID zenbakia eta izena. 
3. Ezarri **Geldituta** aukera **Bai** iragarpen-ereduaren iragarpen-lerroetan aldaketarik gerta ez dadin. 
4. Eredua lotzen den iragarpen-lerroek kutxa-fluxuen aurreikuspenak sortu behar badituzte liburu nagusian, hautatu **Diru fluxuen aurreikuspenetan sartu** aukeran **Bai**. 
5. Proiektuaren data faktura-data gisa erabiltzeko, hautatu **Iragarpenaren faktura-data** aukeran **Bai**. 
6. **Aurrekontu mota** eremuan, hautatu eredu mota hauetako bat:

   - **Jatorrizko aurrekontua**: Hasierako aurrekontua sortu eta onartzen denean konprometitutako jatorrizko aurrekontuaren zenbatekoak erabili.
   - **Gainerako aurrekontua**: Erabili gainerako aurrekontuaren zenbatekoak proiektuaren bizitzan zehar. Aurreikuspen eredu honetako saldoak benetako transakzioen bidez murrizten dira eta aurrekontuen berrikuspenen arabera handitzen edo murrizten dira.
   - **Aurrera eraman**: Erabili proiektuaren aurrekontuaren zenbatekoak. Aurreratzea aukerako prozesua da, erabili gabeko aurrekontu kopuruak urte fiskal batetik bestera transferitzeko exekutatu daitekeena.

7. Ezarri ondoko aukerak behar ahala:

   - Gaitu **Iragarpenaren faktura-data** proiektuaren data faktura-data gisa erabiltzeko.
   - Gaitu **Iragarpena WIPekin** Aurreikusteko egiten ari den lanaren arabera (WIP), eta gero hautatu WIP mota. 
   - Lehenespenez **Aurrekontu mota** **Bat ere ez** gisa utz dezakezu edo idatzi mota berri bat. Aurrekontu mota ezin da aldatu erregistro bat aldatu ondoren.     
    > [!NOTE]
    > Aurrekontu mota lehenetsia aldatzen baduzu, gainerako aukera guztiak ez dira erabilgarri egongo eguneratzeetarako, eta ezin duzu iragarpen eredu hau berrerabili. 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]