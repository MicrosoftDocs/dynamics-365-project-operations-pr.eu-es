---
title: Project Service Automation eguneratzearen 26, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 26. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: 11f722c1f31c0e8aa08192cc955aabbe97018225
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928785"
---
# <a name="project-service-automation-update-release-26-v3"></a>Project Service Automation 26, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Artikulu honek Project Service Automation 26, V3 eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.44.59 zenbakia du eta orokorrean eskuragarri dago 2020ko abenduan auto-eguneratze baten bidez.

## <a name="update-release-26"></a>26. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira:

- Erabiltzaileek zeregina aldatu edo bidali duten denbora-sarrera batean alda dezakete.
- "Objektuaren erreferentzia ez da ezarri" errorea denbora sarrera gordetzean.
- Baliabideen esleipenetatik ordu sarrera inportatzeak denbora sarrera sortzen du okerreko Data eta Balioekin.
- Project Service Automation eta Field Service aplikazioa instalatuta daudenean, **Berria** botoia birritan bistaratzen ari da komando-barran Field Service aplikazioan denbora sartzeko.
- **Baimendu Unitatea** eta **Unitatea taldea** gelaxken eguneratzeak **Gastuen kalkuluak** saretan.
- **Eguneratu denbora sarrera editatu** inprimakia barne **Denbora-lerroa**.
- Proiektuak ez diren denbora-sarreretarako denbora onartzeak sistema blokeatzen du proiektuak onartzeko eginkizuna bilatzean.

**Baliabideen kudeaketa**

Arazo hauek konpondu dira:

- Fitxategian baliozkotzea gehitu da **PostProjectCreate** plugina, lehen sortu behar den baldintza bat egiaztatzeko.
- **Proiektu Taldeko kidea** azkar sortzeko inprimakiak erreferentzia nuluko salbuespena sortzen du eremuak inprimakitik kentzen badira.
- Sortu urtebetean 12 orduz eskakizunak huts egingo du.
- Errore-mezuaren erreferentzia nuluko salbuespena hobetu da baliabide-eskakizunak sortzean.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- Fitxategian sortutako erreferentzia nuluen salbuespenari aurre egiteko baliozkotzea hobetu da **Aurreproiektuaren eguneratzea** plugina.
- Microsoft Project mahaigaineko gehigarriak argitaratutako proiektuek esleitu gabeko lanak ezabatzen dituzte.
- Hemen gehitu da baliozkotze berria zeregin baten proiektuaren erreferentzia baliogabea denean erreferentzia nuluko salbuespenagatik **PreValidateProjectTaskUpdate** plugina.
- Taldekideen saretak ez ditu zeregin desberdinak erakusten taldekideen erregistroan.
- Hemen gehitu dira baliozkotze eta errore mezu berriak erreferentzia nuluko salbuespenagatik **PreProjectTaskDelete** plugina.

**Sales**

Arazo hauek konpondu dira:

- Aurrekontuan edo kontratuan proiektuan oinarritutako lerro bat hautatzerakoan **Iradokizuna** botoiak lehendik dagoen produktu batekin lotutako produktuan oinarritutako linea hautatzerakoan soilik egon behar du ikusgai.
- Zatitu **Sortu_Product** pribilegioa **Create_ProjectContract** pribilegiotik.
- Faktura lerro bat ezabatzeak erreferentzia huts hutsa eragiten du **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
