---
title: Sinkronizatu proiektuaren benetako datuak zuzenean Project Service Automation-etik proiektuaren integrazio aldizkarira finantza eta eragiketetan argitaratzeko
description: Artikulu honek proiektuaren benetakoak zuzenean sinkronizatzeko erabiltzen diren txantiloiak eta azpiko zereginak deskribatzen ditu Microsoft Dynamics 365 Project Service Automation finantzaketari eta eragiketei.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 34a0a0f7277777895077d221cd95e8d962d2a902
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028963"
---
# <a name="synchronize-project-actuals-directly-from-project-service-automation-to-the-project-integration-journal-for-posting-in-finance-and-operations"></a>Sinkronizatu proiektuaren benetako datuak zuzenean Project Service Automation-etik proiektuaren integrazio aldizkarira finantza eta eragiketetan argitaratzeko

[!include[banner](../includes/banner.md)]

Artikulu honek proiektuaren benetakoak zuzenean sinkronizatzeko erabiltzen diren txantiloiak eta azpiko zereginak deskribatzen ditu Dynamics 365 Project Service Automation to Dynamics 365 Finance.

Txantiloiak Project Service Automation-etik egindako transakzioak sinkronizatzen ditu Finantzetan. Sinkronizazioa amaitu ondoren, zuk **behar** inportatu datuak taulako taulako integrazio aldizkarian.

> [!NOTE]
> - Proiektuaren integrazioa eskuragarri dago 8.0.1 bertsioan hasita.
> - KB 4132657 eta KB 4132660 instalatu ondoren Enterprise edition 7.3.0 erabiltzen ari bazara, txantiloiak erabil ditzakezu proiektuaren zereginak, gastuen transakzioen kategoriak, orduen kalkuluak, gastuen kalkuluak eta benetakoak konfiguratzeko eta konfiguratzeko. funtzionalitate blokeoa. Kontabilitate banaketak berrezarri behar badituzu, KB 4131710 ere instalatzea gomendatzen dizugu.
> - 7.3.0 bertsioa erabiltzen ari bazara eta Project Service Automation-etik kuoten transakzioak ekartzen badituzu, KB 4345320 instalatu behar duzu tasak proiektuaren fakturan sartzeko.
> - Salmenten gaineko zergaren zenbatekoak denboran edo gastuen transakzioetan sartzen ari bazara Project Service Automation zerbitzuan, Project Service Automation Update 7 instalatu behar duzu. Bestela, zerga-datuak ez dira lotuta dauden denbora edo gastuen fakturekin lotuko eta ez dira Finantzarekin sinkronizatuko. Informazio gehiagorako, kontaktatu Laguntza.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation Finantzararen datu-fluxua

Project Service Automation to Finance integrazio irtenbideak Datu integrazio funtzioa erabiltzen du datuak Project Service Automation eta Finance-ren instantzia guztietan sinkronizatzeko. Datuak integratzeko funtzioarekin eskuragarri dauden integrazio txantiloiek proiektuaren uneko inguruko datuen fluxua ahalbidetzen dute Project Service Automation-etik Finantzara.

Ondorengo ilustrazioak erakusten du nola sinkronizatzen diren datuak Project Service Automation eta Finance artean.

