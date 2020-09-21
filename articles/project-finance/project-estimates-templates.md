---
title: Sinkronizatu proiektuaren kalkuluak zuzenean Project Service Automation-etik Finance and Operations
description: Gai honek proiektuaren orduen kalkuluak eta proiektuaren gastuen kalkuluak Microsoft-etik zuzenean sinkronizatzeko erabiltzen diren txantiloiak eta azpiko atazak deskribatzen ditu Microsoft Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: d688ce9a-41e3-4ebe-952e-700f8351fbe9
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: a24a967d82c2e005e61234d34da8a583b61ff7b1
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "3748853"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a>Sinkronizatu proiektuaren kalkuluak zuzenean Project Service Automation-etik Finance and Operations

[!include[banner](../includes/banner.md)]

Gai honek proiektuaren orduen kalkuluak eta proiektuaren gastuen kalkuluak zuzenean sinkronizatzeko erabiltzen diren txantiloiak eta azpiko atazak deskribatzen ditu Dynamics 365 Project Service Automation hurrengora Dynamics 365 Finance.

> [!NOTE]
> - Proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa eskuragarri daude 8.0 bertsioan.
> - Datu bateratuen integrazioa eskuragarri dago 8.0.1 bertsioan edo hurrengoan.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation Finantzararen datu-fluxua

Project Service Automation to Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko. Datuak integratzeko funtzioarekin eskuragarri dauden integrazio txantiloiek proiektuaren orduen kalkuluen eta proiektuaren gastuen kalkuluen inguruko datuen fluxua ahalbidetzen dute Project Service Automation-etik Finantzara.

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.

[![Project Service Automation Finantzarekin integratzeko datuen fluxua](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)

## <a name="project-hour-estimates"></a>Proiektuaren orduaren aurreikuspenak

### <a name="template-and-tasks"></a>Txantiloia eta zereginak

Eskuragarri dauden txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.

Ondorengo txantiloia eta azpiko zereginak proiektuaren orduen kalkuluak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:

- **Datuen integrazioko txantiloiaren izena:** Proiektuaren orduen kalkuluak (PSA Fin eta Ops)
- **Proiektuko zereginaren izena:**

    - Transakzio-harremanak
    - Expense estimates

### <a name="entity-set"></a>Entitate multzoaren

| Project Service Automation | Finantzak                                       |
|----------------------------|-----------------------------------------------|
| Proiektuen zereginak              | Integrazio entitatea proiektuaren orduen kalkuluen arabera |

### <a name="entity-flow"></a>Entitate fluxua

Proiektuaren orduen kalkuluak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren orduen iragarpen gisa.

### <a name="prerequisites"></a>Aurrebaldintzak

Proiektuaren orduen kalkuluen sinkronizazioa gertatu aurretik, proiektuak, proiektuaren zereginak eta proiektuaren gastuen transakzio kategoriak sinkronizatu behar dituzu.

### <a name="power-query"></a>Power Query

Proiektuaren orduen kalkuluen txantiloian, Microsoft Power Query Excel erabili behar duzu zeregin hauek burutzeko:

- Ezarri integrazioak ordu iragarpen berriak sortzen dituenean erabiliko den iragarpen eredu lehenetsia.
- Ordu iragarpenetan integrazioa huts egingo duen atazan baliabide espezifikoen erregistroak iragazi.
- Iragazi transakzio kategoriako errenkada hutsak. Zeregin hori ez betetzeak ordu iragarpen okerrak sor ditzake.

#### <a name="set-the-default-forecast-model-id"></a>Ezarri iragarpen eredu lehenetsiaren IDa

Txantiloian aurreikusitako modeloaren ID lehenetsia eguneratzeko, egin klik **Mapa** gezia mapa irekitzeko. Ondoren, hautatu **Kontsulta eta iragazki aurreratuak** esteka.

- Proiektuaren ordu-estimazio lehenetsiak (PSA to Fin eta Ops) txantiloia erabiltzen ari bazara, hautatu **Txertatutako baldintza** zerrendan **Urrats Aplikatuak**. **Funtzioa** sarrera, ordeztu **O\_iragarpena** integrazioarekin batera erabili behar den aurreikuspen ereduaren IDaren izenarekin. Txantiloi lehenetsiak iragarpen eredu IDa du demo datuetatik.
- Txantiloi berria sortzen ari bazara, zutabe hau gehitu behar duzu. Power Query atalean, hautatu **Gehitu baldintzazko zutabea**, eta idatzi zutabe berriaren izena, adibidez **ID eredua**. Idatzi zutabearen baldintza. Proiektuaren zeregina nulua ez bada, orduan \<idatzi iragarpen ereduaren IDa\>; bestela nulua.

#### <a name="filter-out-resource-specific-records"></a>Iragazi baliabide espezifikoen erregistroak

Project hour estimations (PSA to Fin and Ops) txantiloiak iragazki lehenetsia du, baliabide espezifikoen erregistroak ezabatzen dituena. Zure txantiloia sortzen baduzu, iragazki hau gehitu behar duzu. Aukeratu **Kontsulta eta iragazki aurreratuak** fitxategian iragazteko esteka **msdyn\_islinetask** zutabea soilik beraz **Gezurra** erregistroak sartzen dira.

#### <a name="filter-out-empty-transaction-category-rows"></a>Iragazi transakzio kategoriako errenkada hutsak

Iragazki bat gehitu behar duzu transakzio kategoria hutsak dituzten errenkadak ezabatzeko. Zeregin hori beharrezkoa da, txantiloi lehenetsia erabiltzen ari zaren edo zeure txantiloia sortzen ari zaren kontuan hartu gabe. Iragazki honek Project Service Automation-en laburpen-errenkadak kentzen ditu Finantzako orduen iragarpenak okerrak izan daitezkeen. Aukeratu **Kontsulta eta iragazki aurreratuak** esteka erregistro nuluak iragazteko **msdyn\_transakziokategoria\_balioa** zutabea.

### <a name="template-mapping-in-data-integration"></a>Datuen integrazioan txantiloien mapaketa

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du. Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Txantiloien mapaketa](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)

