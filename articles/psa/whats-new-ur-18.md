---
title: Project Service Automation eguneratzearen 18, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 18. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: 8c76672e63fc4b01d5c6f8cce2831782b9c22326
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8598749"
---
# <a name="project-service-automation-update-release-18-v3"></a>Project Service Automation 18, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 18. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honen konpilazio-zenbakia V3.10.8.12 da eta, oro har, 2020ko apirileko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-18"></a>18. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

- Konponduta: **Berreskuratu**, **Eskatu** eta **Utzi onespena** fluxuek salbuespenak botatzen dituzte errore-mezu ilunekin.
- Konponduta: **Utzi onespena** aukerak huts egiten duenean gastu batean, dagokion salbuespen-errorea ez da erakusten.
- Konponduta: Orduaren sarrera saretak oker kudeatzen ditu lanegunak ez diren egunak Australian, neguko ordutegira (DST) aldatzean urrian.
- Konponduta: Lehenesteko logika okerrak ez du uzten gastuak bidaltzen.
- Konponduta: Orduaren sarrera onesteak huts egiten duenean, onespena **Zain** egoeran geratzen da.
- Konponduta: SQL erroreak onespen masiboetan (blokeoa/denbora-muga).
- Konponduta: Errendimendu-arazo nabarmenak erabiltzaile-esperientzian denbora-sarrerak onesten diren bitartean taldeko kideak eguneratzeak eragindakoa.

**Proiektuen kudeaketa**

- Konponduta: Ordu-zonaren jakinarazpena **Adiskidetzea** ikuspegitik **Proiektua** inprimaki nagusira aldatu da.
- Konponduta: Egutegiko txantiloia ez da behar bezala lehenesten proiektuaren inprimaki berri bat irekitzean.
- Konponduta: Chromium-en oinarritutako arakatzaileetan, erabiltzaileek ezin dute erraz hautatu aurrekoaren zereginak ezabatzeko.
- Konponduta: **Txantiloia hutsetako proiektua** sortzean edo kopiatzean, loturarik gabeko zereginak eskuratzen ditu.
- Konponduta: Edge kasu zehatzetan, zereginen saretatik zeregin berri bat sortzean erregistro bikoiztuak sortzen dira.
- Konponduta: Eskuzko moduan, erabiltzaileek ezin dituzte eguneratu zereginen hasiera-datak gordetako uneko data baino geroago.

**Baliabideen kudeaketa**

- Konponduta: **Adiskidetzea** ikuspegiko subtotalen errenkadak oker kalkulatzen ditu erreserben aldaera erreserbak luzatu ondoren.
- Konponduta: **Adiskidetzea** ikuspegiak oker bistaratzen ditu baliabideen esleipenak baliabide erreserbagarriak proiektuaren egutegiarekin bat ez datorren egutegia duenean.

**Sales**

- Konponduta: Denbora-sarrerak berriro onartzen direnean (**Onartu > Utzi >** onartu berriro), kargatu ezin daitekeen benetako datuen kopia bat sortzen da.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
