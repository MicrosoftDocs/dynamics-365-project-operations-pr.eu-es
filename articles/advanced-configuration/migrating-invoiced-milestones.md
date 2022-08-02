---
title: Migratu guztiz fakturatutako fakturazio-mugarriak mozketan
description: Artikulu honek proiektu irekiko kontratuengatik bezeroari fakturatutako prezio finkoko fakturazio-mugarriak nola migratu azaltzen du abiarazteko data baino lehen.
author: sigitac
ms.date: 01/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 05cd71f9860b5698e3a26bc72660b0b2044206c8
ms.sourcegitcommit: a798fed5c59e3fefa62cdfa42c852d529b33fd35
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/18/2022
ms.locfileid: "9028687"
---
# <a name="migrate-fully-invoiced-billing-milestones-at-cutover"></a>Migratu guztiz fakturatutako fakturazio-mugarriak mozketan

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

## <a name="scenario"></a>Egoera

Contoso Microsoft-ekin zuzenean jarriko da Dynamics 365 Project Operations baliabide/hornitu gabeko eszenatokietarako. Mozketaren jardueren barruan, ezarpen-taldeak sistema zaharretik proiektu irekiko kontratuak migratu behar ditu. Proiektu-kontratu batzuek prezio finkoko fakturazio-metodoa erabiltzen duten eta azken bezeroari partzialki fakturatu zaizkion kontratu-lerroak barne hartzen dituzte. Ezarpen-taldeak fakturazio-mugarri hauek gisa migratu behar ditu **Bezeroaren faktura argitaratu da**, kontratuaren balio osoaren barruan sartu behar direlako diru-sarreren aitorpenaren ondorioetarako. Hala ere, kobratzeko eta Liburu Nagusiko bezeroen saldoek ez dute eraginik izan behar.

## <a name="solution"></a>Soluzioa

### <a name="prerequisites"></a>Aurrebaldintzak

- Dynamics 365 Finance 10.0.24 edo berriagoa instalatu behar da.
- Migrazio-urratsak burutuko diren inguruneak mantentze moduan egon behar du. Ez da beste jarduerarik egin behar mugarriak migratzen diren bitartean.
- Migrazio-urratsak hemen deskribatzen den bezala jarraitu behar dira eta mozketa-jarduerarako soilik erabil daitezke. Microsoft-ek ez du gaitasun honen beste erabilerarik onartzen.

### <a name="create-a-cutover-version-of-the-project-operations-integration-contract-line-milestones-dual-write-map"></a>Sortu Project Operations integrazioaren kontratu-lerroaren mugarrien bertsio bikoitzeko idazketa bikoitzeko mapa 

1. Ziurtatu xede-mapaketa dela **Proiektu Eragiketak integrazio-kontratuaren ildoaren mugarriak** entitatea eguneratuta dago. 

    1. Finantzan, joan hona **Datuen kudeaketa** \> **Datu-entitateak**, eta hautatu **Proiektu Eragiketak integrazio-kontratuaren ildoaren mugarriak** entitate. 
    2. Hautatu **Aldatu xede-mapeak**. 
    3. Gainean **Maparen eszenaratzea bideratzeko** orrialdea, hautatu **Sortu mapak**, eta gero berretsi mapak sortu nahi dituzula.

2. Gelditu eta freskatu **Proiektu Eragiketak integrazio-kontratuaren ildoaren mugarriak** (**msdyn\_ kontratu-lerroen egutegia**) idazketa bikoitzeko mapa. 

    1. Joan **Datuen kudeaketa** \> **Idazketa bikoitza**, hautatu mapa eta ireki haren xehetasunak. 
    2. Hautatu **Gelditu**, eta itxaron sistemak mapa geldiarazi arte. 
    3. Hautatu **Freskatu taulak**.

