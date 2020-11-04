---
title: Sortu proiektuaren taldea
description: Gai honek proiektu-taldeak sortzeari eta kudeatzeari buruzko informazioa ematen du.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kdwns
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a7eb9101352afd27b527bf6b8acc6f92198f44ea
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4071201"
---
# <a name="create-a-project-team"></a>Sortu proiektuaren taldea

[!include [banner](../includes/banner.md)]

Aurretik proiektu batean konfiguratutako eginkizunak erabiltzeko, proiektuaren kudeatzaileak eginkizunak proiektuarekin lotu behar ditu. Hainbat eginkizun esleitu daitezke proiektu baterako. Nahasmena ekiditeko, funtzio hauek automatikoki etiketatzen dira erreserbatu bitartean. Adibidez, proiektuaren zuzendariak hiru software ingeniari behar baditu, hiru Software ingeniari funtzio betetzen dituzte **software ingeniaria 1** , **software ingeniaria 2** , eta **software ingeniaria 3** haien etiketak automatikoki sortzen baitira. Aurretik rolaren ezaugarriak rolerako ezarri badira, iragazki gisa aplikatuko dira baliabide bat bilatzerakoan. Ezaugarri osagarriak gehi daitezke, bilaketa gehiago zehazteko beharrezkoak diren moduan.

Ikuspegi ezarpenak pertsonaliza daitezke, baliabideen erabilgarritasuna hobeto ikusteko. Ordubeteko, eguneroko, asteko, hileko, hiruhileko eta urteko erabilgarritasuna erakusteko aukerak daude. Baliabideetan eskuragarri eta geratzen den gaitasuna erakusteko aukera ere badago. Aukera hau erabilgarria da denbora kudeatzeko, jardueretarako edo baliabideen erabilgarritasunerako denbora librea kalkulatzen duzunean.

Proiektuaren kudeatzaileak orrialdeko rol bat hauta dezake eta, gero, eskakizunera egokitzen den baliabide erabilgarri bat badago, hautatu papera betetzeko baliabide bat gordetzea. Kontuan izan baliabideak ez direla zertan erreserbatu plangintza faseko une honetan. WBS bat sortzen duzunean, eginkizunak proiektuko langileekin ordezkatu ditzakezu. Rolak WBSn langileekin hornitutako baliabideekin ordezkatzen badira, baliabideen konfigurazioak proiektuaren taldeen zerrenda eta programazioa automatikoki eguneratuko ditu.

[![Eginkizunak eta benetako baliabideak biltzen dituen proiektu taldeen zerrenda](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg) 

Proiektuaren kudeatzaileak proiektu baterako baliabide bat erreserbatzeko hainbat aukera ditu, adibidez **Gainerako gaitasuna** , **Edukiera osoa** , **Edukiera ehunekoa** , eta **Zehaztu orduak**. Erreserba aukera hauek edozein unetan bertan behera utzi daitezke baliabideen esleipenak aldatzen badira. Bi erreserba mota onartzen dira:

- **Liburu gogorra** - Baliabideen erreserba onartu eta baieztatu zen konpromisoan zehaztutako iraupenean lan egiteko.
- **Behin behineko erreserba** - Baliabideen erreserbak behin-behinean zen konpromisoan zehaztutako iraupenean lan egiteko.

Prozedura honetan azaltzen nola proiektuaren taldea sortu:

## <a name="create-a-project-team"></a>Sortu proiektuaren taldea

1. Gainean **Proiektu guztiak** zerrendaren orria, hautatu proiektu bat eta, ondoren, hautatu **Editatu**.
2. Gainean **Proiektu taldea eta programazioa** fitxan, **Egitarauaren amaiera data** eremuan, sartu programazioaren hasiera data gehi hilabete bat. Adibidez, ordutegia hasteko data 2017ko ekainaren 24a bada (2017/06/24), sartu **2017/07/24**.
3. Hautatu **Gehitu**.
4. **Gehitu eginkizunak proiektuari** panelean, **Rola** eremua, hautatu **Proiektu zuzendari nagusia**.
5. Aukeratu **Eskatutako gaitasunak**.
6. Gainean **Aukeratu ezaugarriak** orrialdean, lehenago zuzendari nagusiaren eginkizunerako zehaztutako ezaugarriak lehenespenez hautatzen dira. Hautatu **Ados**.
7. Gainean **Gehitu rolak proiektuari** orrialdean, **Baliabide kopurua** eremua, sartu **1**.
8. **Baliabidea** eremuan, bilaketak beharrezko gaitasunak dituzten baliabide guztiak erakusten ditu. Aukeratu **Daniel Goldschmidt** eta, ondoren, hautatu **Sortu**.
9. **Proiektua** orrian, hautatu **Gehitu**.
10. **Gehitu eginkizunak proiektuari** panelean, **Rola** eremua, hautatu **Taldekidea**. **Baliabide-kopurua** eremua, sartu **5**.
11. Hautatu **Sortu**.
12. Gainean **Proiektuak** orrialdea, hautatu **Baliabidea bete**.

## <a name="monitor-project-teams"></a>Proiektu taldeak kontrolatu
1. **Proiektu guztiak** orria, hautatu **Proiektuaren ID-a** esteka **XYZ Bertsio berritu fasea 2** proiektua.
2. Gainean **Proiektu taldea eta programazioa** FastTab, egiaztatu zerrendan agertzen diren proiektuaren baliabideak zuzenak direla.
