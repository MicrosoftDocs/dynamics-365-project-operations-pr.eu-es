---
title: Erabili proiektuaren antolaketa APIak Power Automate-rekin
description: Artikulu honek lagin-fluxu bat eskaintzen du, Proiektuak antolatzeko aplikazioen programazio interfazeak (API) erabiltzen dituena.
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

Artikulu honek lagin-fluxu bat deskribatzen du, Microsoft Power Automate erabiliz proiektuaren plan osoa erabiliz nola sortu erakusten duena, eragiketa multzo bat nola sortu eta entitate bat nola eguneratu. Adibideak proiektu bat, proiektuko taldekidea, eragiketa multzoak, proiektuko zereginak eta baliabide-esleipenak nola sortu erakusten du. Artikulu honek entitate bat nola eguneratu eta eragiketa multzo bat exekutatu ere azaltzen du.

Jarraian, artikulu honetako lagin-fluxuan dokumentatzen diren urratsen zerrenda osoa da:

1. [Sortu PowerApps abiarazle bat](#1)
2. [Sortu proiektua](#2)
3. [Abiarazi aldagai bat taldekidearentzat](#3)
4. [Taldekide generikoko kidea bat sortu](#4)
5. [Aukera multzoak sortu](#5)
6. [Sortu proiektu-ontzi bat](#6)
7. [Abiarazi aldagai estekaren egoerarentzat](#7)
8. [Abiarazi zeregin kopuruaren aldagaia](#8)
9. [Abiarazi proiektuaren zereginaren IDaren aldagaia](#9)
10. [Egin hona arte](#10)
11. [Ezarri proiektuaren zeregina](#11)
12. [Sortu proiektuaren zeregin bat](#12)
13. [Sortu baliabide-esleipen bat](#13)
14. [Murriztu aldagaia](#14)
15. [Zeregin baten izena aldatu](#15)
16. [Aukera multzoa exekutatu](#16)

## <a name="assumptions"></a>Suposizioak

Artikulu honek Dataverse plataforma, hodeiko fluxuak eta Proiektuak antolatzeko aplikazio-programen interfazeari (API) buruzko oinarrizko ezagutzak dituzula suposatzen du Informazio gehiago lortzeko, ikusi [Erreferentziak](#references) sekzioa artikuluan geroago.

## <a name="create-a-flow"></a>Sortu fluxu bat

### <a name="select-an-environment"></a>Hautatu ingurune bat

Ezin duzu Power Automate fluxua sortu ingurunean.

1. Joan <https://flow.microsoft.com>-ra eta saioa hasi administratzailearen kredentzialak erabiliz.
2. Goiko eskuineko izkinan, hautatu **Inguruneak.**.
3. Zerrendan, hautatu Dynamics 365 Project Operations instalatuta dagoen ingurunea.

### <a name="create-a-solution"></a>Sortu soluzio bat

[Soluzioan oinarritutako fluxua](/power-automate/overview-solution-flows) sortzeko, jarraitu hurrengo urratsei. Soluzioan oinarritutako fluxua sortuz gero, errazago esporta dezakezu fluxua geroago erabiltzeko.

1. Ezkerreko nabigazio-panelean, hautatu **Soluzioak**.
2. **Soluzioen** orrian, hautatu **Soluzio berria**.
3. **Soluzio berria** elkarrizketa-koadroan, ezarri beharrezko eremuak eta hautatu **Sortu**.

## <a name="step-1-create-a-powerapps-trigger"></a><a id="1"></a>1. urratsa: PowerApps abiarazlea sortu

1. **Soluzioak** orrian, hautatu sortutako soluzioa eta, ondoren, hautatu **Berria**.
2. Ezkerreko panelean, hautatu **Hodei-fluxuak** \> **Automatizazioa** \> **Hodei-fluxua** \> **Berehala**.
3. **Fluxuaren izena** eremuan, sartu **Programatu API Demo fluxua**.
4. **Aukeratu fluxu hau nola abiarazi** zerrendan, hautatu **Power Apps**. Power Apps abiarazle bat sortzen duzunean, logika zure esku dago egilea gisa. Artikulu honetan, utzi sarrera-parametroak hutsik probak egiteko.
5. Hautatu **Sortu**.

## <a name="step-2-create-a-project"></a><a id="2"></a>2. pausoa: Sortu proiektu bat

Jarraitu urrats hauei adibide-proiektua sortzeko.

1. Sortu duzun fluxuan, hautatu **Urrats berria**.

    ![Beste urrats bat gehitzea.](media/newstep.png)

2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.

    ![Eragiketa hautatzea.](media/chooseactiontab.png)

3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.

![Urrats bat berrizendatu.](media/renamestep.png)

4. Aldatu izena **Sortu Proiektua** urratsari.
5. **Ekintzaren izena** eremuan, hautatu **msdyn\_CreateProjectV1**.
6. **msdyn\_subject** eremuan, hautatu **Gehitu eduki dinamikoa**.
7. **Adierazpena** fitxan, funtzio eremuan, sartu **Proiektuaren izena - utcNow()**.
8. Hautatu **Ados**.

## <a name="step-3-initialize-a-variable-for-the-team-member"></a><a id="3"></a>3. urratsa: Abiarazi aldagai bat taldekidearentzat

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena urratsari **Hasieratu taldeko kidea**.
5. **Izena** eremuan, sartu **TeamMemberAction**.
6. **Mota** eremuan, hautatu **Katea** aukera.
7. **Balioa** eremuan, sartu **msdyn\_CreateTeamMemberV1**.

## <a name="step-4-create-a-generic-team-member"></a><a id="4"></a>4. urratsa: Taldekide generikoko kidea bat sortu

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena urratsari **Sortu taldeko kidea**.
5. **Ekintzaren izena** eremuan, hautatu **TeamMemberAction** **Eduki dinamikoak** elkarrizketa-koadroan.
6. **Ekintza-parametroak** eremuan, idatzi parametroen informazioa.

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

    - **\@\@odata.type** – Entitatearen izena. Adibidez, sartu **"Microsoft.Dynamics.CRM.msdyn\_projectteam"**.
    - **msdyn\_projectteamid** – Proiektu taldearen IDaren gako nagusia. Balioa identifikatzaile esklusibo orokorraren (GUID) adierazpena da.   IDa espresioaren fitxatik sortzen da.

    - **msdyn\_project\@odata.bind** – Proiektuaren jabearen proiektuaren IDa. Balioa "Sortu proiektua" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_projects(GEHITU EDUKI DINAMIKOA)"**.
    - **msdyn\_name** – Taldeko kidearen izena. Adibidez, idatzi **"ScheduleAPIDemoTM1"**.

## <a name="step-5-create-an-operation-set"></a><a id="5"></a>5. urratsa: Aukera multzoak sortu

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu **Sortu eragiketa multzoa** urratsa.
5. **Ekintzaren izena** eremuan, hautatu **msdyn\_CreateOperationSetV1** Dataverse ekintza pertsonalizatua.
6. **Azalpena** eremuan, sartu **ScheduleAPIDemoOperationSet**.
7. **Proiektua** eremuan sartu **/msdyn\_projects(**.
8. **Eduki dinamikoa** elkarrizketa-koadroan, hautatu **msdyn\_CreateProjectV1Response ProjectId**.
9. **Proiektua** eremuan, sartu **)**.

## <a name="step-6-create-a-project-bucket"></a><a id="6"></a>6. pausoa: Sortu proiektu ontzia

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **gehitu errenkada berria**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena **Sortu ontzia** urratsari.
5. **Taularen izena** eremuan, hautatu **Proiektu ontziak.**
6. **Izena** eremua, sartu **ScheduleAPIDemoBucket1**.
7. **Proiektua** eremuan, hautatu **msdyn\_CreateProjectV1Response ProjectId** **Eduki dinamikoa** elkarrizketa-koadroan.

## <a name="step-7-initialize-a-variable-for-the-link-status"></a><a id="7"></a>7. urratsa: Abiarazi aldagai estekaren egoerarentzat

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu **Init linkstatus** urratsaren izena.
5. **Izena** eremuan, sartu **linkstatus**.
6. **Mota** eremuan, hautatu **Osoko zenbakia** aukera.
7. **Balioa** eremuan, sartu **192350000**.

## <a name="step-8-initialize-a-variable-for-the-number-of-tasks"></a><a id="8"></a>8. urratsa: Abiarazi zeregin kopuruaren aldagaia

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena **Hasier Zeregin kopurua** urratsa.
5. **Izena** eremuan, sartu **zeregin kopurua**.
6. **Mota** eremuan, hautatu **Osoko zenbakia** aukera.
7. **Balioa** eremuan, sartu **5**.

## <a name="step-9-initialize-a-variable-for-the-project-task-id"></a><a id="9"></a>9. urratsa: Abiarazi proiektuaren zereginaren IDaren aldagaia

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **hasieratu aldagaia**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena urratsari **Init ProjectTaskID**.
5. **Izena** eremuan, sartu **zeregin kopurua**.
6. **Mota** eremuan, hautatu **Katea** aukera.
7. **Balioa** eremuan, sartu **guid ()** adierazle eraikitzailean.

## <a name="step-10-do-until"></a><a id="10"></a>10. urratsa: honen aurretik egin

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **honen aurretik egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Ezarri baldintzazko adierazpeneko lehen balioa **ataza kopurua** aldagaira **Eduki dinamikoak** elkarrizketa-koadrotik.
4. Ezarri baldintza honetara **berdina baino gutxiago**.
5. Ezarri baldintzazko adierazpenean bigarren balioa hona: **0**.

## <a name="step-11-set-a-project-task"></a><a id="11"></a>11. urratsa: Ezarri proiektuaren zeregina

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **ezarri aldagaia**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urrats berrian, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena urratsari **Ezarri proiektuaren zeregina**.
5. **Izena** eremuan, hautatu **msdyn\_projecttaskid**.
6. **Balioa** eremuan, sartu **guid ()** adierazle eraikitzailean.

## <a name="step-12-create-a-project-task"></a><a id="12"></a>12. pausoa: Sortu proiektuaren zeregin bat

Jarraitu urrats hauek uneko proiektuari eta zuk sortutako proiektu-ontziari dagokion ID esklusibo bat duen proiektu-zeregin bat sortzeko.

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena urratsari **Sortu proiektuaren zeregina**.
5. **Ekintzaren izena** eremuan, hautatu **msdyn\_PssCreateV1**.
6. **Entitatea** panelean, idatzi hurrengo parametroaren informazioa.

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

    - **\@\@odata.type** – Entitatearen izena. Adibidez, sartu **"Microsoft.Dynamics.CRM.msdyn\_projecttask"**.
    - **msdyn\_projecttaskid** – Zereginaren ID esklusiboa. Balioa aldagai dinamiko batean ezarri behar da **msdyn\_ projecttaskid** elementutik.
    - **msdyn\_project\@odata.bind** – Proiektuaren jabearen proiektuaren IDa. Balioa "Sortu proiektua" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_projects(GEHITU EDUKI DINAMIKOA)"**.
    - **msdyn\_subject** – Edozein zereginen izena.
    - **msdyn\_projectbucket\@odata.bind** – Zereginak biltzen dituen proiektu-ontzia. Balioa "Sortu ontzia" urratsaren erantzunetik datorren eduki dinamikoa izango da. Ziurtatu bide osoa sartzen duzula eta parentesi artean eduki dinamikoa gehitzen duzula. Komatxoak behar dira. Adibidez, sartu **"/msdyn\_projectbuckets(GEHITU EDUKI DINAMIKOA)"**.
    - **msdyn\_start** – Hasiera datarako eduki dinamikoa. Esaterako, bihar **"addDays(utcNow(), 1)"** bezala irudikatuko da
    - **msdyn\_scheduledstart** – Programatutako hasiera-data. Esaterako, bihar **"addDays(utcNow(), 1)"** bezala irudikatuko da
    - **msdyn\_scheduleend** – Programatutako amaiera-data. Hautatu etorkizuneko data. Adibidez, zehaztu **"addDays(utcNow(), 5)"**.
    - **msdyn\_LinkStatus** – Estekaren egoera. Esaterako, idatzi **"192350000"**.

7. **OperationSetId** eremuan, hautatu **msdyn\_CreateOperationSetV1Response** **Eduki dinamikoa** elkarrizketa-koadroan.

## <a name="step-13-create-a-resource-assignment"></a><a id="13"></a>13. urratsa: Sortu baliabide -esleipen bat

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena **Sortu esleipena** urratsari.
5. **Ekintzaren izena** eremuan, hautatu **msdyn\_PssCreateV1**.
6. **Entitatea** panelean, idatzi hurrengo parametroaren informazioa.

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

7. **OperationSetId** eremuan, hautatu **msdyn\_CreateOperationSetV1Response** **Eduki dinamikoa** elkarrizketa-koadroan.

## <a name="step-14-decrement-a-variable"></a><a id="14"></a>14. urratsa: Murriztu aldagaia

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **murriztu aldagaia**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. **Izena** eremuan, hautatu **zeregin kopurua**.
4. **Balioa** eremuan, sartu **1**.

## <a name="step-15-rename-a-project-task"></a><a id="15"></a>15. urratsa: aldatu izena proiektuaren zereginari

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu izena urratsari **Aldatu izena proiektuaren zereginari**.
5. **Ekintzaren izena** eremuan, hautatu **msdyn\_PssUpdateV1**.
6. **Entitatea** panelean, idatzi hurrengo parametroaren informazioa.

    ```
    {
        "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_projecttask",
        "msdyn_projecttaskid": "@{variables('msdyn_projecttaskid')}",
        "msdyn_subject": "ScheduleDemoTask1-UpdatedName"
    }
    ```

7. **OperationSetId** eremuan, hautatu **msdyn\_CreateOperationSetV1Response** **Eduki dinamikoa** elkarrizketa-koadroan.

## <a name="step-16-run-an-operation-set"></a><a id="16"></a>16. urratsa: Aukera multzoak exekutatu

1. Fluxuan hautatu **Urrats berria**.
2. **Aukeratu eragiketa bat** elkarrizketa-koadroan, bilaketa-eremuan, sartu **lotu gabeko ekintza egin**. Ondoren, **Ekintzak** fitxan, hautatu eragiketa emaitzen zerrendan.
3. Urratsean, hautatu elipsia (**...**), eta hautatu **Aldatu izena**.
4. Aldatu **Exekutatu eragiketa multzoa** urratsa.
5. **Ekintzaren izena** eremuan, hautatu **msdyn\_ExecuteOperationSetV1**.
6. **OperationSetId** eremuan, hautatu **msdyn\_CreateOperationSetV1Response OperationSetId** **Eduki dinamikoa** elkarrizketa-koadroan.

## <a name="references"></a>Erreferentziak

- [Fluxuak Dataverse-rekin integratzeko moduari buruzko informazio orokorra - Power Automate](/power-automate/dataverse/overview?WT.mc_id=email)
- [Erabili Proiektuak programatzeko APIak Planifikazio entitateekin eragiketak egiteko](schedule-api-preview.md)
- [Hodeiko fluxuen ikuspegi orokorra -Power Automate](/power-automate/overview-cloud?WT.mc_id=email)
- [Soluzioetan oinarritutako fluxuen informazio orokorra - Power Automate](/power-automate/overview-solution-flows?WT.mc_id=email)
