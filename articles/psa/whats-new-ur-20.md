---
title: Project Service Automation eguneratzearen 20, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 20. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: ee3be43da401af405ab329b9b5a724a2e95c0219
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147098"
---
# <a name="project-service-automation-update-release-20-v3"></a>Project Service Automation 20, V3 eguneratze-bertsioa

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 20. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honen konpilazio-zenbakia V 3.10.31.37 da eta, oro har, 2020ko ekaineko eguneratze automatikoaren baten bidez dago eskuragarri.

## <a name="update-release-20"></a>20. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- Orduak eskatzen dituen esleipen-metodoak dituen proiektuko taldekideak inportatzean garbi geratzen ez den errore-mezu agertzen da zero ordu zehazten direnean.
- Erabiltzaileek akats okerra jasotzen dute gehieneko karaktere kopurua idatzi dutenean proiektu-zeregin baten **Deskribapena** eremuan.
- **Microsoft Dynamics 365 Project Service Automation gehigarrien deskarga** orrialdeak ingeleseko deskargen orrialdera birbideratzen du erabiltzailearen hizkuntza-ezarpenak japonieraz ezarrita daudenean.
- Zerbitzariaren errorea gertatzen denean, **Antolaketa** fitxaren sinkronizazio-etiketa, **Proiektuak** inprimakian, batzuetan geratu egiten da.
- Beharrezkoak ez diren zeregin-eguneratzeak bidaltzen ari dira zeregin bat aldatzen denean.

**Sales**

Arazo hauek konpondu dira:

- **Kontratua** inprimakian, **Sortu faktura** bi aldiz sakatzean, benetako datuen erregistro baten bi faktura sortzen ditu.
- Internet Explorer 11-n, erabiltzaileek ezin dute sortu gastuen sarrerarik.
- Kostuen itzulera eta Fakturatu gabeko salmenten benetako datuen itzulketa lotu gabe daude.
- **Freskatu benetako datuak** botoiak, **Proiektua** inprimakian, ez du freskatzen **Zereginaren benetako ordutegia**.
- **PreValidateProjectTeamMemberCreate** plug-inak baliabide deskargagarri orokor bikoiztuak sor ditzake **msdyn_isgenericresourceprojectscoped** atributua **Gezurra** gisa ezarrita dagoenean.
- **Birkalkulatu** eremuak produktuetan oinarritutako eskaintzaren lerroaren xehetasunen eta kontratuaren lerroaren xehetasunen kobra daitezkeen kostuak garbitzen ditu.
- Egoera zehatzetan, **PostEstimateLineUpdate** pluginak erreferentzia nuluaren salbuespen-errorea erakusten du.
- **Errentagarritasunaren analisia taulako** denbora-fasearen iraupena ez dator bat eskaintzako kostuen iraupenarekin prezio finkoaren eskaintzaren lerroaren xehetasunean.
- Unitateko eta unitate-taldeko balioak ez dira behar bezala lehenesten gastu kategorietan **Kontratuaren lerroko xehetasunak** eta **Eskaintzaren lerroaren xehetasunak** inprimakietan.
- **Erakundearen unitateko kostuaren prezioa** zerrenden baimena gainjarri egiten da data-eraginkortasunean.
- Erabiltzaileek ez dute **OrgUnit** aldatzeko baimenik eskaera mota ez denean lanean oinarritutakoa, erreferentzia nuluaren salbuespen-errorea sortuko duelako.
- **Eskaintzaren lerroaren xehetasunak** inprimakitik **Eskaintza** fitxara itzultzen saiatzean, inprimakia freskatu egiten da eta **Laburpena** fitxa erakusten du.
