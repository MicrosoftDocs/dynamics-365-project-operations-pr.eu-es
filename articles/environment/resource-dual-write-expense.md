---
title: Gastu-kudeaketaren integrazioa
description: Artikulu honek gastu-txostenen integrazioari buruzko informazioa eskaintzen du Project Operations-en idazketa bikoitza erabiliz.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: da37adcf63a10b9f245283d377e70fd08b3aa9c5
ms.sourcegitcommit: 385081ecc839d7d4a557eda2bb1578ca073f7e41
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/19/2022
ms.locfileid: "9527972"
---
# <a name="expense-management-integration"></a>Gastu-kudeaketaren integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honek gastu-txostenen integrazioari buruzko informazioa eskaintzen du Project Operations-en [gastuen hedapen osoa](../expense/expense-overview.md) idazkera bikoitza erabiliz.

## <a name="expense-categories"></a>Gastu-kategoriak

Gastuen hedapen oso batean, gastu-kategoriak finantza- eta operazio-aplikazioetan sortzen eta mantentzen dira. Gastu-kategoria berria sortzeko, jarraitu urrats hauek:

1. Microsoft Dataverse-n, sortu **Transakzioa** kategoria. Idazketa bikoitzeko integrazioak transakzio-kategoria hau finantza- eta eragiketa-aplikazioekin sinkronizatuko du. Informazio gehiagorako, ikusi [Konfiguratu proiektuen kategoriak](/dynamics365/project-operations/project-accounting/configure-project-categories) eta [Project Operations konfiguratzeko eta konfiguratzeko datuen integrazioa](resource-dual-write-setup-integration.md). Integrazio horren ondorioz, sistemak partekatutako lau kategoria-erregistro sortzen ditu finantza- eta operazio-aplikazioetan.
2. Finantzetan, joan **Gastuen kudeaketa** > **Konfigurazioa** > **Kategoria partekatuak** eta hautatu partekatutako kategoria bat **Gastua** transakzio klasea. Ezarri **Gastuetan erabil daiteke** parametroa **Egia** eta zehaztu erabili beharreko gastu mota.
3. Partekatutako kategoria erregistro hau erabiliz, sortu gastuen kategoria berri bat joan **Gastuen kudeaketa** > **Konfigurazioa** > **Gastu kategoriak** aukerara eta hautatu **Berria**. Erregistroa gordetzen denean, idazketa bikoitzak taula mapa erabiltzen du, **Project Operations integratzeko proiektuaren gastuen kategoriak esportazio entitatea (msdyn\_gastu-kategoriak)** erregistro hau sinkronizatzeko Dataverse-ra.

  ![Gastu-kategorien integrazioa.](./media/DW6ExpenseCategories.png)

Finantza- eta eragiketa-aplikazioetako gastu-kategoriak enpresaren edo entitate juridikoaren espezifikoak dira. Pertsona juridiko bakoitzari dagozkion erregistro bereiziak daude Dataverse-n. Proiektu kudeatzaile batek gastuak kalkulatzen dituenean, ezin ditu aukeratu lantzen ari diren proiektuaren jabea den beste enpresa batena den proiektu baterako sortutako gastu kategoriak. 

## <a name="expense-reports"></a>Gastuen txostenak

Gastuen txostenak finantza eta eragiketen aplikazioetan sortzen eta onartzen dira. Informazio gehiagorako, ikusi [Sortu eta prozesatu gastuen txostenak Dynamics 365 Project Operations-en](/training/modules/create-process-expense-reports/). Proiektuaren kudeatzaileak gastuen txostena onartu ondoren, liburu nagusian argitaratuko da. Project Operations-en, proiektuari lotutako gastu-txostenen lerroak argitaratzeko arau bereziak erabiliz argitaratzen dira:

  - Proiektuarekin lotutako kostua (berreskuraezina den zerga barne) ez da berehala kontabilitate proiektuan liburu nagusian kontabilizatzen, gastuen integrazio kontura baizik. **Proiektuen kudeaketa eta kontabilitatea** > **Konfigurazioa** > **Proiektuen kudeaketa eta kontabilitate parametroak** aukeran dago konfiguratuta kontua, **Dynamics 365 Customer Engagement-en Project Operations** fitxan.
  - Idazketa bikoitza sinkronizatzen du Dataverse-ra **Project Operations integratzeko proiektuaren gastuak esportatzeko entitatea (msdyn\_expenses)** taulako mapa erabiliz.
  - Zerga azpiegitura, saltzailearen azpiegitura eta bestelako finantza bidalketak aplikagarri gisa erregistratzen dira gastuen txostenak argitaratzean.

  ![Gastu-txostenen integrazioa.](./media/DW6ExpenseReports.png)

Diskoan idazten denean **Gastua** entitatea Dataverse-n, sistemak erregistroaren onarpen prozesu automatizatua abiarazten du. Behar izanez gero, onartutako prozesuen egoera automatikoa berrikusi daiteke Dataverse-n, **Ezarpen aurreratuak** > **Sistema** > **Sistemako lanak** aukerara joanda. Onarpena amaitu ondoren, gastuen transakzio motaren erregistroak sortzen dira **Benetako datuak** entitatean.

Gastuekin lotutako errealitateak idazketa bikoitzeko taulako mapa erabiliz prozesatzen dira, **Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)**. Informazio gehiago lortzeko, ikusi [Proiektuaren kalkuluak eta benetako datuak](resource-dual-write-estimates-actuals.md).

Aldizkako prozesua, **Inportatu eszenaratzetik** Gastuen txostenarekin lotutako aldizkari-lerroak sortzen ditu Project Operations-en integrazioko egunkarian. Desplazatutako kontuak lehenespenez gastuen integrazio kontua. Argitalpenen integrazio-egunkariak gastuen transakzioaren kontuaren balantzea garbitzen du eta gastuaren zenbatekoa proiektuaren kostuaren kontura eramaten du. Sistemak, gainera, proiektuen azpiegituren transakzioak sortzen ditu fakturazio eta diru-sarrerak ezagutzeko helburuetarako.
