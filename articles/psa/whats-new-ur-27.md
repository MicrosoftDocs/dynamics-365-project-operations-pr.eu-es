---
title: Project Service Automation eguneratzearen 27, V3 bertsioko berrikuntzak edo aldaketak
description: Gai honek Project Service Automation V3, 27. eguneratzean erabilgarri dauden eginbideak eta konponketak ditu.
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
ms.openlocfilehash: aab77411760c3d64daa377bffc06391c8e4ed54a
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8599577"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-27-v3"></a>Project Service Automation eguneratzearen 27, V3 bertsioko berrikuntzak edo aldaketak

[!include [banner](../includes/psa-now-project-operations.md)]

Atseginez iragartzen dizuegu Dynamics 365 aplikaziorako Project Service Automation aplikazioaren azken eguneratzea. Argitalpen honek kalitatearen, errendimenduaren eta erabilgarritasunaren hobekuntza garrantzitsuak ditu. Argitalpen hau bateragarria da Dynamics 365 9.x bertsioarekin. Argitalpen honetara eguneratzeko, bisitatu Dynamics 365 (online) aplikazioaren administrazio-zentroko soluzioen orrira eguneratzea instalatzeko. Informazio gehiago lortzeko, ikusi [Instalatu, eguneratu edo kendu soluzio hobetsi bat](/power-platform/admin/install-remove-preferred-solution).

Gai honek Project Service Automation V3, 27. eguneratzea bertsioan berriak diren edo aldatu diren eginbideak eta konponketak ditu. Bertsio honek V3.10.45.98 konpilazio-zenbakia du eta, oro har, 2021eko urtarrilean jarriko da erabilgarri automatikoki eguneratzeko moduan.

## <a name="update-release-27"></a>27. eguneratze-bertsioa

### <a name="bug-fixes"></a>Akatsen zuzenketa

**Orokorra**

Arazo hauek konpondu dira:

- Plugin-ek Project Service Automation-en sortutako erregistroak ez dira automatikoki ezabatzeko ezarri.
- Bertsio-berritzeak huts egiten du Project Service Automation irtenbideak NavBarArea eta izenburuko elementu zaharrak dituelako.

**Denbora eta gastua**

Arazo hauek konpondu dira:

- **Denbora-sarrera** saretak datu okerrak erakusten ditu **Ordu-zona independentea** data-portaerarako.
- **Denbora-sarrera** saretak ordu okerrak sortzen ditu **Ordu-zona independentea** data-portaerarako.
- Zereginen bilaketa ez da hautatutako proiektuan soilik **Editatu denbora-sarrera** orrialdean.
- Proiektuak ez diren denbora-sarreretarako denbora onartzeak sistema blokeatzen du proiektu-onartzailea bilatzean.
- Benetako datuen sarrera zuzenak errore mezu okerra bistaratzen du.
- Zeregin batek benetako kosturako balio nulua duenean eta proiektuaren guztirakoak freskatzen direnean, errore hau gertatzen da, "Hiztegian ez dagoen gakoa emanda".
- Zenbait kasutan, **Taldekatu** iragazkiak **Proiektuaren aurrekontua** fitxan ez dira gastuen kalkuluak agertzen.
- **Udako ordutegia** tartea ez da zuzena denbora sarreretarako.

**Proiektuen kudeaketa**

Arazo hauek konpondu dira:

- Caching hobekuntzak, hau da, kargatzearekin erlazionatutako errendimendua hobetzen du **Proiektua** orrialdea.
- Negozio arau zaharkitua proiektuaren zereginak burutzea eragozten du.
- Microsoft Project gehigarrien inguruneak ez dira gehigarriaren egutegia errespetatzen eta ondorioz baliabideen eskakizun okerrak daude.
- Proiektuak txantiloietatik sortzeak esleipen datak gaizki ezartzen ditu eta baliabide eskakizunak sortzeko gaitasuna eragozten du.
- Erabiltzailea ezin da sartu **Kategoria**, **Deskribapena**, **Egoera** aukerak teklatua erabiliz.
- Proiektuaren benetako salmenten balioak ez dira kuoten eta materialen salmenten balioak barne.
- Benetako salmenten eta benetako kostuaren batuketa oker egiten da truke-tasa desberdinak erabiltzen direnean.
- **Lan-ordutegiaren txantiloia lehenetsia** eremuko azalpena engainagarria da.
- Zeregin bat koska ez da kentzen **Kategoria** erabiltzailearen interfazean freskatu arte.
- Proiektua amaierako datatik aurrera eramateko ziurtatzeko baliozkotzea falta da.

**Sales**

Arazo hauek konpondu dira:

- Proiektuaren aurrekontu lerroan erreferentzia nuluko salbuespena sortzen da **Inportatu proiektuaren zenbatespenetik** ikusgai dago proiektua hautatu ez denean.
- Honako errore hau, "Objektuaren erreferentzia ez da objektu baten instantziarekin ezarrita" gertatzen da aurrekontua honela ixterakoan **Irabazita**.
- Egokitzapen egoera zehaztu gabe dago atzera egitean proiektu bat kontratu linea batetik lotzen duzun bitartean.
- Dynamics 365 Field Service eta Project Service Automation instalatuta badaude, **Blokeatu prezioak** eta **Erabili uneko prezioak** aukerak ez dira aldi berean bistaratzen **Faktura** orrialdean.
- Japoniako hizkuntzari dagokionez, ez dago itzulpen koherenterik egutegian oinarritutako beste orriekin.
- **Aktibatu** eta **Desaktibatu** kendu dira **Prezio-zerrenden elkartea** entitateak Project Service Automation-en.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
