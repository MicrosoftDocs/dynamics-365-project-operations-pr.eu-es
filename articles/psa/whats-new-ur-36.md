---
title: Project Service Automation eguneratzearen 36, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honetan eskuragarri dauden eginbideak eta konponketak zerrendatzen dira Microsoft Dynamics 365 Project Service Automation Eguneratu 36. bertsioa, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/06/2021
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
ms.openlocfilehash: 9b85aed79acb7e7784a23f54a2e9af1cc83f5f4d
ms.sourcegitcommit: 6d9fc4dc851814664bf71729904ab4bedd85fe70
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/06/2021
ms.locfileid: "7606716"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-36-v3"></a>Project Service Automation eguneratzearen 36, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Dynamics 365 9.x-rekin bateragarria da. Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation 36, V3 eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.57.152 konpilazio-zenbakia du eta, oro har, 2021eko urrian jarriko da erabilgarri automatikoki eguneratzeko moduan.

## <a name="update-release-36"></a>36. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

Arazo hauek konpondu dira.

**Orokorrak**
- **Lanorduaren txantiloia lehenetsia** eremuaren izena gaizki itzulita dago **Proiektuaren parametroak** orrialdean.
- Async pluginak ez dira behar bezala kudeatzen **SharedVariableService**.

**Denbora eta gastua**
- Aldizkari lerroak falta direnean edo erabiltzaileak egunkari lerroak irakurtzeko pribilegio zuzenak ez dituenean, errore okerra gertatzen da proiektuen onarpenak bertan behera uzten direnean.
- Erabiltzaileek ezin dute utzi onarpena gastuak edo denborak sartzeak proiektuaren onarpen bat baino gehiago dituenean.
- **Absentzia** eta **Oporrak** ez dago txinera txinerako itzulpenean **Denbora-sarrera** orrialdea azkar sortzeko.

**Baliabide-kudeaketa**
- Erabiltzaileak ezin ditu baliabideak bilatu **Ordutegi laguntzailea** ikuspegi modua ezarrita dagoenean **Eguna**, **Astea** edo **Hilabetea**.
- Baliabide generikoek gaizki baimentzen dute posizio izen hutsak izatea. 
- Galdutako kontratua ixteak ez ditu geroko erreserbak bertan behera uzten.

**Salmentak**
- Ingurune batek produktu kopuru handia duenean, errendimendua degradatu egiten da **Materialen aurrekontua** sareta.
- Txantiloi batetik proiektu bat sortzerakoan, proiektuaren moneta ez da lehenetsi dagokion proiektuaren kudeatzailearen kontratazio unitatearekin.
- Benetako zenbatekoak ez datoz beti bat proiektuan islatutakoarekin, edo zenbatekoak negatiboak bihurtzen dira gogora ekartzeko eszenatoki zehatzetan.
- Akats bat gertatzen da proiektuaren txantiloitik sortutako proiektu bat kontratu lerro batera lotzen duzunean.
- Erabiltzaileek mugarriekin kontratu lerro bat ezaba dezakete, **Fakturatzeko prest** eta **Faktura sortua**. Ez litzateke baimendu behar.
- Aurrekontuak proiektu batetik inportatzen direnean, aurrekontuaren lerroaren xehetasunak kargatzeko gaitasuna gaizki ezartzen da zereginetan oinarritutako fakturazioa aurrekontu lerroan gaituta dagoenean.
- Prezio finkoko fakturazio mugarria gehitzen duzunean, mugarria ez da mugarri azpisarean islatzen orria berritu arte.
- Erreferentzia nuluko salbuespena sortzen da nulua den aurrekontuaren izenarekin proiektuaren kontratua sortzen duzunean.
- Eskuzko moduko zereginetan, proiektuaren moneta baliabidearen monetatik ezberdina denez, prezioen estimazio okerrak sortzen dira.
- Erabiltzaileek ezin dute faktura zuzentzaile baten bidez zuzendu den transakzioa gogoratu.
- Desaktibatutako transakzio kategoriak **Gastuen aurrekontuak** sareta.