3. Gehitu transakzio egoeraren mapa bat.

    1. Hautatu **Gehitu mapak**.
    2. Lerro berrian, aldean **Finantza eta eragiketa aplikazioak** zutabea, hautatu **TRANSSTATUSA\[ TRANSSTATUSA\]** eremua.
    3. urtean **Microsoft Dataverse** zutabea, hautatu **msdyn\_ fakturaren egoera\[ Fakturaren egoera\]**.
    4. urtean **Mapa mota** zutabea, hautatu eskuineko gezia (**\>**).
    5. Agertzen den elkarrizketa-koadroan, atalean **Sinkronizazio norabidea** eremua, hautatu **Dataverse Finantza eta Operazio aplikazioetara**.
    6. Hautatu **Gehitu transformazioa**.
    7. urtean **Transformazio mota** eremua, hautatu **Balio-Mapa**.
    8. Hautatu **Gehitu balio-mapaketa**.
    9. Ezkerreko eremuan, sartu **4**. Eskuineko eremuan, sartu **192350001**. 
    10. Hautatu **Gorde**, eta gero itxi elkarrizketa-koadroa.

4. Hautatu **Gorde** idazketa bikoitzeko maparen bertsioa gordetzeko. 
5. urtean **Gehitu taula** panelean, in **Argitaletxea** eremua, hautatu **Argitaratzaile lehenetsia**.
6. urtean **Bertsioa** eremuan, sartu bertsioa.
7. urtean **Deskribapena** eremuan, idatzi maparen bertsio ebakigarri honi buruzko ohar bat. 
8. Sakatu **Gorde**.
9. Hasi mapa.

### <a name="migrate-invoiced-milestones-to-the-dataverse-environment"></a>Migratu fakturatutako mugarriak Dataverse ingurunea

1. Proiektuaren Eragiketetan Dataverse ingurunea, sortu faktura egoera duten mugarriak **Fakturak egiteko prest**. Une honetan, ez migratu fakturatu gabeko mugarririk.

    > [!NOTE]
    > Fakturazio-mugarriak migratu aurretik, ziurtatu proiektuaren kontratu-lerroarekin erlazionatutako finantza-dimentsioak espero bezala ezartzen direla. Finantza-dimentsioak ezin dira editatu migrazioa amaitu ondoren.

2. Mugarri guztiak migratu ondoren, gelditu idazketa bikoitzeko mapa hauek:

    - Project Operations integrazio-kontratuaren lerroaren mugarriak (msdyn\_ kontratu-lerroen balio-egutegia)
    - Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)
    - Proiektuaren faktura-proposamena V2 (fakturak)

    Mapak gelditzeko, jarraitu urrats hauek:

    1. Finantzan, joan hona **Datuen kudeaketa** \> **Idazketa bikoitza**, hautatu mapa bat eta ireki haren xehetasunak.
    2. Hautatu **Gelditu**, eta itxaron sistemak mapa gelditu arte.

3. Proiektuaren Eragiketetan Dataverse ingurumena, fakturazio-mugarrien pro-formako fakturak sortu eta berrestea. 

    1. Gunearen mapan, joan proiektuaren kontratuetara, hautatu kontratuak eta, ondoren, hautatu **Sortu fakturak**.
    2. Fakturak sortu ondoren, ireki itzazu **Fakturak** menua guneko mapan, eta gero hautatu **Berretsi**.

    Urrats honek beharrezko erregistroak sortzen ditu Dataverse ingurunea. Hala ere, ez die eragiten finantza- eta kobratzeko kontuei, aurretik zerrendatutako idazketa bikoitzeko mapak gelditu egin zirelako.

4. Proformako faktura guztiak baieztatu ondoren, itzuli idazketa bikoitzeko mapa guztiak hasierako egoerara.

    1. Eguneratu bertsioa **Proiektu Eragiketak integrazio-kontratuaren ildoaren mugarriak** (**msdyn\_ kontratu-lerroen egutegia**) idazketa bikoitzeko mapa jatorrizkora itzuli. 
    2. Hautatu idazketa bikoitzeko mapa mapa zerrendan, hautatu **Taulen maparen bertsioa**, eta, ondoren, hautatu taula-maparen jatorrizko bertsioa.
    3. Sakatu **Gorde**.
    4. Berrabiarazi idazketa bikoitzeko mapa hauek:

        - Project Operations integrazio-kontratuaren lerroaren mugarriak (msdyn\_ kontratu-lerroen balio-egutegia)
        - Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)
        - Proiektuaren faktura-proposamena V2 (fakturak)

Mugarriak migratu dira orain, eta sistema prest dago mozketaren jardueraren hurrengo urratsetarako.
