---
title: Project Service Automation eguneratzearen 25, V3 bertsioko berrikuntzak edo aldaketak
description: Artikulu honek Project Service Automation Update Release 25, V3-n eskuragarri dauden funtzioak eta konponketak zerrendatzen ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 2330c7dc5d2dfb148d5c7fb9a5ce643fded84dde
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922529"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a>Project Service Automation eguneratzearen 25, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Artikulu honek Project Service Automation V3rako berriak edo aldatutako ezaugarriak eta konponketak zerrendatzen ditu, 25. bertsioaren eguneraketa Bertsio honek V 3.10.43.76 eraikitze-zenbakia du eta, oro har, 2020ko urrian auto-eguneratze baten bidez eskuragarri dago.

## <a name="update-release-25"></a>25. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hau konpondu da:

- Lortutako tarte handiegia oinarritzat hartuta datu osagarriak erakusten dituen denbora sartzeko taula.

**Baliabideen kudeaketa**

Arazo hau konpondu da:

- Package Deployer-en kodea gehitu da Universal Resource Scheduling adabakien inportazioa bertsio altuagoa badago dagoeneko.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- Biribiltze eta truke-tasaren desadostasunak zuzendu dira, proiektuaren jarraipen-sarean planifikatutako kostu okerrak sortuz.
- Onartu bi erreakzio - sare edo gehiago bistaratzeko gaitasuna **Proiektua** forma.
- Egutegiaren amaiera-datatik ataza bat esleitzeko gaitasuna zuzentzeko balioztapena eman da, eta horrek huts egin du baliabideen esleipenean.
- Erroreen kudeaketa hobetu da honetatik sortutako Null Erreferentzia Salbuespenari aurre egiteko:

    - **PreValidateProjectTeamMemberCreate** plugina
    - **PreValidateProjectTaskCreate** proiektuaren zeregina lotutako proiekturik gabe sortzen denean
    - **PreProjectTeamMemberCreate** plugina
    - **PostProjectTeamMemberDelete** plugina
    - **PreValidateProjectTaskDelete** plugina

**Sales**

Arazo hauek konpondu dira:

- Erroreen tratamendua hobetu da Sortutako erreferentzia nuluen salbuespenak zuzentzeko **Kopiatu proiektua: Aurrekontuen HelperResource Management**.
- **Ez dago fakturatzeko prest** batean **Denboraren eta materialaren fakturazio-zorroa** ez du fakturazio egoera garbitzen.
- Zuzendu da gaizki etiketatuta **Prezioak** botoiak botoian **Rolaren prezioa** eta **Katalogoko elementuak** fitxa.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
