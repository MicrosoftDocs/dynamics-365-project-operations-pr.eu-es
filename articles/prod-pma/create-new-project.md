---
title: Sortu proiektua
description: Gai honek proiektu berri bat sortzeari buruzko informazioa ematen du.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ee576561e9d360c198a57f5885c27aa782267fd1
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/04/2022
ms.locfileid: "8685041"
---
# <a name="create-a-new-project"></a>Sortu proiektua

[!include [banner](../includes/banner.md)]

Osatu urrats hauek proiektu berria sortzeko.

1. **Proiektuaren kudeaketa** orria, hautatu **Proiektu berria**, eta idatzi hurrengo balioak:

    - **Proiektu mota:** Denbora eta materiala
    - **Proiektuaren izena:** XYZ berritzea 2. fasea
    - **Proiektu taldea:** TM\_WIP
    - **Proiektuaren kontratua ID:** 00000002

2. Hautatu **Sortu proiektua**.

## <a name="assign-a-resource-to-a-project"></a>Esleitu baliabide bat proiektu bati

1. Gainean **Langileak** orrialdean, **Langileak** zerrenda, hautatu erregistroa langilearentzat aurretik konfiguratu gaitasunak horretarako, eta ireki langilearen erregistroa.
2. Ekintza panelean, **Proiektua** fitxan, **Konfigurazioa** taldea, hautatu **Esleitu proiektuak**.
3. Gainean **Baliabideak balioztatzeko proiektuaren esleipenak** orrialdean, **Proiektuak** fitxan, **Gehitu proiektua hautatutako proiektuei** eremua, iragazkia **XYZ berritzea 2. fasea** proiektua.
4. **Gainerako proiektuak** panelean, hautatu proiektu bat eta, ondoren, hautatu gezi botoia gehitzeko **Aukeratutako proiektuak** panela.

Baliabide batentzako kategoriak ere eska ditzakezu nahi duzun moduan. Kategoria mota bai da **Kostua** edo **Diru-sarrerak**. Kategoria mota zure erakundeak zehazten du. Baliabide batentzako kategoriarik esleitzen ez bada, Finantzak kostuen eta diru-sarreren orduen prezioen kategoria lehenetsia bilatzen du.

## <a name="set-up-project-resource-and-role-characteristics"></a>Ezarri proiektuaren baliabideen eta rolen ezaugarriak

Proiektu kudeatzaile batek proiektuaren baliabideen funtzionalitatea erabil dezake proiektuan beharrezkoak diren rolak sortzeko. Rolak erabil daitezke baliabideak erreserbatzen direnean berretsitako baliabideak oraindik ezezagunak badira. Eginkizunak aldi baterako gorde daitezke aurreikusitako baliabide gisa, proiektuaren plangintza faseak jarraitu ahal izateko.

