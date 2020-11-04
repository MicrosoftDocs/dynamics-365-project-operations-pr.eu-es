---
title: Baliabideen berdinkatzearen informazio orokorra
description: Gai honek baliabide-erreserbak eta esleipenak proiektuekin lerrokatuta daudela ziurtatzeari buruzko informazioa eskaintzen du.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e2b16a6e1c48769ed4d903e546804ba1c4e1c4fa
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070978"
---
# <a name="resource-reconciliation-overview"></a>Baliabideen berdinkatzearen informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Taldekideentzat, erreserbak eta zereginak bateratu egiten dira. Alegia, baliabideek zereginak izan ditzakete baina erreserbarik ez, edo erreserbak izan ditzakete baina zereginik ez. Egokiena, erreserbak eta zereginak lerrokatuta egotea izango litzateke, baliabideek zereginak betetzeko gaitasuna konprometituta izan dezaten. Hala ere, erreserbak erabilgarritasunean oinarrituta egon litezke, eta zereginen aldaketak proiektuak aurrera egin ahala alda litezke. Hori dela eta, erreserbak eta zereginen akoplamendu solteak malgutasuna ematen du.

**Proiektua** inprimakiko **Kontziliazioa** fitxari esker, kudeatzaileei taldekideen erreserbak eta proiektuko taldeen zereginak bateratzeko aukera.

**Kontziliazioa** fitxak ere erreserbak eta zereginak erakusten ditu zereginen esleipen bakoitzaren mailan taldekide bakoitzarentzat. Orduak erakusten ditu gelaxkatan, hilabetetik egunera arteko epeak.

Fitxak proiektuaren guztizko garbi osoa ere erakusten du, **Guztira** zutabearekin batera.

Baliabide bakoitzerako, fitxak taldekidearen erreserben desberdintasunak kalkulatzen ditu eta taldekideen zereginen esleipenekin bateratzen ditu. Egokiena, aldea 0 (zero) izatea da. Beste modu batera esanda, ez litzateke alderik egon behar erreserbaren eta esleipenen artean. Desberdintasunak koloreztatuta eta itzalpean daude bi baldintzetan arreta jartzeko:

- **Erreserba eskasia** : erreserba eskasia gertatzen da baliabideek erreserbak baino esleipen gehiago dituztenean. Ez denez erreserbatu gaitasun hori, baliteke proiektu-kudeatzaileak baldintza hori zuzentzea baliabideen erreserbak hedatuz defizita estaltzeko.
- **Gehiegizko erreserbak** - Gehiegizko erreserbak baliabide bat proiektuan erreserbatuta dagoenean baina zereginetara esleitu ez denean gertatzen da. Baldintza hau onargarria izan daiteke zereginen esleipena gertatu baino lehen proiektuan erreserbatu den kasuetan. Hala ere, baliteke beste kasu batzuetan baliabidea ez izatea aurreikusita zereginei esleitzeko. Kasu horietan, proiektu-kudeatzaileak baliabidearen erreserbak bertan behera uztea pentsatu beharko luke, gaitasuna beste proiektu baterako erabili ahal izateko.

Zenbait kasutan, eguneko maila baino maila altuagoan ikusten baduzu (adibidez, hilabetearen maila), baliteke zero diferentzia garbia izatea baliabide batentzat (beste modu batera esanda, erreserbak = zereginak). Hala ere, Astea mailari erreparatuz gero, baliteke 0 (zero) orduko esleipenak eta 40 orduko erreserbak daudela ikustea lehenengo astean, baina 40 orduko esleipenak eta 0 (zero) orduko erreserbak bigarren astean. Oro har, erreserbak eta zereginak bateratu egiten dira, baina aste batetik bestera desberdinak dira.

Denbora-maila altuagoak ikusten dituzunean, **Kontziliazioa** fitxak gelaxkak adierazle bat du denbora maila baxuagoetan desberdintasunak daudela jakinarazteko. Gelaxka batean klik bikoitza eginez, handiagotu dezakezu aldea ikusteko. Ondoren, egin klik eskuineko botoiarekin hurbiltzeko. Baliabide bat hautatuta eta, ondoren, erabilita **Hurrengo aldea** kontrola saretako tresna-barran, baliabide horren erreserbak eta zereginen arteko hurrengo diferentziara joan zaitezke. Ondoren, erabil dezakezu **Aurreko aldea** kontrola atzera egiteko. Alderantzizko adierazlea eta nabigazio portaera ere desaktiba ditzakezu **Ezarpenak** aukeran.


Zereginen esleipenak dituzun baina erreserbarik ez baduzu, **Proiektuak** aorrian, **Kontziliazioa** fitxan, erreserba eskasia aukeratu dezakezu eta, ondoren, hautatu **Hedatu erreserba**. **Luzatu Erreserba** elkarrizketa-koadroa agertuko da eta baliabidearen eskasiari aurre egiteko beharrezkoa den erreserba erakusten du. Gainera, baliabideek dituzten erreserbak agertzen dira proiektu guztietan edo beste erakunde antolatzaile batzuetan. Aukeratzen baduzu **Ados** baliabidearen erreserba sortzeko, baliabidearen erabilgarritasuna edozein dela ere, gerta daiteke erreserba gehiegi egotea.

Orduan, proiektu-kudeatzaileak edo baliabide-kudeatzaileak antolaketa-panela erabil dezake baliabide batek bere ahalmenetatik harago gaitasunak gainditutako edozein egoera kudeatzeko.

