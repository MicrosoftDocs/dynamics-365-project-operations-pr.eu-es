---
title: Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa
description: Artikulu honetan Project Operations-en idazkera dualeko mapak nola konfiguratu eta konfiguratu adierazten da.
author: sigitac
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 173ff01e938af48d2d6488d5e59cf4e74b3af8e4
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914525"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a>Project Operations-en konfigurazioa eta konfigurazio-datuen integrazioa

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Artikulu honetan, Instalazio- eta konfigurazio-erakundeentzako Project Operations-en eskritura dualaren integrazioari buruzko informazioa ematen da.

## <a name="project-contracts-contract-lines-and-projects"></a>Proiektu-kontratuak, kontratuaren lerroak eta proiektuak

Proiektu-kontratuak, kontratu-lerroak eta proiektuak kontabilitate gehigarri baterako Finantza eta Eragiketen aplikazioekin Dataverse sortu eta sinkronizatzen dira. Erakunde horietako erregistroak hemen bakarrik sortu eta ezabatu daitezke Dataverse-n. Hala ere, kontabilitate-atributuak, hala nola salmenten gaineko zergen taldearen aurrez zehaztutako balioak eta finantza-dimentsioak, erregistro horiei Finantzak eta Eragiketak aplikazioetan erans daitezke.

  ![Proiektuko kontratua integratzeko kontzeptuak.](./media/1ProjectContract.jpg)

Bezero potentzialak, salmenta-jardueraren aukerak eta kotizazioak arakatzen dira eta ez dira sinkronizatzen Dataverse Finantza eta Eragiketen aplikazioekin, ez baitago geroko kontabilitaterik jarduera horrekin lotuta.

Proiektu-kontratuaren Dataverse funtzionaltasuna, Finance and Operations-en aplikazioetan proiektu-kontratuaren erregistro bat sortzen duena, proiektu-kontratuaren taula-maparen bidez **(salmenta-eskaerak**). Urtean proiektuaren kontratua gordetzea Dataverse-n, proiektuaren kontratuaren bezeroen entitate erregistroa sortzen hasten da. Erregistro hori Finance and Operations-en aplikazioekin sinkronizatzen da, proiektuaren finantzaketa-jatorriko taula-maparen bidez **(msdyn\_ projectcontractssplitbillingrules**). Mapa honek proiektuaren kontratuaren bezeroen gehikuntzak, eguneratzeak eta ezabatzeak ere sinkronizatzen ditu. Proiektu-kontratuetako bezeroen artean banatutako fakturazio-ehunekoak Finantza eta Eragiketen aplikazioetan Dataverse bakarrik menderatzen dira, eta ez dira horiekin sinkronizatzen.

Proiektu-kontratu Dataverse bat sortu ondoren, proiektu-kontagailuak proiektu-kontratu honen kontabilitate-atributuak eguneratu ditzake Finantza- eta eragiketa-aplikazioetan, **eta proiektu-kontratuak** > **eta kontabilitatea** > **aurrez zehaztutako kontabilitatea** > **erakus** ditzake. Kontagailuak proiektu operatiboaren kontratuaren atributuak berrikusi ditzake, hala nola eskatutako entrega-data eta kontratuaren zenbatekoa, eta proiektuaren kontratuaren IDa hautatu dezake, finantza- eta eragiketa-aplikazioetan, zeinak proiektu horren Dataverse kontratuaren erregistroa irekitzen baitu.

Proiektuaren garrantzia Finance and Operations-en aplikazioekin sinkronizatzen da Projects V2 (msdyn **projects\_) taula-maparen bidez**. Proiektuaren kontulariak hau egin dezake:

  - Proiektuak Finantza eta Eragiketen aplikazioetan berrikusten ditu, eta proiektu **guztiak kudeatu** > **eta kontabilitatera** joan. 
  - Proiektuaren kontabilitate-ezaugarriak finantza- eta eragiketa-aplikazioetan eguneratzen ditu, eta administraziora eta proiektuen **kontabilitatera** > **joanez, aurrez** > **zehaztutako kontabilitatea** > **erakustea.**  
  - Aztertu proiektuaren ezaugarri operatiboak, hala nola hasierako eta amaierako data zenbatetsiak, eta proiektuaren identifikatzailea hautatu behar da Finantza aplikazioetan eta eragiketetan, hau da, proiektu horren erregistroa irekitzen duten eragiketetan Dataverse.

Proiektu bat proiektuaren kontratuarekin lotzen da **Proiektuaren kontratu lerroa** entitatea.

