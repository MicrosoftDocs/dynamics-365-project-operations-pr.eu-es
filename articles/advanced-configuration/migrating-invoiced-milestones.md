---
title: Trantsizio garaian erabat fakturatutako fakturazio mugarriak migratzea
description: Artikulu honetan azaltzen da nola migratu bezeroari fakturatu zaizkion prezio finkoko fakturazioaren mugarriak, abian jarri aurretik irekitako proiektu-kontratuetarako.
author: sigitac
ms.date: 01/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: d7bb3dbb5acd9be447c405ec17f18d00c500f655
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912225"
---
# <a name="migrate-fully-invoiced-billing-milestones-at-cutover"></a>Trantsizio garaian erabat fakturatutako fakturazio mugarriak migratzea

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

## <a name="scenario"></a>Egoera

Contoso Microsoftekin Dynamics 365 Project Operations harremanetan jartzen ari da biltegiratutako baliabide/ ez-biltegietarako. Trantsizio-jardueren artean, inplementazio-taldeak aurreko sistemaren proiektu irekien kontratuak migratu behar ditu. Proiektuko kontratuetako batzuek kontratu-lerroak dituzte, prezio finkoaren fakturazio-metodoa erabiltzen dutenak, eta azken bezeroari zati batean fakturatu zaizkio. Inplementazio-taldeak fakturazio-mugarri horiek migratu behar ditu bezeroaren faktura kontabilizatzen **den neurrian**, kontratuaren balio osoan sartu behar baitira diru-sarrerak aitortzeko. Hala ere, kobratzeagatik eta liburu orokorragatik bezeroek dituzten saldoak ez dira kaltetu behar.

## <a name="solution"></a>Soluzioa

### <a name="prerequisites"></a>Aurrebaldintzak

- Dynamics 365 Finance 10.0.24 edo ondorengoak instalatuta egon behar du.
- Migrazio-pasaguneak osatuko diren inguruneak mantentze-lanetan egon behar du. Mugarriak migratzen diren bitartean, ez da beste jarduerarik egin behar.
- Migrazio-pausoak hemen deskribatzen diren bezala jarraitu behar dira, eta transferentzia-jarduerarako bakarrik erabil daitezke. Microsoftek ez du gaitasun hori beste erabilerarik onartzen.

### <a name="create-a-cutover-version-of-the-project-operations-integration-contract-line-milestones-dual-write-map"></a>Project Operations integratzeko kontratu-lineako mugarrien eskritura bikoitzaren mapa mozteko bertsio bat sortzea 

1. Ziurtatu Project Operations-en integrazio-kontratuaren **mugarri**-entitatearentzat destino-esleipena eguneratuta dagoela. 

    1. Finantzei dagokienez, joan datuak **administratzeko** \> **datu-erakundeetara**, eta hautatu proiektu-eragiketak **integratzeko kontratu-lerroaren** mugarrien erakundea. 
    2. Aukeratu **Destino-esleipenak** aldatzea. 
    3. **Orria entzun Orria entzun Diru-izendapena** **sortzea** eta, ondoren, esleipena sortu nahi duzula baieztatzea.

2. Project Operations (msdyn **contractlinescheduleofvalues**) integratzeko kontratu-lineako **mugarrien idazkera dualaren mapa atxilotu eta eguneratu\_.** 

    1. **Datu-kudeaketa** \> **duala**, aukeratu mapa eta ireki xehetasunak. 
    2. Aukeratu **gelditu** eta itxaron sistemak mapa gelditu arte. 
    3. Aukeratu Taulak **eguneratzea**.

