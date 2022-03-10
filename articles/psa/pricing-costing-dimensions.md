---
title: Prezioak eta kostuen neurriak hasierako orria
description: Gai honek prezioen dimentsioen ikuspegi orokorra eskaintzen du.
author: rumant
ms.custom:
- dyn365-projectservice
- intro-internal
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: d17939777a6670bafc41b372adc922f8bdcc0411f3fdb399e7c9ab01eca87dd0
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6998446"
---
# <a name="pricing-and-costing-dimensions-home-page"></a>Prezioak eta kostuen neurriak hasierako orria

[!include [banner](../includes/psa-now-project-operations.md)]

Proiektuetan oinarritutako erakundeetan eskulanaren prezioak eta kostuak ezartzeko erabilitako dimentsioek atributu hauek eragiten dituzte:

- Esperientzia, funtzio edo geografiaren antzeko lanak egiten dituzten pertsonak
- Bere konplexutasunaren edo eguneko orduaren antzera egin beharreko lana

Lanaren joera hauen izaera tipikoa eta lana burutzeko behar diren pertsonak kontuan hartuta, bi zerbitzu mota daude eskuragarri Project Service Automation-en: 

- **Aukera multzoak**: balio multzo baterako enumerazio finkoak diren atributuak.
- **Entitateetan oinarritutako balioak** - Mugatuak diren baina denbora zehar alda daitezkeen balio multzo anitza izan dezaketen atributuak.

## <a name="pricing-dimensions"></a>Prezioen dimentsioak

PSA prezioen dimentsio multzo lehenetsia da. Hauek ikus ditzakezu **Project Service** > **Parametroak** atalean. Parametroen erregistroan, **Zenbatekoan oinarritutako prezioen dimentsioak** fitxan, egiaztatu **msdyn_resourcecategory** funtzioak eta **msdyn_organizationalunit** baliabideak antolatzeko unitateak **Salmentetan aplikagarria** eta **Kostuetan aplikagarria** eremuetan **Bai** aukera ezarrita dutela. Horri esker, eginkizun eta antolaketa unitateen konbinazio bakoitzeko prezioa eta kostua konfiguratu ahal izango dituzu.

![Project Service-en parametroen pantaila-argazkia, "Salmentetan aplikagarria" eremua nabarmenduta dutela.](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> PSAren 3. bertsioaren berezko funtzio eta antolaketa unitateak prezioen dimentsio gisa erabiltzen aritu bazara, ez da aldaketarik egongo. Project Service erabiltzen jarraitu dezakezu ohi bezala. 

Baliabideen prezioa edo kostua behar baduzu atributu osagarriak erabiliz, eremu, entitate eta dimentsio pertsonalizatuak sor ditzakezu. Informazio gehiago lortzeko, ikusi honako gai hauek; hala ere, kontuan izan prozedurak bete behar dituzula beheko zerrendako ordenean:

- [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities.md)
- [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan](field-references.md)
- [Konfiguratu eremu pertsonalizatuak prezio-dimentsio gisa ](set-up-pricing-dimensions.md)
- [Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a>Giza baliabideen denborari prezio jartzea
Erakunde batek giza baliabideen denborari prezioa nola jartzen dion kontuan izan ohi da, erakundearen errentagarritasunean zuzenean eragiten duelako. Lan egin finantza taldeekin eta praktikatu arduradunekin zure erakundea giza baliabideen denboraren faktura eta kostu tasak nola ezarri nahi dituen identifikatzeko prest dagoenean.

Prezioei buruzko beste gogoeta batzuk dira gaur egun prezioen dimentsioak ez dituzten eremuak edo entitateak berriro erabiltzea, baina zure erakundeak prezio dimentsio gisa aplikatzea. **Transakzioen kategoria** (**msdyn_transactioncategory**) eta **Baliabide erreserbagarria** (**bookableresource**) motako eremuak hautagaien dimentsioen adibideak dira. 

Zure prezioen dimentsioa taula bat edo aukera multzo izan behar den ere hausnartu beharko zenuke. 10 edo 12 gaindituko duten dimentsioen balioen aldaketak aurreikusten badituzu eta balio horietarako atributu gehigarriak behar badituzu, sortu entitate bat aukera multzo bat sortu beharrean. Aukera multzoa mantentzeak, hala nola balioak gehitzea edo kentzea, administratzailea edo garatzailea eskatzen du, mahai batean errenkada berriak gehitzea negozio-erabiltzaile gehienek egin dezakete.

Hurrengo adibidean, baliabideari dagokion funtzioaren eta hornikuntza-unitatearen arabera konfiguratutako fakturen tasak erakusten dira. Kostu tasak, normalean, langilearen soldata-banda eta kide diren entitate unitatearen araberakoak dira. Adibide honetan, faktura-tasa eta kostu-tasen taulak ondorengoak izango dira.

**Faktura-tasaren adibidea**

| Funtzioa        | Erakunde-unitatea    |Unitatea      |Prezioa      |Moneta  |
| ------------|-------------|----------|----------:|----------|
| Garatzailea   | Contoso AEBetan  |Ordu | 200|USD     |
| Garatzailea   | Contoso India |Ordu|   112|USD     |


**Kostu-tasen adibidea**

| Soldata Banda     | Erakunde-unitatea    |Unitatea      |Prezioa      |Moneta  |
| ----------------|-------------|----------|----------:|----------|
| Nire company_Band1 | Contoso AEBetan  |Ordu | 145|USD     |
| Nire company_Band2 | Contoso India |Ordu|   67|USD     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]