[![Rol baten adibidea.](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg) 

**Eszenatokia:** Contoso kontratatu zen onartutako proiektuen karta duen Denbora eta material proiektu bat osatzeko. Proiektu zuzendari gaztea proiektuaren esparrua osatzen ari da oraindik. Baliabideen kudeatzailea proiektu berrian lan egiteko gordetako baliabide zehatzak identifikatzen ari da. Proiektuaren izaera kritikoa dela eta, proiektuaren babesleak proiektu nagusiko zuzendaria eskatu zuen eginkizunetako bat izateko. Baliabideen kudeatzaileak baliabide berria eskuratu behar du eta sistemako rola definitu behar du, proiektuaren kudeatzaile juniorrak proiektuaren plangintza egitean baliabideen informazioa behar badu.

Ondorengo pausoek erakusten dute baliabideen kudeatzaileak proiektuaren arduradun nagusiaren eginkizuna nola konfigura dezakeen eta baliabideen ezaugarriak harekin lotzen dituen. Geroago, eginkizuna eskatutako baliabideen eskumenekin bat datozen baliabide erabilgarriak bilatzeko erabil daiteke.

1. **Konfigurazio-funtzioak** orria, hautatu **Berria**, eta idatzi hurrengo balioak:

    - **Rolaren IDa:** Proiektu zuzendari nagusia
    - **Deskribapena:** Proiektu zuzendari nagusia

2. Hautatu **Sortu**.
3. Aukeratu **Proiektu zuzendari nagusia** rola, eta hautatu **Ezaugarriak konfiguratu**.
4. **Ezaugarri mota** eremua, hautatu **Gaitasuna**.
5. **Erabilgarri dauden ezaugarriak** eremuan, sartu bilatu beharreko trebetasuna.
6. **Ezaugarrien mota** eremua, hautatu **Ziurtagiria**.
7. **Erabilgarri dauden ezaugarriak** eremuan, sartu bilatu beharreko ziurtagiri mota.

## <a name="assign-a-project-resource-to-a-project"></a>Esleitu proiektuaren baliabide bat proiektu bati

1. Gainean **Proiektu guztiak** orria, hautatu **XYZ berritzea 2. fasea** proiektua.
2. Gainean **Proiektu taldea eta programazioa** fitxa, hautatu **Gehitu**.
3. **Rola** eremua, hautatu **Taldekidea**.
4. Hautatu **Erreserbatu egutegia**.
5. Gainean **Baliabideen erabilgarritasuna** orrialdea, hautatu **Ikusi ezarpenak**.
6. Gainean **Doitu ikuspegiaren ezarpenak** orrian, sartu balio hauek:

    - **Data tartea ikusteko formatua:** Eguna
    - **Bistaratu erabilgarritasunaren deskribapenak:** Bai
    - **Gainerako edukiera bistaratu:** Bai

7. Baliabide-zerrendan, hautatu baliabidea.
8. Aukeratu **Liburu gogorra** eta **Edukiera osoa**.

## <a name="assign-a-resource-to-a-default-role"></a>Esleitu baliabidea lehenetsitako funtzioa

Proiektu edo baliabideen kudeatzaileek proiektu baterako gorde daitezkeen baliabideak sakondu ditzakete. Rol lehenetsia lehendik dagoen baliabide batekin edo eskuratu berri den baliabide batekin lotu dezakezu. Adibidez, Daniel kontratatu zutenean, esperientzia eta trebetasunak zituen Enpresa analista papera betetzeko. Baliabideen kudeatzaileak rol hau Danielen lehenetsitako rol gisa izendatu du. Hori dela eta, baliabideen zuzendariak Daniel gehitu zuen proiektuetan lan egiteko erabilgarri dauden negozio analista multzo batean.

Baliabideak erreserbatu bitartean, proiektuen arduradunek proiektuetan lan egiteko erabilgarri dauden rol baliabideak iragazi ditzakete. Informazio hori irizpide gisa erabil dezakete, baliabideen betetzean irizpide anitzeko erabakien analisia egiten dutenean. Iragazkiari beste baliabide batzuen ezaugarriak ere gehi ditzakete proiektu jakin baterako trebetasunak, hezkuntza eta esperientzia zehatzak dituzten baliabideak bilatzeko.

**Eszenatokia:** Onartutako proiektua hasi da, eta proiektuaren zuzendari nagusiaren eginkizuna planifikatutako baliabide gisa gorde da proiektuaren plangintza fasean. Baliabideen kudeatzaileak baliabide bat eskuratu du orain Senior proiektuaren kudeatzaile rola betetzeko.

1. Gainean **Baliabideen zerrenda** orrialdea, hautatu **Daniel Goldschmidt**.
2. **Baliabide-funtzioa** orria, hautatu **Berria**, eta idatzi hurrengo balioak:

    - **Eraginkorra:** Sartu uneko data.
    - **Iraungipena:** Sartu **Inoiz ez**.
    - **Funtzioa:** Idatzi **Proiektu zuzendari nagusia**.

3. Aukeratu **Gorde**, eta gero itxi orria.
4. Gainean **Konpetentziak** fitxa, gehitu **ProjectMgmt** trebetasuna eta **PMP** ziurtagiria.


[!INCLUDE[footer-include](../includes/footer-banner.md)]