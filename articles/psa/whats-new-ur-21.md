---
title: Project Service Automation eguneratzearen 21, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 21. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: b1194c1cf1997b68030fe88360c6ebb756c715fd
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147008"
---
# <a name="project-service-automation-update-release-21-v3"></a>Project Service Automation 21, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 21. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honen konpilazio-zenbakia V 3.10.32.50 da eta, oro har, 2020ko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-21"></a>21. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Denbora eta gastua**

Arazo hauek konpondu dira:

- Biltegiratzean **Ordua sartzeko saretaren kontrola** Arbeletan, sareak ez du arbelaren sarearen edukiontziaren zabalera osoa.
- Ordu-zona zehatzetarako, **Ordua Sarrera** sareta kontrolak ez ditu erregistroak bistaratzen.
- Gaueko 21:00ak baino lehenagoko ordu sarrerak gaizki agertzen dira.
- Erabiltzaileak ezin dira gastuak bidali gastu kategoria bada, **Gastuen ordainagiria beharrezkoa da** ez du baliorik.

**Baliabideen kudeaketa**

Arazo hauek konpondu dira:

- Erreserbak aktibo daude **Adiskidetzea** ikusteko.
- Baliabideen betetze generikoa falta zen balioztapena erreserbatzeko egoera baliozkoa dela ziurtatzeko.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- **Proiektua** eratutako sareta (**Baliabideen esleipena**, **Zeregin**, **Adiskidetzea** ikuspegia, **Gastuen kalkuluak**) jarraitu editagarriak, proiektu bat aktibo ez dagoenean ere.
- Bezero bikoiztuak ezin dira berretsi proiektuaren kontratuei lotuta dauden bezeroekin.
- Baliozko egutegirik ez duen baliabidea gehitzen denean, sistemak ez du erabiltzaileen errore-mezurik itzultzen.
- **Gehitu Ataza** Zereginen saretako botoian gaituta dago proiektua lotuta dagoenean **Microsoft Project gehigarria**.
- Ahalegina kontrolik gabe hazten da kategoria bateko zereginak kostu prezioa definituta daukan zereginarekin.

**Sales**

Hobekuntza hauek egin dira:

- **Fakturen maiztasuna** eta **Fakturazio hasiera** aldatu dira **Fakturen egutegia** fitxa.

Arazo hauek konpondu dira:

- **Salmenta prezioa, guztira** zero da (0) **Kategoria** nahiz eta **Funtzioa** zero ez den salmenta prezioa du.
- Bezeroek ezin dute aldatu balioa **Fakturaren egoera** eremua **Fakturatzeko prest** Neurrira egindako beste prozesu bat eremu gehigarri bat eguneratzen denean.
- **Eguneratu faktura-ildoak** botoiak bikoiztu lerro bat baino gehiago sor ditzake behin eta berriz hautatzen bada.
- **Eguneratu Prezioak** botoiak ez du funtzionatzen **Funtzioaren prezioak** azpisarea **Ikuspegi azkarra** forma.
- **Salmenta prezioen zerrenda ebaztea** logikak gaizki kudeatzen ditu ordu-zonak, prezioen zerrenden aukeraketa okerra sortuz.
- Proiektu batena **Benetako kostu totala** Zatiki kopuru bat desgaitu daiteke, sarrera bakar bat onartu ondoren.
- **Prezioen Ebazpena** logikak ez du erabilgarritasun errorerik ematen **Berreskuratutako RolePrice** ez du balorean **"Lehen Unitatea"** eta **"Prezioa Lehen Unitatean"** eremuak.
