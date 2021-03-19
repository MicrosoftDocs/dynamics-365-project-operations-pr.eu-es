---
title: Project Operations-eko integrazio-aldizkaria
description: Gai honek Project Operations-en Integrazio aldizkariarekin lan egiteari buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0021147530d1aa9f82cc54ca8c92b9977c1eea2c
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287223"
---
# <a name="integration-journal-in-project-operations"></a>Project Operations-eko integrazio-aldizkaria

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Denbora eta gastu sarrerak sortzen dira **Benetakoa** proiektu baten aurka egindako lanaren ikuspegi operatiboa adierazten duten eragiketak. Dynamics 365 Project Operations-ek kontulariei tresna bat eskaintzen die transakzioak berrikusteko eta kontabilitate atributuak behar bezala doitzeko. Berrikuspena eta doikuntzak amaitu ondoren, transakzioak Proiektuaren liburu nagusian eta liburu nagusian argitaratzen dira. Kontulari batek jarduera hauek egin ditzake **Project Operations-en integrazioa** aldizkaria (**Dynamics 365 Finance** > **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkariak** > **Project Operations-en Integrazioa** aldizkaria).

![Integrazio aldizkariaren fluxua](./media/IntegrationJournal.png)

### <a name="create-records-in-the-project-operations-integration-journal"></a>Sortu erregistroak Project Operations-eko integrazio-aldizkarian

Project Operations Integration aldizkarian erregistroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu taulako taulatik**. Prozesu hau joan zaitezke **Dynamics 365 Finance** > **Proiektuen kudeaketa eta kontabilitatea** > **Aldizkakoa** > **Project Operations-en Integrazioa** > **Inportatu taulako taulatik**. Prozesua modu interaktiboan exekutatu edo atzeko planoan exekutatzeko konfiguratu dezakezu beharren arabera.

Aldian aldiko prozesua exekutatzen denean, oraindik Project Operations-en Integrazio aldizkarian gehitzen ez diren egiazkoak aurkitzen dira. Benetako transakzio bakoitzeko egunkari lerro bat sortzen da.
Sistemak aldizkari lerroak aldizkari banatan taldekatzen ditu fitxategian hautatutako balioaren arabera **Project Operations Integration aldizkariaren aldiko unitatea** eremua (**Finantzak** > **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak**, **Proiektuaren eragiketak aktibatuta Dynamics 365 Customer Engagement** fitxa). Eremu honetarako balore posibleak hauek dira:

  - **Egunak**: benetako datuak transakzio dataren arabera biltzen dira. Egun bakoitzeko aldizkari bat sortzen da.
  - **Hilabeteak**: Egunak hilabete naturalaren arabera biltzen dira. Hilabete bakoitzeko aldizkari bat sortzen da.
  - **Urteak**: Urteak hilabete naturalaren arabera biltzen dira. Urte bakoitzeko aldizkari bat sortzen da.
  - **Guztiak**: Benetako transakzio guztiak integrazio aldizkari berean sartzen dira. Aldizkaria eskuragarri ez badago aldian aldiko prozesua exekutatzen denean, adibidez, aldizkaria transakzioak bidaltzeko prozesuan badago, egunkari berria sortzen da.

Aldizkari-lerroak proiektuaren errealitatean oinarrituta sortzen dira. Ondorengo zerrendan lehenespen eta transformazio arau aipagarrienetako batzuk daude:

  - Proiektuaren benetako transakzio bakoitzak lerro bat du Project Operations Integration aldizkarian. Denboraren eta materialaren fakturazio motaren kostuaren eta fakturatu gabeko salmenten transakzioak linea desberdinetan agertzen dira.
  - **Data** eremuak transakzioaren data adierazten du. **Kontabilitate data** eremuak transakzioa liburuan erregistratu den data adierazten du. Kontabilitate data [itxitako ekitaldi ekonomikoa](https://docs.microsoft.com/dynamics365/finance/general-ledger/close-general-ledger-at-period-end), eta parametroa **Ezarri automatikoki kontabilitate data liburuaren epea irekitzeko** ezartzen da **Finantzarioa** fitxategiaren fitxa **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdean, sistemak transakzioaren kontabilitate-data egokituko du liburu irekiaren hurrengo aldiko lehenengo datara.
  - **Bonua** eremuak benetako transakzio bakoitzaren bonuaren zenbakia erakusten du. Bonuaren zenbakien sekuentzia **Zenbaki-sekuentziak** fitxan, **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea. Lerro bakoitzari zenbaki berria esleitzen zaio. Bonoa argitaratu ondoren, kostua eta fakturaziorik gabeko salmenta transakzioa nola erlazionatzen diren ikus dezakezu hautatuta **Lotutako bonuak** gainean **Bonuen transakzioa** orrialdea.
  - **Kategoria** eremuak proiektuaren transakzio bat adierazten du eta lehenetsitakoa erlazionatutako proiektuaren transakzio kategorian oinarrituta dago.
    - **Transakzio-kategoria** Proiektuaren benetakoa eta erlazionatutakoa da **Proiektuaren kategoria** pertsona juridiko jakin batean dago, kategoria proiektuaren kategoria honetan lehenetsita dago.
    - **Transakzio-kategoria** ez dago egiazko proiektuan ezarrita, sistemak balioa erabiltzen du **Proiektuaren kategoria lehenetsiak** eremuan **Proiektuaren eragiketak aktibatuta Dynamics 365 Customer Engagement** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.
  - **Baliabidea** eremuak transakzio honekin lotutako proiektuaren baliabidea adierazten du. Baliabidea erreferentzia gisa erabiltzen da bezeroei proiektuen faktura proposamenetan.
  - **Truke-tasa** eremuko lehenetsiak **Moneta truke-tasa** jarri Dynamics 365 Finance. Truke tasaren konfigurazioa falta bada, **Inportatu eszenaratzetik** aldian aldiko prozesuak ez du erregistroa egunkari batean gehituko eta errore mezu bat gehituko da lanaren exekuzio erregistroan.
  - **Linearen jabetza** eremuak proiektuaren fakturen fakturazio mota adierazten du. Linearen propietateak eta fakturazio motaren mapak definitzen dira **Proiektuaren eragiketak aktibatuta Dynamics 365 Customer Engagement** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

Kontabilitate atributu hauek soilik egunera daitezke Project Operations bateratzeko egunkari lerroetan:

- **Fakturazio salmenten gaineko zerga taldea** eta **Fakturazio elementuen salmenten gaineko zerga taldea**
- **Finantza dimentsioak** (erabiliz **Zenbatekoak banatu** ekintza)

Integrazio egunkariaren lerroak ezabatu daitezke, hala ere, argitaratu gabeko lerroak egunkarian berriro txertatuko dira berriro exekutatu ondoren **Inportatu eszenaratzetik** aldian aldiko prozesua.

Integrazio aldizkaria argitaratzen duzunean, proiektuaren azpiegitura eta liburu nagusien transakzioak sortzen dira. Hauek beheranzko bezeroen fakturazioan, diru sarreren ezagutzan eta finantza txostenetan erabiltzen dira.


[!INCLUDE[footer-include](../includes/footer-banner.md)]