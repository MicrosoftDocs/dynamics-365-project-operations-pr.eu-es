---
title: Project Service Automation eguneratzearen 17, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 17. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: bb93208217972639f91b39b7b6705d9897373ef7
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126783"
---
# <a name="project-service-automation-update-release-17-v3"></a>Project Service Automation 17, V3 eguneratze-bertsioa

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu.  Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

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