[![Project Service Automation finantza eta eragiketekin integratzeko datu-fluxua.](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)

## <a name="project-actuals-from-project-service-automation"></a>Proiektuaren unekoa hurrengotik Project Service Automation

### <a name="template-and-tasks"></a>Txantiloia eta zereginak

Eskuragarri dauden txantiloietara sartzeko, Microsoft Power Apps administratzaile zentroa, hautatu **Proiektuak** eta, ondoren, goiko eskuineko izkinan, hautatu **Proiektu berria** txantiloi publikoak hautatzeko.

Ondorengo txantiloia eta azpiko zereginak proiektuaren uneko Project Service Automation-etik Finantzara sinkronizatzeko erabiltzen dira:

- **Datuen integrazioko txantiloiaren izena:** Proiektuaren unekoak (PSA Fin eta Ops)
- **Proiektuko zereginaren izena:**

    - Datu bateratuak
    - TransactionConnections

### <a name="entity-set"></a>Entitate multzoaren

| Project Service Automation | Finantzak                                   |
|----------------------------|----------------------------------------------------------|
| Datu bateratuak                    | Proiektuaren benetako integrazio entitatea                   |
| Transakzio-konexioak    | Proiektuen transakzio harremanetarako integrazio entitatea |

### <a name="entity-flow"></a>Entitate fluxua

Proiektuaren unekoak kudeatuta dago Project Service Automation-en, eta sinkronizatuta daude proiektu-integrazioaren agendara Finantzan. Kontabilitatea lehenetsitako finantza dimentsioen eta kontabilitate konfigurazioaren arabera aplikatuko da.

### <a name="prerequisites"></a>Aurrebaldintzak

Egiazkoen sinkronizazioa gertatu aurretik, Project Service Automation integrazio parametroak konfiguratu behar dituzu eta proiektuak, proiektuaren zereginak eta proiektuaren gastuen transakzio kategoriak sinkronizatu behar dituzu.

### <a name="power-query"></a>Power Query

Proiektuaren benetako txantiloian, Microsoft erabili behar duzu Power Query Excel-ek zeregin hauek bete ditzan:

- Eraldatu Project Service Automation-eko transakzio mota Finantza-ko transakzio mota egokira. Transformazio hau dagoeneko definituta dago Project actuals (PSA to Fin eta Ops) txantiloian.
- Eraldatu Project Service Automation-eko fakturazio mota Finantza-ko fakturazio mota egokira. Transformazio hau dagoeneko definituta dago Project actuals (PSA to Fin eta Ops) txantiloian. Fakturazio mota lerroaren propietatera mapatzen da, fitxategiaren konfigurazioan oinarrituta **Project Service Automation integrazio parametroak** orrialdea.
- Iragazi txantiloi honekin sinkronizatu behar diren baliabideen antolaketa unitate zehatzetara.
- Enpresen arteko denbora edo konpainien arteko gastuak Finantzarekin sinkronizatuko badira, kontratuaren antolakuntza unitatea Finantzako entitate juridiko egokira bihurtu beharko duzu. Project actuals (PSA to Fin and Ops) txantiloian, baldintzazko zutabe bat definitzen da demo datuetan oinarrituta. Txertatutako azken baldintzazko zutabea pertsona juridiko zuzenei eguneratu behar diezu. Bestela, integrazio errore bat gerta liteke edo benetako transakzio okerrak Finantzara inporta litezke.
- Enpresen arteko denbora edo konpainien arteko gastuak ez badira Finantzarekin sinkronizatuko, txertatutako azken baldintzazko zutabea ezabatu behar duzu zure txantiloitik. Bestela, integrazio errore bat gerta liteke edo benetako transakzio okerrak Finantzara inporta litezke.

#### <a name="contract-organizational-unit"></a>Kontratatu antolakuntzaren unitatea
Eguneratzeko txertatutako baldintzaren zutabea txantiloian, klik egin **Mapa** gezia mapa irekitzeko. Hautatu **Kontsulta eta Iragazte Aurreratuak** irekitzeko esteka Power Query.

- Proiektuaren benetako (PSA to Fin eta Ops) txantiloi lehenetsia erabiltzen ari bazara, sartu Power Query, hautatu azkena **Baldintza txertatua** tik **Aplikaturiko Urratsak** atala. Hurrengoan **Funtzioa** sarrera, ordezkatu **USSI** legezko entitatearen izenarekin, zeina erabili behar den integrazioarekin. Gehitu baldintza gehigarriak **Funtzioa** sarrera behar duzun moduan eta eguneratu **bestela** baldintza batetik **USMF** pertsona juridiko zuzenari.
- Txantiloi berri bat sortzen ari bazara, enpresen arteko denbora eta gastuak laguntzeko zutabea gehitu behar duzu. Hautatu **Gehitu baldintzazko zutabea**, eta idatzi zutabearen izena, esaterako **LegalEntity**. Idatzi zutabearen baldintza. **msdyn\_contractorganizationalunitid.msdyn\_name** \<organizational unit\> bada, orduan, \<enter the legal entity\>; bestela nulua.

### <a name="template-mapping-in-data-integration"></a>Datuen integrazioan txantiloien mapaketa

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du. Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Txantiloien mapaketa - Egiazko datuak.](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)

