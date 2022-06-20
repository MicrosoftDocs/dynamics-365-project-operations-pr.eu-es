---
title: Project Service Automation eguneratzearen 32, V3 bertsioko berrikuntzak edo aldaketak
description: Artikulu honek Project Service Automation Update Release 32, V3-n eskuragarri dauden funtzioak eta konponketak zerrendatzen ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 5124137c24da9b579ee1365524d66d9135b2d420
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912869"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a>Project Service Automation eguneratzearen 32, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Pozik gaude egunkariaren azken eguneratzea iragarriz Microsoft Dynamics 365 Project Service Automation aplikazioa. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Dynamics 365 9.x-rekin bateragarria da. Bertsio hau eguneratzeko, bisitatu Admin Zentroa Dynamics 365 lineako soluzioen orria eta instalatu eguneratzea. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Artikulu honek Project Service Automation V3, Update Release 32-rako berriak diren edo aldatu diren ezaugarriak eta konponketak zerrendatzen ditu. Bertsio honen konpilazio-zenbakia V3.10.53.108 da eta, oro har, 2021eko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-32"></a>32. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

#### <a name="general"></a>Orokorrak

- Berritze garrantzitsu batek huts egiten duenean, aplikazioaren sarrera puntu nagusiak soilik blokeatu beharko lirateke, partekatutako entitateak oraindik eskuragarriak direla ziurtatzeko.

#### <a name="time-and-expense"></a>Denbora eta gastua

Arazo hauek konpondu dira:

- **TimeEntriesImportFromResourceAssignment** ez ditu baliabideak esleitzeko sestra zatiaren hasiera eta amaiera orduak mantentzen.
- Hautatzen duzunean **Sarrera irekia** **Denbora-sarrera** saretan, baliteke beste inprimaki batzuk hautatzea eragotzi.
- Zereginak denbora sarreretara inportatzen dituzunean, bezeroaren kodearen kontsultak kontsultak huts egiten duen URL luzea sor dezake.
- **Denbora-sarrera** saretan, gelaxka batetik balioa ezabatu ondoren, fokua ez da saretan geratzen.
- **Baztertu** botoia kendu da **Onarpenak tramitatzea** onarpen modernoetarako ikuspegia.
- Denbora sartzeko ontziratutako onarpenaren egonkortasuna eta errendimendua blokeoek eragiten dute eta pertsonalizazioarekin erlazionatutako pertsonalizazioak modu egokian kudeatzen ez badute **Denbora-sarrera** entitatearekin.

#### <a name="project-planning"></a>Proiektuaren antolaketa

- Erreferentzia baliogabeko salbuespena sortzen da fitxategian balio baliogabea duen proiektu bat eguneratzen duzunean **Kontratazio-unitatea** eremuan.
- **Freskatu proiektuaren guztirakoak** proiektu baten gainerako kostua eta gainerako salmentak gaizki kalkulatzen ditu.
- Prezioen kalkulu erredundanteak eragina dute baliabideak esleitzeko inguruneen eguneratzeekin erlazionatutako errendimenduan.

#### <a name="resource-management"></a>Baliabideen kudeaketa

Arazo hau konpondu da:

- Erreserbatzeko baliabideen egutegiaren edukiera 1 baino handiagoa denean, Project Service Automation-ek gaitasuna 0 (zero) gisa gaizki aitortzen du. Hori dela eta, begizta infinitua gertatzen da programazio ikuspegian.

#### <a name="sales"></a>Salmentak

Arazo hauek konpondu dira:

- Transakzio mota pertsonalizatua duen aldizkari lerroa sortzen denean, erreferentzia nuluko salbuespen hau gertatzen da: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.
- Eskaintza baino lehenago inaktibo dauden funtzioak eta kategoriak kopiatzen dira eta ez dira gehitu behar sortu berri den aipamenaren kobra daitezkeen rolak eta kategoriak.
- Dokumentuen data eta kontabilitate data ez daude bat eginda faktura zirriborroan zuzenean sortzen den faktura lerroaren xehetasunean ematen den hasierako datarekin.
- Aipamen bat kopiatu baino lehen rol eta kategorien desaktibazioarekin lotutako eszenatokietan erreferentzia nuluen salbuespenak sortzen dira.
- **Eguneratu Prezioak** ekintza **Proiektuak** orrialdeak ez ditu gastuen kalkuluak eta estimazio materialak eguneratzen.
