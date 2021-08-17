---
title: Gastu-kudeaketaren integrazioa
description: Gai honek idazketa dualeko Project Operations-en gastuen txosten-integrazioari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 06471532d2e41bb80ebf92f0a8b93c324b3f6d3e845cea8033d85d291ea237eb
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986566"
---
# <a name="expense-management-integration"></a>Gastu-kudeaketaren integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek idazketa dualeko Project Operations-en [gastu guztien inplementazioan](../expense/expense-overview.md) gastu-txostenen integrazioari buruzko informazioa eskaintzen du.

## <a name="expense-categories"></a>Gastu-kategoriak

Gastu osoaren hedapenean, gastuen kategoriak sortu eta mantentzen dira Finance and Operations aplikazioak. Gastu-kategoria berria sortzeko, jarraitu urrats hauek:

1. Microsoft Dataverse-n, sortu **Transakzioa** kategoria. Idazketa bikoitzeko integrazioak transakzio kategoria honekin sinkronizatuko du Finance and Operations aplikazioak. Informazio gehiagorako, ikusi [Konfiguratu proiektuen kategoriak](/dynamics365/project-operations/project-accounting/configure-project-categories) eta [Project Operations konfiguratzeko eta konfiguratzeko datuen integrazioa](resource-dual-write-setup-integration.md). Integrazio honen ondorioz, sistemak kategoria partekatuko lau erregistro sortzen ditu Finance and Operations aplikazioetan.
2. Finantzetan, joan **Gastuen kudeaketa** > **Konfigurazioa** > **Kategoria partekatuak** eta hautatu partekatutako kategoria bat **Gastua** transakzio klasea. Ezarri **Gastuetan erabil daiteke** parametroa **Egia** eta zehaztu erabili beharreko gastu mota.
3. Partekatutako kategoria erregistro hau erabiliz, sortu gastuen kategoria berri bat joan **Gastuen kudeaketa** > **Konfigurazioa** > **Gastu kategoriak** aukerara eta hautatu **Berria**. Erregistroa gordetzen denean, idazketa bikoitzak taula mapa erabiltzen du, **Project Operations integratzeko proiektuaren gastuen kategoriak esportazio entitatea (msdyn\_gastu-kategoriak)** erregistro hau sinkronizatzeko Dataverse-ra.

  ![Gastu-kategorien integrazioa.](./media/DW6ExpenseCategories.png)

Gastu kategoriak Finance and Operations aplikazioetan enpresa edo pertsona juridiko zehatzak dira. Pertsona juridiko bakoitzari dagozkion erregistro bereiziak daude Dataverse-n. Proiektu kudeatzaile batek gastuak kalkulatzen dituenean, ezin ditu aukeratu lantzen ari diren proiektuaren jabea den beste enpresa batena den proiektu baterako sortutako gastu kategoriak. 

## <a name="expense-reports"></a>Gastuen txostenak

Gastuen txostenak urtean sortu eta onartzen dira Finance and Operations aplikazioetan. Informazio gehiagorako, ikusi [Sortu eta prozesatu gastuen txostenak Dynamics 365 Project Operations-en](/learn/modules/create-process-expense-reports/). Proiektuaren kudeatzaileak gastuen txostena onartu ondoren, liburu nagusian argitaratuko da. Project Operations-en, proiektuari lotutako gastu-txostenen lerroak argitaratzeko arau bereziak erabiliz argitaratzen dira:

  - Proiektuarekin lotutako kostua (berreskuraezina den zerga barne) ez da berehala kontabilitate proiektuan liburu nagusian kontabilizatzen, gastuen integrazio kontura baizik. **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** aukeran dago konfiguratuta kontua, **Dynamics 365 Customer Engagement-en Project Operations** fitxan.
  - Idazketa bikoitza sinkronizatzen du Dataverse-ra **Project Operations integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn\_expenses)** taulako mapa erabiliz.
  - Zerga azpiegitura, saltzailearen azpiegitura eta bestelako finantza bidalketak aplikagarri gisa erregistratzen dira gastuen txostenak argitaratzean.

  ![Gastu-txostenen integrazioa.](./media/DW6ExpenseReports.png)

Diskoan idazten denean **Gastua** entitatea Dataverse-n, sistemak erregistroaren onarpen prozesu automatizatua abiarazten du. Behar izanez gero, onartutako prozesuen egoera automatikoa berrikusi daiteke Dataverse-n, **Ezarpen aurreratuak** > **Sistema** > **Sistemako lanak** aukerara joanda. Onarpena amaitu ondoren, gastuen transakzio motaren erregistroak sortzen dira **Benetako datuak** entitatean.

Gastuekin lotutako errealitateak idazketa bikoitzeko taulako mapa erabiliz prozesatzen dira, **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)**. Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md).

Aldizkako prozesua, **Inportatu eszenaratzetik** Gastuen txostenarekin lotutako aldizkari-lerroak sortzen ditu Project Operations-en integrazioko egunkarian. Desplazatutako kontuak lehenespenez gastuen integrazio kontua. Argitalpenen integrazio-egunkariak gastuen transakzioaren kontuaren balantzea garbitzen du eta gastuaren zenbatekoa proiektuaren kostuaren kontura eramaten du. Sistemak, gainera, proiektuen azpiegituren transakzioak sortzen ditu fakturazio eta diru-sarrerak ezagutzeko helburuetarako.
