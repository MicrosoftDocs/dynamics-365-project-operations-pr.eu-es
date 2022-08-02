---
title: Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa
description: Artikulu honek Project Operations idazketa bikoitzeko mapak konfiguratzeari eta konfiguratzeari buruzko informazioa eskaintzen du.
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

Artikulu honek Project Operations idazketa bikoitzeko integrazioari buruzko informazioa eskaintzen du konfigurazio eta konfigurazio entitateetarako.

## <a name="project-contracts-contract-lines-and-projects"></a>Proiektu-kontratuak, kontratuaren lerroak eta proiektuak

Proiektu-kontratuak, kontratu-lerroak eta proiektuak urtean sortzen dira Dataverse eta finantza eta eragiketa aplikazioekin sinkronizatuta kontabilitate gehigarrirako. Erakunde horietako erregistroak hemen bakarrik sortu eta ezabatu daitezke Dataverse-n. Hala ere, kontabilitate-atributuak, hala nola, salmenta-zergaren talde lehenetsiak eta finantza-dimentsioak gehi daitezke erregistro horietara finantza- eta eragiketa-aplikazioetan.

  ![Proiektuko kontratua integratzeko kontzeptuak.](./media/1ProjectContract.jpg)

Salmenta-jarduerak, aukerak eta aurrekontuak egiten dira jarraipena Dataverse eta ez sinkronizatu finantza- eta eragiketa-aplikazioekin, ez baitago jarduera honekin lotutako kontabilitatea.

Proiektuaren kontratuaren funtzionaltasuna Dataverse finantza- eta eragiketa-aplikazioetan proiektu-kontratuaren erregistroa sortzen du **Proiektu-kontratuaren goiburuak (salmenta-eskaerak)** mahai mapa. Urtean proiektuaren kontratua gordetzea Dataverse-n, proiektuaren kontratuaren bezeroen entitate erregistroa sortzen hasten da. Erregistro hau finantzaketa eta eragiketa aplikazioekin sinkronizatuta dago **Proiektuaren finantzaketa iturria (msdyn\_ proiektu-kontratuak banatzeko fakturazio-arauak)** mahai mapa. Mapa honek proiektuaren kontratuaren bezeroen gehikuntzak, eguneratzeak eta ezabatzeak ere sinkronizatzen ditu. Proiektu-kontratuko bezeroen arteko fakturazio-portzentajeak bakarrik menderatzen dira Dataverse eta ez dago sinkronizatuta finantza eta operazio aplikazioekin.

Proiektu-kontratua sortu ondoren Dataverse, proiektuko kontu-hartzaileak proiektu-kontratu honen kontabilitate-atributuak egunera ditzake finantza- eta eragiketen aplikazioetan.**Proiektuen kudeaketa eta kontabilitatea** > **Proiektu-kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea**. Kontu-hartzaileak proiektu operatiboko kontratu-atributuak berrikus ditzake, hala nola eskatutako entrega-data eta kontratuaren zenbatekoa, proiektuaren kontratuaren IDa hautatuz finantza- eta eragiketen aplikazioetan, eta horrek erlazionatutako proiektu-kontratuaren erregistroa irekitzen du.Dataverse.

Proiektuaren entitatea finantzaketa eta eragiketa aplikazioekin sinkronizatuta dago **Proiektuak V2 (msdyn\_ proiektuak)** mahai mapa. Proiektuaren kontulariak hau egin dezake:

  - Berrikusi proiektuak finantza- eta eragiketa-aplikazioetan helbidera joanda **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak**. 
  - Eguneratu proiektuaren kontabilitate-atributuak finantza- eta eragiketa-aplikazioetan helbidera joanez **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea**.  
  - Berrikusi proiektu operatiboen atributuak, hala nola, hasierako eta amaiera data estimatuak, proiektuaren IDa hautatuz finantza eta eragiketen aplikazioetan, eta horrek erlazionatutako proiektuaren erregistroa irekitzen du.Dataverse.

Proiektu bat proiektuaren kontratuarekin lotzen da **Proiektuaren kontratu lerroa** entitatea.

Proiektuaren kontratu lerroak Dataverse proiektu-kontratuaren fakturazio-arau bat sortzen du finantza- eta eragiketa-aplikazioetan **Proiektuaren kontratu lerroak (salmenta eskaeraren xehetasunak)** mahai mapa. Fakturazio-metodoak proiektuaren kontratuaren fakturazio-arau mota definitzen du finantza- eta eragiketa-aplikazioetan:

  - Proiektuen kontratu lerroek fakturazio denborarekin eta materialarekin metodoak denbora eta material motaren fakturazio araua sortzen dute.
  - Prezio finkoaren fakturazio metodoaren kontratu lerroek mugarri fakturazio araua sortzen dute.

