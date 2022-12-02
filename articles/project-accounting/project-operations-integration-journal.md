---
title: Project Operations-eko integrazio-aldizkaria
description: Artikulu honek Project Operations-en Integrazio aldizkariarekin lan egiteari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 09/22/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: e947fe895a1caa9c9ea092597957a859cd8d61c9
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541062"
---
# <a name="integration-journal-in-project-operations"></a>Project Operations-eko integrazio-aldizkaria

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Denbora, gastu, tasa eta matarialen sarrerak sortzen dira **Benetakoa** proiektu baten aurka egindako lanaren ikuspegi operatiboa adierazten duten eragiketak. Dynamics 365 Project Operations-ek kontulariei tresna bat eskaintzen die transakzioak berrikusteko eta kontabilitate atributuak behar bezala doitzeko. Berrikuspena eta doikuntzak amaitu ondoren, transakzioak Proiektuaren liburu nagusian eta liburu nagusian argitaratzen dira. Kontulari batek jarduera hauek egin ditzake **Project Operations Integration** egunkaria (**Dynamics 365 Finance** > **Proiektuaren kudeaketa eta kontabilitatea** > **Egunkaria** > **Project Operations integrazioa** egunkaria.

![Integrazio aldizkariaren fluxua.](./media/IntegrationJournal.png)

### <a name="create-records-in-the-project-operations-integration-journal"></a>Sortu erregistroak Project Operations-eko integrazio-aldizkarian

Project Operations Integration aldizkarian erregistroak aldian aldiko prozesuaren bidez sortzen dira, **Inportatu taulako taulatik**. Exekutatu prozesua hona joanez: **Dynamics 365 Finance** > **Proiektuen kudeaketa eta kontabilitatea** > **Periodikoa** > **Project Operations integrazioa** > **Inportatu fase taulatik**. Prozesua modu interaktiboan exekutatu edo atzeko planoan exekutatzeko konfiguratu dezakezu beharren arabera.

Aldian aldiko prozesua exekutatzen denean, oraindik Project Operations-en Integrazio aldizkarian gehitzen ez diren egiazkoak aurkitzen dira. Benetako transakzio bakoitzeko egunkari lerro bat sortzen da.
Sistemak aldizkari lerroak aldizkari banatan taldekatzen ditu fitxategian hautatutako balioaren arabera **Project Operations Integration aldizkariaren aldiko unitatea** eremua (**Finantzak** > **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak**, **Project Operations on Dynamics 365 Customer Engagement** fitxa). Eremu honetarako balore posibleak hauek dira:

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
    - **Transakzio-kategoria** ez dago egiazko proiektuan ezarrita, sistemak balioa erabiltzen du **Proiektuaren kategoria lehenetsiak** eremuan **Project Operations on Dynamics 365 Customer Engagement** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.
  - **Baliabidea** eremuak transakzio honekin lotutako proiektuaren baliabidea adierazten du. Baliabidea erreferentzia gisa erabiltzen da bezeroei proiektuen faktura proposamenetan.
  - **Truke-tasa** eremuko lehenetsiak **Moneta truke-tasa** jarri Dynamics 365 Finance-n. Truke tasaren konfigurazioa falta bada, **Inportatu eszenaratzetik** aldian aldiko prozesuak ez du erregistroa egunkari batean gehituko eta errore mezu bat gehituko da lanaren exekuzio erregistroan.
  - **Linearen jabetza** eremuak proiektuaren fakturen fakturazio mota adierazten du. Linearen propietateak eta fakturazio motaren mapak definitzen dira **Project Operations on Dynamics 365 Customer Engagement** fitxan **Proiektuen kudeaketa eta kontabilitate parametroak** orrialdea.

Kontabilitate atributu hauek soilik egunera daitezke Project Operations bateratzeko egunkari lerroetan:

- **Fakturazio salmenten gaineko zerga taldea** eta **Fakturazio elementuen salmenten gaineko zerga taldea**
- **Finantza dimentsioak** (erabiliz **Zenbatekoak banatu** ekintza)

Integrazio-egunkariaren lerroak ezabatu daitezke. Hala ere, integrazio egunkariaren lerroak ezabatu daitezke, hala ere, argitaratu gabeko lerroak egunkarian berriro txertatuko dira berriro exekutatu ondoren **Inportatu eszenaratzetik** aldian aldiko prozesua.

### <a name="post-the-project-operations-integration-journal"></a>Argitaratu Project Operations Integration-en aldizkaria

Integrazio aldizkaria argitaratzen duzunean, proiektuaren azpiegitura eta liburu nagusien transakzioak sortzen dira. Hauek beheranzko bezeroen fakturazioan, diru sarreren ezagutzan eta finantza txostenetan erabiltzen dira.

Hautatutako Project Operations integrazio aldizkaria erabiliz argitaratu daiteke **Argitalpena** Project Operations integrazio aldizkariaren orrian. Aldizkari guztiak automatikoki bidal daitezke prozesu bat martxan jarrita helbidean **Periodikoak** > **Project Operations integrazioa** > **Post Project Operations integrazio aldizkaria**.

Argitalpena modu interaktiboan edo sorta batean egin daiteke. Kontuan izan 100 lerro baino gehiago dituzten aldizkari guztiak automatikoki sorta batean argitaratuko direla. Lerro asko dituzten aldizkariak sorta batean argitaratzen direnean errendimendu hobea lortzeko, gaitu **Post Project Operations integrazio aldizkaria sortako zeregin anitz erabiliz** ezaugarria **Ezaugarrien kudeaketa** lan-eremua. 

#### <a name="transfer-all-lines-that-have-posting-errors-to-a-new-journal"></a>Bidali akatsak dituzten lerro guztiak aldizkari berri batera

> [!NOTE]
> Gaitasun hori erabiltzeko, gaitu **Transferitu akatsak argitaratzen dituzten lerro guztiak Project Operations integrazio aldizkari berri batera** ezaugarria **Ezaugarrien kudeaketa** lan-eremua.

Ezaugarri honek Project Operations integrazio aldizkariaren esperientzia hobetzen laguntzen du. Gaituta dagoenean, idazketa bikoitzeko denbora-arazoek eta konfigurazio-arazoek ez dute baliozko aldizkariak argitaratzea eragozten. Project Operations integrazio aldizkarian argitaratzean, sistemak aldizkariko lerro guztiak balioztatzen ditu. Akatsik ez duten lerro guztiak argitaratzen ditu eta aldizkari berri bat sortzen du bidalketa-akatsak dituzten lerro guztientzat.

Bidalitako errore-lerroak dituzten aldizkariak berrikusteko, joan hona **Proiektuen kudeaketa eta kontabilitatea** \> **Aldizkariak** \> **Project Operations integrazio aldizkaria**, eta iragazi aldizkarien zerrenda erabiliz **Jatorrizko aldizkaria** eremua. Ondorengo ilustrazioak adibide bat erakusten du non aldizkariak **Project Operations integrazio aldizkaria** orria horrela iragazi da.

![Jatorrizko egunkaria Project Operations Integration aldizkariaren orrian erakutsita.](./media/transferLines-originalJournal.png)

Aldizkako sorta-lan bat integrazio aldizkaria bidaltzeko konfiguratuta badago, bidalketa berriro saiatuko da, eta aldizkariak argitaratuko dira denbora-arazoa konpondu bada. Gainerako aldizkariak eskuz ikertu behar dira erregistroak aztertuz eta beharrezko neurriak hartuz.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
