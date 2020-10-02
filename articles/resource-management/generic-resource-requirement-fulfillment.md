---
title: Baliabide-eskakizun orokorrak betetzea
description: Gai honek baliabide generikoen eskakizunetarako izendatutako baliabideei buruzko informazioa eskaintzen du.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 76dd47fa2451b5cb61298ff332d77bae646a288a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897571"
---
# <a name="generic-resource-requirement-fulfillment"></a>Baliabide-eskakizun orokorrak betetzea

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Izena duen baliabide bat erreserbatu dezakezu baliabide.eskakizuna duten baliabide generikoak ordezkatzeko.baliabide

1. **Proiektuak** orrian, hautatu **Taldea** fitxa.
2. Hautatu zerrendatik baliabide-eskakizunen bat duen baliabide orokorra eta hautatu **Erreserbatu** aukeran. Edo ireki baliabide-eskakizuna eta hautatu **Erreserbatu** aukeran.
3. **Antolaketa-laguntzailea** orrialdean, hautatu izena duen baliabidea proiektu taldean erreserbatzeko eta hautatu **Erreserbatu** aukeran.

Erreserba izena duen baliabide batek osatu eta betetzen duenean, baliabide generikoa izena duen baliabidearen bidez ordezkatuko da.

Antolaketako zereginak izena duen baliabidearekin ere eguneratzen dira.

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a>Bete baliabide generikoa izena duten hainbat baliabiderekin
Baliabide generiko baten eskakizuna izena duten hainbat baliabiderekin betetzea, izena duen baliabide bakarra esleitzearen antzekoa da. Adibidez, bost eguneko eta 120 orduko iraupena duen zeregina dago. Zeregin hau ezin du bost eguneko astean zehar zortzi orduko lanordu tipikoa lantzen duen baliabide batek osatu. 

Eskakizuna 120 egunetan robotikako ingeniaritza bost egunetan zehar egiteko da, hau da, eguneko 24 ordukoa.

Izena duten hainbat baliabide behar direnean eskaera generiko bat betetzeko adibidea. Baliabide ugari erreserbatu beharko dituzu baldintza betetzeko.

Gertaera honen alderik nagusia baliabide generikoa zereginari esleitutako taldean geratzen dela da, eta erreserbatutako izena duten taldekideak ez dira karguaren zati gisa esleitzen. Proiektuaren zuzendariak lana izena duten baliabideei egoki eman diezaieke. The **Kontziliazioa** ikuspegiak lagun diezaioke proiektuaren kudeatzaileari zereginak burutzeko baliabide ugaritan erreserbak hausten. Hori ez da automatikoki egiten, aurreko adibide soilak baino konplikatuagoa den edozein agertokitan, esaterako, eskakizuna osatzen duen zeregin-sorta bat daukazunean edo sistemak proiektuak bere gain hartu nahi duen asmoa. Sistemak ezin duenez ulertu helburua, posible da suposizioak aurreikusitakoengandik desberdinak izatea eta aurreikusitako emaitza okerra edo aurreikusi ezin dena gertatuko dela. Aurreikus daitekeen emaitza baliabide generikoa esleituta mantentzen dela da proiektuaren kudeatzaileak nahitaez zereginak sortu arte, programaren **Kontziliazioa** ikuspegiaren laguntzarekin.


