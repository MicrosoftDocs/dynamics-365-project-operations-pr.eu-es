---
title: Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa
description: Gai honek Project Operations idazketa bikoitzeko esleipenak konfiguratzeari buruzko informazioa eskaintzen du.
author: sigitac
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 1ffa25ff36c39010d6aee31d928c3eaa0086c3d8
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8586881"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a>Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du entitateak konfiguratzeko.

## <a name="project-contracts-contract-lines-and-projects"></a>Proiektu-kontratuak, kontratuaren lerroak eta proiektuak

Proiektu-kontratuak, kontratu-lerroak eta proiektuak urtean sortzen dira Dataverse eta Finantza eta Operazio aplikazioekin sinkronizatuta kontabilitate gehigarrirako. Erakunde horietako erregistroak hemen bakarrik sortu eta ezabatu daitezke Dataverse-n. Hala ere, kontabilitate-atributuak, hala nola, salmenta-zergaren talde lehenetsiak eta finantza-dimentsioak gehi daitezke erregistro horietara Finantza eta Eragiketak aplikazioetan.

  ![Proiektuko kontratua integratzeko kontzeptuak.](./media/1ProjectContract.jpg)

Salmenta-jarduerak, aukerak eta aurrekontuak egiten dira jarraipena Dataverse eta ez sinkronizatu Finantza eta Operazioen aplikazioekin, ez baitago jarduera honekin lotutako beheranzko kontabilitaterik.

Proiektuaren kontratuaren funtzionaltasuna Dataverse proiektu-kontratu-erregistro bat sortzen du Finantza eta Operazioen aplikazioetan **Proiektu-kontratuaren goiburuak (salmenta-eskaerak)** mahai mapa. Urtean proiektuaren kontratua gordetzea Dataverse-n, proiektuaren kontratuaren bezeroen entitate erregistroa sortzen hasten da. Erregistro hau Finantza eta Operazioen aplikazioekin sinkronizatuta dago **Proiektuaren finantzaketa iturria (msdyn\_ proiektu-kontratuak banatzeko fakturazio-arauak)** mahai mapa. Mapa honek proiektuaren kontratuaren bezeroen gehikuntzak, eguneratzeak eta ezabatzeak ere sinkronizatzen ditu. Proiektu-kontratuko bezeroen arteko fakturazio-portzentajeak bakarrik menderatzen dira Dataverse eta ez dago sinkronizatuta Finantza eta Operazioen aplikazioekin.

Proiektu-kontratua sortu ondoren Dataverse, proiektuko kontu-hartzaileak proiektu-kontratu honen kontabilitate-atributuak egunera ditzake Finantza eta Eragiketak aplikazioetan, helbidera joanez.**Proiektuen kudeaketa eta kontabilitatea** > **Proiektu-kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea**. Kontu-hartzaileak proiektu operatiboko kontratu-atributuak berrikus ditzake, hala nola eskatutako entrega-data eta kontratuaren zenbatekoa, proiektu-kontratuaren IDa hautatuz Finantza eta Operazioen aplikazioetan, eta horrek erlazionatutako proiektu-kontratuaren erregistroa irekitzen du.Dataverse.

Proiektuaren entitatea Finantza eta Operazioen aplikazioekin sinkronizatuta dago **Proiektuak V2 (msdyn\_ proiektuak)** mahai mapa. Proiektuaren kontulariak hau egin dezake:

  - Berrikusi proiektuak Finantza eta Operazioen aplikazioetan helbidera joanda **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak**. 
  - Eguneratu proiektuaren kontabilitate-atributuak Finantza eta Eragiketak aplikazioetan helbidera joanez **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea**.  
  - Berrikusi proiektu operatiboen atributuak, hala nola, hasiera eta amaiera data estimatuak, proiektuaren IDa hautatuz Finantza eta Operazioen aplikazioetan eta horrek erlazionatutako proiektuaren erregistroa irekitzen du.Dataverse.

Proiektu bat proiektuaren kontratuarekin lotzen da **Proiektuaren kontratu lerroa** entitatea.

Proiektuaren kontratu lerroak Dataverse proiektu-kontratuaren fakturazio-arau bat sortzen du Finantza eta Operazioen aplikazioetan **Proiektuaren kontratu lerroak (salmenta eskaeraren xehetasunak)** mahai mapa. Fakturazio-metodoak proiektuaren kontratuaren fakturazio-arau mota definitzen du Finantza eta Operazioen aplikazioetan:

  - Proiektuen kontratu lerroek fakturazio denborarekin eta materialarekin metodoak denbora eta material motaren fakturazio araua sortzen dute.
  - Prezio finkoaren fakturazio metodoaren kontratu lerroek mugarri fakturazio araua sortzen dute.

