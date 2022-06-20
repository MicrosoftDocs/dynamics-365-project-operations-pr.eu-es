---
title: Project Operations-eko integrazio-aldizkaria
description: Artikulu honek Project Operations-en Integration aldizkariarekin lan egiteari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 10/27/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: befb1756ad77708805f3cbb06168b93e44296df0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923863"
---
# <a name="integration-journal-in-project-operations"></a>Project Operations-eko integrazio-aldizkaria

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Denbora eta gastu sarrerak sortzen dira **Benetakoa** proiektu baten aurka egindako lanaren ikuspegi operatiboa adierazten duten eragiketak. Dynamics 365 Project Operations-ek kontulariei tresna bat eskaintzen die transakzioak berrikusteko eta kontabilitate atributuak behar bezala doitzeko. Berrikuspena eta doikuntzak amaitu ondoren, transakzioak Proiektuaren liburu nagusian eta liburu nagusian argitaratzen dira. Kontu-hartzaile batek jarduera hauek egin ditzake **Proiektuaren Eragiketen Integrazioa** aldizkaria(**Dynamics 365 Finance** > **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkariak** > **Proiektuaren Eragiketen Integrazioa** aldizkaria.

![Integrazio aldizkariaren fluxua.](./media/IntegrationJournal.png)

### <a name="create-records-in-the-project-operations-integration-journal"></a>Sortu erregistroak Project Operations-eko integrazio-aldizkarian

Project Operations Integration aldizkarian erregistroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu taulako taulatik**. Prozesu hau exekutatu dezakezu helbidera joanez **Dynamics 365 Finance** > **Proiektuen kudeaketa eta kontabilitatea** > **Periodikoa** > **Proiektuaren Eragiketen Integrazioa** > **Inportatu eszenatze-taulatik**. Prozesua modu interaktiboan exekutatu edo atzeko planoan exekutatzeko konfiguratu dezakezu beharren arabera.

Aldian aldiko prozesua exekutatzen denean, oraindik Project Operations-en Integrazio aldizkarian gehitzen ez diren egiazkoak aurkitzen dira. Benetako transakzio bakoitzeko egunkari lerro bat sortzen da.
Sistemak aldizkari-lerroak aldizkari bereizietan biltzen ditu, aukeratutako balioaren arabera **Proiektuaren Eragiketen Integrazio aldizkariari buruzko aldi unitatea** eremua (**Finantza** > **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak**, **Eragiketak Dynamics 365 Customer Engagement-en** fitxa). Eremu honetarako balore posibleak hauek dira:

  - **Egunak**: benetako datuak transakzio dataren arabera biltzen dira. Egun bakoitzeko aldizkari bat sortzen da.
  - **Hilabeteak**: Egunak hilabete naturalaren arabera biltzen dira. Hilabete bakoitzeko aldizkari bat sortzen da.
  - **Urteak**: Urteak hilabete naturalaren arabera biltzen dira. Urte bakoitzeko aldizkari bat sortzen da.
  - **Guztiak**: Benetako transakzio guztiak integrazio aldizkari berean sartzen dira. Aldizkaria eskuragarri ez badago aldian aldiko prozesua exekutatzen denean, adibidez, aldizkaria transakzioak bidaltzeko prozesuan badago, egunkari berria sortzen da.

Aldizkari-lerroak proiektuaren errealitatean oinarrituta sortzen dira. Ondorengo zerrendan lehenespen eta transformazio arau aipagarrienetako batzuk daude:

  - Proiektuaren benetako transakzio bakoitzak lerro bat du Project Operations Integration aldizkarian. Denboraren eta materialaren fakturazio motaren kostuaren eta fakturatu gabeko salmenten transakzioak linea desberdinetan agertzen dira.
  - **Data** eremuak transakzioaren data adierazten du. **Kontabilitate data** eremuak transakzioa liburuan erregistratu den data adierazten du. Kontabilitate data [itxitako ekitaldi ekonomikoa](/dynamics365/finance/general-ledger/close-general-ledger-at-period-end), eta parametroa **Ezarri automatikoki kontabilitate data liburuaren epea irekitzeko** ezartzen da **Finantzarioa** fitxategiaren fitxa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, sistemak transakzioaren kontabilitate-data egokituko du liburu irekiaren hurrengo aldiko lehenengo datara.
  - **Bonua** eremuak benetako transakzio bakoitzaren bonuaren zenbakia erakusten du. Bonuaren zenbakien sekuentzia **Zenbaki-sekuentziak** fitxan, **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea. Lerro bakoitzari zenbaki berria esleitzen zaio. Bonoa argitaratu ondoren, kostua eta fakturaziorik gabeko salmenta transakzioa nola erlazionatzen diren ikus dezakezu hautatuta **Lotutako bonuak** gainean **Bonuen transakzioa** orrialdea.
  - **Kategoria** eremuak proiektuaren transakzio bat adierazten du eta lehenetsitakoa erlazionatutako proiektuaren transakzio kategorian oinarrituta dago.
    - **Transakzio-kategoria** Proiektuaren benetakoa eta erlazionatutakoa da **Proiektuaren kategoria** pertsona juridiko jakin batean dago, kategoria proiektuaren kategoria honetan lehenetsita dago.
    - Bada **Transakzio kategoria** ez dago benetako proiektuan ezarrita, sistemak balioa erabiltzen du **Proiektuaren kategoria lehenetsiak** eremuan **Proiektuaren Eragiketak Dynamics 365 Customer Engagement-en** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.
  - **Baliabidea** eremuak transakzio honekin lotutako proiektuaren baliabidea adierazten du. Baliabidea erreferentzia gisa erabiltzen da bezeroei proiektuen faktura proposamenetan.
  - The **Truke-tasa** Eremu lehenetsiak **Dibisaren truke-tasa** ezarri Dynamics 365 Finance. Truke tasaren konfigurazioa falta bada, **Inportatu eszenaratzetik** aldian aldiko prozesuak ez du erregistroa egunkari batean gehituko eta errore mezu bat gehituko da lanaren exekuzio erregistroan.
  - **Linearen jabetza** eremuak proiektuaren fakturen fakturazio mota adierazten du. Lerro-propietatea eta fakturazio-motaren mapaketa-n definitzen dira **Proiektuaren eragiketak Dynamics 365 Customer Engagement-en** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

Kontabilitate atributu hauek soilik egunera daitezke Project Operations bateratzeko egunkari lerroetan:

- **Fakturazio salmenten gaineko zerga taldea** eta **Fakturazio elementuen salmenten gaineko zerga taldea**
- **Finantza dimentsioak** (erabiliz **Zenbatekoak banatu** ekintza)

Integrazio egunkariaren lerroak ezabatu daitezke, hala ere, argitaratu gabeko lerroak egunkarian berriro txertatuko dira berriro exekutatu ondoren **Inportatu eszenaratzetik** aldian aldiko prozesua.

Integrazio aldizkaria argitaratzen duzunean, proiektuaren azpiegitura eta liburu nagusien transakzioak sortzen dira. Hauek beheranzko bezeroen fakturazioan, diru sarreren ezagutzan eta finantza txostenetan erabiltzen dira.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
