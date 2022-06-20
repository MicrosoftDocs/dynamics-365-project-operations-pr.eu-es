---
title: Erabili proiektuaren antolaketa APIak Power Automate-rekin
description: Artikulu honetan, Project-en programazioko aplikazioen programazio interfazeak (API) erabiltzen dituen adibide-fluxua ematen da.
author: ruhercul
ms.date: 01/26/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: 2527375ff3f3d631f3bb3de1458abb3b8838db54
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 06/03/2022
ms.locfileid: "8916319"
---
# <a name="use-project-schedule-apis-with-power-automate"></a>Erabili proiektuaren antolaketa APIak Power Automate-rekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Artikulu honetan adibide-fluxu bat deskribatzen da, proiektu-plan oso Microsoft Power Automate bat nola sortu, eragiketa-multzo bat nola sortu eta erakunde bat nola eguneratu erakusten duena. Adibidean, proiektu bat nola sortu, proiektuko taldeko kide bat, eragiketa multzoak, proiektu lanak eta baliabideen esleipenak erakusten dira. Artikulu honetan, erakunde bat nola eguneratu eta eragiketa-multzo bat nola gauzatu azaltzen da.

Hona hemen artikulu honen adibide-fluxuan dokumentatzen diren urratsen zerrenda osoa:

