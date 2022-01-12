---
title: Project Service Automation eguneratzearen 38, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honetan eskuragarri dauden eginbideak eta konponketak zerrendatzen dira Microsoft Dynamics 365 Project Service Automation Eguneratu 38. bertsioa, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 12/06/2021
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
ms.openlocfilehash: 1e5175b12c9e06962888bf09c8e07119b9505dda
ms.sourcegitcommit: 2aba2082d50b20b596ee86735045644cd647c2b0
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 12/08/2021
ms.locfileid: "7901503"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-38-v3"></a>Project Service Automation eguneratzearen 38, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Dynamics 365 9.x-rekin bateragarria da. Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation 38, V3 eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.59.117 eraikitze-zenbakia du eta, oro har, eskuragarri dago 2021eko abenduan auto-eguneratze baten bidez.

## <a name="update-release-38"></a>38. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

Arazo hauek konpondu dira.

**Denbora eta gastua**

- Salbuespen bat gertatzen da onarpen multzoen erregistroen luzera 100.000 erregistrotik gorakoa denean.
- Erabiltzaileek ezin dute sartu **Denbora Sarrera** saretik **Denbora Sarrera** orrialde nagusia.
- The **Denbora-sarrera inportatu** elkarrizketa-koadroak ez du testurik erakusten elementurik inportatzeko aukerarik ez dagoenean.
- Erabiltzaileek onarpen multzoak sor ditzakete non **Xede-egoera** eremuan ezarrita dago **Ezezaguna**.

**Proiektuen kudeaketa**

- Inguruak ez dira behar bezala erakusten UTC(+09:30) eta UTC(+10:00) baliabideen esleipenetan, udako ordutegia hasten denean.
- The **Zutabe gehigarria** lan-matxura-egituren eremua toki batzuetan ezkutatuta dago.
- Egutegia kontrolatzeko data-hautatzailea **Proiektuaren zeregina** sareta ez dago behar bezala lokalizatu txinerarako.

**Salmentak**

- **Kontratua betetzea** eta **Proiektuaren Benetako Kostua** balioak ez datoz bat kontratazio-unitate eta moneta desberdinak dituzten baliabide erreserbagarriak denbora-sarrerak bidaltzen dituztenean.
- Fakturak automatikoki berresteko lan-fluxu pertsonalizatuak huts egiten du fakturak kudeatutako soluzio gisa inportatzen direnean. Honako mezu hau erakusten da: "Microsoft.Xrm.Sdk.InvalidPluginExecutionException Mezua: fakturaren egoera baliogabea".
- Noiz **Erroa** laburpen-aukera gisa hautatzen da, eta proiektuak transakzio-klaseen nahasketa bateko estimazioak ditu (adibidez, denbora, gastu eta estimazio materialen konbinazioa), sistemak transakzio-klaseen artean laburbiltzen du kuota-lerro bakar gisa.
- Kontratu-lerroa proiektu bati lotu aurretik gastu-lerroa gehitzen den agertokietan, prezio zuzena ez da balio lehenetsi gisa sartzen.**Eguneratu prezioa** eremua.
- Salmenten kopuru negatiboak ezin dira aktibatu **Proiektua** eta **Zeregin** entitateak.
