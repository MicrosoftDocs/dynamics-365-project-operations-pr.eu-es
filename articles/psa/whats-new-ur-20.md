---
title: Project Service Automation eguneratzearen 20, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 20. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 12edae76dbc6de63d3e2d36058c4092f80ede77d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/16/2020
ms.locfileid: "4070985"
---
# <a name="project-service-automation-update-release-20-v3"></a>Project Service Automation 20, V3 eguneratze-bertsioa

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
