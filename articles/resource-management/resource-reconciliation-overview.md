---
title: Baliabideen berdinkatzearen informazio orokorra
description: Gai honek proiektuetarako baliabideen erreserbak eta zereginak bat datozela ziurtatzen lagunduko dizun informazioa eskaintzen du.
author: ruhercul
ms.date: 01/08/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: intro-internal
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 5c48589e745dbf6e3a51ae749b9b45491d26406e
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368191"
---
# <a name="resource-reconciliation-overview"></a>Baliabideen berdinkatzearen informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Taldekideentzat, erreserbak eta zereginak bateratu egiten dira. Alegia, baliabideek zereginak izan ditzakete baina erreserbarik ez, eta erreserbak izan ditzakete eta zereginik ez. Egokiena, erreserbak eta zereginak lerrokatuta egotea izango litzateke, baliabideek zereginak betetzeko gaitasuna konprometituta izan dezaten. Hala ere, erreserbak erabilgarritasunean oinarrituta egon litezke, eta zereginen aldaketak proiektuak aurrera egin ahala alda litezke. Hori dela eta, erreserbak eta zereginen akoplamendu solteak malgutasuna ematen du.

**Kontziliazioa** fitxak **Proiektuak** orrian, proiektu-kudeatzaileei taldekideen erreserbak eta proiektuko taldeen zereginak bateratzeko aukera ematen die.

**Kontziliazioa** fitxak erreserbak eta zereginak erakusten ditu zereginen esleipen bakoitzaren mailan taldekide bakoitzarentzat. Ordutegia erakusten du gelaxkatan, hilabetetik egunera arteko epeak. Fitxak proiektuaren guztizko garbi osoa ere erakusten du, **Guztira** zutabearekin batera.

Baliabide bakoitzerako, **Kontziliazioa** fitxak taldekidearen erreserben desberdintasunak kalkulatzen ditu eta taldekideen zereginen esleipenekin bateratzen ditu. Egokiena, aldea 0 (zero) izatea da. Beste modu batera esanda, ez litzateke alderik egon behar erreserbaren eta esleipenen artean. Desberdintasunak koloreztatuta eta itzalpean daude bi baldintzetan arreta jartzeko:

- **Erreserba eskasia**: erreserba eskasia gertatzen da baliabideek erreserbak baino esleipen gehiago dituztenean. Ez denez erreserbatu gaitasun hori, baliteke proiektu-kudeatzaileak baldintza hori zuzentzea baliabideen erreserbak hedatuz defizita estaltzeko.
- **Gehiegizko erreserbak** - Gehiegizko erreserbak baliabide bat proiektuan erreserbatuta dagoenean baina zereginetara esleitu ez denean gertatzen da. Baldintza hau onargarria izan daiteke zereginen esleipena gertatu baino lehen proiektuan erreserbatu den kasuetan. Hala ere, beste kasu batzuetan, baliabidea zereginei esleitzeko asmorik ez dagoenean, proiektuaren kudeatzaileak baliabidearen erreserbak bertan behera uztea pentsatu beharko luke. Modu horretan, edukiera beste proiektu baterako erabil daiteke.

Zenbait kasutan, eguneko maila baino maila altuagoan ikusten baduzu (adibidez, hilabetearen maila), baliteke zero diferentzia garbia izatea baliabide batentzat (beste modu batera esanda, erreserbak berdin zereginak). Hala ere, Astea mailari erreparatuz gero, baliteke 0 (zero) orduko esleipenak eta 40 orduko erreserbak daudela ikustea lehenengo astean, baina 40 orduko esleipenak eta 0 (zero) orduko erreserbak bigarren astean. Oro har, erreserbak eta zereginak bateratu egiten dira, baina aste batetik bestera desberdinak dira.

Denbora-maila altuagoak ikusten dituzunean, **Kontziliazioa** fitxak gelaxkak adierazle bat du denbora maila baxuagoetan desberdintasunak daudela jakinarazteko. Gelaxka bat bi aldiz sakatuta edo klik bikoitza eginez, handiagotu dezakezu aldea ikusteko. Ondoren, hautatu eta eutsi (edo egin klik eskuineko botoiarekin) hurbiltzeko. Baliabide bat hautatuta eta, ondoren, erabilita **Hurrengo aldea** kontrola saretako tresna-barran, baliabide horren erreserbak eta zereginen arteko hurrengo diferentziara joan zaitezke. Ondoren, erabil dezakezu **Aurreko aldea** kontrola atzera egiteko. Alderantzizko adierazlea eta nabigazio portaera ere desaktiba ditzakezu **Ezarpenak** aukeran.

Zereginen esleipenak dituzun baina erreserbarik ez baduzu, hautatu erreserba-falta **Kontziliazioa** fitxan, **Proiektuak** orrian, erreserba eskasia aukeratu dezakezu eta, ondoren, hautatu **Hedatu erreserba**. Agertzen den **Luzatu Erreserba** elkarrizketa-koadroan eta baliabidearen eskasiari aurre egiteko beharrezkoa den erreserba erakusten du. Elkarrizketa-koadroan baliabideek dituzten erreserbak agertzen dira proiektu guztietan edo beste erakunde antolatzaile batzuetan. Aukeratzen baduzu **Ados** baliabidearen erreserba sortzeko, baliabidearen erabilgarritasuna edozein dela ere, gerta daiteke erreserba gehiegi egotea.

Webgunearen bidez sortzen diren erreserbak **Luzatu erreserba** ekintza lehen proiektuaren eskakizunarekin lotzen da. Luzapen bat hasten denean, ezin da zehaztu luzatu behar den eskakizun zehatza, baliabidea proiekturako baldintza bat baino gehiagorekin lotu baitaiteke.

Orduan, proiektu-kudeatzaileak edo baliabide-kudeatzaileak antolaketa-panela erabil dezake baliabide batek bere ahalmenetatik harago gaitasunak gainditutako edozein egoera kudeatzeko.


[!INCLUDE[footer-include](../includes/footer-banner.md)]