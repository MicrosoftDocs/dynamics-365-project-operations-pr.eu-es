---
title: Sinkronizatu proiektuaren gastuen kategoriak Finance and Operations eta Project Service Automation
description: Gai honek deskribatzen du txantiloiak eta azpiko zereginak erabiliak direnak sinkronizatzeko proiektuaren gastuaren kategoriak Microsoft Dynamics 365 Finance eta Dynamics 365 Project Service Automation artean.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 52c79f8b641d4b2df3b30964331633f2487402f8f8d229b540f9544c0f848557
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7001101"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a>Sinkronizatu proiektuaren gastuen kategoriak Finance and Operations eta Project Service Automation

[!include[banner](../includes/banner.md)]

Gai honek deskribatzen du txantiloiak eta azpiko zereginak erabiliak direnak sinkronizatzeko proiektuaren gastuaren kategoriak Dynamics 365 Finance eta Dynamics 365 Project Service Automation artean.

> [!NOTE]
> - Proiektuaren zereginen integrazioa, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta funtzionalitate blokeoa eskuragarri daude 8.0 bertsioan.
> - Datu bateratuen integrazioa eskuragarri dago 8.0.1 bertsioan edo hurrengoan.
> - KB 4132657 eta KB 4132660 instalatu ondoren Enterprise edition 7.3.0 erabiltzen ari bazara, txantiloiak erabil ditzakezu proiektuaren zereginak, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta benetakoak konfiguratzeko eta konfiguratzeko funtzionalitate blokeoa. Kontabilitate banaketak berrezarri behar badituzu, KB 4131710 ere instalatzea gomendatzen dizugu.

## <a name="data-flow-for-project-service-automation-and-finance"></a>Project Service Automation eta Finantzararen datu-fluxua

Project Service Automation eta Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko. Integrazio txantiloiak eskuragarri daude Datu-integrazio eginbidearekin gaitzen du fluxuaren datuak proiektuaren gastuari buruz transakzio-kategoriak artean Finantza eta Project Service Automation.

Proiektuaren gastuen kategoriak Finantzan menderatzen badira, integrazio-fluxua lehenik Finantzetatik Project Service Automation-era da. Proiektuaren gastuen kategorien integrazio IDak eguneratzen dira sinkronizazioaren bidez, Project Service Automation-etik Finantzara.

Proiektuaren gastuen kategoriak Project Service Automation menderatzen badira, integrazio-fluxua lehenik Finantzetatik Project Service Automation-era Finantza da. Proiektuen kategoriak dagoeneko Finantzan konfiguratuta egon behar dira Project Service Automation-etik sinkronizatu aurretik. Ondoren, sinkronizatu Finantzatik Project Service Automation-era eta, ondoren, Project Service Automation-etik Finance-ra berriro. Horrela, kategoriak lotuta daudela eta bikoizturik sortuko ez dela bermatzen lagunduko duzu.

> [!NOTE]
> Normalean, proiektuaren gastuen kategoriak Finantzan menderatzen dira. Hala ere, hala ez bada edo Project Service Automation dagoeneko gastuen kategoriak sortu badira, lehenengo sinkronizatu behar duzu Proiektuaren gastuen transakzioen kategoriak (PSA Fin eta Ops) txantiloia erabiliz. Ondoren, sinkronizatu Proiektuaren gastuen transakzio kategoriak (Fin eta Ops PSA) txantiloia erabiliz. Project Service Automation Finantzara sinkronizazioa beste behin exekutatu beharko zenuke.
>
> Project Service Automation-etik lehen sinkronizatzen baduzu, baldintza hauek bete beharko dira Finantzan sinkronizazioa exekutatu aurretik:
>
> - Project Service Automation-en konfiguratutako proiektuaren kategoriarekin bat datorren kategoria partekatua existitu behar da eta bietarako gaituta egon behar du **Proiektua** eta **Gastua**.
> - Horrekin batera integratu behar den Finantza entitate juridiko bakoitzerako proiektuen kategoria hauek egon behar dira:
>
>     - **Proiektuaren kategoria** existitzen da. 
>     - **Erabilera Gastuan** gaituta dago.
>     - **Aktibo egunkarian** gaituta dago.
>     - **Transakzio mota** ezarrita dago **Gastua**.

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.

