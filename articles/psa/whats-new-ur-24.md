---
title: Project Service Automation eguneratzearen 24, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 24. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 3a37e71be2cce259d8aed0621d13393b6bbe4199
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126558"
---
# <a name="project-service-automation-update-release-24-v3"></a>Project Service Automation 24, V3 eguneratze-bertsioa

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 24. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.42.43 konpilazio-zenbakia du eta, oro har, 2020ko urrian jarriko da erabilgarri automatikoki eguneratzeko moduan.

## <a name="update-release-24"></a>24. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Sales**

Arazo hauek konpondu dira:

- Arazoa produktuen prezio-zerrenda lehenetsia ezartzean.
- Eskaintza irabaztearen errendimendua motela da txertatutako prezioen zerrenda eta funtzio-prezioen erregistroen kopia dela-eta.
- **Proiektuaren kontratua/Salmenten atala** > **Produktu-lerroaren elementua / Eskaera-lerroaren kantitatea** automatikoki biribiltzen da hurbilen dagoen zenbaki osora.
- Igo sistemaren pribilegioak prezio-zerrendak irakurtzean.
- Kopiatu bezeroaren **address1_freighttermscode** eta **address1_shippingmethodcode** helbide-eremuak Eskaintza/Eskaera eremuetan. 


**Denbora eta gastua**

Arazo hauek konpondu dira:

- **Denbora sartzeko sareta** eremuak ez du onartzen **Data soilik** denboraren portaera.
- **Denboraren sarrera** ez da automatikoki freskatzen. Eskuz freskatu behar da.
- Ezin dira inportatu esleipen bateko denbora-sarrerak baliabidearen esleipenetako etenaldi bat (0 ordu) dagoenean.
- Denbora-sarrera bat sortzerakoan, ezarri hasiera **msdyn_date** gisa.
- Gaitu berriro denbora-sarreraren edizio masiboa.

**Baliabideen kudeaketa**

Arazo hauek konpondu dira:

- Eskakizunik ez duen egun barneko erreserba baten egoera eguneratzen saiatzean null-ref salbuespena agertuko da.
- Errorea **Adiskidetzearen ikuspegia** kargatzean.


**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- **Proiektuaren antolaketa** eremuan, **Eskuzkoa** aukera **Automatikoa** aldatzean, automatikoki gordetzea ez da osatzen.
- Gastuen kostuak ez dira kalkulatu behar **Proiektuaren jarraipen-sareta** eremuaren bariantzan.
- **Aurreikuspenen etiketa** zutabeen portaera ez da koherentea kargatzean, **Denbora-fasea** mota aldatzean.
- Baliteke proiektuaren benetako kostuak ez islatzea **Benetako datuak** aukeraren guztizkoak.
- **Aurreikuspeneko amaiera-data** aukera, **Laburpena** fitxakoa, ez dator bat **WBS antolaketa** aukerakoarekin.
- Koska kentzeko **Eguneratu benetako orduak** eremuak ez du ongi funtzionatzen.
- **BU** erroak ez du sortu proiektu baten kanpoko Proiektu-kudeatzailea.
- **Gastuen aurreikuspenak** eremuko zereginean edo kategorian egindako aldaketak ez dira iraun.
- **Kontratuaren kopia** eremuak fakturen antolaketak kopiatzen ditu eta egoera exekutatzen du.
- **Freskatu benetako datuak** botoiak gaizki kalkulatzen ditu laburpen-zereginak.
- Microsoft Project Add-in: konpondu erreferentzia-errore hutsa talde-kideren batek baliabide-unitate huts bat baldin badu.