1. [Desenkadenagailu bat PowerApps sortzea](#1)
2. [Sortu proiektua](#2)
3. [Aldagai bat inizializatzea taldeko kidearentzat](#3)
4. [Taldeko kide generiko bat sortzea](#4)
5. [Eragiketa multzo bat sortzea](#5)
6. [Proiektu bukket bat sortzea](#6)
7. [Loturaren egoerarako aldagai bat inizializatzea](#7)
8. [Lan-kopururako aldagai bat inizializatzea](#8)
9. [Proiektuaren lan-identifikatzailerako aldagai bat inizializatzea](#9)
10. [Egin](#10)
11. [Proiektu-lan bat ezartzea](#11)
12. [Proiektu-lan bat sortzea](#12)
13. [Baliabideen esleipena sortzea](#13)
14. [Aldagai bat gutxitzea](#14)
15. [Proiektu-lan baten izena aldatzea](#15)
16. [Eragiketa-multzo bat gauzatzea](#16)

## <a name="assumptions"></a>Suposizioak

Artikulu honetan, plataformaren oinarrizko ezagutza, hodeiko fluxuak Dataverse eta project schedule aplikazioen programazio interfazea (API) dituela suposatzen da. Informazio gehiago lortzeko, kontsultatu [erreferentziak](#references) atala artikulu honetan aurrerago.

## <a name="create-a-flow"></a>Sortu fluxu bat

### <a name="select-an-environment"></a>Hautatu ingurune bat

Bere ingurunean fluxua Power Automate sor dezake.

1. Zoaz <https://flow.microsoft.com>, eta erabili administratzaile-kredentzialak saioa hasteko.
2. Goiko eskuineko izkinan, inguruak **aukeratu**.
3. Zerrendan, aukeratu Dynamics 365 Project Operations non dagoen instalatuta.

### <a name="create-a-solution"></a>Sortu soluzio bat

Jarraitu urrats horiek konponbidearekin bateragarria den fluxua [sortzeko](/power-automate/overview-solution-flows). Konponbidearekin bateragarria den fluxua sortzean, fluxua errazago esporta dezake aurrerago erabiltzeko.

1. Nabigazio-panelean, aukeratu **Konponbideak**.
2. **Orria entzun Orria entzun Konponbide** **berria**.
3. Elkarrizketa-koadroan **irtenbide** berria, derrigorrezko eremuak ezarri eta, ondoren, Sortu **aukeratu**.

## <a name="step-1-create-a-powerapps-trigger"></a><a id="1"></a> 1. pausoa: Desenkadenadore bat PowerApps sortzea

1. **Soluciones** orrian, aukeratu sortu zuen irtenbidea eta, ondoren, selekzio **berria**.
2. Ezkerreko panelean, Cloud flows **Automation**\> Cloud **flow**\> Instant aukeratu.**·** \> **·**
3. Fluxuaren izenan **,** idatzi Schedule API Demo Flow **.**
4. **Zerrendan aukeratu** fluxu hori nola aktibatu, aukeratu **Power Apps**. Desenkadenatzaile bat Power Apps sortzen duenean, logika zure esku autore gisa. Artikulu honetan, utzi sarrera zuriaren parametroak proba-helburuetarako.
5. Hautatu **Sortu**.

## <a name="step-2-create-a-project"></a><a id="2"></a>2. pausoa: Sortu proiektu bat

Jarraitu urrats hauek adibide-proiektu bat sortzeko.

1. Sortu duen fluxuan, urrats **berria aukeratu**.

    ![Pauso berri bat eman.](media/newstep.png)

2. Elkarrizketa-koadroan **, bilaketa-esparruan, eragiketa** bat aukeratu, lotu **gabeko ekintza** bat idatzi. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.

    ![Eragiketa bat hautatzea.](media/chooseactiontab.png)

3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.

![Pauso baten izena aldatu.](media/renamestep.png)

4. Aldatu izena urratsa **Sortu Proiektua**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ SortuProiektuaV1**.
6. azpian **msdyn\_ gaia** eremua, hautatu **Gehitu eduki dinamikoa**.
7. Gainean **Adierazpena** fitxan, funtzio eremuan, sartu **Proiektuaren izena - utcNow()**.
8. Hautatu **Ados**.

## <a name="step-3-initialize-a-variable-for-the-team-member"></a><a id="3"></a> 3. urratsa: hasieratu taldekidearentzat aldagai bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Init taldeko kidea**.
5. urtean **Izena** eremua, sartu **TaldekideEkintza**.
6. urtean **Mota** eremua, hautatu **Katea**.
7. urtean **Balioa** eremua, sartu **msdyn\_ Sortu TaldekideaV1**.

## <a name="step-4-create-a-generic-team-member"></a><a id="4"></a> 4. urratsa: Sortu taldekide generiko bat

1. Fluxuan, hautatu **Urrats berria**.
2. Elkarrizketa-koadroan **, bilaketa-esparruan, eragiketa** bat aukeratu, lotu **gabeko ekintza** bat idatzi. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Sortu taldekidea**.
5. rentzat **Ekintzaren izena** eremua, hautatu **TaldekideEkintza** urtean **Eduki dinamikoak** elkarrizketa-koadroa.
6. urtean **Ekintza-parametroak** eremuan, idatzi parametroen informazioa.

    ```
    {
        "TeamMember": {
            "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_projectteam",
            "msdyn_projectteamid": "@{guid()}",
            "msdyn_project@odata.bind": "/msdyn_projects(@{outputs('Create_Project')?['body/ProjectId']})",
            "msdyn_name": "ScheduleAPIDemoTM1"
        }
    } 
    ```

    Hona hemen parametroen azalpena:

    - **\@\@ odata.mota** – Erakundearen izena. Adibidez, sartu **"Microsoft.Dynamics.CRM.msdyn\_ proiektu taldea"**.
    - **msdyn\_ projectteamid** – Proiektu-taldearen IDaren lehen gakoa. Balioa identifikatzaile bakarra (GUID) adierazpena da.   IDa espresioaren fitxatik sortzen da.

    - **msdyn\_ proiektua\@ odata.bind** – Proiektu jabearen proiektuaren IDa. Balioa "Sortu proiektua" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_ proiektuak(GEHITU EDUKIA DINAMIKOA)"**.
    - **msdyn\_ izena** – Taldekidearen izena. Adibidez, sartu **"ScheduleAPIDemoTM1"**.

## <a name="step-5-create-an-operation-set"></a><a id="5"></a> 5. urratsa: Sortu eragiketa multzo bat

1. Fluxuan, hautatu **Urrats berria**.
2. Elkarrizketa-koadroan **, bilaketa-esparruan, eragiketa** bat aukeratu, lotu **gabeko ekintza** bat idatzi. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Sortu eragiketa multzoa**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ Sortu OperationSetV1** Dataverse ekintza pertsonalizatua.
6. urtean **Deskribapena** eremua, sartu **ScheduleAPIDemoOperationSet**.
7. urtean **Proiektua** eremua, sartu **/msdyn\_ proiektuak(**.
8. urtean **Eduki dinamikoak** elkarrizketa-koadroa, hautatu **msdyn\_ SortuProiektuaV1Erantzun Proiektuaren Id**.
9. urtean **Proiektua** eremua, sartu **)**.

## <a name="step-6-create-a-project-bucket"></a><a id="6"></a> 6. urratsa: Sortu proiektu-ontzi bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **gehitu errenkada berria**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Sortu Bucket**.
5. urtean **Taularen izena** eremua, hautatu **Project Buckets**.
6. urtean **Izena** eremua, sartu **ScheduleAPIDemoBucket1**.
7. rentzat **Proiektua** eremua, hautatu **msdyn\_ SortuProiektuaV1Erantzun Proiektuaren Id** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-7-initialize-a-variable-for-the-link-status"></a><a id="7"></a> 7. urratsa: hasieratu aldagai bat estekaren egoerarako

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Hasi estekaren egoera**.
5. urtean **Izena** eremua, sartu **estekaren egoera**.
6. urtean **Mota** eremua, hautatu **Zenbaki osoa**.
7. urtean **Balioa** eremua, sartu **192350000**.

## <a name="step-8-initialize-a-variable-for-the-number-of-tasks"></a><a id="8"></a> 8. urratsa: Hasta ezazu ataza kopuruaren aldagai bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Init Zeregin kopurua**.
5. urtean **Izena** eremua, sartu **ataza kopurua**.
6. urtean **Mota** eremua, hautatu **Zenbaki osoa**.
7. urtean **Balioa** eremua, sartu **5**.

## <a name="step-9-initialize-a-variable-for-the-project-task-id"></a><a id="9"></a> 9. urratsa: hasieratu proiektuaren ataza IDrako aldagai bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Hasi ProjectTaskID**.
5. urtean **Izena** eremua, sartu **ataza kopurua**.
6. urtean **Mota** eremua, hautatu **Katea**.
7. rentzat **Balioa** eremua, sartu **gidari ()** esamoldearen eraikitzailean.

## <a name="step-10-do-until"></a><a id="10"></a> 10. urratsa: egin arte

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **egin arte**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Ezarri baldintzazko adierazpenaren lehen balioa **ataza kopurua** aldagaitik **Eduki dinamikoak** elkarrizketa-koadroa.
4. Ezarri baldintza honetara **berdina baino txikiagoa**.
5. Ezarri baldintzazko adierazpeneko bigarren balioa honela **0**.

## <a name="step-11-set-a-project-task"></a><a id="11"></a> 11. urratsa: Ezarri proiektuko zeregin bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **ezarri aldagaia**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Pauso berrian, aukeratu puntu suspentsiboak (**...)** eta, ondoren, izena **aldatu**.
4. Aldatu izena urratsa **Ezarri proiektuaren ataza**.
5. urtean **Izena** eremua, hautatu **msdyn\_ projecttaskid**.
6. rentzat **Balioa** eremua, sartu **gidari ()** esamoldearen eraikitzailean.

## <a name="step-12-create-a-project-task"></a><a id="12"></a> 12. urratsa: Sortu proiektuko ataza

Jarraitu urrats hauek uneko proiektuaren eta zuk sortutako proiektu-ontziaren ID esklusibo bat duen proiektu-zeregin bat sortzeko.

1. Fluxuan, hautatu **Urrats berria**.
2. Elkarrizketa-koadroan **, bilaketa-esparruan, eragiketa** bat aukeratu, lotu **gabeko ekintza** bat idatzi. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Sortu proiektuaren ataza**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ PssCreateV1**.
6. urtean **Entitatea** eremuan, idatzi parametroen informazioa.

    ```
    {
        "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_projecttask",
        "msdyn_projecttaskid": "@{variables('msdyn_projecttaskid')}",
        "msdyn_project@odata.bind": "/msdyn_projects(@{outputs('Create_Project')?['body/ProjectId']})",
        "msdyn_subject": "ScheduleAPIDemoTask1",
        "msdyn_projectbucket@odata.bind": "/msdyn_projectbuckets(@{outputs('Create_Project_Buckets')?['body/msdyn_projectbucketid']})",
        "msdyn_start": "@{addDays(utcNow(), 1)}",
        "msdyn_scheduledstart": "@{utcNow()}",
        "msdyn_scheduledend": "@{addDays(utcNow(), 5)}",
        "msdyn_LinkStatus": "192350000"
    }
    ```

    Hona hemen parametroen azalpena:

    - **\@\@ odata.mota** – Erakundearen izena. Adibidez, sartu **"Microsoft.Dynamics.CRM.msdyn\_ proiektuaren zeregina"**.
    - **msdyn\_ projecttaskid** – Zereginaren ID bakarra. Balioa aldagai dinamiko batean ezarri behar da **msdyn\_ projecttaskid**.
    - **msdyn\_ proiektua\@ odata.bind** – Proiektu jabearen proiektuaren IDa. Balioa "Sortu proiektua" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_ proiektuak(GEHITU EDUKIA DINAMIKOA)"**.
    - **msdyn\_ gaia** – Edozein zereginen izena.
    - **msdyn\_ proiektu-ontzia\@ odata.bind** – Zereginak biltzen dituen proiektu-ontzia. Balioa "Sortu Bucket" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_ projectbuckets(GEHITU EDUKIA DINAMIKOA)"**.
    - **msdyn\_ hasi** – Hasiera datarako eduki dinamikoa. Esaterako, bihar bezala irudikatuko da **"gehituEgunak(utcNow(), 1)"**.
    - **msdyn\_ hasiera programatua** – Programatutako hasiera-data. Esaterako, bihar bezala irudikatuko da **"gehituEgunak(utcNow(), 1)"**.
    - **msdyn\_ ordutegiaren amaiera** – Programatutako amaiera-data. Hautatu etorkizuneko data. Adibidez, zehaztu **"addDays(utcNow(), 5)"**.
    - **msdyn\_ Estekaren egoera** – Estekaren egoera. Adibidez, sartu **"192350000"**.

7. rentzat **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Response** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-13-create-a-resource-assignment"></a><a id="13"></a> 13. urratsa: Sortu baliabide-esleipena

1. Fluxuan, hautatu **Urrats berria**.
2. Elkarrizketa-koadroan **, bilaketa-esparruan, eragiketa** bat aukeratu, lotu **gabeko ekintza** bat idatzi. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Sortu zeregina**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ PssCreateV1**.
6. urtean **Entitatea** eremuan, idatzi parametroen informazioa.

    ```
    {
        "@odata.type": "Microsoft.Dynamics.CRM.msdyn_resourceassignment",
        "msdyn_resourceassignmentid": "@{guid()}",
        "msdyn_name": "ScheduleAPIDemoAssign1",
        "msdyn_taskid@odata.bind": "/msdyn_projecttasks(@{variables('msdyn_projecttaskid')})",
        "msdyn_projectteamid@odata.bind": "/msdyn_projectteams(@{outputs('Create_Team_Member')?['body/TeamMemberId']})",
        "msdyn_projectid@odata.bind": "/msdyn_projects(@{outputs('Create_Project')?['body/ProjectId']})"
    }
    ```

7. rentzat **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Response** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-14-decrement-a-variable"></a><a id="14"></a> 14. urratsa: aldagai bat gutxitu

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **dekretu aldagaia**. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. urtean **Izena** eremua, hautatu **ataza kopurua**.
4. urtean **Balioa** eremua, sartu **1**.

## <a name="step-15-rename-a-project-task"></a><a id="15"></a> 15. urratsa: aldatu izena proiektu bati

1. Fluxuan, hautatu **Urrats berria**.
2. Elkarrizketa-koadroan **, bilaketa-esparruan, eragiketa** bat aukeratu, lotu **gabeko ekintza** bat idatzi. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Aldatu izena proiektuaren ataza**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ PssUpdateV1**.
6. urtean **Entitatea** eremuan, idatzi parametroen informazioa.

    ```
    {
        "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_projecttask",
        "msdyn_projecttaskid": "@{variables('msdyn_projecttaskid')}",
        "msdyn_subject": "ScheduleDemoTask1-UpdatedName"
    }
    ```

7. rentzat **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Response** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-16-run-an-operation-set"></a><a id="16"></a> 16. urratsa: Exekutatu eragiketa multzo bat

1. Fluxuan, hautatu **Urrats berria**.
2. Elkarrizketa-koadroan **, bilaketa-esparruan, eragiketa** bat aukeratu, lotu **gabeko ekintza** bat idatzi. Ondoren, betilean **·**, aukeratu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Eragiketa multzoa exekutatu**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ ExecuteOperationSetV1**.
6. rentzat **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Erantzun OperationSetId** urtean **Eduki dinamikoa** elkarrizketa-koadroa.

## <a name="references"></a>Erreferentziak

- [Fluxuak nola integratzeko ikuspegi orokorra Dataverse -Power Automate](/power-automate/dataverse/overview?WT.mc_id=email)
- [Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko](schedule-api-preview.md)
- [Hodei-fluxuen ikuspegi orokorra -Power Automate](/power-automate/overview-cloud?WT.mc_id=email)
- [Irtenbideen jakitun diren fluxuen ikuspegi orokorra -Power Automate](/power-automate/overview-solution-flows?WT.mc_id=email)