3. Gaineratu transakzioaren egoerarako esleipen bat.

    1. Aukeratu **Esleipena eranspena**.
    2. Ildo berrian **, Aplicaciones** de Finance and Operations zutabean, TRANSSTATUS **TRANSSTATUS\[ zelaia \]** aukeratu.
    3. **Microsoft Dataverse** Zutabean, msdyn **invoicestatus fakturen \_\[estatua aukeratu\]**.
    4. **Mapa motako** zutabean, aukeratu eskuineko gezia (**\>**).
    5. Agertzen den elkarrizketa-koadroan **, sinkronizazio-zuzendaritzaren** arloan, aukeratu **Dataverse Finance and Operations-en aplikazioak**.
    6. Hautatu **Eraldaketa agregatu**.
    7. Transformazio-motaren **arloan**, ValueMap **aukeratu**.
    8. Aukeratu **Balio-esleipena eransteko aukeratzea**.
    9. Ezkerreko zelaian, idatzi **4**. Eskuineko alo mailan, idatzi **192350001**. 
    10. Hautatu **gorde eta,** ondoren, itxi elkarrizketa-koadroa.

4. Aukeratu **idazkera dualaren maparen bertsioa gordetzeko modua**. 
5. Agregar taula **panelean, Argitatzaile** zelaian **, aurrez zehaztutako selekzioa** **.**
6. Bertsioa alorraren **arabera**, idatzi bertsioa.
7. Deskribapen-eremuan **·**, idatzi ohar bat maparen mozketa-bertsio honi buruz. 
8. Sakatu **Gorde**.
9. Hasi mapa.

### <a name="migrate-invoiced-milestones-to-the-dataverse-environment"></a>Inguruneari fakturatutako mugarriak migratzea Dataverse

1. Proiektu-eragiketen Dataverse inguruan, fakturaziorako **Listoren** faktura-egoera duten mugarriak direla uste du. Puntu honetan, ez iezan fakturatu ez den mugarririk.

    > [!NOTE]
    > Fakturazio mugarriak migratu aurretik, ziurtatu proiektuaren kontratu-linearekin lotutako finantza-dimentsioak espero bezala ezarrita daudela. Finantza-dimentsioak ezin dira argitaratu migrazioa amaitu ondoren.

2. Mugarri guztiak migratu ondoren, idazkera dualeko mapa hauek ditu:

    - Proiektu-eragiketak integratzeko kontratu-linearen mugarriak (msdyn\_ contractlinescheduleofvalues)
    - Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)
    - Proiektuaren faktura-proposamena V2 (fakturak)

    Mapak geldiarazteko, jarraitu pauso hauek:

    1. Finantzei dagokienez, joan datu-administrazio **·** \> **dualera**, aukeratu mapa bat eta ireki xehetasunak.
    2. Aukeratu **gelditu** eta itxaron sistemak mapa gelditu arte.

3. Proiektu-eragiketen Dataverse inguruan, fakturazio mugarrietarako fakturak sortzen ditu. 

    1. Webgunearen mapan, joan proiektuaren kontratuetara, aukeratu kontratuak eta, ondoren, **fakturak** sortu.
    2. Fakturak sortu ondoren, ireki gunearen mapako fakturak menuan **eta, ondoren, aukeratu**.**·**

    Pauso horrek ingurunean beharrezkoak diren erregistroak sortzen ditu Dataverse. Hala ere, ez die finantza eta kontuei eragiten kobratzeagatik, aurretik zerrendatutako idazkera dualeko mapak gelditu egin baitziren.

4. Proforma faktura guztiak baieztatu ondoren, eskritura dualeko mapa guztiak bere hasierako egoerara itzultzen ditu.

    1. Project Operations (**msdyn contractlinescheduleofvalues**) jatorrizkora integratzeko kontratu-linearen **mugarriak idazten dituen \_ biko maparen bertsioa eguneratzen** du. 
    2. Aukeratu idazkera dualaren mapa mapen zerrendan, taula-maparen bertsioa **hautatu** eta, ondoren, taula-maparen jatorrizko bertsioa hautatu.
    3. Sakatu **Gorde**.
    4. Hasi idazkera dualeko mapa hauek:

        - Proiektu-eragiketak integratzeko kontratu-linearen mugarriak (msdyn\_ contractlinescheduleofvalues)
        - Project Operations-en integrazioaren benetako datuak (msdyn\_actuals)
        - Proiektuaren faktura-proposamena V2 (fakturak)

Orain mugarriak migratzen ari dira eta sistema prest trantsizio-jardueran hurrengo urratsetarako.