Proiektuaren kontratu-lerroak proiektuko kontu-hartzaileak finantza eta eragiketen aplikazioetan berrikusi ditzake, helbidera joanda **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu-kontratuak** > **Konfiguratu** > **Erakutsi lehenetsitako kontabilitatea**, eta xehetasunak berrikustea **Kontratu-lerroak** fitxa. Kontu-hartzaileak prezio finkoko fakturazio-metodoaren kontratu-lerroetarako finantza-dimentsio lehenetsiak ere ezar ditzake fitxa honetan.

## <a name="billing-milestones"></a>Fakturazio-mugarriak

Prezio finkoko fakturazio metodoa erabiliz proiektuen kontratu lerroak fakturazio mugarrien bidez fakturatzen dira. Fakturazio-mugarriak finantza- eta operazio-aplikazioetan kontuko transakzioak proiektatzeko sinkronizatuta daude **Project Operations integrazio-kontratuaren lerroaren mugarriak (msdyn\_ kontratu-lerroen balio-egutegia)** mahai mapa.

  ![Fakturazio-mugarrien integrazioa.](./media/2Milestones.jpg)

Kontulariak kontuko transakzioak berrikusi eta transakzio horien kontabilitate atributuak doitu ahal izango ditu **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Mantendu** > **Kontuko transakzioak** edo **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Mantendu** > **Kontuko transakzioak** aukeran.

Proiektu jakin baten kontratu lerroaren fakturazio mugarria lehenengo aldiz sortzen duzunean, sistemak automatikoki sortzen du kontratu linea honekin lotutako proiektuaren prezio finkoko diru-sarrerak kalkulatzeko proiektua. Prezio finkoko diru-sarrerak kalkulatzeko proiektuak **Proiektuen kudeaketa eta kontabilitatea** > **Prezio finkoko diru-sarrerak kalkulatzeko proiektuak** aukerara joanda.

### <a name="project-tasks"></a>Proiektuen zereginak

Proiektuaren zereginak finantzaketa eta eragiketa aplikazioekin sinkronizatzen dira **Proiektuaren zereginak (msdyn\_ proiektuko zereginak)** taula-mapa erreferentzia helburuetarako soilik. Eragiketak sortu, eguneratu eta ezabatzea ez da onartzen finantza- eta eragiketa-aplikazioen bidez.

  ![Proiektu-zereginak integratzea.](./media/3Tasks.jpg)

## <a name="project-resources"></a>Proiektuko baliabideak

The **Proiektuaren baliabideen rolak** entitatea finantza eta eragiketa aplikazioekin sinkronizatuta dago **Proiektu-baliabideen rolak enpresa guztientzat (erreserbagarriak diren baliabide-kategoriak)** taula-mapa erreferentzia helburuetarako soilik. Baliabideen rolak baita Dataverse ez dira enpresaren espezifikoak, sistemak automatikoki sortzen ditu enpresaren berariazko baliabide-rolen erregistroak finantza- eta eragiketa-aplikazioetan automatikoki idazketa bikoitzeko integrazio-esparruan sartutako entitate juridiko guztientzat.

![Baliabide-rolen integrazioa.](./media/5Resources.jpg)

Proiektuaren Eragiketetan proiektuko baliabideak bertan mantentzen dira Dataverse eta ez daude sinkronizatuta finantza- eta operazio-aplikazioekin.

### <a name="transaction-categories"></a>Transakzio-kategoriak

Transakzio kategoriak mantentzen dira Dataverse eta finantza eta eragiketa aplikazioekin sinkronizatuta **Proiektuaren transakzio kategoriak (msdyn\_ transakzio-kategoriak)** mahai mapa. Transakzio kategoria erregistroa sinkronizatu ondoren, sistemak automatikoki lau kategoria erregistro partekatu sortzen ditu. Erregistro bakoitza finantza eta eragiketa aplikazioetako transakzio mota bati dagokio eta transakzio kategoriako erregistroarekin lotzen ditu.

![Transakzio-kategorien integrazioa.](./media/4TransactionCategories.jpg)

Transakzio-kategoriak estimazioetarako eta egiazkoetarako erabiltzeko, proiektuaren kontulariak edo sistemaren administratzaileak pertsona juridiko guztietan proiektu-kategoriak sortu behar ditu. Informazio gehiagorako, ikus [Konfiguratu proiektuaren kategoriak](../project-accounting/configure-project-categories.md).
