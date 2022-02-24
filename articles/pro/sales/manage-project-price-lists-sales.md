---
title: Kudeatu proiektuen prezio-zerrendak proiektu-eskaintzetan
description: Gai honek proiektuko prezio-zerrendako eskaintzekin lan egiteari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 912d2fad33ac02c3ba980da7eeb88eef5c331230
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858593"
---
# <a name="manage-project-price-lists-on-project-quotes"></a>Kudeatu proiektuen prezio-zerrendak proiektu-eskaintzetan 

_**Honi aplikatzen zaio:** Oinarrizko inplementazioa: kudeatu proformako fakturak_

Proiektuaren aurrekontuak salmenta prezioen zerrenda eraginkor bat baino gehiagorako diseinatuta daude. Dynamics 365 Project Operations-ekin, izeneko entitate elkartu berria **Proiektuen prezioen zerrendak** gehitzen da. Entitate honek 1etik askorako harremana du proiektuaren aurrekontuarekin.

Proiektuen prezioen zerrendak proiektu bateko denbora, materiala eta gastuen transakzioak preziatzeko erabiltzen dira. Eskaintza batek proiektuen prezio zerrenda bat edo gehiago dituenean, prezio zerrenda hauek denboraren, materialaren, gastuen kalkuluen eta eskaintzari loturiko proiektuen eskaintzaren bidez lotzen diren proiektuen prezioak egiteko erabiltzen dira.

Proiektuaren aurrekontuan proiektuaren prezio zerrendarik ez dagoenean, abisu mezua jasoko duzu. Mezuan esaten da proiektuaren prezioen zerrendarik ez dagoenez, zure proiektuaren eta kalkulatutako egiazko eta lanaren kostuak ez direla tasatuko. Horren ordez, zero (0) prezioa izango dute salmenten balioetarako.

## <a name="associate-or-disassociate-a-project-price-list-on-a-project-quote"></a>Elkartu edo desegin proiektuaren prezioen zerrenda proiektuaren aurrekontuan

Proiektuetan oinarritutako lana eta gastuak kalkulatzeko prezio zerrenda jakin bat sortzeko edo hautatzeko, jarraitu urrats hauek.

1. Aurrekontuan, hautatu **Proiektuaren prezioa** fitxa eta azpisarean, hautatu **+ Gehitu proiektu berriaren prezio zerrenda**.
2. Sortu azkar orrian, hautatu prezioen zerrenda. Goitibeherako zerrendan testuingurua ezarrita duten prezio zerrenda guztiak agertzen dira **Salmentak** eta moneta aurrekontuaren moneta bat dator.
4. Idatzi proiektuaren prezioen zerrenda elkartearen deskribapena eta hautatu **Gorde eta itxi**.

Proiektuaren prezio-zerrendaren lotura sortu da.

Prozesu hau errepika dezakezu proiektuaren prezio zerrenda bat baino gehiago proiektuaren aurrekontuarekin lotu behar baduzu. Sortu proiektuaren prezio zerrenda bat baino gehiago lotutako proiektuaren prezio zerrenda bakoitzean data eraginkor desberdinak badituzu.

> [!NOTE]
> Proiektuaren eragiketek ez dute onartzen proiektuaren prezio zerrenden data gainjarrien eraginkortasuna. Data zehaztutako transakzio batentzako proiektuen prezioen zerrenda bat badago, transakzio horren prezioa zero (0) lehenetsiko da.
Proiektuen prezioen zerrenda elkartea kentzeko, hautatu proiektuaren prezioen zerrenda eta hautatu **Ezabatu aurrekontua proiektuaren prezioen zerrenda**. Prezio zerrenda aurrekontuaren proiektuaren prezio zerrendetatik kentzen da, baina prezio zerrenda bera ez da ezabatzen. Aurrekontuaren elkartea soilik ezabatzen da.

## <a name="set-up-default-project-price-lists-on-a-quote"></a>Konfiguratu lehenetsitako proiektuen prezioen zerrendak aurrekontuan

Proiektuaren prezioen zerrendak proiektuaren aurrekontua lehenetsita ezar daitezke. Konfigurazio honi esker, zure erakundeko aurrekontu guztiak prezio-aldi horretarako zerrenda estandar batekin hasten dira beti.

### <a name="set-up-organizational-default-for-project-price-lists"></a>Konfiguratu erakundeko balio lehenetsiak proiektuen prezioen zerrendak

1. Joan **Ezarpenak** > **Orokorra** > **Parametroak**.
2. **Parametro aktiboak** zerrendaren orria, bilatu erregistroa eta egin klik bikoitza irekitzeko. 
3. **Parametroak** orrian, hautatu **Prezioen zerrenda** fitxa. Prezioen zerrenda lehenetsien zerrenda agertzen da. Hau kostuen eta salmenta prezioen zerrenda estandarrak dira. Hemen saltzen dituzun moneta bakoitzeko salmenta prezioen zerrenda bat izateak ziurtatuko du moneta horretan jarduten duten bezeroentzat sortzen dituzun aurrekontuetan salmenta prezioen zerrenda lehenetsita dagoela.

### <a name="set-up-customer-specific-project-price-lists"></a>Konfiguratu bezeroarentzako proiektuaren prezioen zerrendak

Bezeroen berariazko proiektuen prezioen zerrendak ere ezar daitezke zure bezeroekin prezioen hitzarmen nagusia negoziatu duzunean.

Bezeroarentzako proiektuaren prezioen zerrenda konfiguratzeko, jarraitu urrats hauek.

1. **Salmentak** eremuan, hautatu **Bezeroak**.
2. Zure kontu aktiboen zerrendan, hautatu eta ireki prezioen zerrenda berezia duzun bezeroaren erregistroa.
3. **Proiektuen prezioen zerrendak** fitxan, prezio zerrenda elkarte berri bat sor dezakezu bezeroarentzako berariazko proiektuaren prezio zerrenda edukitzeko.

## <a name="create-custom-pricing-on-a-project-quote"></a>Sortu prezio pertsonalizatuak proiektuaren aurrekontuan

Erakundearen eta bezeroaren berariazko proiektuen prezioen zerrenda lehenetsiak izan ondoren, proiektuaren aurrekontuak automatikoki sortuko dira proiektuen prezioen zerrenda elkarte horiekin. Hala ere, zenbait kasutan, proiektuaren aurrekontu zehatz baterako prezio pertsonalizatuak sortu beharko dituzu. 

1. **Proiektuaren aurrekontua** aukeran, **Proiektuaren prezio-zerrenda** fitxan, egiaztatu azpisarean ez dagoela prezioen zerrendako erregistro zehatzik hautatuta.
2. Hautatu **Sortu prezio pertsonalizatua**. Honek aurrekontuarekin lotzen diren prezio zerrenda estandar guztien kopiak egingo ditu eta kopia horiek aurrekontuarekin lotuko ditu. Prezioen zerrenda estandarretarako dauden elkarteak kenduko dira. Orduan, saltzailea kopia hauen prezioen aldaketak egiten has daiteke. Aldatutako prezio hauek proiektuaren aurrekontu honi soilik aplikatuko zaizkio.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
