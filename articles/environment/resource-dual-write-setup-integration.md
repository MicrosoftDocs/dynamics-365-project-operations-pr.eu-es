---
title: Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa
description: Artikulu honek Project Operations idazketa bikoitzeko esleipenak konfiguratzeari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d03393de893c39ceb53c06a3031395f765a26f55
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9029137"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a>Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du entitateak konfiguratzeko.

## <a name="project-contracts-contract-lines-and-projects"></a>Proiektu-kontratuak, kontratuaren lerroak eta proiektuak

Proiektuen kontratuak, kontratu ildoak eta proiektuak sortzen dira Dataverse-en eta sinkronizatuta finantzen eta eragiketen aplikaziora kontabilitate osagarria lortzeko. Erakunde horietako erregistroak hemen bakarrik sortu eta ezabatu daitezke Dataverse-n. Hala ere, kontabilitate atributuak, hala nola salmenten gaineko zerga taldearen lehenespenak eta finantza dimentsioak, gehitu daitezke erregistro horietan finantzen eta eragiketen aplikazioan.

  ![Proiektuko kontratua integratzeko kontzeptuak.](./media/1ProjectContract.jpg)

Salmenten jardueren abantailen, aukeren eta aurrekontuen jarraipena egiten da Dataverse-n eta ez sinkronizatu finantzen eta eragiketen aplikazioan ez dagoelako jarduera honekin lotutako kontabilitate ibaian behera.

Proiektuaren kontratuaren funtzionalitatea Dataverse-n proiektuaren kontratu erregistroa sortzen du finantzen eta eragiketen aplikazioan **Proiektuen kontratuen goiburuak (salmenten aginduak)** taulako mapa. Urtean proiektuaren kontratua gordetzea Dataverse-n, proiektuaren kontratuaren bezeroen entitate erregistroa sortzen hasten da. Erregistro hau sinkronizatuta dago finantzen eta eragiketen aplikazioan **Proiektua finantzatzeko iturria (msdyn\_projectcontractssplitbillingrules)** taulako mapa. Mapa honek proiektuaren kontratuaren bezeroen gehikuntzak, eguneratzeak eta ezabatzeak ere sinkronizatzen ditu. Proiektuaren kontratuko bezeroen arteko fakturazio portzentaje zatituak hemen bakarrik menderatzen dira Dataverse-n eta ez sinkronizatuta finantzen eta eragiketen aplikazioan.

Proiektuaren kontratua sortu ondoren Dataverse-n proiektuaren kontulariak proiektuaren kontratu honetako kontabilitate atributuak eguneratu ditzake finantzen eta eragiketen aplikazioan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea** aukerara joanda. Kontulariak proiektuaren kontratu operatiboaren atributuak berrikusi ditzake, hala nola, eskatutako entrega data eta kontratuaren zenbatekoa proiektuaren kontratuaren IDa hautatuta Dataverse lotutako proiektuaren kontratuaren erregistroa irekitzen duten finantzen eta eragiketen aplikazioak.

Proiektuaren entitatea sinkronizatuta dago finantzen eta eragiketen aplikazioan **Proiektuak V2 (msdyn\_projects)** taulako mapa erabiliz. Proiektuaren kontulariak hau egin dezake:

  - Berrikusi proiektuak finantzen eta eragiketen aplikazioan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** aukerara joanda. 
  - Eguneratu proiektuaren kontabilitate atributuak finantzen eta eragiketen aplikazioan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea** aukerara joanda.  
  - Berrikusi proiektuaren atributu operatiboak, esate baterako hasierako eta amaierako datak, proiektuaren IDa hautatuta Dataverse-ri lotutako proiektuaren erregistroa irekitzen duen finantzen eta eragiketen aplikazioan .

Proiektu bat proiektuaren kontratuarekin lotzen da **Proiektuaren kontratu lerroa** entitatea.

Proiektuaren kontratuaren lerroak Dataverse-n proiektu-kontratuaren fakturazio-araua sortzen du finantzen eta eragiketen aplikazioetan **Proiektuen kontratuaren lerroen goiburuak (salesorderdetails)** taulako mapa. Fakturazio-metodoak proiektuaren kontratuaren fakturazio-arau mota definitzen du finantza- eta eragiketa-aplikazioetan:

  - Proiektuen kontratu lerroek fakturazio denborarekin eta materialarekin metodoak denbora eta material motaren fakturazio araua sortzen dute.
  - Prezio finkoaren fakturazio metodoaren kontratu lerroek mugarri fakturazio araua sortzen dute.

