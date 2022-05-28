---
title: Eginbide aldaketak Project Service Automationetik Project Operationsetara
description: Gai honek Project Service Automation-era eginbide-aldaketen ikuspegi orokorra eskaintzen du Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 7e41b381d6da267f58174305f33fc229c66cd7b7
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: eu-ES
ms.lasthandoff: 04/14/2022
ms.locfileid: "8595391"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Eginbide aldaketak Project Service Automationetik Project Operationsetara

Bertatik eguneratzea Dynamics 365 Project Service Automation to Dynamics 365 Project Operations Lite hiru fasetan emango da. Gai honek bertsio berritzea amaitzean ikusiko dituzun aldaketa nagusiei buruzko informazioa eskaintzen du.

| Berritu entrega | 1. fasea <br>(2022ko urtarrila) | 2. fasea <br>(2022ko apirileko olatua) | 3. fasea  |
|------------------|------------------------|---------------------------|---------------------------|
| Proiektuen lanaren banaketa egituraren (WBS) menpekotasunik ez. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| WBS gaur egun onartzen diren proiektuen eragiketen mugetan sartzen da. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| WBS Project Operations-ek gaur egun onartzen dituen mugetatik kanpo, Project mahaigaineko bezeroaren laguntza barne. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>Proiektuen kudeaketa

