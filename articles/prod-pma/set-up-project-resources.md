---
title: Konfiguratu proiektuan baliabideak
description: Gai honek proiektuko baliabideak konfiguratzeari edo eskatzeari buruzko informazioa ematen du.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 49e0ca6254518079d2e01d92ac2e31d119468c4b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997676"
---
# <a name="set-up-project-resources"></a>Konfiguratu proiektuan baliabideak

[!include [banner](../includes/banner.md)]

Egutegia konfiguratu eta langile batekin edo langile batekin lotu behar duzu. Egutegia proiektua eta proiekturako gordetako baliabideen lanaldia antolatzeko erabiltzen da. Egutegia konfiguratzerakoan, proiektuen kudeatzaileek baliabideen berdinketa egin dezakete baliabideak optimizatzearen barruan. Egutegiaren ordutegian oinarrituta, baliabideetan murrizketak jar daitezke. Egutegia konfigura dezakezu **Egutegiak** orrialdea.

Langile bat proiektuaren baliabide gisa konfiguratzen duzunean, enpresan lan egiten duten langileen artean baliabideak konfiguratzen ari zarenetik hauta dezakezu. Bestela, zure erakundeko beste enpresa batzuetako langileak hauta ditzakezu. Langile horiek enpresen arteko baliabideak bezala ezagutzen dira.

Ondorengo prozedurek langile bat zure enpresan proiektuaren baliabide gisa nola konfiguratu eta enpresen arteko proiektuaren baliabide bat nola konfiguratu azaltzen dute.

## <a name="set-up-a-worker-as-a-project-resource"></a>Konfiguratu langilea proiektuaren baliabide gisa

1. Gainean **Langileak** orrialdean, **Langileak** zerrenda, hautatu proiektuaren baliabide gisa gehitzen ari zaren langilea eta ireki langilearen erregistroa.
2. Ekintza panelean, hautatu **Proiektua** &gt; **Konfigurazioa** &gt; **Proiektuaren konfigurazioa**.
3. Aukeratu egutegi bat eta itxi orria.

Baliabide baterako proiektu lehenetsiak ere zehaztu ditzakezu aurrez esleitzeko mota gisa. Aurrez esleipenak baliabideen kudeatzaileak edo proiektuaren kudeatzaileak baliabideak aldez aurretik zein proiektutan landuko dituen dakienean erabil daitezke. Aurretiazko esleipenak proiektuaren babesle edo bezero baten eskaeran oinarrituta ere egin daitezke. Proiektu bat aurrez esleitzeko, **Proiektuak esleitu** orrialdean, **Proiektuak** fitxan, **Gainerako proiektuak** zerrenda, hautatu proiektu egokia.

## <a name="set-up-an-intercompany-resource"></a>Konfiguratu enpresen arteko baliabide bat

Langilea enpresen arteko baliabide gisa konfiguratzen duzunean, konfigurazioa osatu behar duzu bai mailegu-enpresan bai mailegu-enpresan.

### <a name="in-the-lending-company"></a>Mailegu-enpresan

1. Finantzetan, egiaztatu enpresa mailegu-emailea hautatuta dagoela eta, ondoren, osatu aurreko ataleko prozedura, "Konfiguratu langilea proiektuaren baliabide gisa."
2. **Konpainia arteko kontua** orrian, hautatu **Berria**.
3. **Pertsona juridikoaren IDa** eremuan, hautatu mailegu-enpresa. Bete gainerako eremuak egoki gisa, eta gero hautatu **Gorde**.
4. **Transferitzeko prezioa** orrian, hautatu **Berria**.
5. **Hartu legezko entitatea** eremuan, hautatu konpainia egokia.
6. Mailegu-enpresari atal honen hasieran sortu zenituen baliabideak soilik emateko **Baliabidea** eremuan, hautatu sortu duzun baliabidearen izena. Mailegu-enpresaren baliabide guztiak mailegu-enpresaren eskura jartzeko, utzi **Baliabidea** eremua hutsik.
7. Gainean **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, **Enpresa artekoa** fitxa, ezarri **Gaitu enpresen arteko baliabideen programazioa eta denbora-orriak** aukera **Bai**.

### <a name="in-the-borrowing-company"></a>Hartutako konpainian

- Gainean **Baliabideen zerrenda** orrian, bilaketa-iragazkian, idatzi mailegu-enpresarentzat sortu duzun baliabidearen izena, izena mailegu-enpresaren baliabideen zerrendan sartuta dagoela egiaztatzeko.

## <a name="request-project-resources"></a>Proiektuaren baliabideen eskaera
Proiektuaren baliabideen antolaketarako funtzionaltasunak baliabideen kudeatzaileek konpromiso edo proiektuetan pertsonaleko baliabideak banatu ditzaten soilik. Funtzionalitate hau gaitzeko, burutu zeregin hauek edo egiaztatu egin direla:

- Konfiguratu zenbaki sekuentziak.
- Konfiguratu proiektuen kudeaketa eta kontabilitate lan-fluxuak.
- Gaitu baliabideen eskaera-fluxuak.

Aurreko zereginak amaitu ondoren, zeregin hauek bete ditzakezu nahi duzun moduan:

- Sortu baliabide eskaera bat gordetako langileen baliabide batetik.
- Monitorizatu baliabide-eskaerak.
- Baliabide-eskaerak bete.
- Eskatu baliabide pertsonal bat WBS bati.
- Erreserbatu baliabideak proiektu batera, pertsonaleko baliabiderik eskatu gabe.


[!INCLUDE[footer-include](../includes/footer-banner.md)]