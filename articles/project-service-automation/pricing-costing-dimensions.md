---
title: Prezioak eta kostuen neurriak hasierako orria
description: Gai honek prezioen dimentsioen ikuspegi orokorra eskaintzen du.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 425d7bb8-9015-4f67-b9c9-cf3602e9afe8
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 2379d0d2e038f28a1a8df87a851e9bf7db7fe33f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748846"
---
# <a name="pricing-and-costing-dimensions-home-page"></a>Prezioak eta kostuen neurriak hasierako orria

Prezioak eta kostuak ezartzeko giza baliabideetan erabiltzen diren dimentsioak bi kategoriatan sartzen dira:

- Jendea
- Planifikatutako lana

Hori dela eta, prezioen dimentsioko bi balore daude eskuragarri Project Service Automation-en (PSA): 

- **Aukera multzoak**: balio multzo baterako enumerazio finkoak diren neurriak.
- **Entitatean oinarritutako balioak**: balio multzo askotarikoak izan daitezkeen neurriak.

## <a name="pricing-dimensions"></a>Prezio-dimentsioak

PSA prezioen dimentsio multzo lehenetsia da. Hauek ikus ditzakezu **Project Service** > **Parametroak** atalean. Parametroen erregistroan, **Zenbatekoan oinarritutako prezioen dimentsioak** fitxan, egiaztatu **msdyn_resourcecategory** funtzioak eta **msdyn_organizationalunit** baliabideak antolatzeko unitateak **Salmentetan aplikagarria** eta **Kostuetan aplikagarria** eremuetan **Bai** aukera ezarrita dutela. Horri esker, eginkizun eta antolaketa unitateen konbinazio bakoitzeko prezioa eta kostua konfiguratu ahal izango dituzu.

![Project Service-en parametroen pantaila-argazkia, "Salmentetan aplikagarria" eremua nabarmenduta dutela](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> PSAren 3. bertsioaren berezko funtzio eta antolaketa unitateak prezioen dimentsio gisa erabiltzen aritu bazara, ez da aldaketarik egongo. Project Service erabiltzen jarraitu dezakezu ohi bezala. 

Baliabideen prezioa edo kostua behar baduzu atributu osagarriak erabiliz, eremu, entitate eta dimentsio pertsonalizatuak sor ditzakezu. Informazio gehiago lortzeko, ikusi honako gai hauek; hala ere, kontuan izan prozedurak bete behar dituzula beheko zerrendako ordenean:

- [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities.md)
- [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan](field-references.md)
- [Ezarri eremu pertsonalizatuak prezio-dimentsio gisa](set-up-pricing-dimensions.md)
- [Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a>Giza baliabideen denborari prezio jartzea
Erakunde batek giza baliabideen denborari prezioa nola jartzen dion kontuan izan ohi da, erakundearen errentagarritasunean zuzenean eragiten duelako. Lan egin finantza taldeekin eta praktikatu arduradunekin zure erakundea giza baliabideen denboraren faktura eta kostu tasak nola ezarri nahi dituen identifikatzeko prest dagoenean.

Prezioei buruzko beste gogoeta batzuk dira gaur egun prezioen dimentsioak ez dituzten eremuak edo entitateak berriro erabiltzea, baina zure erakundeak prezio dimentsio gisa aplikatzea. **Transakzioen kategoria** (**msdyn_transactioncategory**) eta **Baliabide erreserbagarria** (**bookableresource**) motako eremuak hautagaien dimentsioen adibideak dira. 

Zure prezioen dimentsioa taula bat edo aukera multzo izan behar den ere kontuan hartu beharko zenuke. 10 edo 12 gaindituko duten dimentsioen balioen aldaketak aurreikusten badituzu eta balio horietarako atributu gehigarriak behar badituzu, entitatea sortuko zenuke aukera multzo bat baino. Aukera multzoa mantentzeak, hala nola balioak gehitzea edo kentzea, administratzailea edo garatzailea eskatzen du, mahai batean errenkada berriak gehitzea erabiltzaile gehienek egin dezakete.

Hurrengo adibidean, baliabideari dagokion funtzioaren eta hornikuntza-unitatearen arabera konfiguratutako fakturen tasak erakusten dira. Kostu tasak, normalean, langilearen soldata-banda eta kide diren entitate unitatearen araberakoak dira. Adibide honetan, faktura-tasa eta kostu-tasen taulak ondorengoak izango dira.

**Faktura-tasaren adibidea**

| Funtzioa        | Erakunde-unitatea    |Unitatea      |Prezioa      |Moneta  |
| ------------|-------------|----------|----------:|----------|
| Garatzailea   | Contoso US  |Hour | 200|USD     |
| Garatzailea   | Contoso India |Hour|   112|USD     |


**Kostu-tasen adibidea**

| Soldata Banda     | Erakunde-unitatea    |Unitatea      |Prezioa      |Moneta  |
| ----------------|-------------|----------|----------:|----------|
| Nire company_Band1 | Contoso US  |Hour | 145|USD     |
| Nire company_Band2 | Contoso India |Hour|   67|USD     |
