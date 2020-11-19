---
title: Project Service Automation eguneratzearen 22, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 22. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: badd87a276d68d9959e9cca4220daf61ed570638
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070984"
---
# <a name="project-service-automation-update-release-22-v3"></a>Project Service Automation 22, V3 eguneratze-bertsioa

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 22. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honen konpilazio-zenbakia V 3.10.33.48 da eta, oro har, 2020ko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.

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