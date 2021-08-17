---
title: Proiektuaren kalkuluak eta benetako dauten integrazioa
description: Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du proiektuaren kalkuluak eta egiazkoak lortzeko.
author: sigitac
ms.date: 4/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c558ab1eb5070f6d1a2db06b630e8807cc67819f9bdd57c15ec346f484e04fe9
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "7006276"
---
# <a name="project-estimates-and-actuals-integration"></a>Proiektuaren kalkuluak eta benetako dauten integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du proiektuaren kalkuluak eta egiazkoak lortzeko.

## <a name="project-estimates"></a>Proiektuaren aurreikuspenak

Proiektuaren eskulanaren, gastuen eta materialen estimazioak urtean sortu eta mantentzen dira Microsoft Dataverse eta sinkronizatutako Finance and Operations aplikazioak kontabilitate helburuetarako. Sortu, eguneratu eta ezabatu eragiketak ez dira onartzen Finance and Operations aplikazioak.

Aurrekontuak sortzeko proiektuak baliozko kontabilitate konfigurazioa behar du. Kontratu-lerroekin lotzen diren proiektuek proiektuaren kostu eta diru-sarreren profila baliozkoa izan behar dute Proiektuaren kostu eta diru-sarreren profileko arauetan zehaztuta. Informazio gehiagorako, ikusi [Konfiguratu fakturagarriak diren proiektuen kontabilitatea](../project-accounting/configure-accounting-billable-projects.md#configure-project-cost-and-revenue-profile-rules).

## <a name="labor-estimates"></a>Lan-kalkuluak

Lan-kalkuluak proiektuaren kudeatzaileak edo baliabideen kudeatzaileak sortzen ditu, eta proiektuaren zereginari baliabide generiko edo izendatutako bat ere esleitzen dio. Baliabideak esleitzeko erregistroak **Baliabideen esleipena** fitxan **Proiektuaren xehetasunak** orrialdea Dataverse-n. Baliabideak esleitzeko erregistroak Dataverse-n sortu orduen iragarpen erregistroak Finance and Operations aplikazioetan **Project Operations integratzeko entitatea orduen kalkuluen arabera (msdyn\_resourceassigments)**.

   ![Lanak integrazioa kalkulatzen du.](./Media/DW4LaborEstimates.png)

Idazketa bikoitzak baliabideak esleitzeko erregistroak taulako taularekin sinkronizatzen ditu (**ProjCDSEstimateHoursImport**), eta gero negozioaren logika erabiltzen du orduen iragarpen erregistroak sortzeko eta eguneratzeko (**ProjForecastEmpl**).

Proiektuaren kontulariak urtean sortutako orduen erregistroak berrikusten ditu Finance and Operations aplikazioetan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Plana** > **Orduen iragarpenak** aukerara joanda.

## <a name="expense-estimates"></a>Expense estimates

Gastuen kalkuluak proiektuaren kudeatzaileak sortzen ditu **Gastuen aurrekontuak** fitxan **Proiektuaren xehetasunak** orrialdea Dataverse-n. Gastuen aurrekontuen erregistroak biltegian gordetzen dira **Kalkuluaren lerroa** entitatea Dataverse-n. Estimazio erregistro hauek transakzio klasea dute, **Gastua** eta sinkronizatuta daude gastuen aurreikuspenen erregistroekin Finance and Operations aplikazioetan **Project Operations integratzeko gastua kalkulatzeko (msdyn\_estimatelines)** erabiliz.

   ![Gastuen kalkuluen integrazioa.](./Media/DW4ExpenseEstimates.png)

Idazketa bikoitzak baliabideak esleitzeko erregistroak taulako taularekin sinkronizatzen ditu **(ProjCDSEstimateExpenseImport)**, eta gero negozioaren logika erabiltzen du gastuen iragarpen erregistroak sortzeko eta eguneratzeko (**ProjForecastCost**). Lerroen kalkuluen arabera, salmenten estimazioa eta kostuen kalkuluak bereizita gordetzen dira. Enpresa logika Finance and Operations aplikazioetan Gastuen iragarpenen erregistro bakarra betetzen dute xehetasun hori taularen taulan.

Proiektuaren kontulariak urtean sortutako gastuak berrikusten ditu Finance and Operations aplikazioetan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Plana** > **Gastuen iragarpenak** aukerara joanda.

## <a name="material-estimates"></a>Materialaren aurreikuspenak

Materialen kalkuluak proiektuaren kudeatzaileak sortzen ditu **Materialaren aurrekontuak** fitxan **Proiektuaren xehetasunak** orrialdea Dataverse-n. Materialen aurrekontuen erregistroak biltegian gordetzen dira **Kalkuluaren lerroa** entitatea Dataverse-n. Estimazio erregistro hauek transakzio klasea dute, **Materiala** eta sinkronizatuta daude elementuen aurreikuspenen erregistroekin Finance and Operations aplikazioetan **Project Operations integratzeko taula materialak kalkulatzeko (msdyn\_estimatelines)** erabiliz.

   ![Materialen kalkuluen integrazioa.](./Media/DW4MaterialEstimates.png)

Idazketa bikoitzak baliabideak esleitzeko erregistroak taulako taularekin sinkronizatzen ditu **ProjForecastSalesImpor**, eta gero negozioaren logika erabiltzen du elementuen iragarpen erregistroak sortzeko eta eguneratzeko (**ForecastSales**). Lerroen kalkuluen arabera, salmenten estimazioa eta kostuen kalkuluak bereizita gordetzen dira. Enpresa logika Finance and Operations aplikazioetan Elementuen iragarpenen erregistro bakarra betetzen dute xehetasun hori taularen taulan.

Proiektuaren kontulariak elementu kalkulu-erregistroak berrikusten ditu Finance and Operations aplikazioetan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Plana** > **Elementuen iragarpenak** aukerara joanda.

## <a name="project-actuals"></a>Proiektuaren benetako datuak

Proiektuaren errealitatea urtean sortzen da Dataverse-n, denbora, gastu, material eta fakturazio jardueran oinarrituta. Transakzio horien atributu operatibo guztiak, zenbatekoa, kostuaren prezioa, salmenta prezioa eta proiektua barne hartzen dira Dataverse entitate honetan. Informazio gehiago lortzeko, ikusi [Benetako datuak](../actuals/actuals-overview.md). Benetako erregistroak sinkronizatuta daude Finance and Operations aplikazioak idazketa bikoitzeko taulako mapa erabiliz **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)** kontabilitaterako.

   ![Benetako datuen integrazioa.](./Media/DW4Actuals.png)