Proiektuaren kontratu-lerroak proiektuko kontu-hartzaileak Finantza eta Eragiketen aplikazioetan berrikusi ditzake hona joanez **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu-kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea**, eta xehetasunak berrikustea **Kontratu-lerroak** fitxa. Kontu-hartzaileak prezio finkoko fakturazio metodoaren kontratu-lerroetarako finantza-dimentsio lehenetsiak ere ezar ditzake fitxa honetan.

## <a name="billing-milestones"></a>Fakturazio-mugarriak

Prezio finkoko fakturazio metodoa erabiliz proiektuen kontratu lerroak fakturazio mugarrien bidez fakturatzen dira. Fakturazio-mugarriak Finantza eta Operazioen aplikazioetan kontuko transakzioak proiektatzeko sinkronizatuta daude **Project Operations integrazio-kontratuaren lerroaren mugarriak (msdyn\_ kontratu-lerroen balio-egutegia)** mahai mapa.

  ![Fakturazio-mugarrien integrazioa.](./media/2Milestones.jpg)

Kontulariak kontuko transakzioak berrikusi eta transakzio horien kontabilitate atributuak doitu ahal izango ditu **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Mantendu** > **Kontuko transakzioak** edo **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Mantendu** > **Kontuko transakzioak** aukeran.

Proiektu jakin baten kontratu lerroaren fakturazio mugarria lehenengo aldiz sortzen duzunean, sistemak automatikoki sortzen du kontratu linea honekin lotutako proiektuaren prezio finkoko diru-sarrerak kalkulatzeko proiektua. Prezio finkoko diru-sarrerak kalkulatzeko proiektuak **Proiektuen kudeaketa eta kontabilitatea** > **Prezio finkoko diru-sarrerak kalkulatzeko proiektuak** aukerara joanda.

### <a name="project-tasks"></a>Proiektuen zereginak

Proiektuaren zereginak Finantza eta Operazioen aplikazioekin sinkronizatzen dira **Proiektuaren zereginak (msdyn\_ proiektuko zereginak)** taula-mapa erreferentzia helburuetarako soilik. Eragiketak sortu, eguneratu eta ezabatzea ez da onartzen Finantza eta Operazioen aplikazioen bidez.

  ![Proiektu-zereginak integratzea.](./media/3Tasks.jpg)

## <a name="project-resources"></a>Proiektuko baliabideak

The **Proiektuaren baliabideen rolak** entitatea Finantza eta Operazioen aplikazioekin sinkronizatuta dago **Proiektu-baliabideen rolak enpresa guztientzat (erreserbagarriak diren baliabide-kategoriak)** taula-mapa erreferentzia helburuetarako soilik. Baliabideen rolak baita Dataverse ez dira enpresaren espezifikoak, sistemak automatikoki sortzen ditu enpresaren berariazko baliabide-rolen erregistroak Finantza eta Operazioen aplikazioetan automatikoki idazketa bikoitzeko integrazio-esparruan sartutako entitate juridiko guztientzat.

![Baliabide-rolen integrazioa.](./media/5Resources.jpg)

Proiektuaren Eragiketetan proiektuko baliabideak bertan mantentzen dira Dataverse eta ez daude sinkronizatuta Finantza eta Operazioen aplikazioekin.

### <a name="transaction-categories"></a>Transakzio-kategoriak

Transakzio kategoriak mantentzen dira Dataverse eta Finantza eta Operazioen aplikazioekin sinkronizatuta dago **Proiektuaren transakzio kategoriak (msdyn\_ transakzio-kategoriak)** mahai mapa. Transakzio kategoria erregistroa sinkronizatu ondoren, sistemak automatikoki lau kategoria erregistro partekatu sortzen ditu. Erregistro bakoitza Finantza eta Operazioen aplikazioetako transakzio mota bati dagokio eta transakzio kategoriako erregistroarekin lotzen ditu.

![Transakzio-kategorien integrazioa.](./media/4TransactionCategories.jpg)

Transakzio-kategoriak estimazioetarako eta egiazkoetarako erabiltzeko, proiektuaren kontulariak edo sistemaren administratzaileak pertsona juridiko guztietan proiektu-kategoriak sortu behar ditu. Informazio gehiagorako, ikus [Konfiguratu proiektuaren kategoriak](../project-accounting/configure-project-categories.md).
