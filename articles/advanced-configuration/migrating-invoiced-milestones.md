---
title: Migratu guztiz fakturatutako fakturazio-mugarriak trantsizioan
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
# <a name="migrate-fully-invoiced-billing-milestones-at-cutover"></a>Migratu guztiz fakturatutako fakturazio-mugarriak trantsizioan

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

## <a name="scenario"></a>Egoera

Contoso zuzenean jarriko da Microsoft Dynamics 365 Project Operations-ekin baliabide/hornitu gabeko eszenatokietarako. Mozketaren jardueren barruan, ezarpen-taldeak sistema zaharretik proiektu irekiko kontratuak migratu behar ditu. Proiektu-kontratu batzuek prezio finkoko fakturazio-metodoa erabiltzen duten eta azken bezeroari partzialki fakturatu zaizkion kontratu-lerroak barne hartzen dituzte. Ezarpen-taldeak fakturazio-mugarri hauek gisa migratu behar ditu **Bezeroaren faktura argitaratu da**, kontratuaren balio osoaren barruan sartu behar direlako diru-sarreren aitorpenaren ondorioetarako. Hala ere, kobratzeko kontuak eta liburu nagusiak ez dute eraginik izan behar.

## <a name="solution"></a>Soluzioa

### <a name="prerequisites"></a>Aurrebaldintzak

- Dynamics 365 Finance 10.0.24 edo berriagoa instalatu behar da.
- Migrazio-urratsak burutuko diren inguruneak mantentze moduan egon behar du. Ez da beste jarduerarik egin behar mugarriak migratzen diren bitartean.
- Migrazio-urratsak hemen deskribatzen den bezala jarraitu behar dira eta mozketa-jarduerarako soilik erabil daitezke. Microsoft-ek ez du gaitasun honen beste erabilerarik onartzen.

### <a name="create-a-cutover-version-of-the-project-operations-integration-contract-line-milestones-dual-write-map"></a>Sortu Project Operations integrazioaren kontratu-lerroaren mugarrien bertsio bikoitzeko idazketa bikoitzeko mapa 

1. Ziurtatu xede-mapaketa dela **Project Operations-en integrazioaren kontratu-lerroaren mugarriak** entitatea eguneratuta dagoela. 

    1. Finantzan, joan hona **Datuen kudeaketa** \> **Datu-entitateak**, eta hautatu **Project Operations-en integrazioaren kontratu-lerroaren mugarriak** entitate. 
    2. Hautatu **Aldatu xede-esleipenak**. 
    3. **Esleipenaren eszenaratzea xedera** orrialdea, hautatu **Sortu esleipena**, eta gero berretsi esleipena sortu nahi dituzula.

2. Gelditu eta freskatu **Project Operations-en integratzeko kontratu lerroaren mugarriak** (**msdyn\_contractlinescheduleofvalues**) idazketa dualeko esleipena. 

    1. Joan **Datuen kudeaketa** \> **Idazketa duala**, hautatu esleipena eta ireki haren xehetasunak. 
    2. Hautatu **Gelditu**, eta itxaron sistemak esleipena geldiarazi arte. 
    3. Aukeratu **Freskatu taulak**.

3. Gehitu transakzio egoeraren esleipen bat.

    1. Hautatu **Gehitu esleipena**.
    2. Lerro berrian, **finantzen eta eragiketen aplikazioak** zutabea, hautatu **TRANSSTATUS \[TRANSSTATUS\]** eremua.
    3. **Microsoft Dataverse** zutabean, hautatu **msdyn\_invoicestatus \[Invoice status\]**.
    4. **Esleipen mota** zutabean, hautatu eskuineko gezia (**\>**).
    5. Agertzen den elkarrizketa-koadroan, **Sinkronizazio norabidea** eremuan, hautatu **Dataverse to finantzen eta eragiketen aplikazioak**.
    6. Hautatu **Gehitu eraldaketa**.
    7. **Eraldaketa mota** eremuan, hautatu **ValueMap** aukera.
    8. Hautatu **Gehitu balio-esleipena**.
    9. Ezkerreko eremuan, sartu **4**. Eskuineko eremuan, sartu **192350001**. 
    10. Hautatu **Gorde** eta itxi elkarrizketa-koadroa

4. Hautatu **Gorde** idazketa bikoitzeko esleipenaren bertsioa gordetzeko. 
5. **Gehitu taula** panelean, **Argitaratzailea** eremuan, hautatu **Argitaratzaile lehenetsia**.
6. **Bertsioa** eremua, idatzi bertsioa.
7. **Deskribapena** eremuan, idatzi esleipenaren bertsio ebakigarri honi buruzko ohar bat. 
8. Sakatu **Gorde**.
9. Hasi mapa.

### <a name="migrate-invoiced-milestones-to-the-dataverse-environment"></a>Migratu fakturatutako mugarriak Dataverse ingurunera

1. Project Operations Dataverse ingurunean, sortu faktura egoera duten mugarriak **Fakturak egiteko prest**. Une honetan, ez migratu fakturatu gabeko mugarririk.

    > [!NOTE]
    > Fakturazio-mugarriak migratu aurretik, ziurtatu proiektuaren kontratu-lerroarekin erlazionatutako finantza-dimentsioak espero bezala ezartzen direla. Finantza-dimentsioak ezin dira editatu migrazioa amaitu ondoren.

2. Mugarri guztiak migratu ondoren, gelditu idazketa bikoitzeko mapa hauek:

    - Project Operations-en integrazioaren kontratuaren lerroaren mugarria (msdyn\_contractlinescheduleofvalues)
    - Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)
    - Proiektuaren faktura-proposamena V2 (fakturak)

    Mapak gelditzeko, jarraitu urrats hauei:

    1. Finance-n, joan **Datuen kudeaketa** \> **Idazketa duala**, hautatu esleipena eta ireki haren xehetasunak.
    2. Hautatu **Gelditu**, eta itxaron sistemak esleipena geldiarazi arte.

3. Project Operations Dataverse ingurunean, fakturazio-mugarrien pro-formako fakturak sortu eta berrestea. 

    1. Gunearen mapan, joan proiektuaren kontratuetara, hautatu kontratuak eta, ondoren, hautatu **Sortu fakturak**.
    2. Fakturak sortu ondoren, ireki itzazu **Fakturak** menua guneko mapan, eta gero hautatu **Berretsi**.

    Urrats honek beharrezko erregistroak sortzen ditu Dataverse ingurunean. Hala ere, ez du finantza- eta kobratzeko kontuetan eragiten, aurretik zerrendatutako idazketa bikoitzeko mapak gelditu egin zirelako.

4. Proformako faktura guztiak baieztatu ondoren, itzuli idazketa bikoitzeko mapa guztiak hasierako egoerara.

    1. Eguneratu **Project Operations-en integratzeko kontratu lerroaren mugarriak** (**msdyn\_contractlinescheduleofvalues**) idazketa dualeko esleipena jatorrizko bertsiora. 
    2. Hautatu idazketa bikoitzeko esleipena esleipenen zerrendan, hautatu **Taulen esleipen bertsioa**, eta, ondoren, hautatu taula-esleipenaren jatorrizko bertsioa.
    3. Sakatu **Gorde**.
    4. Berrabiarazi idazketa bikoitzeko esleipen hauek:

        - Project Operations-en integrazioaren kontratuaren lerroaren mugarria (msdyn\_contractlinescheduleofvalues)
        - Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)
        - Proiektuaren faktura-proposamena V2 (fakturak)

Mugarriak migratu dira orain, eta sistema prest dago mozketaren jardueraren hurrengo urratsetarako.
