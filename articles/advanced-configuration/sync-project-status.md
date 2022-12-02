---
title: Sinkronizatu proiektuaren egoera itxitako proiektuetarako sarbidea saihesteko
description: Artikulu honek proiektuaren egoera nola sinkronizatu azaltzen du proiektu inaktibo edo itxien aurka sartzea saihesteko.
author: ryansandnessMSFT
ms.date: 08/09/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ryansandnessMSFT
ms.openlocfilehash: 7a306da164235f36d9ed5e69196508dce6d257de
ms.sourcegitcommit: 6b6c2bfd04e3e613ed1f38355c7cd47c3a56748d
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 08/24/2022
ms.locfileid: "9348092"
---
# <a name="sync-project-status-to-prevent-entry-against-closed-projects"></a>Sinkronizatu proiektuaren egoera itxitako proiektuetarako sarbidea saihesteko

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

## <a name="scenario"></a>Egoera

Contoso zuzenean jarriko da Microsoft Dynamics 365 Project Operations-ekin baliabide/hornitu gabeko eszenatokietarako. Enpresa-jarduera arrunten barruan, proiektuak amaitu edo geldiarazi daitezke. Proiektua desaktiba dezakezu gasturik edo fakturarik sortzen ez dela ziurtatzeko.

## <a name="solution"></a>Soluzioa

### <a name="prerequisites"></a>Aurrebaldintzak

-   Microsoft Dynamics Dynamics 365 Finance 10.0.29 edo berriagoa instalatu behar da.
-   Idazketa bikoitzeko mapa 1.0.0.3 Proiektuak V2rako (msdyn\_projects) instalatu edo eskuz konfiguratu behar dira behean azaltzen den moduan.

### <a name="create-an-updated-version-of-the-project-operations-integration-projects-v2-dual-write-map"></a>Sortu Project Operations integratzeko Projects V2 idazketa bikoitzeko maparen bertsio eguneratua

Project Operations Projects V2 zerbitzuaren idazketa dualeko esleipena eguneratzeko:

1. **Datuen kudeaketa** lan-eremuan, hautatu **Idazketa bikoitza**.
2. Hautatu **Idazketa bikoitza** teila.
3. **Taula mapa** zutabea, kokatu eta hautatu **V2 proiektua (msdyn\_projects)**, eta, gero, hautatu Gelditu.
4. Hautatu maparen izena mapa irekitzeko eta, ondoren, hautatu **[Inor ez]**.
5. Hautatu zutabea elkarrizketa-koadroan, hautatu **egoera-kodea \[Proiektuaren egoera\]** eta gero hautatu Ados. Idatzi dezakezu **estatu** iragazki-balioan zerrenda murrizteko.
6.  Hautatu **Gehitu edo editatu transformazioa** urtean **mapa mota** zutabea eraldatzea editatzeko.
7.  Bertatik **Transformazio mota** hautatu **ValueMap**.
8.  Hautatu **Gehitu balio-mapaketa**, eta gero gehitu ondorengoa **Giltzak** eta **Balioak**:

   Tekla       | Balioa 
   ----------|-------
   InProcess | 0     
   Osatuta | 1     

![Idazketa bikoitzeko mapen xehetasunen pantaila](media/projectstage-dw-mapping.png)

9. Sakatu **Gorde**.
10. Goitik **Idazketa bikoitza > Proiektuak V2 (msdyn_projects)** orrialdea, hautatu **Gorde**.
11. **Gehitu taula** panelean, **Argitaratzailea** eremuan, hautatu **CDS argitaratzaile lehenetsia**.
12. Ezarri **Bertsioa** eremura 1.0.0.3.
13. Idatzi **Deskribapena**, eta gero hautatu **Gorde**.
14. Goitik **Idazketa bikoitza > Proiektuak V2 (msdyn_projects)** orrialdea, hautatu **Exekutatu** mapa hasteko, eta gero select **Bai** korrika egin aurretik berresteko eskatuz gero. 

### <a name="close-a-newly-completed-project"></a>Itxi amaitu berri den proiektu bat

Dynamics 365 Finance-k erabiltzen du **proiektuaren fasea** proiektuak bereizteko eremua **prozesuan** edo **amaitu**. **Amaitu** proiektuek ezin diete gasturik egin edo bezeroei fakturatu.

1. Ireki proiektu bat desaktibatzeko.
2. Aukeratu **Desaktibatu** zintan.

> [!NOTE]
> Proiektu bat desaktibatu edo itxi dezakezu, biek berdin jokatuko baitute Finantzen testuinguruan.

3. Finantza atalean, ireki **Proiektu guztien zerrenda** orrialdea.
4. Egiaztatu desaktibatuta dagoen proiektua ez dela zerrendan agertzen.
5. **Proiektuak erakutsi** iragazi zerrendaren gainetik, aldatu balioa honetatik **Aktiboa** hona: **Denak**.
6. Orain desaktibatuta dagoen proiektua ikusiko duzu.

Proiektu honen aurka denbora edo gastua erregistratzen saiatzen bazara Finantzan, ez zenuke proiektua ikusi beharko hautatze aldera. Gastu batean proiektuaren zenbakia eskuz sartzen baduzu, "Proiektuaren faseak ez du onartzen proiektuan grabatzen" bezalako mezu bat ikusiko duzu. Fakturazioa eta beste fakturazio-funtzioak desgaitu egin behar dira proiektu itxi baten testuinguruan egongo baitira.

