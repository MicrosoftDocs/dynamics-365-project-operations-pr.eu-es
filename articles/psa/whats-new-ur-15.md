---
title: Project Service Automation eguneratzearen 15, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation eguneratzea 15, V3 bertsioko berritasunei buruzko informazioa ematen du.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/27/2020
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
ms.openlocfilehash: 0ec6746c0d3a1a03ee56440c73d044df844046f8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143948"
---
# <a name="project-service-automation-update-release-15-v3"></a>Project Service Automation 15, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atsegin handiz adierazten dugu Dynamics 365 Project Service Automation (PSA) aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroa eta joan soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek PSA V3, 15. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.5.28 konpilazio-zenbakia du eta, oro har, 2020ko urtarrilean jarriko da erabilgarri automatikoki eguneratzeko moduan.

## <a name="update-release-15"></a>15. eguneratze-bertsioa 

### <a name="enhancements"></a>Hobekuntzak

- Proiektuen kudeaketa

### <a name="bug-fixes"></a>Akatsen zuzenketa

- Denbora eta gastua

  - Konponduta: karga-erroreen kudeaketa gehitu da bateratze-ikuspegian.
  - Konponduta: Proiektuaren baliabide-gunea: **Zenbatekoa** berrizendatu da anbiguotasuna gutxitzeko.
  - Konponduta: **Kopiatu ordu-sarreren zutabeak** ikuspegia doitu da, mota barneratzeko.
  - Konponduta: sareta-ikuspegian denbora-sarreraren iraupena zenbaki hamartarren emaitzekin editatzean, errore ezezaguna sortzea zenbait zenbakirekin.

- Proiektuen kudeaketa

  - Konponduta: **Erabili Jarraipen-ikuspegian** goitibeherako menua aukeren zabaleran oinarrituta hedatzen da orain.
  - Konponduta: +13 ordu-eremutako baino gehiagotako proiektuak kudeatzean, zereginen kalkuluek emaitza okerrak bistara ditzakete.
  - Konponduta: **Taldekideen amaiera-ordua** zuzendu da 24 orduko egutegia erabiltzean.
  - Konponduta: Berriro aktibatu da **BPF** **msdyn_project** inprimaki nagusian.
  - Konponduta: Esleipenen kalkuluak ez du egun bat baztertzen.
  - Konponduta: jakinarazpen iragankor berri bat gehitu da proiektuaren inprimakian, erabiltzailearen eta proiektuaren ordu-eremuak desberdinak direnean.

- Sales

  - Konponduta: Gutxi gorabeherako gastuen kategorien bilaketa erabil daiteke bikoiztuak iragazteko.
  - Konponduta: **PluginDomain.ExecuteInTryCatchBlock(..)** eremuko kodeak ez du ezkutatzen jada salbuespenaren jatorria.
  - Konponduta: Ez duzu errore-mezurik jasoko **Proiektuaren bilaketa** eremuan **Eskaintzaren lerroa** inprimakian, 1000 proiektu baino gehiago daudenean.
  - Konponduta: gutxi gorabeherako lanen eta gutxi gorabeherako gastuen **Gutxi gorabeherakoak** saretak moneta-ikur zuzena bistaratzen du.
  - Konponduta: Erakunde batek PSA 14. eguneratze-bertsiotik 15. eguneratze-bertsiora eguneratu ondoren, **Antolaketa** fitxa ez da agertuko hutsik **Proiektua** inprimakian.


[!INCLUDE[footer-include](../includes/footer-banner.md)]