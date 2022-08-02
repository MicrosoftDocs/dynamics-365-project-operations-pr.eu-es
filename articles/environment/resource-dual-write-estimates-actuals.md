---
title: Proiektuaren kalkuluak eta benetako dauten integrazioa
description: Artikulu honek Project Operations-en idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du proiektuaren estimazioetarako eta benetako datuetarako.
author: sigitac
ms.date: 4/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: dc8f65aec6f2328ccef5f9591a0f4d9c792b0d8f
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029065"
---
# <a name="project-estimates-and-actuals-integration"></a>Proiektuaren kalkuluak eta benetako dauten integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honek Project Operations-en idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du proiektuaren estimazioetarako eta benetako datuetarako.

## <a name="project-estimates"></a>Proiektuaren aurreikuspenak

Proiektuaren eskulana, gastua eta materialaren estimazioak sortu eta mantentzen dira Microsoft Dataverse eta finantza- eta eragiketa-aplikazioekin sinkronizatuta kontabilitate-helburuetarako. Sortu, eguneratu eta ezabatu eragiketak ez dira onartzen finantza eta eragiketen aplikazioen bidez.

Aurrekontuak sortzeko proiektuak baliozko kontabilitate konfigurazioa behar du. Kontratu-lerroekin lotzen diren proiektuek proiektuaren kostu eta diru-sarreren profila baliozkoa izan behar dute Proiektuaren kostu eta diru-sarreren profileko arauetan zehaztuta. Informazio gehiagorako, ikusi [Konfiguratu fakturagarriak diren proiektuen kontabilitatea](../project-accounting/configure-accounting-billable-projects.md#configure-project-cost-and-revenue-profile-rules).

## <a name="labor-estimates"></a>Lan-kalkuluak

Lan-kalkuluak proiektuaren kudeatzaileak edo baliabideen kudeatzaileak sortzen ditu, eta proiektuaren zereginari baliabide generiko edo izendatutako bat ere esleitzen dio. Baliabideak esleitzeko erregistroak **Baliabideen esleipena** fitxan **Proiektuaren xehetasunak** orrialdea Dataverse-n. Baliabideak esleitzeko erregistroak Dataverse sortu ordu-iragarpen-erregistroak finantza- eta eragiketa-aplikazioetan erabiliz **Project Operations integrazio entitatea orduen estimazioetarako (msdyn\_ baliabideen esleipena)**.

   ![Lanak integrazioa kalkulatzen du.](./Media/DW4LaborEstimates.png)

Idazketa bikoitzak baliabideak esleitzeko erregistroak taulako taularekin sinkronizatzen ditu (**ProjCDSEstimateHoursImport**), eta gero negozioaren logika erabiltzen du orduen iragarpen erregistroak sortzeko eta eguneratzeko (**ProjForecastEmpl**).

Proiektuko kontu-hartzaileak finantza- eta eragiketa-aplikazioetan sortutako ordu-erregistroak berrikusten ditu hona joanez **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Plana** > **Ordu-iragarpenak**.

## <a name="expense-estimates"></a>Expense estimates

Gastuen kalkuluak proiektuaren kudeatzaileak sortzen ditu **Gastuen aurrekontuak** fitxan **Proiektuaren xehetasunak** orrialdea Dataverse-n. Gastuen aurrekontuen erregistroak biltegian gordetzen dira **Kalkuluaren lerroa** entitatea Dataverse-n. Estimazio-erregistro hauek transakzio klasea dute, **Gastua** eta finantza- eta operazio-aplikazioetan gastu-aurreikuspenen erregistroekin sinkronizatuta daude **Project Operations integratzeko entitatea gastuen estimazioetarako (msdyn\_ estimazio-lerroak)**.

   ![Gastuen kalkuluen integrazioa.](./Media/DW4ExpenseEstimates.png)

Idazketa bikoitzak baliabideak esleitzeko erregistroak taulako taularekin sinkronizatzen ditu **(ProjCDSEstimateExpenseImport)**, eta gero negozioaren logika erabiltzen du gastuen iragarpen erregistroak sortzeko eta eguneratzeko (**ProjForecastCost**). Lerroen kalkuluen arabera, salmenten estimazioa eta kostuen kalkuluak bereizita gordetzen dira. Finantza- eta eragiketa-aplikazioetako negozio-logikak Gastuen iragarpen-erregistro bakar bat betetzen du antolakuntza-taulan dagoen xehetasun hau erabiliz.

Proiektuko kontu-hartzaileak finantza- eta eragiketa-aplikazioetako gastu-aurreikuspenen erregistroak berrikus ditzake hona joanda **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Plana** > **Gastuen aurreikuspenak**.

## <a name="material-estimates"></a>Materialaren aurreikuspenak

Materialen kalkuluak proiektuaren kudeatzaileak sortzen ditu **Materialaren aurrekontuak** fitxan **Proiektuaren xehetasunak** orrialdea Dataverse-n. Materialen aurrekontuen erregistroak biltegian gordetzen dira **Kalkuluaren lerroa** entitatea Dataverse-n. Estimazio-erregistro hauek transakzio-klasea dute, **Materiala** eta elementuen iragarpen-erregistroekin sinkronizatzen dira finantza- eta eragiketa-aplikazioetan erabiliz **Materialen estimazioetarako proiektuaren integrazio taula (msdyn\_ estimazio-lerroak)**.

   ![Materialen kalkuluen integrazioa.](./Media/DW4MaterialEstimates.png)

Idazketa bikoitzak baliabideak esleitzeko erregistroak taulako taularekin sinkronizatzen ditu **ProjForecastSalesImpor**, eta gero negozioaren logika erabiltzen du elementuen iragarpen erregistroak sortzeko eta eguneratzeko (**ForecastSales**). Lerroen kalkuluen arabera, salmenten estimazioa eta kostuen kalkuluak bereizita gordetzen dira. Finantza- eta eragiketa-aplikazioetako negozio-logikak elementuen iragarpen-erregistro bakar bat betetzen du antolakuntza-taulan dagoen xehetasun hau erabiliz.

Proiektuko kontu-hartzaileak finantza- eta eragiketen aplikazioetako elementuen aurreikuspen-erregistroak berrikus ditzake hona joanez **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Plana** > **Elementuen aurreikuspenak**.

## <a name="project-actuals"></a>Proiektuaren benetako datuak

Proiektuaren errealitatea urtean sortzen da Dataverse-n, denbora, gastu, material eta fakturazio jardueran oinarrituta. Transakzio horien atributu operatibo guztiak, zenbatekoa, kostuaren prezioa, salmenta prezioa eta proiektua barne hartzen dira Dataverse entitate honetan. Informazio gehiago lortzeko, ikusi [Benetako datuak](../actuals/actuals-overview.md). Benetako erregistroak finantza eta eragiketen aplikazioekin sinkronizatzen dira idazketa bikoitzeko taularen mapa erabiliz **Project Operations integrazio errealak (msdyn\_ benetakoak)** beheranzko kontabilitatearako.

   ![Benetako datuen integrazioa.](./Media/DW4Actuals.png)

**Project Operations integratzeko datuak** taulako mapak erregistro guztiak sinkronizatzen ditu **Benetako datuak** entitatea Dataverse-n, atributuarekin **Saltatu sinkronizazioa (barne erabileran soilik)** ezarri **Gezurra** gisa. Atributuaren balio hau ezarrita dago Dataverse-n erregistroa sortzen denean automatikoki. Atributu hau ezarrita dagoen adibideak **Egia** dira:

  - Enpresen arteko transakzioen proiektuaren kostua. Informazio gehiagorako, ikusi [Enpresen arteko transakzioak sortu](../project-accounting/create-intercompany-transactions.md). Erregistro hauek saltatzen dira, sistemak finantza- eta operazio-aplikazioetan proiektuaren benetako kostua birsortzen duelako enpresa arteko hornitzaileen faktura argitaratzen denean.
  - Proforma faktura berresten denean sortutako fakturazio gabeko salmenten erregistro negatiboak. Erregistro hauek saltatu egiten dira finantza- eta eragiketa-aplikazioetako proiektuaren azpiliburuak ez duelako fakturatu gabeko salmenta-erregistroa alderantzikatzen fakturazioan, baina egoera guztiz fakturatuta uzten duelako.

Idazketa bikoitzeko taula mapak benetako erregistroak taulako taularekin sinkronizatzen ditu, **ProjCDSActualsImport**. Erregistro horiek aldian aldiko prozesuaren bidez prozesatzen dira **Inportatu taulako taulatik** Project Operations integrazio egunkari lerroak eta proiektuen faktura proposamen lerroak sortzerakoan. Informazio gehiagorako, ikusi [Integrazio aldizkaria Project Operations-en](../project-accounting/project-operations-integration-journal.md).

Dataverse proiektuan benetako transakzioen arteko loturak ere jasotzen ditu **Transakzio konexioa** entitatea. Informazio gehiagorako, ikusi [Lotu errealak jatorrizko erregistroekin](../actuals/linkingactuals.md). Benetako transakzioen arteko loturak finantza eta eragiketa aplikazioekin ere sinkronizatzen dira idazketa bikoitzeko taularen mapa erabiliz, **Proiektuaren transakzio harremanetarako integrazio entitatea (msdyn\_ transakzio-konexioak)**. Erregistro horiek aldian aldiko prozesuaren bidez erabiltzen dira **Inportatu taulako taulatik** Project Operations integrazio egunkari lerroak eta proiektuen faktura proposamen lerroak sortzerakoan.

Project Operations integrazio aldizkaria eta proiektuaren faktura proposamenak bidaltzeak eguneratze bat eragiten du taulako erregistroetan, **ProjCDSActualsImport**. Sistemak kontabilitate atributu hauek harrapatzen eta erregistratzen ditu benetako transakzioetarako:

- Kontabilitatearen monetaren zenbatekoa
- Kanbio-tasa
- Kupoiaren zenbakia
- Salmenten zergen zenbatekoa

**Project Operations integratzeko datuak** taulako mapak dagozkion benetako erregistroak eguneratzen ditu Dataverse informazio horrekin.
