---
title: Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa
description: Gai honek Project Operations idazketa bikoitzeko esleipenak konfiguratzeari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6d263f7c5ef0d562edde6a603340a3b8746195df190fdb527bfa40297f68eed2
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986521"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a>Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du entitateak konfiguratzeko.

## <a name="project-contracts-contract-lines-and-projects"></a>Proiektu-kontratuak, kontratuaren lerroak eta proiektuak

Proiektuen kontratuak, kontratu ildoak eta proiektuak urtean sortzen dira Dataverse eta sinkronizatuta Finance and Operations aplikazioak kontabilitate osagarria lortzeko. Erakunde horietako erregistroak hemen bakarrik sortu eta ezabatu daitezke Dataverse-n. Hala ere, kontabilitate atributuak, hala nola salmenten gaineko zerga taldearen lehenespenak eta finantza dimentsioak, gehitu daitezke erregistro horietan Finance and Operations aplikazioak.

  ![Proiektuko kontratua integratzeko kontzeptuak.](./media/1ProjectContract.jpg)

Salmenten jardueren abantailen, aukeren eta aurrekontuen jarraipena egiten da Dataverse-n eta ez sinkronizatu Finance and Operations aplikazioak ez dagoelako jarduera honekin lotutako kontabilitate ibaian behera.

Proiektuaren kontratuaren funtzionalitatea Dataverse-n proiektuaren kontratu erregistroa sortzen du Finance and Operations aplikazioak **Proiektuen kontratuen goiburuak (salmenten aginduak)** taulako mapa. Urtean proiektuaren kontratua gordetzea Dataverse-n, proiektuaren kontratuaren bezeroen entitate erregistroa sortzen hasten da. Erregistro hau sinkronizatuta dago Finance and Operations aplikazioak **Proiektua finantzatzeko iturria (msdyn\_projectcontractssplitbillingrules)** taulako mapa. Mapa honek proiektuaren kontratuaren bezeroen gehikuntzak, eguneratzeak eta ezabatzeak ere sinkronizatzen ditu. Proiektuaren kontratuko bezeroen arteko fakturazio portzentaje zatituak hemen bakarrik menderatzen dira Dataverse eta ez sinkronizatuta Finance and Operations aplikazioak.

Urtean proiektuaren kontratua sortu ondoren Dataverse proiektuaren kontulariak proiektuaren kontratu honetako kontabilitate atributuak eguneratu ditzake Finance and Operations aplikazioak **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea** aukerara joanda. Kontulariak proiektuaren kontratu operatiboaren atributuak berrikusi ditzake, hala nola, eskatutako entrega data eta kontratuaren zenbatekoa proiektuaren kontratuaren IDa hautatuta Finance and Operations lotutako proiektuaren kontratuaren erregistroa irekitzen duten aplikazioak Dataverse.

Proiektuaren entitatea sinkronizatuta dago Finance and Operations aplikazioak **Proiektuak V2 (msdyn\_projects)** taulako mapa. Proiektuaren kontulariak hau egin dezake:

  - Berrikusi proiektuak Finance and Operations aplikazioak **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** aukerara joanda. 
  - Eguneratu proiektuaren kontabilitate atributuak Finance and Operations aplikazioak **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea** aukerara joanda.  
  - Berrikusi proiektuaren atributu operatiboak, esate baterako hasierako eta amaierako datak, proiektuaren IDa hautatuta Finance and Operations lotutako proiektuaren erregistroa irekitzen duen aplikazioak Dataverse.

Proiektu bat proiektuaren kontratuarekin lotzen da **Proiektuaren kontratu lerroa** entitatea.

Proiektuaren kontratuaren lerroak Dataverse-n proiektu-kontratuaren fakturazio-araua sortzen du Finance and Operations aplikazioetan **Proiektuen kontratuaren lerroen goiburuak (salesorderdetails)** taulako mapa. Fakturazio metodoak proiektuaren kontratuaren fakturazio arau mota definitzen du Finance and Operations aplikazioak:

  - Proiektuen kontratu lerroek fakturazio denborarekin eta materialarekin metodoak denbora eta material motaren fakturazio araua sortzen dute.
  - Prezio finkoaren fakturazio metodoaren kontratu lerroek mugarri fakturazio araua sortzen dute.

