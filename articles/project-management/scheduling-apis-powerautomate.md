---
title: Erabili proiektuaren antolaketa APIak Power Automate-rekin
description: Artikulu honek Project schedule aplikazioen programazio interfazeak (API) erabiltzen dituen lagin-fluxu bat eskaintzen du.
author: ruhercul
ms.date: 01/26/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: afec082c680596e8dcb8ec0b350b4bb7853c49ff
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 09/02/2022
ms.locfileid: "9404449"
---
# <a name="use-project-schedule-apis-with-power-automate"></a>Erabili proiektuaren antolaketa APIak Power Automate-rekin

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Artikulu honek lagin-fluxu bat deskribatzen du, proiektuaren plan osoa erabiliz nola sortu erakusten duena Microsoft Power Automate, eragiketa multzo bat nola sortu eta entitate bat nola eguneratu. Adibideak proiektu bat, proiektuko taldekidea, eragiketa multzoak, proiektuko zereginak eta baliabide-esleipenak nola sortu erakusten du. Artikulu honek entitate bat nola eguneratu eta eragiketa multzo bat exekutatu ere azaltzen du.

Jarraian, artikulu honetako lagin-fluxuan dokumentatzen diren urratsen zerrenda osoa da:

1. [Sortu a PowerApps trigger](#1)
2. [Sortu proiektua](#2)
3. [Hasierako aldagai bat taldekidearentzat](#3)
4. [Sortu taldekide generiko bat](#4)
5. [Sortu eragiketa multzo bat](#5)
6. [Sortu proiektu-ontzi bat](#6)
7. [Hasieratu estekaren egoerarako aldagai bat](#7)
8. [Hasta ezazu ataza kopuruaren aldagai bat](#8)
9. [Hasieratu proiektuaren ataza IDrako aldagai bat](#9)
10. [Egin arte](#10)
11. [Ezarri proiektuko zeregin bat](#11)
12. [Sortu proiektu-zeregin bat](#12)
13. [Sortu baliabide-esleipena](#13)
14. [Aldagai bat gutxitu](#14)
15. [Aldatu izena proiektuko ataza bati](#15)
16. [Exekutatu eragiketa multzo bat](#16)

## <a name="assumptions"></a>Hipotesiak

Artikulu honek oinarrizko ezagutzak dituzula suposatzen du Dataverse plataforma, hodeiko fluxuak eta Project Schedule Application Programming Interface (API). Informazio gehiagorako, ikusi [Erreferentziak](#references) atala artikulu honetan geroago.

## <a name="create-a-flow"></a>Sortu fluxu bat

### <a name="select-an-environment"></a>Hautatu ingurune bat

Sortu dezakezu Power Automate fluxua zure ingurunean.

1. Joan<https://flow.microsoft.com>, eta erabili administratzailearen kredentzialak saioa hasteko.
2. Goiko eskuineko izkinan, hautatu **Inguruneak**.
3. Zerrendan, hautatu ingurunea non Dynamics 365 Project Operations instalatuta dago.

### <a name="create-a-solution"></a>Sortu soluzio bat

Jarraitu urrats hauek bat sortzeko [konponbidez jabetzen den fluxua](/power-automate/overview-solution-flows). Soluzioz jabetzen den fluxua sortuz gero, errazago esporta dezakezu fluxua geroago erabiltzeko.

1. Nabigazio-panelean, hautatu **Irtenbideak**.
2. Gainean **Irtenbideak** orrialdea, hautatu **Irtenbide berria**.
3. urtean **Irtenbide berria** elkarrizketa-koadroa, ezarri beharrezko eremuak eta, ondoren, hautatu **Sortu**.

## <a name="step-1-create-a-powerapps-trigger"></a><a id="1"></a> 1. urratsa: Sortu a PowerApps trigger

1. Gainean **Irtenbideak** orrialdean, hautatu sortu duzun soluzioa eta, ondoren, hautatu **Berria**.
2. Ezkerreko panelean, hautatu **Hodei-fluxuak** \> **Automatizazioa** \> **Hodei-fluxua** \> **Berehala**.
3. urtean **Fluxuaren izena** eremua, sartu **Programatu API Demo Flow**.
4. urtean **Aukeratu fluxu hori nola abiarazi** zerrenda, hautatu **Power Apps**. Bat sortzen duzunean Power Apps trigger, logika zure esku dago egilea gisa. Artikulu honetan, utzi sarrera-parametroak hutsik probak egiteko.
5. Hautatu **Sortu**.

## <a name="step-2-create-a-project"></a><a id="2"></a>2. pausoa: Sortu proiektu bat

Jarraitu urrats hauei lagin-proiektu bat sortzeko.

1. Sortu duzun fluxuan, hautatu **Urrats berria**.

    ![Urrats berri bat gehitzea.](media/newstep.png)

2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.

    ![Eragiketa bat hautatzea.](media/chooseactiontab.png)

3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.

![Urrats bati izena aldatzea.](media/renamestep.png)

4. Aldatu izena urratsa **Sortu Proiektua**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ SortuProiektuaV1**.
6. azpian **msdyn\_ gaia** eremua, hautatu **Gehitu eduki dinamikoa**.
7. Gainean **Adierazpena** fitxan, funtzio eremuan, sartu **Proiektuaren izena - utcNow()**.
8. Hautatu **Ados**.

## <a name="step-3-initialize-a-variable-for-the-team-member"></a><a id="3"></a> 3. urratsa: hasieratu taldekidearentzat aldagai bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Init taldeko kidea**.
5. urtean **Izena** eremua, sartu **TaldekideEkintza**.
6. urtean **Mota** eremua, hautatu **Katea**.
7. urtean **Balioa** eremua, sartu **msdyn\_ Sortu TaldekideaV1**.

## <a name="step-4-create-a-generic-team-member"></a><a id="4"></a> 4. urratsa: Sortu taldekide generiko bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Sortu taldekidea**.
5. Horretarako **Ekintzaren izena** eremua, hautatu **TaldekideEkintza** urtean **Eduki dinamikoak** elkarrizketa-koadroa.
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

    - **\@\@ odata.mota** – Entitatearen izena. Adibidez, sartu **"Microsoft.Dynamics.CRM.msdyn\_ proiektu taldea"**.
    - **msdyn\_ projectteamid** – Proiektu-taldearen IDaren lehen gakoa. Balioa identifikatzaile bakarra (GUID) adierazpena da.   IDa espresioaren fitxatik sortzen da.

    - **msdyn\_ proiektua\@ odata.bind** – Proiektu jabearen proiektuaren IDa. Balioa "Sortu proiektua" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_ proiektuak(GEHITU EDUKIA DINAMIKOA)"**.
    - **msdyn\_ izena** – Taldekidearen izena. Adibidez, sartu **"ScheduleAPIDemoTM1"**.

## <a name="step-5-create-an-operation-set"></a><a id="5"></a> 5. urratsa: Sortu eragiketa multzo bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Sortu eragiketa multzoa**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ Sortu OperationSetV1** Dataverse ekintza pertsonalizatua.
6. urtean **Deskribapena** eremua, sartu **ScheduleAPIDemoOperationSet**.
7. urtean **Proiektua** eremua, sartu **/msdyn\_ proiektuak(**.
8. urtean **Eduki dinamikoak** elkarrizketa-koadroa, hautatu **msdyn\_ SortuProiektuaV1Erantzun Proiektuaren Id**.
9. urtean **Proiektua** eremua, sartu **)**.

## <a name="step-6-create-a-project-bucket"></a><a id="6"></a> 6. urratsa: Sortu proiektu-ontzi bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **gehitu errenkada berria**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Sortu Bucket**.
5. urtean **Taularen izena** eremua, hautatu **Project Buckets**.
6. urtean **Izena** eremua, sartu **ScheduleAPIDemoBucket1**.
7. Horretarako **Proiektua** eremua, hautatu **msdyn\_ SortuProiektuaV1Erantzun ProiektuarenId** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-7-initialize-a-variable-for-the-link-status"></a><a id="7"></a> 7. urratsa: hasieratu aldagai bat estekaren egoerarako

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Hasi estekaren egoera**.
5. urtean **Izena** eremua, sartu **estekaren egoera**.
6. urtean **Mota** eremua, hautatu **Zenbaki osoa**.
7. urtean **Balioa** eremua, sartu **192350000**.

## <a name="step-8-initialize-a-variable-for-the-number-of-tasks"></a><a id="8"></a> 8. urratsa: ataza kopuruaren aldagai bat hasieratu

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Init Zeregin kopurua**.
5. urtean **Izena** eremua, sartu **ataza kopurua**.
6. urtean **Mota** eremua, hautatu **Zenbaki osoa**.
7. urtean **Balioa** eremua, sartu **5**.

## <a name="step-9-initialize-a-variable-for-the-project-task-id"></a><a id="9"></a> 9. urratsa: hasieratu aldagai bat proiektuaren ataza IDrako

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Hasi ProjectTaskID**.
5. urtean **Izena** eremua, sartu **ataza kopurua**.
6. urtean **Mota** eremua, hautatu **Katea**.
7. Horretarako **Balioa** eremua, sartu **gidari ()** esamoldearen eraikitzailean.

## <a name="step-10-do-until"></a><a id="10"></a> 10. urratsa: egin arte

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **egin arte**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Ezarri baldintzazko adierazpenaren lehen balioa **ataza kopurua** aldagaitik **Eduki dinamikoak** elkarrizketa-koadroa.
4. Ezarri baldintza honetara **berdina baino gutxiago**.
5. Ezarri baldintzazko adierazpenean bigarren balioa **0**.

## <a name="step-11-set-a-project-task"></a><a id="11"></a> 11. urratsa: Ezarri proiektuko zeregin bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **ezarri aldagaia**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Ezarri proiektuaren zeregina**.
5. urtean **Izena** eremua, hautatu **msdyn\_ projecttaskid**.
6. Horretarako **Balioa** eremua, sartu **gidari ()** esamoldearen eraikitzailean.

## <a name="step-12-create-a-project-task"></a><a id="12"></a> 12. urratsa: Sortu proiektuko ataza

Jarraitu urrats hauek uneko proiektuari eta zuk sortutako proiektu-ontziari dagokion ID esklusibo bat duen proiektu-zeregin bat sortzeko.

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
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

    - **\@\@ odata.mota** – Entitatearen izena. Adibidez, sartu **"Microsoft.Dynamics.CRM.msdyn\_ proiektuaren zeregina"**.
    - **msdyn\_ projecttaskid** – Zereginaren ID bakarra. Balioa aldagai dinamiko batean ezarri behar da **msdyn\_ projecttaskid**.
    - **msdyn\_ proiektua\@ odata.bind** – Proiektu jabearen proiektuaren IDa. Balioa "Sortu proiektua" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_ proiektuak(GEHITU EDUKIA DINAMIKOA)"**.
    - **msdyn\_ gaia** – Edozein zereginen izena.
    - **msdyn\_ proiektu-ontzia\@ odata.bind** – Zereginak biltzen dituen proiektu-ontzia. Balioa "Sortu Bucket" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_ projectbuckets(GEHITU EDUKI DINAMIKOA)"**.
    - **msdyn\_ hasi** – Hasiera datarako eduki dinamikoa. Esaterako, bihar bezala irudikatuko da **"gehituEgunak(utcNow(), 1)"**.
    - **msdyn\_ hasiera programatua** – Programatutako hasiera-data. Esaterako, bihar bezala irudikatuko da **"gehituEgunak(utcNow(), 1)"**.
    - **msdyn\_ ordutegiaren amaiera** – Programatutako amaiera-data. Hautatu etorkizuneko data. Adibidez, zehaztu **"addDays(utcNow(), 5)"**.
    - **msdyn\_ Estekaren egoera** – Estekaren egoera. Adibidez, sartu **"192350000"**.

7. Horretarako **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Response** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-13-create-a-resource-assignment"></a><a id="13"></a> 13. urratsa: Sortu baliabide-esleipena

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Sortu zeregina**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ PssCreateV1**.
6. urtean **Entitatea** eremuan, idatzi parametroen informazioa.

    ```
    {
        "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_resourceassignment",
        "msdyn_resourceassignmentid": "@{guid()}",
        "msdyn_name": "ScheduleAPIDemoAssign1",
        "msdyn_taskid@odata.bind": "/msdyn_projecttasks(@{variables('msdyn_projecttaskid')})",
        "msdyn_projectteamid@odata.bind": "/msdyn_projectteams(@{outputs('Create_Team_Member')?['body/TeamMemberId']})",
        "msdyn_projectid@odata.bind": "/msdyn_projects(@{outputs('Create_Project')?['body/ProjectId']})"
    }
    ```

7. Horretarako **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Response** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-14-decrement-a-variable"></a><a id="14"></a> 14. urratsa: aldagai bat gutxitu

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **dekretu aldagaia**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. urtean **Izena** eremua, hautatu **ataza kopurua**.
4. urtean **Balioa** eremua, sartu **1**.

## <a name="step-15-rename-a-project-task"></a><a id="15"></a> 15. urratsa: izena aldatu proiektuaren ataza

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
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

7. Horretarako **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Response** urtean **Eduki dinamikoak** elkarrizketa-koadroa.

## <a name="step-16-run-an-operation-set"></a><a id="16"></a> 16. urratsa: Exekutatu eragiketa multzo bat

1. Fluxuan, hautatu **Urrats berria**.
2. urtean **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, gainean **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta gero hautatu **Aldatu izena**.
4. Aldatu izena urratsa **Eragiketa multzoa exekutatu**.
5. urtean **Ekintzaren izena** eremua, hautatu **msdyn\_ ExecuteOperationSetV1**.
6. Horretarako **OperationSetId** eremua, hautatu **msdyn\_ Sortu OperationSetV1Erantzun OperationSetId** urtean **Eduki dinamikoa** elkarrizketa-koadroa.

## <a name="references"></a>Erreferentziak

- [Fluxuak nola integratzeko ikuspegi orokorra Dataverse -Power Automate](/power-automate/dataverse/overview?WT.mc_id=email)
- [Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko](schedule-api-preview.md)
- [Hodei-fluxuen ikuspegi orokorra -Power Automate](/power-automate/overview-cloud?WT.mc_id=email)
- [Irtenbideen jakitun diren fluxuen ikuspegi orokorra -Power Automate](/power-automate/overview-solution-flows?WT.mc_id=email)
