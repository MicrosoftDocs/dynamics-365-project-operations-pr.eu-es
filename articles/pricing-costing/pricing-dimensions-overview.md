---
title: Prezioen dimentsioen informazio orokorra
description: Gai honek Dynamics 365 Project Operations-eko prezio-dimentsioei buruzko informazioa eskaintzen du.
author: rumant
ms.date: 11/30/2020
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 5f1fa83b52c3812f26e3ab75a8b08ebd40d82aa8
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8579200"
---
# <a name="pricing-dimensions-overview"></a>Prezioen dimentsioen informazio orokorra

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Prezioak eta kostuak ezartzeko giza baliabideetan erabiltzen diren dimentsioak bi kategoriatan sartzen dira:

- Jendea
- Planifikatutako lana

Hori dela eta, prezioen dimentsioko bi balore daude eskuragarri:

- **Aukera multzoak**: balio multzo baterako enumerazio finkoak diren neurriak.
- **Entitatean oinarritutako balioak**: balio multzo askotarikoak izan daitezkeen neurriak.

## <a name="pricing-dimensions"></a>Prezioen dimentsioak

Dynamics 365 Project Operations prezioen dimentsio multzo lehenetsia da. Prezio-dimentsio horiek ikus ditzakezu **Project Operations** > **Parametroak** atalean. Parametroen erregistroan, **Zenbatekoan oinarritutako prezioen dimentsioak** fitxan, egiaztatu **msdyn_resourcecategory** funtzioak eta **msdyn_organizationalunit** baliabideak antolatzeko unitateak **Salmentetan aplikagarria** eta **Kostuetan aplikagarria** eremuetan **Bai** aukera ezarrita dutela. Eremu horiek gaituta dituzula, eginkizun eta antolaketa unitateen konbinazio bakoitzeko prezioa eta kostua konfiguratu ahal izango dituzu.

![Project Service-en parametroen pantaila-argazkia, "Salmentetan aplikagarria" eremua nabarmenduta dutela.](media/PS-OOB-parameters.png)

Baliabideen prezioa edo kostua behar baduzu atributu osagarriak erabiliz, eremu, entitate eta dimentsio pertsonalizatuak sor ditzakezu. Informazio gehiagorako, ikus gai hauek. 
  
  > [!NOTE]
  > Izapideak zerrendatutako ordenan bete behar dira.

1. [Sortu prezio-dimentsio pertsonalizatuetarako soluzioa](../sales/create-solution-custompd.md)
2. [Sortu eremu eta entitate pertsonalizatuak](create-custom-fields-entities-pricing-dimensions.md)
3. [Gehitu eremu pertsonalizatuak prezioen konfigurazioan eta entitate transakzionaletan ](add-custom-fields-price-setup-transactional-entities.md)
4. [Konfiguratu eremu pertsonalizatuak prezio-dimentsio gisa ](set-up-custom-fields-pricing-dimensions.md)
5. [Eguneratu plugin atributuak prezio-dimentsio berriak sartzeko](update-plugin-attributes-pd.md)


## <a name="pricing-human-resource-time"></a>Giza baliabideen denborari prezio jartzea
Erakunde batek giza baliabideen denborari prezioa nola jartzen dion kontuan izan ohi da, erakundearen errentagarritasunean zuzenean eragiten duelako. Lan egin finantza taldeekin eta praktikatu arduradunekin zure erakundea giza baliabideen denboraren faktura eta kostu tasak nola ezarri nahi dituen identifikatzeko prest dagoenean.

Prezioei buruzko beste gogoeta batzuk dira gaur egun prezioen dimentsioak ez dituzten eremuak edo entitateak berriro erabiltzea, baina zure erakundeak prezio dimentsio gisa aplikatzea. **Transakzioen kategoria** (**msdyn_transactioncategory**) eta **Baliabide erreserbagarria** (**bookableresource**) motako eremuak hautagaien dimentsioen adibideak dira. 

Zure prezioen dimentsioa taula bat edo aukera multzo izan behar den ere hausnartu beharko zenuke. 10 edo 12 gaindituko duten dimentsioen balioen aldaketak aurreikusten badituzu eta balio horietarako atributu gehigarriak behar badituzu, entitatea sortuko zenuke aukera multzo bat baino. Aukera multzoa mantentzeak, hala nola balioak gehitzea edo kentzea, administratzailea edo garatzailea eskatzen du, mahai batean errenkada berriak gehitzea erabiltzaile gehienek egin dezakete.

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


[!INCLUDE[footer-include](../includes/footer-banner.md)]