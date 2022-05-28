---
title: Project Service Automation eguneratzearen 17, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 17. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: 70749646f5b67db3cf868a6d9a83c14dc490793a
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8585076"
---
# <a name="project-service-automation-update-release-17-v3"></a>Project Service Automation 17, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.  Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek PSA V3, 17. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.6.34 konpilazio-zenbakia du eta, oro har, 2020ko martxoan jarriko da erabilgarri automatikoki eguneratzeko moduan.


## <a name="update-release-17"></a>17. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Orokorra**

- Konponduta: Project Service Automation eguneratu da Team Member lizentziak betearazteko (Proiektuen baliabide-guneak Taldekidea zerbitzu-planaren 3.x metadatuak ditu)
 
**Denbora eta gastua**

- Konponduta: ezin da gastuen aurreikuspen bat aldatu zerotik zero ez den zenbateko batera (0). Aldaketa baztertu egin da.

**Proiektuen kudeaketa**

- Konponduta: nuluak ez diren egiaztapenak gehitu dira taldekidearen posizioaren izenean.
- Konponduta: **msdyn_userresourceid** eremua zaharkitu egin da **msdyn_resourceassignment** entitatean.
- Konponduta: Bertsio berritu 2.x bertsiotik 3.x bertsiora ahalegin hutsalen ingeradak kudeatzeko zereginen esleipenetan.

**Sales**

- Konponduta: **Invoice.PreValidateInvoiceUpdate** parametroak berresleitutako erregistroaren jabeak ongi kudeatzen ditu orain.
- Konponduta: Transakzioaren klasea **Ordua** denean, **UnitGroup** ezin da editatu erakunde guztietan: **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail** eta **ContractLineDetails**. Alabaina, **Unitatea** ez da editagarria **JournalLine** eta **InvoiceLineDetails** parametroetan soilik.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