Proiektuaren kontratu lerroak proiektuaren kontulariak berrikusi ditzake finantzen eta eragiketen aplikazioan **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea** aukerara joanda, eta webguneko xehetasunak berrikustea **Kontratu-lineak** fitxa. Kontulariak fitxa honetako prezio finkoko fakturazio metodoaren kontratu lerroetarako finantza dimentsio lehenetsiak ere ezar ditzake.

## <a name="billing-milestones"></a>Fakturazio-mugarriak

Prezio finkoko fakturazio metodoa erabiliz proiektuen kontratu lerroak fakturazio mugarrien bidez fakturatzen dira. Fakturazio mugarriak kontuko transakzioak proiektatzeko sinkronizatzen dira finantzen eta eragiketen aplikazioetan erabiliz **Project Operations integrazioaren kontratu-lerroaren mugarriak (msdyn\_contractlinescheduleofvalues)** taulako mapa.

  ![Fakturazio-mugarrien integrazioa.](./media/2Milestones.jpg)

Kontulariak kontuko transakzioak berrikusi eta transakzio horien kontabilitate atributuak doitu ahal izango ditu **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Mantendu** > **Kontuko transakzioak** edo **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Mantendu** > **Kontuko transakzioak** aukeran.

Proiektu jakin baten kontratu lerroaren fakturazio mugarria lehenengo aldiz sortzen duzunean, sistemak automatikoki sortzen du kontratu linea honekin lotutako proiektuaren prezio finkoko diru-sarrerak kalkulatzeko proiektua. Prezio finkoko diru-sarrerak kalkulatzeko proiektuak **Proiektuen kudeaketa eta kontabilitatea** > **Prezio finkoko diru-sarrerak kalkulatzeko proiektuak** aukerara joanda.

### <a name="project-tasks"></a>Proiektuen zereginak

Proiektuaren zereginak sinkronizatuta daude finantzen eta eragiketen aplikazioan **Proiektuaren zereginak (msdyn\_projecttasks)** taula mapa erreferentzia helburuetarako soilik. Eragiketak sortzea, eguneratzea eta ezabatzea ez da onartzen finantzen eta eragiketen aplikazioen bidez.

  ![Proiektu-zereginak integratzea.](./media/3Tasks.jpg)

## <a name="project-resources"></a>Proiektuko baliabideak

**Proiektuaren baliabide rolak** entitatearekin sinkronizatuta dago finantzen eta eragiketen aplikazioekin **Proiektuak baliabide guztiak enpresa guztientzat (bookableresourcecategories)** taula mapa erreferentzia helburuetarako soilik erabiliz. Baliabide rolak Dataverse-n ez dira konpainiaren espezifikoak, sistemak automatikoki sortzen ditu konpainiaren berariazko baliabide rolen erregistroak finantzen eta eragiketen aplikazioak automatikoki idazketa bikoitzeko integrazio esparruan sartutako pertsona juridiko guztientzat.

![Baliabide-rolen integrazioa.](./media/5Resources.jpg)

Project Operations-eko proiektuaren baliabideak urtean mantentzen dira Dataverse-en eta ez daude sinkronizatuta finantzen eta eragiketen aplikazioak.

### <a name="transaction-categories"></a>Transakzio-kategoriak

Transakzio kategoriak mantentzen dira Dataverse eta sinkronizatuta finantzen eta eragiketen aplikazioetan **Proiektuen transakzio-kategoriak\_(msdyn‑transactoncategories)** taulako mapa. Transakzio kategoria erregistroa sinkronizatu ondoren, sistemak automatikoki lau kategoria erregistro partekatu sortzen ditu. Erregistro bakoitza transakzio mota bati dagokio finantzen eta eragiketen aplikazioak eta transakzio kategoria erregistroarekin lotzen ditu.

![Transakzio-kategorien integrazioa.](./media/4TransactionCategories.jpg)

Transakzio-kategoriak estimazioetarako eta egiazkoetarako erabiltzeko, proiektuaren kontulariak edo sistemaren administratzaileak pertsona juridiko guztietan proiektu-kategoriak sortu behar ditu. Informazio gehiagorako, ikus [Konfiguratu proiektuaren kategoriak](../project-accounting/configure-project-categories.md).