Proiektuaren kontratu lerroak proiektuaren kontulariak berrikusi ditzake Finance and Operations aplikazioak **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea** aukerara joanda, eta webguneko xehetasunak berrikustea **Kontratu-lineak** fitxa. Kontulariak fitxa honetako prezio finkoko fakturazio metodoaren kontratu lerroetarako finantza dimentsio lehenetsiak ere ezar ditzake.

## <a name="billing-milestones"></a>Fakturazio-mugarriak

Prezio finkoko fakturazio metodoa erabiliz proiektuen kontratu lerroak fakturazio mugarrien bidez fakturatzen dira. Fakturazio mugarriak kontuko transakzioak proiektatzeko sinkronizatzen dira Finance and Operations aplikazioak **Project Operations integratzeko kontratu lerroaren mugarriak (msdyn\_contractlinescheduleofvalues)** taulako mapa.

  ![Fakturazio-mugarrien integrazioa.](./media/2Milestones.jpg)

Kontulariak kontuko transakzioak berrikusi eta transakzio horien kontabilitate atributuak doitu ahal izango ditu **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Mantendu** > **Kontuko transakzioak** edo **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Mantendu** > **Kontuko transakzioak** aukeran.

Proiektu jakin baten kontratu lerroaren fakturazio mugarria lehenengo aldiz sortzen duzunean, sistemak automatikoki sortzen du kontratu linea honekin lotutako proiektuaren prezio finkoko diru-sarrerak kalkulatzeko proiektua. Prezio finkoko diru-sarrerak kalkulatzeko proiektuak **Proiektuen kudeaketa eta kontabilitatea** > **Prezio finkoko diru-sarrerak kalkulatzeko proiektuak** aukerara joanda.

### <a name="project-tasks"></a>Proiektuen zereginak

Proiektuaren zereginak sinkronizatuta daude Finance and Operations aplikazioak **Proiektuaren zereginak (msdyn\_projecttasks)** taula mapa erreferentzia helburuetarako soilik. Eragiketak sortzea, eguneratzea eta ezabatzea ez da onartzen Finance and Operations aplikazioen bidez.

  ![Proiektu-zereginak integratzea.](./media/3Tasks.jpg)

## <a name="project-resources"></a>Proiektuko baliabideak

**Proiektuaren baliabide rolak** entitatearekin sinkronizatuta dago Finance and Operations aplikazioekin **Proiektuak baliabide guztiak enpresa guztientzat (bookableresourcecategories)** taula mapa erreferentzia helburuetarako soilik erabiliz. Baliabide rolak Dataverse ez dira konpainiaren espezifikoak, sistemak automatikoki sortzen ditu konpainiaren berariazko baliabide rolen erregistroak Finance and Operations aplikazioak automatikoki idazketa bikoitzeko integrazio esparruan sartutako pertsona juridiko guztientzat.

![Baliabide-rolen integrazioa.](./media/5Resources.jpg)

Project Operations-eko proiektuaren baliabideak urtean mantentzen dira Dataverse eta ez daude sinkronizatuta Finance and Operations aplikazioak.

### <a name="transaction-categories"></a>Transakzio-kategoriak

Urtean transakzio kategoriak mantentzen dira Dataverse eta sinkronizatuta Finance and Operations aplikazioak **Proiektuaren transakzioen kategoriak (msdyn\_transactoncategories)** taulako mapa. Transakzio kategoria erregistroa sinkronizatu ondoren, sistemak automatikoki lau kategoria erregistro partekatu sortzen ditu. Erregistro bakoitza transakzio mota bati dagokio Finance and Operations aplikazioak eta transakzio kategoria erregistroarekin lotzen ditu.

![Transakzio-kategorien integrazioa.](./media/4TransactionCategories.jpg)

Transakzio-kategoriak estimazioetarako eta egiazkoetarako erabiltzeko, proiektuaren kontulariak edo sistemaren administratzaileak pertsona juridiko guztietan proiektu-kategoriak sortu behar ditu. Informazio gehiagorako, ikus [Konfiguratu proiektuaren kategoriak](../project-accounting/configure-project-categories.md).