## <a name="project-expense-estimates"></a>Proiektuaren gastuen aurreikuspenak

### <a name="template-and-tasks"></a>Txantiloia eta zereginak

Ondorengo txantiloia eta azpiko zereginak proiektuaren gastuen kalkuluak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:

- **Datuen integrazioko txantiloiaren izena:** Proiektuaren gastuen kalkuluak (PSA Fin eta Ops)
- **Proiektuko zereginaren izena:**

    - Transakzio-harremanak 
    - Expense estimates

### <a name="entity-set"></a>Entitate multzoaren

| Project Service Automation | Finantzak                                                  |
|----------------------------|----------------------------------------------------------|
| Transakzio-konexioak    | Proiektuen transakzio harremanetarako integrazio entitatea |
| Aurreikuspenen lerroak             | Integrazio entitatea proiektuaren gastuen kalkuluen arabera         |

### <a name="entity-flow"></a>Entitate fluxua

Proiektuaren gastuen kalkuluak Project Service Automation-en kudeatzen dira eta Finantzarekin sinkronizatzen dira proiektuaren gastuen iragarpen gisa.

### <a name="prerequisites"></a>Aurrebaldintzak

Proiektuaren gastuen kalkuluen sinkronizazioa gertatu aurretik, proiektuak, proiektuaren zereginak eta proiektuaren gastuen transakzio kategoriak sinkronizatu behar dituzu.

### <a name="power-query"></a>Power Query

Proiektuaren gastuen kalkuluen txantiloian, Power Query erabili behar duzu hurrengo zeregin hauek burutzeko:

- Iragazi gastuen kalkuluen lerro erregistroak soilik sartzeko.
- Ezarri integrazioak ordu iragarpen berriak sortzen dituenean erabiliko den iragarpen eredu lehenetsia.
- Eraldatu fakturazio motak.
- Eraldatu transakzio motak.

#### <a name="filter-to-include-only-expense-estimate-lines"></a>Iragazi gastuen kalkuluen lerroak soilik sartzeko

