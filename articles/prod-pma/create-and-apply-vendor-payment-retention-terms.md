---
title: Sortu eta aplikatu saltzailearen ordainketa atxikitzeko baldintzak
description: Gai honetan saltzailearen ordainketetarako atxikipen baldintzak konfiguratzeko eta mantentzeko moduari buruzko informazioa ematen da.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
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
ms.openlocfilehash: 1970a24a5073de6af43db1f1c068332c9ba9c8fe
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071173"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a>Sortu eta aplikatu saltzailearen ordainketa atxikitzeko baldintzak

[!include [banner](../includes/banner.md)] 

Saltzaileari ordainketa atxikitzeko baldintzak konfiguratzea proiektu baterako erabilgarria da zure erakundeak saltzaile bati egindako ordainketen zati bat gorde nahi duenean. Adibidez, saltzaile bati ordainketa egin nahi diozunean entregatutako produktuek zure itxaropenak bete arte. Saltzailearen ordainketa atxikitzeko baldintzak zehaztu daitezke saltzailearen kontratua negoziatzen duzunean.

## <a name="create-vendor-payment-retention-terms"></a>Sortu saltzailearen ordainketa atxikitzeko baldintzak

Atxikitzeko saltzailearen ordainketaren portzentajea eta aurrez gordetako zenbatekoen zenbatekoa sartu ditzakezu. Kopuruak automatikoki gordetzen dira saltzailearen fakturetan, kontratua zehaztutako amaierako egoerara iritsi arte. Atxikitzeko baldintzak konfiguratu ondoren, saltzaile horrentzako edozein proiektutan aplika ditzakezu.

Erabili urrats hauek saltzailearen ordainketetarako atxikipen baldintzak konfiguratzeko eta mantentzeko. 

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Atxikipena** > **Saltzailearen ordainketa atxikitzeko baldintzak**.
2. Aukeratu **Berria** saltzailearen atxikipen epe berria gehitzeko. **Arauaren IDa** termino berriaren balioa automatikoki sartzen da. 
3. Idatzi deskribapen laburra fitxategian **Deskribapena** eremuan eta **Baldintzak** FastTab-en, hautatu **Gehitu lerroa** hauetarako terminoen balioak sartzeko:

   - **Entregatutako unitateen ehunekoa** : Idatzi epea osatzearen ehunekoa. Kopuruak automatikoki gordetzen dira saltzailearen fakturetan, proiektuaren osatze-fasea eta zehaztutako ehunekoa bera den arte. Adibidez, 50,00 idazten baduzu, zenbatekoak mantenduko dira proiektua ehuneko 50 arte osatu arte.
   - **Atxikitzeko ehunekoa** : Sartu nahi den saltzailearen fakturaren zenbatekoaren ehunekoa. Adibidez, 10,00 idazten baduzu, saltzailearen fakturaren zenbatekoaren ehuneko 10 mantenduko da, proiektuak atalean ezarritako amaierako ehunekoa lortu arte **Emandako eremuen ehunekoa**.
   - **Askatzeko ehunekoa** : Aukeratu **Gehitu lerroa** hautatutako proiektuaren amaierarako askatu beharreko zenbatekoen ehunekoa sartzeko.

> [!NOTE]
> Proiektua osatzeko maila desberdinetarako mugarri bat baino gehiago badituzu, idatzi saltzailearen atxikipen epe lerro bereizi atxikipen arau bakoitzerako. Lerro bakoitzak atxikipen portzentaje desberdina eta askapen portzentaje desberdina zehaztu dezake proiektuaren amaierako maila bakoitzerako.

Saltzailearen atxikitzeko baldintzak sortu ondoren, saltzaile horrentzako edozein proiektutan aplika ditzakezu.

## <a name="apply-vendor-retention-terms-to-a-project"></a>Aplikatu saltzaileari atxikitzeko baldintzak proiektu bati

1. Joan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuak** > **Proiektu guztiak** eta ireki proiektu bat proiektuen zerrendatik.
2. **Saltzaileen akordioak** FastTab-en, hautatu **Gehitu lerroa**.
3. **Kontuaren kodeaeremuan** , hautatu aukera hauetako bat: 

   - **Taula** : Saltzailearen atxikitze-baldintzak saltzaile bakar bati aplikatzen zaizkio.
   - **Taldea** : Saltzailearen atxikitze-baldintzak saltzaile talde bateko saltzaile guztiei aplikatzen zaizkie.
   - **Guztia** : Saltzailearen atxikitze-baldintzak saltzaile guztiei aplikatzen zaizkie.

4. **Saltzailea/Saltzaile taldearen eremuan** , hautatu saltzailea edo saltzaile taldea zein saltzaileren atxikitze baldintzak aplikatzen diren. Aukeratu baduzu **Guztiak** aurreko urratsean, eremu hau ez dago erabilgarri.
5. **Saltzailearen atxikitze baldintzak** eremuan, hautatu aurreko prozeduran sortutako atxikitze terminoak.
6. Proiektuak saltzailearentzako ordaindutako ordainketa (PWP) baldintzak ere baditu, sartu proiektuaren atalase portzentajea **PWP atalasearen ehunekoa** eremua.

Saltzaileari atxikitzeko baldintzak saltzailearentzat sortzen dituzun erosketa-eskaeretan ere agertzen dira.


[!INCLUDE[footer-include](../includes/footer-banner.md)]