---
title: Project Service Automation eguneratzearen 35, V3 bertsioko berrikuntzak edo aldaketak
description: Artikulu honetan eskuragarri dauden funtzioak eta konponketak zerrendatzen dira Microsoft Dynamics 365 Project Service Automation Eguneratu 35. bertsioa, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 09/03/2021
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
ms.openlocfilehash: 28b4a5ccbfff83c9b1a18cb0b4062af9cdaf8f6e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912823"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-35-v3"></a>Project Service Automation eguneratzearen 35, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Dynamics 365 9.x-rekin bateragarria da. Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Artikulu honek Project Service Automation Update Release 35, V3rako berriak diren edo aldatu diren eginbide eta konponketak zerrendatzen ditu. Bertsio honek V3.10.56.110 sorrera-zenbakia du eta orokorrean 2021eko irailean auto-eguneratze baten bidez eskuragarri dago.

## <a name="update-release-35"></a>35. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

Arazo hauek konpondu dira.

**Denbora eta gastua**

- Proiektuaren onartzaileak irakurtzeko pribilegio errore bat jasotzen du gastu sarrerak onartzen dituenean **Proiektuaren onartzailea** rola.
- Proiektuaren onartzaileak idazteko pribilegio errore bat jasoko du **msdyn_projectapproval** onartutako denbora sarrera bat bertan behera uzten dutenean **Proiektuaren onartzailea** rola.
- Hautatzen duzunean **Kopiatu astea** Dynamics 365 for phone - Project Resource Hub aplikazioaren moduluko denbora sarrera batean, errore hau gertatzen da: "...\OfficeProductivity_RibbonRules.js.map: HTTP errorea: 404 egoera kodea, garbia::ERR_HTTP_RESPONSE_CODE_FAILURE."
- **Saiatu berriro** gidalerroak lehenago baztertutako sarrerak automatikoki onartzen ditu.
- **Onarpen multzoak** azpisarek aplikagarriak ez diren zinta ekintzak erakusten ditu.
- Ikonoak falta dira **Proiektuaren zeregina** eta **Baliabideen eginkizuna** gainean **Denbora Sarrera** entitatea.
- Baliabideen esleipenak inportatzen dituzunean, inportatutako denbora-sarrerek ez dute iraupen zuzena eskuzko moduko atazen bidez sortutako lanetarako.
- **Ezabatu** fitxategian falta da **Denbora sartzeko erregistroen bilaketa aurreratua** orrialdea.
- **Gorde** fitxategian falta da **Ordua sartzeko informazioa** orrialdea. Arazo honek orria ixten denean aldaketak gordetzea eragozten du.

**Proiektuaren antolaketa**

- **Baliabideen esleipena** eta **Baliabideen bateratzea** sareek ez dituzte multzokatutako atributuak alfabetikoki ordenatzen.
- Zereginak ezin dira sortu data portaera pertsonalizatuta badago **Data soilik**.

**Baliabide-kudeaketa**

- Biak badira Dynamics 365 Field Service eta Project Service Automation instalatuta daude. Gainjarritako arazoak gertatzen dira **Baliabideen eskakizunari lotutako ikuspegia** orri nagusi batekin lotzen da.
- Egin klik bikoitza **Gorde** urtean **Taldeko kidea azkar sortzeko** Elkarrizketa-koadroak baliabide-eskakizuna sortzea eragozten du.

**Salmentak**

- Salbuespen bat sortzen da egoera duen aipu batekin lotutako zeregin bat ezabatzen baduzu **Irabazita**.