[![Project Service Automation Finantzarekin integratzeko datuen fluxua.](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a>Proiektuaren gastuaren kategoriaren sinkronizazioa hurrengotik Finantza hurrengora Project Service Automation

### <a name="template-and-task"></a>Txantiloia eta zeregina

Txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.

Ondorengo txantiloia eta azpiko zeregina proiektuaren gastuen kategoriak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:

- **Datuen integrazioko txantiloiaren izena:** Proiektuaren gastuen transakzioaren kategoriak (PSA Fin eta Ops)
- **Zereginaren izena proiektuan:** Sinkronizatu kategoriak PSArekin

### <a name="entity-set"></a>Entitate multzoaren

| Finantzak                           | Project Service Automation |
|-----------------------------------|----------------------------|
| Kategoriak datu-bateratuak integrazio entitatea | Transakzio-kategoriak     |

### <a name="entity-flow"></a>Entitate fluxua

Proiektuaren gastuen kategoriak Finantza-ren kudeatzen dira eta Project Service Automation sinkronizatzen dira transakzio-kategoriak gisa.

### <a name="power-query"></a>Power Query

Project Service Automation-ekin sinkronizatzen ari zarenean, Microsoft Power Query erabili behar duzu Excel-erako fakturazio transakzio kategorian ezartzeko. Proiektuaren gastuen transakzioen kategoriak (Fin eta Ops PSA) txantiloiak zutabe eta mapaketa lehenetsiak eskaintzen ditu. Zure txantiloia sortzen baduzu, baldintzazko zutabearen hau gehitu behar duzu Power Query. Jarraitu urrats hauei.

1. Egin klik gezian proiektuaren gastuen kategorien zereginaren mapaketa irekitzeko, Proiektuaren gastuen transakzioen kategoriak (Fin eta Ops to PSA) txantiloian.
2. Klik egin **Kontsulta eta iragazki aurreratuak** esteka irekitzeko Power Query.
2. Aukeratu **Gehitu baldintzazko zutabea**.
3. Idatzi zutabe berriaren izena, adibidez **Fakturazio mota**.
4. Idatzi baldintza hau: **CATEGORYID ez bada nulua bezainbeste 19235001, Bestela nulua**.
5. Klik egin **Ados** zutabean.
6. Ziurtatu mapen orrian zutabe berri hau mapeatzen.

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du. Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Proiektuaren gastuaren kategoria Project Service Automation txantiloiei esleitzea.](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a>Proiektuaren gastuaren kategoriaren sinkronizazioa hurrengotik Finantza hurrengora Project Service Automation

### <a name="template-and-task"></a>Txantiloia eta zeregina

Ondorengo txantiloia eta azpiko zeregina proiektuaren gastuen kategoriak Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:

- **Datuen integrazioko txantiloiaren izena:** Proiektuaren gastuen transakzioaren kategoriak (PSA Fin eta Ops)
- **Zereginaren izena proiektuan:** Sinkronizatu kategoriak Fin Ops

### <a name="entity-set"></a>Entitate multzoaren

| Project Service Automation | Finantzak                           |
|----------------------------|-----------------------------------|
| Transakzio-kategoriak     | Kategoriak datu-bateratuak integrazio entitatea |

### <a name="entity-flow"></a>Entitate fluxua

Proiektuaren gastuen kategoriak Finantza-ren kudeatzen dira eta Project Service Automation sinkronizatzen dira transakzio-kategoriak gisa. Sinkronizazioaren atzeko Finantza eguneratzeak proiektuaren kategoria Finantzan integrazioarekin ID-a hurrengoarekin Project Service Automation.

### <a name="template-mapping-in-data-integration"></a>Datuen integrazioan txantiloien mapaketa

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du.

> [!NOTE]
> Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Project Service Automation Finance txantiloiei esleitzea.](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]