Proiektuaren gastuen kalkuluak (PSA to Fin eta Ops) txantiloiak iragazki lehenetsia du, eta integrazioan gastu lerroak bakarrik biltzen ditu. Zure txantiloia sortzen baduzu, iragazki hau gehitu behar duzu. Aukeratu **Transakzio harremanak** zereginaren gainean eta egin klik **Mapa** gezia mapa irekitzeko. Hautatu **Kontsulta eta iragazki aurreratuak** esteka. Iragazi **msdyn\_transakzio mota1** zutabea soilik barne izan dezan **msdyn\_estimateline**.

#### <a name="set-the-default-forecast-model-id"></a>Ezarri iragarpen eredu lehenetsiaren IDa

Eguneratu lehenetsitako iragarritako ereduaren ID txantiloian, hautatu **Gastuaren balioztatzea** zeregina, eta gero klik egin **Mapa** gezitu irekiz jarraipena. Hautatu **Kontsulta eta iragazki aurreratuak** esteka.

- Proiektuaren gastu-estimazio lehenetsiak (PSA to Fin eta Ops) txantiloia erabiltzen ari bazara Power Query-n, hautatu lehen **Txertatutako baldintza** hurrengotik **Urrats Aplikatuak** sekzioa. **Funtzioa** sarrera, ordeztu **O\_iragarpena** integrazioarekin batera erabili behar den aurreikuspen ereduaren IDaren izenarekin. Txantiloi lehenetsiak iragarpen eredu IDa du demo datuetatik.
- Txantiloi berria sortzen ari bazara, zutabe hau gehitu behar duzu. Power Query atalean, hautatu **Gehitu baldintzazko zutabea**, eta idatzi zutabe berriaren izena, adibidez **ID eredua**. Idatzi zutabearen baldintza. Balioztatze-lerroaren ID-a nulua ez bada, orduan \<idatzi iragarpen ereduaren IDa\>; bestela nulua.

#### <a name="transform-the-billing-types"></a>Eraldatu fakturazio motak

Proiektuaren gastuen kalkuluak (PSA to Fin eta Ops) txantiloiak integrazio garaian Project Service Automation-etik jasotzen diren fakturazio motak eraldatzeko erabiltzen den baldintzazko zutabe bat dauka. Zure txantiloia sortzen baduzu, baldintzazko zutabearen hau gehitu behar duzu. Aukeratu **Kontsulta eta iragazki aurreratuak** estekatu eta hautatu **Gehitu baldintzazko zutabea**. Idatzi zutabe berriaren izena, adibidez **Fakturazio mota**. Orduan idatzi hurrengo baldintza:

Bada **msdyn\_fakturazio mota** = 192350000, orduan **Kargagabea**  
Edozer gauza bada **msdyn\_fakturazio mota** = 192350001, orduan **Kargagarria**  
Edozer gauza bada **msdyn\_fakturazio mota** = 192350002, orduan **Osagarria**  
Bestela **Ez dago erabilgarri**

#### <a name="transform-the-transaction-types"></a>Eraldatu transakzio motak

Proiektuaren gastuen kalkuluak (PSA to Fin eta Ops) txantiloiak integrazio garaian Project Service Automation-etik jasotzen diren transakzio motak eraldatzeko erabiltzen den baldintzazko zutabe bat dauka. Zure txantiloia sortzen baduzu, baldintzazko zutabearen hau gehitu behar duzu. Aukeratu **Kontsulta eta iragazki aurreratuak** estekatu eta hautatu **Gehitu baldintzazko zutabea**. Idatzi zutabe berriaren izena, adibidez **TransakzioMota**. Orduan idatzi hurrengo baldintza:

Bada **msdyn\_transakzio mota** = 192350000, orduan **Kostua**  
Beste edozein bada **msdyn\_transakzio mota** = 192350005, orduan **Salmentak**  
Bestela **nulua**

### <a name="template-mapping-in-data-integration"></a>Datuen integrazioan txantiloien mapaketa

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du. Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Txantiloien mapaketa](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)

[![Txantiloien mapaketa](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)