Erabiltzailearen esperientzian aldaketarik esanguratsuenak proiektuen plangintzaren arloan izango dira. Project Operations-ek esperientzia moderno berri bat hartzen du lan-matxura-egitura (WBS) kudeatzeko, eskaintzen dituen programazio-gaitasunak aprobetxatuz.[Weberako proiektua](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>Desberdintasunak antolatzeko esperientzian

Hurrengo taulak laburbiltzen ditu Project Service Automation eta Project Operations arteko programazio desberdintasunak.

|  Antolatzen     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| Proiektu-txantiloiak - Proiektu bat sortzen denean proiektu-txantiloiak definitzeko eta aplikatzeko gaitasuna  |  &nbsp;    | :heavy_check_mark: |
| Project work breakdown structure (WBS) mahaigaineko bezeroarekin integratzea   |    &nbsp;  | :heavy_check_mark: |
| Murrizketak - Ez hasi baino lehenago, beranduago amaitu  | :heavy_check_mark: |   &nbsp;  |
| Mugarriak - Zero iraupena duten zereginak   | :heavy_check_mark:  |  &nbsp;  |
| Baliabideen araberako zereginek esleitutako baliabideen erabilgarritasuna errespetatuko dute   | :heavy_check_mark: |  &nbsp;    |
| Denbora-mailako edizioa - Editatu planak eta lan egin egunez egun   |   &nbsp;  | :heavy_check_mark: |
| Programazio automatikoa/eskuz - Erabili Proiektua antolatzeko motorra zereginak automatikoki edo eskuz programatzeko |  &nbsp; | :heavy_check_mark:  |
| Editatu proiektu handiak zuzenean erabiltzailearen interfazean: ez dago mugarik editagarriak diren planen tamainan  | 500 zeregin muga  | :heavy_check_mark:       |
| Osatutako ehunekoa - Markatu zereginaren aurrerapena   | :heavy_check_mark:  |  &nbsp;  |
| [Proiektuaren egutegia moduak](../project-management/scheduling-modes.md) - Proiektua unitate finko, esfortzu finko edo iraupen finko gisa definitzea | :heavy_check_mark: | &nbsp; |
| Denbora-lerroa - Eraiki eta pertsonalizatu denbora-lerroaren ikuspegia ordutegiaren xehetasunak ikusteko eta interesdunekin komunikatzeko. | :heavy_check_mark:  | &nbsp; |
| Ahaleginak bultzatutako zereginak - Motorearen euskarria programatzea, zeregin bat esfortzuaren arabera antolatzeko  | :heavy_check_mark:  | &nbsp; |
| **Zereginaren informazioa** elkarrizketa-koadroa - Gorde zereginaren xehetasunak elkarrizketa-koadro bat erabiliz | :heavy_check_mark:  |  &nbsp;  |
| Arrastatu eta jaregin - Aukeratu zereginak eta aldatu haien posizioa WBSn | :heavy_check_mark: | &nbsp;  |
| Ikuspegi iraunkor malguak - Definitu zereginen atributuen ikuspegi zehatzagoak   | :heavy_check_mark:  | &nbsp; |
| Ordenatu eta iragazi WBS  | :heavy_check_mark:  | &nbsp; |
| Taulen ikuspegia ur-jauziak ez diren proiektuak entregatzeko  | :heavy_check_mark:   | &nbsp; |
| Denbora-lerroaren ikuspegia - WBSa ikusteko eta editatzeko erabiltzen den Gantt diagrama interaktiboa   | :heavy_check_mark:  | &nbsp; |
| Teklatu lasterbideak - Erabili teklatuko lasterbideak ohiko eragiketetarako, hala nola koska edo txertatzeko  | :heavy_check_mark:  |  &nbsp; |
| Maila anitzeko desegin - Egin zer gertatuko den azterketa, aldaketen eragina guztiz ulertzeko, eragiketa multzo oso bat alderantziz eta berriro aplikatuz. | :heavy_check_mark: | &nbsp; |
| Moztu/Kopiatu/Itsatsi - Elkarlanean egutegiaren garapenean, aplikazioen artean ordutegiaren xehetasunak kopiatu eta itsatsiz  | :heavy_check_mark: | &nbsp; |
| Zereginen kontrol-zerrendak - Gehitu gehienez 20 kontrol-zerrendako elementu ataza bati   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>Proiektuaren antolaketa

The **Proiektua** Proiektuaren Eragiketak orrialdean desberdintasun kopuru esanguratsuak ditu **Proiektua** orrialdean Project Service Automation.

Honako ekintza hauek kendu dira **Proiektuak** orrialdea 1. faseko bertsio berritzearen barruan:

  - **Ireki MS Project-en**
  - **Sortu txantiloia**
  - **Kendu esteka MS Project-etik**

The **Proiektua** Proiektuaren Eragiketak atalean fitxa berri hauek ditu.

- **Materialaren aurreikuspenak**
- **Zereginak fakturatzeko konfigurazioa**

The **Egoera** fitxa kendu da eta **Egoera** eremuan dago orain **Laburpen** fitxa proiektuaren programazio moduarekin.

   ![Proiektuaren orrialdearen eguneraketak.](media/projectform.png)

The **Ordutegia** fitxa izena jarri zaio **Zeregin** fitxan eta proiektuak planifikatzeko esperientzia berria eskaintzen du Weberako Project-ekin.

   ![Proiektuaren ataza berriak fitxa.](media/tasktab.png)

## <a name="scheduling-modes"></a>Antolaketa moduak

Project Operations-ek eginbide berri bat aurkeztu du, [Programazio moduak](../project-management/scheduling-modes.md). Lehendik dauden Project Service Automation proiektu guztiak lehenetsiko dira **Iraupen Finkoa** Proiektu Eragiketetan. Hala ere, proiektu berrien lehenetsia helbidera joanda kudeatu daiteke **Ezarpenak** > **Parametroak** > **Parametroa** > **Ordutegi modua**.

   ![Programazio modurako proiektuaren parametroen ezarpenak.](media/projectparameter.png)

## <a name="project-planning-limits"></a>Proiektuaren plangintzaren mugak

Project Operations Weberako Project-ean oinarritzen da proiektuak antolatzeko eragiketa guztietarako. Weberako proiektuak lanaren banaketa-egitura kudeatzen du hurrengo taulako mugak erabiliz.

| **Eremua**                                          | **Muga**             |
|----------------------------------------------------|-----------------------|
| Proiektu baterako gehieneko zereginak                  | 500                   |
| Proiektu baten gehieneko iraupena               | 3650 egun (10 urte)  |
| Proiektu baterako gehieneko baliabideak              | 300                   |
| Proiektu bateko gehieneko estekak (ondorengoak soilik) | 600                   |
| Proiektu baterako gehieneko eremu pertsonalizatuak          | 1,0                    |
| Gehieneko hierarkia-maila                            | 10 maila             |
| Gehieneko estekak (ondorengoa + aurrekoa)            | 20                    |
| Hosto-zereginaren gehienezko iraupena                      | 1250 egun             |
| Laburpen-zeregin baten gehieneko iraupena                 | 3650 egun (10 urte)  |
| Zeregin bati esleitutako gehieneko baliabideak               | 20 baliabide          |
| Zeregin baterako onartutako data-tartea                    | 2000/1/1 - 2149/12/31 |
| Zerrendako elementuak                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>Proiektuen plangintzaren hedagarritasuna eta garapena

Project Operations-era eguneratu ondoren, Project Scheduling APIak erabili behar dituzu sortu, eguneratu eta ezabatzeko eragiketak entitate hauetan exekutatzeko:

|   Entitatearen izena           |   Entitatearen izen logikoa       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| Proiektuaren zeregina            | msdyn_projecttask           |
| Proiektuaren zereginen mendekotasuna | msdyn_projecttaskdependency |
| Baliabide-esleipena     | msdyn_resourceassignment    |
| Proiektuaren ontzia          | msdyn_projectbucket         |
| Proiektu-taldeko kidea     | msdyn_projectteam           |

Une honetan entitate horiek inplikatzen dituzten pertsonalizazioak badituzu, ikus [Erabili Project schedule APIak Scheduling entitateekin eragiketak egiteko](../project-management/schedule-api-preview.md) ezarpen orientabideetarako.

## <a name="data-model-changes"></a>Datu-eredu aldaketak

1. Berritze Fasearen barruan, aldaketak daude datu-ereduan. Aldaketa hauek lehendik dauden entitateen eremu-aldaketak dira batez ere. 1. fasean, entitateek, **msydn_project** eta **msdyn_projectteam** pertsonalizazioen birfactorizazioa dira. 

> [!IMPORTANT]
> Atal hau entitate gehigarriekin eguneratuko da etorkizuneko bertsio berritze faseak amaitu ahala.

Ondorengo eremuak eremu berriekin ordezkatu dira.

|   Entity          |   Izen logiko zaharra   |   Izen logiko berria    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

Ondorengo eremuak gehitu dira.

|   Entity          |   Izen logikoa                               |   Deskribapenak |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | Proiektuaren benetako kuoten salmenten agregatua erakusten du. Project Service Automation-en soilik erabiltzeko. |
| msdyn_project     | msdyn_actualmaterialcost                     | Proiektuko materialaren benetako kostuaren agregatua erakusten du. Project Service Automation-en soilik erabiltzeko. |
| msdyn_project     | msdyn_actualmaterialsales                    | Proiektuko benetako materialen salmentaren agregatua erakusten du. Project Service Automation-en soilik erabiltzeko. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | Proiektu honi lotutako kontratu-lerroa. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | Hau erabiltzen den barne-sistemaren eremua da **Kopiatu proiektua** Korrelazio Identifikatzaileari lotuta. Project Service Automation-en soilik erabiltzeko. |
| msdyn_project     | msdyn_copyprojectsessionid                   | Hau barne-sistemaren eremu bat da, horretarako erabiltzen da **Kopiatu proiektua** Saioaren Identifikatzaileari lotutakoa. Project Service Automation-en soilik erabiltzeko. |
| msdyn_project     | msdyn_globalrevisiontoken                    | Azken sinkronizazioa xRM Global Revision Token Proiektua antolatzeko zerbitzutik. |
| msdyn_project     | msdyn_msprojectdocument                      | Proiektuari dagokion Microsoft Project dokumentua. |
| msdyn_project     | msdyn_plannedmaterialcost                    | Proiektuan aurreikusitako materialaren kostuaren agregatua. Project Service Automation-en soilik erabiltzeko. |
| msdyn_project     | msdyn_plannedmaterialsales                   | Proiektuan aurreikusitako material salmentaren agregatua. Project Service Automation-en soilik erabiltzeko. |
| msdyn_project     | msdyn_programa                                | Proiektu hau dagokion programa. |
| msdyn_project     | msdyn_quotelineproject                       | Proiektu honekin lotutako aurrekontu-lerroa. |
| msdyn_project     | msdyn_replaylogheader                        | Erreprodukzio-erregistroen goiburua. |
| msdyn_project     | msdyn_schedulemode                           | Proiektuko zeregin guztietan erabiltzen den programazio modu lehenetsia.  |
| msdyn_project     | msdyn_taskearlieststart                      | Proiektuko edozein zereginen lehenengo hasiera-data.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Proiektu-taldekide hau kopiatu den proiektu-taldekidea. |
| msdyn_projectteam | msdyn_creategenericteammember eskakizunarekin | Sortu berri den taldekide generiko baterako baliabide-eskakizuna sortu behar den adierazten du.  |
| msdyn_projectteam | msdyn_deletestatus                           | Taldekidearen ezabatze-egoera Proiektua antolatzeko zerbitzura bidalitako ezabatze-eskaerarik dagoen eta espero den denbora-leihoan erantzuna behar bezala bidaltzen duen jarraitzeko. |
| msdyn_projectteam | msdyn_effortcompleted                        | Taldekideak bere zereginetan egindako esfortzuaren jarraipena egiten du. |
| msdyn_projectteam | msdyn_effortremaining                        | Taldekideak bere zereginetan oraindik egin beharreko ahaleginaren jarraipena egiten du. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | Taldekideak Proiektua antolatzeko zerbitzura ezabatzeko eskaera bidaltzen duenetik taldekidea benetan ezabatzen den arte itxaronaldia Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | Taldekidea ezabatzeko eskaera Proiektua antolatzeko zerbitzura bidaltzen denean grabatu beharreko denbora-zigilua. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | Proiektuaren taldeko kidea hau kopiatutako proiektuaren taldeko kidea erakusten du.  |

## <a name="project-templates"></a>Proiektuen txantiloiak

Project Operations-ek ez du proiektuen txantiloietarako laguntzarik eskaintzen. Hala eta guztiz ere, oinarrizko funtzionalitatearen zati handi bat errepika dezakezu [Project Copy APIa](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>Mahaigaineko gehigarrien laguntza

Microsoft Project Desktop gehigarriaren euskarria ez da erabilgarri egongo eguneratzearen lehen 2 faseetan. 3. fasean, Project for Web-en gaur egun onartzen dituen mugak baino proiektu handiagoak dituzten bezeroek mahaigaineko gehigarria erabili ahal izango dute.

## <a name="editing-resource-assignment-contours"></a>Baliabideen esleipenaren sestrak editatzea

Baliabideen esleipenaren sestrak editatzeko aukera erabilgarri egongo da eguneratzearen 2. fasea erabilgarri dagoenean.

## <a name="billing-and-pricing"></a>Fakturazioa eta prezioak

Honako ezaugarri berriak gehitu dira Proiektuaren Eragiketetan. Ezaugarri hauek izaera gehigarriak dira eta ez dute eraginik Project Service Automation datu-ereduan.

- [Proiektuetan eta proiektuetako zereginetan materialaren erabilera erregistratzea](../material/material-usage-log.md)
- [Azpikontratazio kudeaketa](../pro/subcontracting/managing-subcontracts-overview.md)
- [Aurrerakinak eta atxikipenetan oinarritutako kontratuak](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [Kontratuaren egoera ez gainditzeko eta baliozkotzeak](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [Zereginetan oinarritutako fakturazioa](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>Zaharkitutako osagaiak

Ondorengo taulek bertsio zaharkituta dauden osagaien soluziora eguneratu ondoren mugitzen diren eremu zaharkitu guztiak dokumentatzen dituzte. Informazio gehiagorako eta irtenbiderako estekarako, ikus [Dynamics 365 Project Service Automation 3x Project Operations 4x zaharkitutako osagaietara](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>Fakturaren xehetasuna

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinesscheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_template                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduldurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocompleted                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicants eskuragarri dago                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hours eskatuta                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinesscheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_izena                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>salmenta-eskaeraren xehetasuna

| Eremuak                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