**Project Operations integratzeko datuak** taulako mapak erregistro guztiak sinkronizatzen ditu **Benetako datuak** entitatea Dataverse-n, atributuarekin **Saltatu sinkronizazioa (barne erabileran soilik)** ezarri **Gezurra** gisa. Atributuaren balio hau ezarrita dago Dataverse-n erregistroa sortzen denean automatikoki. Atributu hau ezarrita dagoen adibideak **Egia** dira:

  - Enpresen arteko transakzioen proiektuaren kostua. Informazio gehiagorako, ikusi [Enpresen arteko transakzioak sortu](../project-accounting/create-intercompany-transactions.md). Erregistro hauek saltatu egiten dira, sistemak proiektuaren kostua benetako birsortzen duelako Finance and Operations aplikazioak enpresen arteko saltzailearen faktura argitaratzen denean.
  - Proforma faktura berresten denean sortutako fakturazio gabeko salmenten erregistro negatiboak. Erregistro hauek saltatu egiten dira, proiektuaren azpiegitura delako Finance and Operations aplikazioek ez dute fakturazioan fakturatutako salmenten erregistroa alderantzikatzen, baina egoera guztiz fakturatzen dute.

Idazketa bikoitzeko taula mapak benetako erregistroak taulako taularekin sinkronizatzen ditu, **ProjCDSActualsImport**. Erregistro horiek aldian aldiko prozesuaren bidez prozesatzen dira **Inportatu taulako taulatik** Project Operations integrazio egunkari lerroak eta proiektuen faktura proposamen lerroak sortzerakoan. Informazio gehiagorako, ikusi [Integrazio aldizkaria Project Operations-en](../project-accounting/project-operations-integration-journal.md).

Dataverse proiektuan benetako transakzioen arteko loturak ere jasotzen ditu **Transakzio konexioa** entitatea. Informazio gehiagorako, ikusi [Lotu errealak jatorrizko erregistroekin](../actuals/linkingactuals.md). Benetako transakzioen arteko loturak ere sinkronizatuta daude Finance and Operations idazketa bikoitzeko taulako mapa erabiltzen duten aplikazioak, **Proiektuaren transakzio harremanetarako integrazio entitatea (msdyn\_transactionconnections)**. Erregistro horiek aldian aldiko prozesuaren bidez erabiltzen dira **Inportatu taulako taulatik** Project Operations integrazio egunkari lerroak eta proiektuen faktura proposamen lerroak sortzerakoan.

Project Operations integrazio aldizkaria eta proiektuaren faktura proposamenak bidaltzeak eguneratze bat eragiten du taulako erregistroetan, **ProjCDSActualsImport**. Sistemak kontabilitate atributu hauek harrapatzen eta erregistratzen ditu benetako transakzioetarako:

- Kontabilitatearen monetaren zenbatekoa
- Kanbio-tasa
- Kupoiaren zenbakia
- Salmenten zergen zenbatekoa

**Project Operations integratzeko datuak** taulako mapak dagozkion benetako erregistroak eguneratzen ditu Dataverse informazio horrekin.
