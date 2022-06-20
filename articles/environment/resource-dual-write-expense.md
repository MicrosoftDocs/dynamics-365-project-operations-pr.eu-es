---
title: Gastu-kudeaketaren integrazioa
description: Artikulu honek gastu-txostenen integrazioari buruzko informazioa eskaintzen du Project Operations-en idazketa bikoitza erabiliz.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: c64c318dc1915a9a87b6ae3c6b8a2aa6d3c9cd36
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8924599"
---
# <a name="expense-management-integration"></a>Gastu-kudeaketaren integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honek gastu-txostenen integrazioari buruzko informazioa eskaintzen du Proiektu Eragiketetan [gastuen hedapen osoa](../expense/expense-overview.md) idazkera bikoitza erabiliz.

## <a name="expense-categories"></a>Gastu-kategoriak

Gastuen hedapen oso batean, gastu-kategoriak sortu eta mantentzen dira Finantza eta Operazioen aplikazioetan. Gastu-kategoria berria sortzeko, jarraitu urrats hauek:

1. Microsoft Dataverse-n, sortu **Transakzioa** kategoria. Idazketa bikoitzeko integrazioak transakzio-kategoria hau Finantza eta Operazioen aplikazioekin sinkronizatuko du. Informazio gehiagorako, ikusi [Konfiguratu proiektuen kategoriak](/dynamics365/project-operations/project-accounting/configure-project-categories) eta [Project Operations konfiguratzeko eta konfiguratzeko datuen integrazioa](resource-dual-write-setup-integration.md). Integrazio horren ondorioz, sistemak partekatutako lau kategoria-erregistro sortzen ditu Finantza eta Operazioen aplikazioetan.
2. Finantzetan, joan **Gastuen kudeaketa** > **Konfigurazioa** > **Kategoria partekatuak** eta hautatu partekatutako kategoria bat **Gastua** transakzio klasea. Ezarri **Gastuetan erabil daiteke** parametroa **Egia** eta zehaztu erabili beharreko gastu mota.
3. Partekatutako kategoria erregistro hau erabiliz, sortu gastuen kategoria berri bat joan **Gastuen kudeaketa** > **Konfigurazioa** > **Gastu kategoriak** aukerara eta hautatu **Berria**. Erregistroa gordetzen denean, idazketa bikoitzak taula mapa erabiltzen du, **Project Operations integratzeko proiektuaren gastuen kategoriak esportazio entitatea (msdyn\_gastu-kategoriak)** erregistro hau sinkronizatzeko Dataverse-ra.

  ![Gastu-kategorien integrazioa.](./media/DW6ExpenseCategories.png)

Finantza eta Operazioen aplikazioetako gastu-kategoriak enpresaren edo entitate juridikoen espezifikoak dira. Pertsona juridiko bakoitzari dagozkion erregistro bereiziak daude Dataverse-n. Proiektu kudeatzaile batek gastuak kalkulatzen dituenean, ezin ditu aukeratu lantzen ari diren proiektuaren jabea den beste enpresa batena den proiektu baterako sortutako gastu kategoriak. 

## <a name="expense-reports"></a>Gastuen txostenak

Gastuen txostenak Finantza eta Operazioen aplikazioetan sortzen eta onartzen dira. Informazio gehiagorako, ikusi [Sortu eta prozesatu gastuen txostenak Dynamics 365 Project Operations-en](/learn/modules/create-process-expense-reports/). Proiektuaren kudeatzaileak gastuen txostena onartu ondoren, liburu nagusian argitaratuko da. Project Operations-en, proiektuari lotutako gastu-txostenen lerroak argitaratzeko arau bereziak erabiliz argitaratzen dira:

  - Proiektuarekin lotutako kostua (berreskuraezina den zerga barne) ez da berehala kontabilitate proiektuan liburu nagusian kontabilizatzen, gastuen integrazio kontura baizik. **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** aukeran dago konfiguratuta kontua, **Dynamics 365 Customer Engagement-en Project Operations** fitxan.
  - Idazketa bikoitza sinkronizatzen du Dataverse-ra **Project Operations integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn\_expenses)** taulako mapa erabiliz.
  - Zerga azpiegitura, saltzailearen azpiegitura eta bestelako finantza bidalketak aplikagarri gisa erregistratzen dira gastuen txostenak argitaratzean.

  ![Gastu-txostenen integrazioa.](./media/DW6ExpenseReports.png)

Diskoan idazten denean **Gastua** entitatea Dataverse-n, sistemak erregistroaren onarpen prozesu automatizatua abiarazten du. Behar izanez gero, onartutako prozesuen egoera automatikoa berrikusi daiteke Dataverse-n, **Ezarpen aurreratuak** > **Sistema** > **Sistemako lanak** aukerara joanda. Onarpena amaitu ondoren, gastuen transakzio motaren erregistroak sortzen dira **Benetako datuak** entitatean.

Gastuekin lotutako errealitateak idazketa bikoitzeko taulako mapa erabiliz prozesatzen dira, **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)**. Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md).

Aldizkako prozesua, **Inportatu eszenaratzetik** Gastuen txostenarekin lotutako aldizkari-lerroak sortzen ditu Project Operations-en integrazioko egunkarian. Desplazatutako kontuak lehenespenez gastuen integrazio kontua. Argitalpenen integrazio-egunkariak gastuen transakzioaren kontuaren balantzea garbitzen du eta gastuaren zenbatekoa proiektuaren kostuaren kontura eramaten du. Sistemak, gainera, proiektuen azpiegituren transakzioak sortzen ditu fakturazio eta diru-sarrerak ezagutzeko helburuetarako.
