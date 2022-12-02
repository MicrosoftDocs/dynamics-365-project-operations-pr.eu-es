---
title: Erreserbatu izendatutako baliabideak baliabide-eskakizunetatik
description: Gai honek baliabide generikoen eskakizunetarako izendatutako baliabideei buruzko informazioa eskaintzen du.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 9598490da1905227e517da8ba90f8ffd1df88566
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8916227"
---
# <a name="book-named-resources-from-resource-requirements"></a>Erreserbatu izendatutako baliabideak baliabide-eskakizunetatik

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Izena duen baliabide bat erreserbatu dezakezu baliabide.eskakizuna duten baliabide generikoak ordezkatzeko.baliabide

1. Project Service Automation-en (PSA), **Proiektuak** orrialdean, egin klik **Taldea** fitxan.
2. Hautatu zerrendatik baliabide-eskakizunen bat duen baliabide orokorra eta egin klik **Erreserbatu** aukeran. Edo ireki baliabide-eskakizuna eta egin klik **Erreserbatu** aukeran.


![Taldekide generiko bat erreserbatzea.](media/RM-how-to-14.png)


3. **Antolaketa-laguntzailea** orrialdean, hautatu izena duen baliabidea proiektu taldean erreserbatzeko eta egin klik **Erresrbatu** aukeran.

![Taldekide generiko bat erreserbatu, antolaketa-laguntzailea erabilita.](media/RM-how-to-15.png)

Erreserba izena duen baliabide batek osatu eta betetzen duenean, baliabide generikoa izena duen baliabidearen bidez ordezkatuko da.

![Izena duen taldekidea talde generikoko kide bat ordezkatuz.](media/RM-how-to-16.png)

Antolaketako zereginak izena duen baliabidearekin ere eguneratzen dira.

![Izena duen taldekidea proiektu-zereginari esleituta.](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a>Bete baliabide generikoa izena duten hainbat baliabiderekin
Baliabide generiko baten eskakizuna izena duten hainbat baliabiderekin betetzea, izena duen baliabide bakarra esleitzearen antzekoa da. Adibidez, bost eguneko eta 120 orduko iraupena duen zeregina dago. Zeregin hau ezin du bost eguneko astean zehar zortzi orduko lanordu tipikoa lantzen duen baliabide batek osatu. 

![Bost egunetan 120 orduko ahalegina behar duen zeregina.](media/RM-how-to-21.png)

Eskakizuna 120 egunetan robotikako ingeniaritza bost egunetan zehar egiteko da, hau da, eguneko 24 ordukoa.

![Eguneko eskakizuna.](media/RM-how-to-22.png)

Izena duten hainbat baliabide behar direnean eskaera generiko bat betetzeko adibidea. Baliabide ugari erreserbatu beharko dituzu baldintza betetzeko.

![Baliabide ugari erreserbatu baldintza betetzeko.](media/RM-how-to-23.png)

Gertaera honen alderik nagusia baliabide generikoa zereginari esleitutako taldean geratzen dela da, eta erreserbatutako izena duten taldekideak ez dira karguaren zati gisa esleitzen. Proiektuaren zuzendariak lana izena duten baliabideei egoki eman diezaieke. The **Kontziliazioa** ikuspegiak lagun diezaioke proiektuaren kudeatzaileari zereginak burutzeko baliabide ugaritan erreserbak hausten. Hori ez da automatikoki egiten, aurreko adibide soilak baino konplikatuagoa den edozein agertokitan, esaterako, eskakizuna osatzen duen zeregin-sorta bat daukazunean, sistemak proiektuak bere gain hartu nahi duen asmoa. Sistemak ezin duenez intentzioa ulertu, posible da suposizioak aurreikusitakoa baino desberdinak izango direla eta aurreikusitako emaitza okerra edo ezustea gertatuko dela. Aurreikus daitekeen emaitza baliabide generikoa esleituta mantentzen dela da proiektuaren kudeatzaileak nahitaez zereginak sortu arte, programaren **Kontziliazioa** ikuspegiaren laguntzarekin.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