[![Txantiloien mapaketa - Transakzioen konexioak.](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)

## <a name="import-from-staging-table-after-integration-from-project-service-automation"></a>Inportatu etapako taulatik integratu ondoren Project Service Automation-etik

Inportazioa taulen taularen aldian aldiko prozesua gauzatu behar da Project Service Automation Finantzara eguneratutakoen sinkronizazioaren ondoren. Prozesu honek proiektuaren transakzioak faseko taulatik inportatuko ditu Project Service Automation integrazio aldizkarian, eta bertan kontabilitatea aplikatu eta inportatutako transakzioak argitaratu ahal izango dira. Prozesu hau batch moduan exekutatzea gomendatzen dizugu; aukeran konfiguratu daiteke errepikatzen den sorta gisa exekutatzeko.

## <a name="update-actuals-from-finance"></a>Eguneratu Ogasuneko datuak

### <a name="template-and-tasks"></a>Txantiloia eta zereginak

Ondorengo txantiloia eta azpiko zereginak bonoaren zenbakia eta salmenten gaineko zergak sinkronizatzeko erabiltzen dira argitaratutako proiektuen transakzioetarako Finantzetatik Project Service Automation-era:

- **Datuen integrazioko txantiloiaren izena:** Proiektuaren unekoak eguneratzea (PSA Fin Ops)
- **Proiektuko zereginaren izena:**

    - Datu bateratuak 
    - TransactionConnections

### <a name="entity-set"></a>Entitate multzoaren

| Finantzak                                                  | Project Service Automation |
|----------------------------------------------------------|----------------------------|
| Proiektuaren benetako integrazio entitatea                   | Datu bateratuak                    |
| Proiektuen transakzio harremanetarako integrazio entitatea | Transakzio-konexioak    |

### <a name="entity-flow"></a>Entitate fluxua

Proiektuaren unekoak kudeatuta dago Project Service Automation-en, eta sinkronizatuta daude proiektu-integrazioaren agendara Finantzan. Eguneratzeak Finantzan argitaratu ondoren, Project Service Automation eguneratuko dira Finantzaren bonuaren zenbakiarekin. Salmenten gaineko zergak gehitzen badira Finantzan, zerga-faktore berriak sortzen dira Project Service Automation-en.

### <a name="power-query"></a>Power Query

Proiektuaren benetako eguneratze txantiloian, erabili behar duzu Power Query zeregin hauek burutzeko:

- Eraldatu Project Service Automation-eko transakzio mota transakzio mota egokira Project Service Automation. Transformazio hau dagoeneko definituta dago Project actuals eguneratzea (PSA Fin eta Ops) txantiloian.
- Eraldatu fakturazio-mota Finantzan hurrengo fakturazio-mota zuzenera Project Service Automation. Transformazio hau dagoeneko definituta dago Project actuals eguneratzea (PSA Fin eta Ops) txantiloian.

### <a name="template-mapping-in-data-integration"></a>Datuen integrazioan txantiloien mapaketa

Ondorengo ilustrazioak Datuen integrazioan txantiloien atazen maparen adibide bat erakusten du. Kartografiak Project Service Automation-etik Finantzara sinkronizatuko den eremuko informazioa erakusten du.

[![Txantiloien mapaketa - Egiazko datuen eguneratzea.](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)

[![Txantiloien mapaketa - Transakzioen eguneratzea.](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]