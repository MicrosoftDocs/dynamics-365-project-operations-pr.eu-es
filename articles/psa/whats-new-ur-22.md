---
title: Project Service Automation eguneratzearen 22, V3 bertsioko berrikuntzak edo aldaketak
description: Artikulu honek Project Service Automation Update Release 22, V3-n eskuragarri dauden funtzioak eta konponketak zerrendatzen ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
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
ms.openlocfilehash: 733ee6e0d3583f21d0f58f9651920be3e3fd8cb0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930625"
---
# <a name="project-service-automation-update-release-22-v3"></a>Project Service Automation 22, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Artikulu honek Project Service Automation V3, Update Release 22rako berriak diren edo aldatu diren ezaugarriak eta konponketak zerrendatzen ditu. Bertsio honen konpilazio-zenbakia V 3.10.33.48 da eta, oro har, 2020ko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-22"></a>22. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa



**Denbora eta gastua**

Arazo hauek konpondu dira:

- **Denboraren sarrerak** ez dira automatikoki inportatu ondoren Ordua sarreren egutegian gehitzen.
- **Ordua Sarrera** sareko data hautatzaileak ez ditu erabiltzailearen eskualdeko ezarpenak ezagutzen.

**Baliabideen kudeaketa**

Arazo hauek konpondu dira:

- Eskuzko moduan, aldaketetara **Baliabideen esleipena** sarrerak ez dira ezagutzen sortzen **Baliabide Eskakizunak**.
- **Baliabide eskaerak** ez onartzen eskaera-egoera pertsonalizatuak.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- EstimateGridControl gainean klik bikoitza erabiliz ez duzu holandeseko formatuko zenbakiak behar bezala analizatuko.
- Esleitutako orduak ez dira behar bezala eguneratzen zereginak Microsoft Project mahaigaineko bezero gehigarria erabiliz aldatzen direnean.
- Proiektuaren jarraipena eta zenbatespenen sareek salmenta okerraren moneta kodea erakusten dute kontratuaren moneta bezeroaren moneta baino ez denean eta erakundea moneta-kodeak ordez moneta ikurrak bistaratzeko konfiguratuta dago.
- Taldekide batek bukatutako datak egun bat gehituko du laneko ordutegia eguneko 24 ordukoa bada.
- Proiektuen egutegian, zeregin bati Transakzio kategoria gehitzeak ez du auto-aurrezpena aktibatzen.
- Ondorengo errorea taldekide bat proiektuko txantiloiak gehitzerakoan agertzen da: "Baliabide eskakizunak ezin dira proiektuaren txantiloiekin lotu". 
- Zintaren arau script-ak "msdyn.Approval.CanApproveOrReject" denboraren akatsa bistaratzen du.

**Sales**

Arazo hauek konpondu dira:

- Balidazio-errore mezua ez da agertzen Kostuen Prezio Zerrenda hautatutakoan Prezio Zerrendako bilaketa-proiektuan "Aurrekontu Berrien Proiektuen Prezioen Zerrenda" inprimakian/erakundean.
- Irabazitako aurrekontua ixteak ez du sortutako kontratura nabigatuko aurrekontuari atxikitako BPF bat azken fasean badago.
- **Saldu gabeko salmentak** kentzea Denborako sarrera gogorarazten denean kostu originalarekin lotzen da.
- Hautatu ondoren **Baieztatu** botoian, fakturaren egoera ez da aldatuko **baieztatu** faktura freskatu ezean.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
