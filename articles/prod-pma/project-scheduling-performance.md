---
title: Proiektuko baliabideen antolaketa-errendimendua
description: Gai honetan proiektu ugarientzako baliabideen programazioaren errendimendua hobetzeko moduari buruzko informazioa ematen da.
author: Yowelle
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 726788e9ecb7fc70648d06d0a5036becd7a45d2a
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8682861"
---
# <a name="project-resource-scheduling-performance"></a>Proiektuko baliabideen antolaketa-errendimendua

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


Baliabideen antolaketarekin lotutako errendimendu arazoak gerta daitezke proiektu kopurua milaka izatera iristen denean. Baliabideen antolaketa errendimendua hobetzeko, erabiltzaileek baliabideen erabilgarritasun inprimakia abiarazteko behar duten denbora murriztu dezaketen funtzioa dago eskuragarri. Zehazki, honek baliabideen gaitasuna biltzeko sinkronizazio prozesua kentzen du eta **ResProjectResource** taula baliabideen bilaketa azkartzeko. Kontuan izan **ResRollup** mahaia ez da gehiago erabiliko.

> [!IMPORTANT]
> Baliabideen gaitasuna biltzeko sinkronizazio prozesuaren edo **ResProjectResource** taula, ez erabili funtzio hau.

## <a name="enable-resource-scheduling-performance-enhancement"></a>Gaitu baliabideak antolatzeko errendimendua hobetzea
Baliabideen programazioaren errendimendua hobetzeko gaitu, jarraitu urrats hauek.

1. Joan **Ezaugarrien kudeaketa** > **Guztiak**, eta eginbideen zerrendan, bilatu **Gaitu proiektuaren baliabideen antolaketa errendimendua hobetzeko eginbidea**.
2. Hautatu **Gaitu orain**.

> [!NOTE]
> Eginbidea zerrendan aurkitzen ez baduzu, hautatu **Egiaztatu eguneratzeak** zerrenda freskatzeko.

3. Freskatu arakatzailea eta joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Proiektuaren baliabideak** > **Sinkronizatu baliabideen egutegien gaitasuna enpresa guztietan**.
4. Ezarri **Kendu dauden gaitasun erregistroak** **Bai** aurreko datuak kentzeko. Datu inkrementalak sortu nahi badituzu, ezarri **Ez**.
5. **Garai-kodea** eremuan, hautatu datuak zein alditan sortu behar diren. Garai kode bat hautatzen baduzu, ez da hasiera eta amaiera data zehaztu behar.
6. **Garai kodea** eremua hutsik uzten baduzu, hautatu hasiera eta amaiera data zehatzak datuak sortzeko.
7. Hautatu **Ados**.

 > [!NOTE]
 > Honek datu orokorrak banatuko ditu **ResCalendarCapacity** zure inguruneko enpresa guztien artean egin ezazu, beraz, sorta lana pertsona juridiko bakarrean exekutatu behar da. Loteko lan honetako datuak beharrezkoak dira baliabideen ahalmena lotutako egutegiaren bidez kalkulatzeko.

8. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Proiektuaren baliabideak** > **Bideratu proiektuaren baliabideak enpresa guztietan** eta, ondoren, hautatu **Ados**. Hau da datuen bertsio berriaren gidoia **ResProjectResource**, **ResCalendarDateTimeRange** eta **ResEffectiveDateTimeRange** mahaiak. **PSAPRojSchedRole.RootActivity** eremuko balioak ere eguneratu dira. Hau exekutatzen ez bada, abisu bat jasoko duzu baliabideak antolatzeko eragiketak egiten saiatzean.
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a>Desaktibatu baliabideak antolatzeko errendimendua hobetzea

1. Joan **Ezaugarrien kudeaketa** > **Guztiak** eta bilatu **Gaitu proiektuaren baliabideen antolaketa errendimendua hobetzeko eginbidea**.
2. Aukeratu funtzioa eta, ondoren, hautatu **Desgaitu** botoia.
3. Freskatu arakatzailea.
4. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Edukiera sinkronizatzea** > **Sinkronizatu baliabideen ahalmenak** aukerara.
5. **Edukiera biltzeko sinkronizazioa** orrialdean, ezarri **Kendu dauden gaitasun erregistroak** **Bai** aurreko datuak kentzeko. Datu inkrementalak sortu nahi badituzu, ezarri **Ez**.
6. **Garai-kodea** eremuan, hautatu datuak zein alditan sortu behar diren. Garai kode bat hautatzen baduzu, ez da hasiera eta amaiera data zehaztu behar.
7. **Garai kodea** eremua hutsik uzten baduzu, hautatu hasiera eta amaiera data zehatzak datuak sortzeko.
8. Hautatu **Ados**.

> [!NOTE]
> Honek datu orokorrak banatuko ditu **ResRollup** zure inguruneko enpresa guztien artean egin ezazu, beraz, sorta lana pertsona juridiko bakarrean exekutatu behar da. Batch lan hau beharrezkoa da guztientzat **Baliabideen erabilgarritasuna** ikuspegiak. Batch lan hau exekutatzen ez bada, **ResRollup** datuak hegan sortuko dira eta horrek denbora behar dezake.


[!INCLUDE[footer-include](../includes/footer-banner.md)]