Proiektu-kontratuko lineak, Finance and Operations aplikazioetan Dataverse proiektu-kontratuaren fakturazio-arau bat sortzen ari dira, project (salesorderdetails **) kontratu-linearen taula-maparen bidez**. Fakturazio-metodoak proiektuaren kontratuaren fakturazio-arau mota definitzen du Finance and Operations aplikazioetan:

  - Proiektuen kontratu lerroek fakturazio denborarekin eta materialarekin metodoak denbora eta material motaren fakturazio araua sortzen dute.
  - Prezio finkoaren fakturazio metodoaren kontratu lerroek mugarri fakturazio araua sortzen dute.

Proiektu-kontagailuak Finantza- eta eragiketa-aplikazioetako kontratu-ildoak berrikusi ditzake, proiektu-kontratuak eta **proiektu-kontratuak** > **·** > **kudeatuz** > **, aurrez zehaztutako kontabilitatea** erakutsiz eta kontratu-lineen **xehetasunak** berrikusiz. Kontagailuak, halaber, betile honetan prezio finkoko fakturazioaren metodoaren kontratu-lerroetarako aurrez zehaztutako finantza-dimentsioak ezar ditzake.

## <a name="billing-milestones"></a>Fakturazio-mugarriak

Prezio finkoko fakturazio metodoa erabiliz proiektuen kontratu lerroak fakturazio mugarrien bidez fakturatzen dira. Fakturazio mugarriak Finance and Operations aplikazioetan konturako proiektuaren transakzioekin sinkronizatzen dira, Project Operations (msdyn **contractlinescheduleofvalues) integrazio-kontratuko linea-lerroko mugarri-taulen maparen \_ bidez.**

  ![Fakturazio-mugarrien integrazioa.](./media/2Milestones.jpg)

Kontulariak kontuko transakzioak berrikusi eta transakzio horien kontabilitate atributuak doitu ahal izango ditu **Proiektuen kudeaketa eta kontabilitatea** > **Proiektuen kontratuak** > **Mantendu** > **Kontuko transakzioak** edo **Proiektuen kudeaketa eta kontabilitatea** > **Proiektu guztiak** > **Mantendu** > **Kontuko transakzioak** aukeran.

Proiektu jakin baten kontratu lerroaren fakturazio mugarria lehenengo aldiz sortzen duzunean, sistemak automatikoki sortzen du kontratu linea honekin lotutako proiektuaren prezio finkoko diru-sarrerak kalkulatzeko proiektua. Prezio finkoko diru-sarrerak kalkulatzeko proiektuak **Proiektuen kudeaketa eta kontabilitatea** > **Prezio finkoko diru-sarrerak kalkulatzeko proiektuak** aukerara joanda.

### <a name="project-tasks"></a>Proiektuen zereginak

Proiektuaren lanak Finance and Operations-en aplikazioekin sinkronizatzen dira, proiektuaren Tareas (msdyn **projecttasks)\_ taula-maparen** bidez, erreferentzia-helburuekin soilik. Eragiketak sortu, eguneratu eta ezabatzea ez da onartzen Finance and Operations aplikazioetan.

  ![Proiektu-zereginak integratzea.](./media/3Tasks.jpg)

## <a name="project-resources"></a>Proiektuko baliabideak

**Project-en baliabideen erakunde rolak** Finance and Operations-en aplikazioekin sinkronizatzen dira, enpresa guztientzat Project-en baliabideen taula Rolesen maparen bidez **(bookableresourcecategories),** erreferentzia-helburuetarako bakarrik. Baliabide-rolak Dataverse enpresarenak ez direnez espezifikoak, sistemak automatikoki sortzen ditu finance and Operations-en aplikazioetan enpresaren baliabide espezifikoen rolen erregistroak, eskritura dualaren integrazio-eremuan sartzen diren erakunde juridiko guztientzat.

![Baliabide-rolen integrazioa.](./media/5Resources.jpg)

Proiektuaren baliabideak mantendu egiten dira eta ez dira finantza eta Dataverse operazio aplikazioekin sinkronizatzen.

### <a name="transaction-categories"></a>Transakzio-kategoriak

Transakzioen kategoriak mantendu eta sinkronizatzen Dataverse dira Finance and Operations aplikazioekin, project (msdyn **transactioncategories\_) transakzioen taula-maparen bidez**. Transakzio kategoria erregistroa sinkronizatu ondoren, sistemak automatikoki lau kategoria erregistro partekatu sortzen ditu. Erregistro bakoitza Finance and Operations aplikazioen transakzio mota bati dagokio, eta transakzio-kategoriako erregistroarekin lotzen ditu.

![Transakzio-kategorien integrazioa.](./media/4TransactionCategories.jpg)

Transakzio-kategoriak estimazioetarako eta egiazkoetarako erabiltzeko, proiektuaren kontulariak edo sistemaren administratzaileak pertsona juridiko guztietan proiektu-kategoriak sortu behar ditu. Informazio gehiagorako, ikus [Konfiguratu proiektuaren kategoriak](../project-accounting/configure-project-categories.md).
